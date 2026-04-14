---
title: Teste de artigo Balckbird sobre SCIM
article_id: 25902000474898
translation_id: 25902000474898
locale: pt-br
sidebar_position: 3
created_at: '2025-04-08T15:00:21Z'
updated_at: '2025-05-07T11:29:05Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

Artigo de teste!!!

O sistema de gerenciamento de identidades entre domínios (SCIM) permite automatizar o gerenciamento e provisionamento de usuários entre a Miro e o seu provedor de identidade (IdP).

> **Disponível para:**[plano Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Configurado por:** Admins da empresa

## Importante saber

- **O SSO baseado em SAML deve estar configurado corretamente e em funcionamento no seu plano Enterprise antes de começar a configurar o provisionamento automatizado.**
  Veja [o guia](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) para configurar o SSO por SAML.
- **Sincronizar grupos com os times da Miro é opcional.**
  Você pode opcionalmente sincronizar seus grupos IdP com times na Miro. No entanto, para evitar problemas em que um grupo IdP seja excluído de forma não intencional ou temporária, o que resulta na desativação de todos os usuários desse grupo na Miro e aciona a reatribuição de boards e Espaços, não sincronize grupos IdP com times da Miro. Os times podem ser criados e gerenciados usando a [API de Times](https://developers.miro.com/reference/enterprise-create-team). Para mais informações sobre como a API SCIM permite que você gerencie grupos, consulte [Miro Developers](https://developers.miro.com/docs/groups).
- **As alterações de e-mail no SCIM incluem as seguintes regras de validação:**
  - **Verificação de Usuário Gerenciado:** Se o domínio atual do usuário não for reivindicado pela organização que está iniciando a solicitação SCIM, a atualização de e-mail é bloqueada e gera um erro 400.
  - **Verificação do Domínio de E-mail Alvo:** Se o domínio de e-mail alvo for reivindicado por uma organização diferente daquela que iniciou a solicitação SCIM, a atualização do e-mail é bloqueada e gera um erro 400. Se o domínio de e-mail de destino for reivindicado pela organização que está iniciando a solicitação SCIM, a atualização do e-mail é permitida sem necessidade de confirmação de e-mail. Os logs de auditoria registram a atualização em cada organização onde o usuário é membro.
  - **Controle de domínio e logon único (SSO):** As atualizações de e-mail são permitidas com base na verificação de domínio através do Controle de Domínio (IDC) ou Logon Único (SSO). Se o domínio de e-mail de destino for verificado através de CD ou logon único pela organização que iniciou, a atualização pode proceder.
    ![scim-diagram-2.png](images/26547037917330_scim-diagram-2.png)
    *Um diagrama do fluxo de trabalho de validação de mudança de e-mail do SCIM*

### Regras sob as quais o SCIM da Miro opera

- As alterações sincronizadas pelo SCIM são aplicadas principalmente a usuários recém-atribuídos. O status daqueles que já estão sob sua assinatura será complementado, mas não poderá ser substituído, pois as alterações serão aplicadas no nível do grupo ou time. Por exemplo:
  a) Se um usuário for membro do Time1 no lado da Miro e seu IDP enviar uma atualização para adicioná-lo ao Time2, seu status no Time1 permanecerá inalterado.
  b) Se o seu IDP enviar uma atualização contendo alterações no Usuário1, outros membros do time não serão afetados. Conforme mencionado em **Funcionalidades suportadas** > **Grupos de notificação push e sincronização** para substituir o status do time e sincronizar novamente todos os usuários de uma só vez, tente iniciar um novo push.
- Todos os usuários provisionados em SCIM são atribuídos a *licença padrão* da sua assinatura:
  a) Para assinaturas Enterprise sem Programa de licenças flexíveis: uma licença completa. Se a sua assinatura ficar sem licenças, os usuários começarão a ser provisionados sob a licença [gratuita restrita](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
  b) Para assinaturas Enterprise com [Programa de licenças flexíveis](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) ativado: Licença gratuita ou licença gratuita limitada, dependendo da [licença de assinatura padrão](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).
  *- Se você precisar que alguns usuários sejam provisionados sob uma licença diferente da padrão:*
  *conforme declarado acima, todos os usuários recebem a licença padrão. No entanto, você pode atualizar imediatamente todos ou alguns deles usando o atributo **UserType** com um valor Total. Os usuários atualizados com o atributo receberão o upgrade para a licença completa, sem tempo de inatividade no usuário final.*
