---
title: "Logon \xFAnico (SSO)"
article_id: 360017571414
translation_id: 360017571414
locale: pt-br
sidebar_position: 9
created_at: '2019-02-11T10:08:59Z'
updated_at: '2026-01-07T13:25:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Com o logon único (SSO) baseado em SAML, os usuários podem acessar a Miro por meio de um provedor de identificação (IdP) de sua escolha.

> **Disponível para:** planos Business, Enterprise
> **Função necessária:** Admin da empresa

## Como funciona o SSO por SAML

1. Quando um usuário da Miro tenta fazer login na Miro usando SSO, a Miro envia uma solicitação SAML (Linguagem de marcação de asserção de segurança) para o provedor de identificação (IdP).
2. O provedor de identificação valida as credenciais do usuário e envia uma resposta de volta à Miro para confirmar a identificação do membro.
3. A Miro reconhece a resposta e concede acesso, permitindo que o membro faça login em sua conta da Miro.

## O que acontece após a ativação do SSO?

**Como ativar o SSO pela primeira vez**

Na primeira vez que você configurar o SSO, os usuários existentes podem continuar trabalhando na Miro sem interrupção. No entanto, da próxima vez que eles saírem, sua sessão expirar ou eles tentarem fazer login a partir de um novo dispositivo, eles precisarão fazer login por SSO.

Outras opções de login serão desabilitadas para usuários, incluindo login padrão + senha, Google, Facebook, Slack, AppleID e O365.

**Tempo limite da sessão ociosa**

Se você tiver habilitado [o tempo limite da sessão ociosa](../../security-integrations/security-management/02-idle-session-timeout.md), os usuários serão desconectados automaticamente do seu perfil da Miro e precisarão autorizar por SSO novamente.

**Vários times e organizações**

Se seus usuários tiverem vários times ou organizações da Miro, você pode configurá-los para usar o mesmo provedor de identificação (IdP) para autenticação.

**Quem é obrigado a fazer login com SSO?**

O login pelo SSO é necessário para usuários ativos que fazem parte da sua assinatura Enterprise *e* têm um domínio listado nas configurações do SSO.

- Os usuários que acessam a Miro a partir de domínios não adicionados nas suas configurações de SSO não precisam fazer login com o SSO e devem fazer login usando os métodos de login padrão.
- Usuários de um domínio verificado que não fazem parte da sua assinatura do plano Miro Enterprise precisam fazer login via logon único (SSO) somente se o [provisionamento just-in-time (JIT)](../../user-management/13-user-provisioning-on-enterprise-plan.md) estiver habilitado. Esses usuários serão adicionados automaticamente a um time pré-configurado e precisarão usar o SSO para fazer login.
- [Usuários gerenciados](../../user-management/06-managed-users-on-enterprise-plan.md), que são quaisquer usuário dentro dos seus domínios verificados, incluindo qualquer usuário gerenciado que também seja membro de um time fora da sua assinatura Enterprise . Para restringir o acesso a times específicos, atualize suas configurações de  [controle de domínio](../../canvas-25-admin-features/domain-control/01-domain-control.md).
  > ✏️ Para uma assinatura Enterprise , uma organização pode ter domínios verificados e não verificados. Para domínios verificados, os usuários se tornam usuários gerenciados que devem se autenticar com SSO. Para usuários de domínio não verificados na mesma organização, e-mail e senha são necessários para autenticação.

**Como gerenciar os detalhes do usuário**

Os dados do usuário são atribuídos automaticamente na Miro pelo seu provedor de identificação após o sucesso do login. Alguns parâmetros como nome e senha não podem ser alterados. Outros parâmetros, como fotos do departamento e do perfil, são opcionais.  /span>