- Todos os usuários provisionados no SCIM também são afetados pelo recurso [Controle de domínio](../../enterprise-administration/canvas-25-admin-features/domain-control/01-domain-control.md). Isso significa que, se um usuário for membro de apenas um grupo de segurança no seu provedor de identidade, mas suas configurações de controle de domínio definirem 3 times como designados, o usuário também será adicionado a esses 3 times.
- Para proteger o serviço, a Miro limita o número de chamadas de API disponíveis a cada 30 segundos:

  | Tipo de solicitação | Nível de limite |
  | --- | --- |
  | GET scim/users    GET scim/users/\{userId\} | Primeiro limite de taxa nível 1 |
  | POST scim/users/\{userId\}    PUT scim/users/\{userId\}    PATCH scim/users/\{userId\}    DELETE scim/users/\{userId\} | Terceiro limite de taxa Nível 3 |
  | GET scim/Groups    PATCH scim/Groups/\{groupId\} | Quarto limite de taxa Nível 4 |
  | GET scim/Groups/\{groupId\} | Terceiro limite de taxa Nível 4 |

  Para mais informações sobre os níveis de limite, consulte [**aqui.**](https://developers.miro.com/reference#ratelimiting)Se o número de solicitações exceder o limite, a Miro retornará o padrão **429 Too many requests**.

## Funcionalidades compatíveis

O esquema detalhado do SCIM da Miro pode ser encontrado [**aqui**](https://developers.miro.com/docs/scim).

A Miro é compatível com as seguintes funcionalidades de provisionamento:

- **Criar novos usuários**
  Novos usuários atribuídos ao aplicativo da Miro no IdP serão criados na sua assinatura Enterprise da Miro como Membros Enterprise. Os usuários que são adicionados a um grupo de usuários sincronizado a um time da Miro com o mesmo nome serão adicionados ao time como membros do Team
- **Enviar atualizações de perfil de usuário**
  Para os atributos e alterações suportados, veja abaixo
- **Grupos de sincronização e push**
  Sincronize seus grupos IDP e seus membros com os times dentro da sua assinatura Miro Enterprise para gerenciar automaticamente a associação de usuários. A sincronização contínua enviará atualizações específicas sobre os usuários do seu grupo para o time sincronizado da Miro, enquanto um push substituirá o status do time, tratando o grupo como a fonte da verdade (se houverem alterações manuais pelos Admins da empresa no lado da Miro)
- **Desvincular os nomes do grupo/time**
  A Miro sincroniza grupos e times por nome, portanto, eles devem ter exatamente o mesmo nome. No entanto, depois que a sincronização inicial for criada, você poderá dar a um ou a ambos os nomes que forem mais convenientes para você. Você pode ver o exemplo de desacoplamento [aqui](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)
- **Remover usuários do grupo/time (não da assinatura Enterprise. Veja abaixo)**
  Remover um usuário de um grupo o removerá do time sincronizado da Miro (durante a próxima notificação push de grupo)
- **Desativar usuários**
  Desativar/excluir um usuário ou desabilitar o acesso de um usuário ao aplicativo no IDP irá *desativar* o usuário no seu plano Enterprise da Miro. Dependendo da situação, desativar um usuário pode reatribuir seu conteúdo aos admins do time mais antigos:
  - se você desativar o usuário no lado do IDP, mas mantê-lo atribuído ao aplicativo da Miro, a associação do time no lado da Miro não é alterada e seu conteúdo não é reatribuído - eles são simplesmente movidos de um **Ativo** para um estado de **Desativado** (e seção de usuários, respectivamente) e param de consumir uma licença.
  - se você acionar a desativação excluindo o usuário no IDP ou desatribuindo-o do aplicativo da Miro, enquanto o usuário for membro de alguns *times sincronizados*, o usuário também será removido desses *times* da Miro e seu conteúdo nesses times será reatribuído aos admins de time mais antigos.
  - se você acionar a desativação *excluindo* o usuário no IDP ou *desatribuindo-o* do aplicativo da Miro, quando o usuário não for membro de nenhum *time sincronizado* a associação do usuário ao time não será alterada e seu conteúdo não será reatribuído.
  **Remoção de um usuário** da assinatura Enterprise não é compatível *por padrão.* Ainda assim, você pode [adicionar manualmente a funcionalidade usando a API](https://developers.miro.com/docs/scim#section-delete-user-by-id) para remover completamente o usuário da assinatura, em vez de configurá-lo para o status **Desativado**. Neste cenário, o conteúdo é reatribuído para os respectivos membros do time. É impossível definir quais admins terão a titularidade sobre o conteúdo reatribuído automaticamente. Mas isso pode ser definido quando você [desativar manualmente um usuário nas configurações da Miro.](../../enterprise-administration/user-management/01-deactivated-users.md)
- **Reativar usuários**
  Atribuir um usuário de volta ao aplicativo ou reativar o perfil de usuário no IdP irá reativá-lo na sua assinatura Enterprise da Miro se ele tiver sido provisionado e desativado anteriormente.
- **Automatizar a alocação do grupo de cobrança**
  Atribua automaticamente novos usuários a [billing groups](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/01-billing-groups.md) usando SCIM. Depois que seu Provedor de Identidade (IdP) estiver configurado, você pode vincular seus centros de custo aos seus grupos de cobrança. Isso garante que todos os usuários atuais e futuros desses centros de custo sejam automaticamente classificados na categoria de cobrança correta.

Você também pode remover usuários do seu plano Enterprise enviando uma chamada **Excluir** direta da API. Veja a documentação [aqui](https://developers.miro.com/docs/scim#section-delete-user-by-id). Observe que apenas as chamadas *diretas* removerão os usuários. Os eventos de **Excluir** iniciados *pela sua solução de identidade* serão tratados como uma solicitação para **Desativar**.

### Atributos compatíveis

:::warning
Observe que:
- **E-mail** / Parâmetro primário / Identificador exclusivo / **Nome de usuário**) é o único valor exigido pela Miro e deve estar no formato de um e-mail.
- A atualização por e-mail só é possível para usuários já sincronizados. Em outras palavras, a primeira sincronização deve acontecer quando o e-mail no IdP e na Miro for o mesmo, caso contrário, a Miro não reconhecerá o usuário e será criado um perfil duplicado da Miro no novo e-mail.
- A atualização de e-mail deve ocorrer no perfil do IdP do usuário, não na lista de atribuições.
- Diferentemente de outros atributos, atualizar o **e-mail** do usuário enviará uma notificação: tanto o endereço de e-mail antigo quanto o novo receberão uma carta informando ao usuário que agora deve usar o novo endereço de e-mail para entrar na Miro.
:::

| Nome do atributo | Atributo do SCIM (Reivindicação) |
| --- | --- |
| E-mail | Nome de usuário.  **Deve estar presente e no formato de e-mail** |
| *Os atributos listados abaixo não são necessários e serão aceitos pela Miro se estiverem presentes (outros atributos enviados para a Miro serão ignorados).* | |
| Nome completo | displayName      formatado;      givenName + " " + familyName;      nome de usuário |
| Tipo de usuário | Tipo de usuário       valor compatível: Completa |
| Ativo | ativo       Valor compatível: "true" ou "false" |
| Imagem do perfil | **photos.^[type=='photo'].value** ou     **photos.^[type==photo].value** (Okta)     **photos[type eq "photo"].value** (Entra)        Deve ser um URL de texto para a imagem.        Tipos de arquivos compatíveis: jpg, jpeg, bmp, png, gif  Para definir o tipo de arquivo, você deve ter a extensão de arquivo definida no URL (ex.: `https://host.com/avatar_user1.jpg`) ou a solicitação para o URL deve retornar, junto com o conteúdo do arquivo, um cabeçalho Content-Type (ex.: Content-Type = 'image/jpeg')        O tamanho máximo do arquivo para baixar é: 31457280 bytes |
| Função do usuário | roles.^[primary==true].value (Okta)      roles[primary eq "True"].value (Entrar)        valores compatíveis:  **ADMIN_INTERNO_DA_ORGANIZAÇÃO** **ORGANIZATION_INTERNAL_USER** |
| Número do funcionário | employeeNumber |
| Centro de custos | costCenter |
| Organização | Organização |
| Divisão | divisão |
| Departamento | departamento |
| Nome do gerente | manager.displayName |
| ID do gerente | gerente.valor  O campo "value" tem o tipo String no padrão SCIM, mas managerId      o campo interno da Miro tem o tipo Long. Se o atributo "value" não for       um valor numérico, ignoramos esse valor |

:::warning
Não há suporte para as alterações de senha e não há planos imediatos para começar a oferecer suporte a essa alteração.
⚠️ **Nome de usuário**, **UserType** e **roles.value** não podem ser atualizados para [Usuários desativados](../../enterprise-administration/user-management/01-deactivated-users.md).
:::

Todos os atributos serão exibidos na lista de usuários CSV exportada que pode ser baixada da [seção de Usuários ativos](../../enterprise-administration/user-management/12-user-management-overview-on-enterprise-plan.md).

![download_as_CSV_in_company_settings.jpg](images/26547037917970_download%20as%20CSV%20in%20company%20settings.jpg)
*A opção de baixar uma lista de usuários*

![mceclip3.png](images/26547037919634_mceclip3.png)

## Como configurar o SCIM

### Passo 1: Habilitar opção SCIM na Miro

Para habilitar o SCIM no seu plano Enterprise da Miro, vá para as **configurações da Empresa** > **Integrações Enterprise,** e habilite a funcionalidade de provisionamento do SCIM**.</strong>** Lá você pode obter o URL base e o token da API para configurar seu IdP.

![scim.png](images/26547037921170_scim.png)
*SCIM nas configurações da Miro*

### Passo 2: Configure seu provedor de identidade

A configuração dependerá do provedor de identidade que você utilizar. A Miro é compatível com Okta e Entra ID pré-configurados, no entanto, você pode usar qualquer provedor de identidade de sua escolha, sempre que a configuração do SCIM permitir.

OKTA - veja as instruções de configuração [aqui](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md).

Entra ID — veja as instruções de configuração [aqui](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

## Gerar novo token

1. Acesse as **Configurações da empresa** > **Integrações Enterprise.**

2. Na seção **Provisionamento SCIM**, clique em **Gerar novo token**.

![scim.png](images/26547037921170_scim.png)
*SCIM nas configurações da Miro*

2. Na janela **Gerar novo token SCIM**, clique em **Gerar**.

![gerar_token.png](images/26547037921938_generate_token.png)

3. Depois de gerar um novo token, você deve configurá-lo no seu provedor IDP.

## Possíveis problemas e como resolvê-los

*1. Os usuários não são provisionados devido a um erro na lista de permissões.*
![mceclip0.png](images/26547037922834_mceclip0.png)
*Um exemplo de erro do provedor de identidade Okta*

Certifique-se de que o endereço de domínio do usuário seja adicionado à sua lista de permissões [nas **configurações de Segurança**](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

*2. Se você autenticar seus usuários finais com uma solução de identidade (IDP1), mas quiser habilitar o SCIM por meio de um IdP diferente (IDP2), isso será possível em duas condições:*

1. O IDP2 pode fazer chamadas de API com o token ao portador.
2. Ambos os provedores de identidade estão sincronizados (para que os usuários provisionados pelo SCIM também existam no IdP1 e, portanto, possam se autenticar com a Miro).

Para mais informações, por favor [entre em contato com o time de suporte da Miro](https://help.miro.com/hc/en-us/requests/new?referer=help-center-article).