- Os nomes de usuário da Miro são atualizados após cada autenticação de sucesso do usuário. Para mais informações sobre como configurar os nomes de usuários da Miro, consulte as configurações avançadas de SSO. Se você precisar alterar o endereço de e-mail de um usuário, pode fazer isso apenas por meio do [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md). Se você não usar o SCIM, [entre em contato com a equipe de suporte](https://help.miro.com/hc/requests/new?referer=help-center-article).

![sso-settings-2.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21027132582290_sso-settings-2.png)
*Seleção de domínio nas configurações de SSO*

> **💡**Para evitar o bloqueio, crie um usuário emergencial para "quebrar a barreira" com um e-mail que tenha um domínio fora do domínio listado nas configurações de SSO, como emailquebrabarreira@gmail.com. Caso contrário, você pode entrar em contato com o suporte e eles podem desabilitar o SSO para toda a organização.

## Como configurar o SSO

### Provedores de identificação (IdP)

Use qualquer provedor de identificação de sua escolha. Abaixo estão as plataformas do provedor de identificação mais populares:

- [OKTA](../../security-integrations/single-sign-on-sso/07-how-to-configure-okta-sso.md)
- [ID de entrada](../../security-integrations/single-sign-on-sso/05-how-to-configure-entra-id-sso.md)da Microsoft
- [OneLogin](../../security-integrations/single-sign-on-sso/08-how-to-configure-onelogin-sso.md)
- [ADFS](../../security-integrations/single-sign-on-sso/02-how-to-configure-adfs-sso.md) da Microsoft
- [Auth0](../../security-integrations/single-sign-on-sso/03-how-to-сonfigure-auth0-sso.md)
- [Google SSO](../../security-integrations/single-sign-on-sso/06-how-to-configure-google-sso.md)
- [Jumpcloud SSO](https://support.jumpcloud.com/support/s/article/single-sign-on-sso-with-miro)

### Como configurar seu IdP

> **💡** [Se sua organização do plano Enterprise quiser adicionar vários provedores de identidade](../../security-integrations/single-sign-on-sso/01-adding-multiple-identity-providers.md) (IdPs), inscreva-se em nosso [beta privado](https://coda.io/form/Miro-Multi-IdP-Private-Beta-Sign-Up_dkoTJMza_jV).

1. Vá para a seção de configuração do seu provedor de identificação e siga as instruções do provedor para configurar o logon único.

2. Adicione os seguintes metadados. Recomendamos pular quaisquer campos opcionais e deixar quaisquer valores padrão como eles estão.

#### Especificações (metadados)

|  |  |
| --- | --- |
| **Protocolo** | SAML 2.0 |
| **Ligação** | Redirecionamento HTTP de SP para IdP Post HTTP para IdP para SP |
| O **URL do serviço** (URL iniciado pelo SP)  Também conhecido como URL de lançamento, URL de resposta, URL do serviço SSO de terceira parte confiável, URL de destino, URL de login do SSO, ponto de extremidade do provedor de identificação, etc. | https://miro.com/sso/saml |
| **URL de serviço ao consumidor da asserção**    Também conhecido como URL de retorno de chamada permitido, URL do ACS personalizado, URL de resposta | https://miro.com/sso/saml |
| **ID da entidade**    Também conhecido como Identificador, identificador de confiança de terceira parte confiável | https://miro.com/ |
| **Estado de retransmissão padrão** | deve ser deixadovazio na sua configuração |
| [**Requisito de assinatura**](https://developers.onelogin.com/saml/examples/response) | Uma resposta SAML não assinada com umaasserção assinada  Uma resposta SAML assinada com uma asserção assinada |
| **SubjectConfirmation Method** | "urn:oasis:names:tc:SAML:2.0:cm:bearer" |
| A resposta SAML do provedor de identificação deve conter umcertificado x509 de chave pública emitido pelo provedor de identificação.  Visualizar exemplos detalhados deSAML. Baixe o [arquivo de metadados da Miro SP](https://drive.google.com/file/d/1BN58fiwC062F5MC-PsO3QN7JlCbKNCSJ/view) (XML). | |

:::warning
A criptografia e o logout único não são compatíveis.
:::

#### Credenciais do usuário

Quaisquer campos adicionais fora do campo abaixo não são necessários. Recomendamos pular quaisquer campos opcionais e deixar quaisquer valores padrão como eles estão.

|  |  |
| --- | --- |
| Atributos de credenciais do usuário necessários | |
| **NameID**(é igual ao endereço de e-mail de um usuário)  Também conhecido como SAML_Subject, chave primária, nome de logon, formato de nome de usuário do aplicativo, etc. | &lt;NameID Format="urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress"&gt; |
| **Atributos opcionais para serem enviados com a asserção**  (atualizado a cada nova autenticação por SSO, usado quando presente/disponível) | - "DisplayName" ou "http://schemas.microsoft.com/identity/claims/displayname" (usado como nome preferido)  [mceclip0.png](http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname)  - “FirstName”, "GivenName" or "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname"; - “LastName”, "Surname" or "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname"; - “ProfilePicture” — O URL codificado da imagem |

### Como habilitar o SSO nas suas configurações da Miro

Plano Business Plano Enterprise

1. Vá para **Configurações da empresa** > **Segurança** > **Logon único**
2. Habilite a opção **SSO/SAML

*![segurança-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20889990489874_security-sso.png)***

1. Vá para **Configurações da empresa** > **Segurança e conformidade** > **Autenticação** > **Logon único**
2. Habilite a opção **SSO/SAML

*![sso-empresa.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366644626_sso-enterprise.png)***

:::note
A ativação do SSO nas suas configurações não habilita imediatamente o SSO para usuários. O login SSO estará disponível após seus [domínios serem verificados](../../canvas-25-admin-features/domain-control/01-domain-control.md). Então, ao configurar o SSO na próxima seção, certifique-se de adicionar seus domínios verificados.
:::

### Como habilitar o SSO nas suas configurações da Miro

Depois de ativar o recurso SSO/SAML nas configurações de logon único , preencha os seguintes campos:

1. **URL de login do SAML** (na maioria dos casos, ele abre a página do seu provedor de identificação, onde seus usuários finais devem inserir suas credenciais)
2. **Certificado x.509 de chave pública** (emitido pelo seu provedor de identificação)
3. Todos os domínios e subdomínios permitidos ou necessários ACME.com ou ACME.dev.com) para autenticar por meio do seu servidor SAML
4. Adicione seu(s) domínio(s) verificado(s). Para **usuários desses domínios que farão login usando SSO**, clique em ***Selecionar um domínio***e selecione qualquer um dos seus domínios para adicionar à lista.

![sso-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366648082_sso-settings.png)
*Configurações do Miro SSO*

### Como renovar seu certificado SSO/SAML

Se o seu Certificado x.509 de chave pública tiver expirado, o SSO continuará funcionando, mas é altamente recomendável renová-lo para continuar usando a Miro com segurança. Os certificados x.509 de chave pública garantem a segurança, privacidade, autenticidade e integridade das informações compartilhadas entre seu provedor de identidade e a Miro.

Esses certificados são válidos somente por um período de tempo que pode ser especificado (e verificado) com seu provedor de identidade. Entre em contato com seu provedor de identidade para verificar a data de validade.

Este processo tem duas etapas:

1. Renove o certificado com seu provedor de identidade. Verifique as instruções sobre como fazer isso.
2. Adicione o certificado renovado à sua configuração de SSO na Miro.

#### Adicionando certificados renovados à Miro

:::warning
Recomendamos substituir seu certificado x.509 durante períodos de menor movimento em sua organização (por exemplo, nos fins de semana ou após o horário comercial) para evitar interrupções de login.
:::

1. Vá para suas configurações da **empresa** > **Autenticação** > **Logon único**
2. Exclua o conteúdo dentro do campo **Certificado de chave x509**
3. Cole a nova chave dentro deste campo
4. Role para baixo e clique em **Salvar**
   ![sso-gif-2.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21027132584850_sso-gif-2.gif)
*Renovando um certificado x.509 no Miro*

## Como testar sua configuração de SSO

Teste sua configuração de SSO antes de habilitá-la para reduzir as chances de problemas de login para seus usuários.

1. Conclua as etapas acima para configurar o SSO.
2. Clique no botão **Testar a configuração de SSO**.
3. Revise os resultados:

- Se não houver nenhum problema, uma mensagem de confirmação **de que o teste de configuração do SSO foi bem-sucedido** será exibida.
- Se forem encontrados problemas, uma mensagem de confirmação **de falha no teste de configuração do SSO** será exibida, seguida por mensagens de erro detalhadas para orientar você sobre o que precisa ser corrigido.

![sso-test.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366649618_sso-test.png)
*Testando configuração SSO*

## Configurações de SSO avançadas opcionais

A seção de configurações opcionais é usada por usuários avançados que estão familiarizados com a configuração de SSO.

### Provisionamento just-in-time para novos usuários

Facilite para seus usuários começarem a usar a Miro imediatamente, sem ter que esperar por um convite ou passar por um longo processo de integração. E certifique-se de que os times gratuitos não sejam criados fora da sua assinatura gerenciada (requer controle de domínio). O SSO é necessário para habilitar o provisionamento just-in-time (JIT) de novos usuários. Todos os usuários provisionados em JIT têm a licença padrão da sua assinatura:

|  |  |  |
| --- | --- | --- |
| **Tipo de assinatura** | **Tipo de licença** | **Comportamento quando as licenças terminam** |
| Plano Business | Licença completa | Os usuários não são adicionados automaticamente; a funcionalidade JIT deixa de funcionar. |
| Plano Enterprise (sem [programa de licenças flexíveis](../../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)) | Licença completa | Usuários provisionados em Licença [gratuita limitada](../../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) |
| Plano Enterprise (com o programa de licenças flexíveis ativado) | Licença gratuita ou licença gratuita limitada | Depende das configurações de [licença padrão](../../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md) |

### Como habilitar o provisionamento just-in-time

Quando você ativar o provisionamento just-in-time, ele se aplicará automaticamente a todos os novos usuários que se registram na Miro. No entanto, os usuários da Miro existentes ainda precisarão de um convite para participar do seu plano.

1. Vá para suas configurações de SSO
2. Marque a caixa **Adicione automaticamente todos os usuários recém-registrados dos domínios listados à sua conta Enterprise**
3. **Escolha um time padrão para usuários recém-registrados** no menu suspenso
4. Clique em **Salvar**

Quando você lista domínios específicos nas configurações de logon único (SSO), quaisquer usuários que se registram com esses domínios serão adicionados automaticamente à sua assinatura Enterprise. Eles serão atribuídos para o time que você selecionou nas suas configurações just-in-time (JIT).

![Copy of user_provisioning_jit_provisioning.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528391698_Copy%20of%20user_provisioning_jit_provisioning.png)*Habilite a funcionalidade de provisionamento just-in-time na página de integrações do Enterprise*

Todos**usuários recém-registrados** dos domínios que você lista nas configurações serão adicionados automaticamente em seu EnterpriseGuarda-chuva para este time específico quando se inscreverem na Miro.

:::warning
No plano Enterprise, este time também será mostrado na lista de times detectáveis se você habilitara descoberta do time.
:::

### Como definir DisplayName como o nome de usuário padrão

Por padrão, a Miro usará os atributos **FirstName** + **LastName**. Como alternativa, você pode solicitar para usar **DisplayName**. Neste caso, a Miro usará **DisplayName** *quando ele estiver presente* na resposta SAML do usuário.

Se o **DisplayName** não estiver presente, mas **FirstName** + **LastName** estiverem, a Miro usará **FirstName** + **LastName.** Entre em contato com o suporte da Miro para tornar o **DisplayName** seu nome de usuário SSO preferido.

Se nenhum dos três atributos estiver presente na sua comunicação SAML, a Miro mostrará o endereço de e-mail do usuário como Nome de usuário

|  |  |
| --- | --- |
| **Como configurar** | **Nome de usuário padrão** |
| Nome de usuário da Miro | FirstName + LastName |
| Configuração alternativa | DisplayName (se presente na solicitação SAML do usuário) |
| Alternativa | FirstName + LastName (se DisplayName não estiver presente) |
| Nome de usuário SSO preferido | DisplayName ([entre em contato com o suporte da Miro](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)) |
| Nenhum atributo presente | Endereço de e-mail exibido como Nome de usuário |

Se você vir algo diferente do esperado, pode ser necessário autenticar por SSO ou é possível que a resposta SAML não contenha os valores necessários para atualizar.

### Como sincronizar fotos do perfil do usuário a partir do IdP

:::warning
Geralmente é recomendado habilitar esta opção se você não habilitar o SCIM ou seu IdP não oferecer suporte **ao** atributo **ProfilePicture**(por exemplo, ProfilePicture não é compatível com o Azure). Em outros casos, é recomendado passar ProfilePictureporSCIM com atualizações imediatas.
:::

Quando esta opção estiver ativada:

- a imagem do perfil definida no lado do IDP será definida como a imagem do perfil no perfil da Miro do usuário
- os usuários não conseguirãoremover sua imagem do perfil

Como com o atributo de nome de usuário, os usuários não poderão alterar seus dados no lado da Miro imediatamente, mas a *sincronização*de dados não é imediata, o lado IDP envia a atualização para a Miro apenas com a*próxima* autenticação SSO do usuário (desde que a configuração “Sincronizar fotos do perfil do usuário do IDP” ainda esteja ativa nesse ponto).

Se a imagem do perfil estiver definida no IDP e você quiser que o atributo seja examinado na comunicação SAML, a Miro esperará o seguinte esquema:

```
<saml2:Attribute Name="ProfilePicture" NameFormat="urn:oasis:names:tc:SAML:2.0:attrname-format:uri">
<saml2:AttributeValue
xmlns:xs="http://www.w3.org/2001/XMLSchema"
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">https://images.app.goo.gl/cfdeBqKfDKsap1icxecsaHF
</saml2:AttributeValue>
</saml2:Attribute>
```

## SSO e residência de dados

Se você usar o suporte de [Residência de Dados](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md)da Miro e tiver uma URL dedicada (workspacedomain.miro.com), deverá ajustar a configuração do seu provedor de identidade.

:::note
Para organizações com residência de dados na Austrália e nos Estados Unidos, o login social não está disponível. Para obter mais informações sobre residência de dados, consulte [Residência de dados no Miro](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md).
:::

Para fazer isso, você precisará adicionar seu [ORGANIZATION_ID] ao URL.

Você pode encontrar seu ORGANIZATION_ID no painel da Miro clicando no seu **perfil** no canto superior direito > **Configurações** > é mostrado no URL na barra de endereços.

|  | Valor padrão | Valor em Residência de dados |
| --- | --- | --- |
| **URL de serviço ao consumidor de asserção**(também conhecido como URL de retorno de chamada permitido, URL do ACS personalizado, URL de resposta): | https://miro.com/sso/saml | https://workspace-domain.miro.com/ sso/saml/ORGANIZATION_ID |
| **ID da Entidade**(Identificador, identificador de confiança de terceira parte confiável): https://miro.com/ | https://miro.com/ | https://workspace-domain.miro.com/ ID DA ORGANIZAÇÃO |

## Como configurar a autenticação multifator (2FA) para usuários fora do SSO

A autenticação de dois fatores (2FA) fornece uma camada adicional de segurança. Com a 2FA, os usuários são obrigados a concluir uma etapa extra durante o login para verificar sua identificação. Esta medida adicional garante que somente indivíduos autorizados possam acessar sua assinatura.
Saiba mais em nosso [guia do admin para autenticação de dois fatores](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md).

## Perguntas frequentes e resolução de possíveis problemas

Meus endereços de domínio não são aceitos nas configurações de SSO — mensagem `DomainName está indisponível`.

Por razões de segurança, oferecemos suporte aos domínios de uma organização em *um guarda-chuva da empresa apenas (assinatura Enterprise)*. É possível que seus domínios já estejam configurados em outro plano Business ou [plano Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md), impedindo que você ative o SSO com o domínio desejado. Você pode querer verificá-lo com seus colegas de antemão.

Meu domínio não está aparecendo no menu suspenso de domínios disponíveis.

Primeiro você precisa reivindicar e verificar seus domínios nas [configurações de Domínio Gerenciado](../../canvas-25-admin-features/domain-control/01-domain-control.md).

Precisamos alterar os endereços de e-mail de nossos usuários finais/Alteramos os e-mails de nossos usuários e agora eles não podem acessar seus boards.

Se sua empresa estiver alterando seu nome de domínio e, portanto, os endereços de e-mail dos usuários finais precisarem de uma alteração de suas credenciais de SSO,  [entre em contato com nossa equipe de suporte](https://help.miro.com/hc/requests/new?referer=help-center-article) para obter assistência.

Gostaríamos de usar um gateway separado (por exemplo, MFA, como Duo Dag) para o procedimento SSO.

Você certamente pode fazer isso. A Miro oferecerá suporte à sua solução preferida enquanto ela funcionar em SAML 2.0.

Habilitamos o SSO, mas os dados dos perfis de usuário (nomes, fotos de perfil — se suportado pelo seu IdP) na Miro não são sincronizados com aqueles no IdP.

O nome de usuário da Miro e a imagem do perfil são atualizados após cada autenticação de usuário bem-sucedida *se* SAMLResponse contiver novos valores não vazios. Para mais informações sobre como configurar o nome de usuário da Miro, consulte as configurações avançadas de SSO opcional.

Qual é o processo para alterar provedores de SSO ?

Ao alterar os provedores de SSO , você precisará configurar o novo IDP do zero, como faria na primeira configuração.

Se um ou todos os seus usuários encontrarem um erro ao tentar fazer login na Miro, verifiqueesta lista de erros comuns e como resolvê-los.
