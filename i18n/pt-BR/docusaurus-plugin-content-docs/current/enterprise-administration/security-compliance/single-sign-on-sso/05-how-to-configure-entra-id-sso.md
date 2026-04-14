---
title: Como configurar logon único no Entra ID
article_id: 360022722233
translation_id: 360022722233
locale: pt-br
sidebar_position: 5
created_at: '2019-05-07T12:03:08Z'
updated_at: '2025-11-25T16:04:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponível para: planos Business e Enterprise Função necessária: Admins
    da empresa'
---

> *💡 É altamente recomendável configurar o logon único em uma janela de modo anônimo separada do seu navegador.* Dessa forma, você mantém a sessão na janela padrão, permitindo que você desligue a autorização de logon único caso algo esteja configurado incorretamente.

Se você quiser configurar uma instância de teste antes de ativar o logon único na produção, por favor [entre em contato com a equipe de Suporte](https://help.miro.com/hc/requests/new?referer=help-center-article) para assistência. Somente aqueles que configurarem o logon único serão adicionados a essa instância de teste.

> **⚠️ Veja nosso artigo principal sobre logon único** [**aqui**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **para regras, funcionalidades suportadas e configuração opcional no final da Miro.**

## Adicionando e configurando o aplicativo

 1. Encontre o aplicativo pré-configurado da Miro na Galeria de Aplicativos Empresariais do Entra ID ([Aplicativos Empresariais](https://portal.Entra.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/) > +Novo Aplicativo).

2. Crie o aplicativo e clique em **2.** **Configurar logon único** (ou selecione **Logon único** no menu à esquerda e selecione o método de entrada **SAML**).

3. Você verá que a **Configuração SAML Básica** já está em vigor:

:::warning
se depois de tudo configurado o logon único falhar, tente alterar o ID da entidade de `https://miro.com`para `https://miro.com/`
:::

:::warning
As URLs de login, estado de retransmissão e de logout (para logout único) devem ser deixadas em branco, pois essas funcionalidades não são compatíveis.
:::

Os **atributos e declarações** também já estão implementados:

:::warning
Observe que:
a) o UPN se tornará o principal parâmetro pelo qual um usuário na Miro será reconhecido e esse parâmetro não poderá ser atualizado do lado da Entra. Quando você precisar atualizar os e-mails de usuários na Miro sem usar o SCIM, por favor, [entre em contato com nossa equipe de suporte](https://help.miro.com/hc/requests/new?referer=help-center-article).
b) A Miro aceitará [**GivenName (nome próprio),** **Surname (sobrenome)**, **DisplayName (nome de exibição)** e **ProfilePicture (foto de perfil)**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Outros atributos não são compatíveis via logon único, mas podem ser transferidos via [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).
:::

### Criando o Certificado

1. No Microsoft Entra, certifique-se de que o **Certificado de Assinatura SAML** > **Opção de Assinatura** seja ou **Assinar Declaração SAML** ou **Assinar resposta e declaração SAML**.

2. **Baixe** o arquivo **Base64**.

## Configurando logon único no seu plano da Miro

1. Abra o arquivo **Base64** baixado em um editor de texto e, em seguida, copie o certificado **x509** do arquivo.

2. Na Miro, em **Segurança > Autenticação**, cole o certificado **x509** copiado na caixa **Certificado de chave x509**.

3. Na interface de configurações do Microsoft Entra, copie o **URL de login**, e depois vá para a página **Segurança > Autenticação** da Miro e cole-o na caixa **URL de login por SAML**.

4. Na página **Segurança >**  **Autenticação** da Miro, na seção **Usuários desses domínios irão acessar usando logon único**, certifique-se de adicionar pelo menos um domínio da empresa.

:::warning
Na Miro, certifique-se de que a opção **Sincronizar fotos de perfil a partir do IdP** não esteja marcada. O Entra ID não suporta a sincronização de fotos de perfil de usuário. Quando a opção **Sincronizar fotos de perfil a partir do IdP** não está marcada, os usuários podem definir suas próprias fotos de perfil.
:::

4. Clique em **Salvar**.

Sua configuração de SSO está agora completa.

## Configurando as declarações quando UPN e e-mail diferem

Você pode configurar as configurações para usar qualquer atributo do Entra que esteja no formato de e-mail como **NameID** na Miro.

#### **Logins iniciados por IDP e SP**

*Para login iniciado pelo IDP*, o Entra envia à Miro o valor que você decidir usar como **NameID** (**user.mail** no exemplo abaixo).

Com esse fluxo, seus usuários finais acessam a Miro por meio do ícone em seu console do portal (por exemplo, em `https://myapplications.microsoft.com/`). De lá, uma solicitação é enviada para a Miro e *o usuário é autenticado usando o **NameID** que você definiu.*A Miro esperará que este atributo corresponda ao **e-mail** do usuário na Miro. Uma incompatibilidade resultará em falha na autenticação.

*Para login iniciado pelo SP*, a Miro enviará uma solicitação especificamente para o **UPN** do usuário e esperará que ele corresponda ao **e-mail** do usuário na Miro. Uma incompatibilidade resultará em falha na autenticação.

Agora, espera-se que o campo **URL de login por SAML** nas suas configurações da Miro contenha o **URL de login** do aplicativo da Miro da sua instância do Entra. Este será o URL para o qual a Miro direcionará o usuário a partir da [página de login da Miro](https://miro.com/sso/login/).

Quando o usuário é direcionado para o URL de login a partir do aplicativo, a solicitação SAML é gerada. Com esse fluxo, o usuário faz login com o endereço de e-mail que ele inseriu na página de login da Miro e que a Miro então solicita à Entra, exigindo que seja o atributo UPN.

#### **Como configurar**

Para permitir que seus usuários acessem a Miro com o **e-mail** do Entra, em vez de com o **UPN**, você pode preencher o campo **URL de Login por SAML** na Miro com o URL do aplicativo a partir do console do Entra. Então, o fluxo iniciado pelo SP será o seguinte:

1. O usuário acessa a Miro inserindo seu e-mail da Miro, que é o e-mail que ele tem na Miro. A Miro entende que a pessoa deve estar conectada ao perfil de usuário definido.
2. O usuário é direcionado para o link do aplicativo usado para o login iniciado pelo IDP.
3. O link utiliza o **atributo NameID** *que você definiu* e o envia para a Miro.
4. O usuário, portanto, faz login na Miro no perfil de usuário definido anteriormente com o **NameID** que você definiu.

Se você também quiser ativar o provisionamento automático para a Miro, confira [este artigo](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

Se você encontrar qualquer problema durante a configuração, confira [este artigo](../../../using-miro/tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## Ferramenta de teste Entra

Para acessar a ferramenta de teste, escolha a guia **Iniciar Sessão** nas configurações do seu aplicativo e role até o final da seção.

A Entra sugere usar o processo de login de teste para verificar a conexão e solucionar uma mensagem de erro. Após o teste, você receberá instruções sobre como resolver a situação.

Por favor, lembre-se de quais credenciais gerenciadas pela Entra/ADFS sua estação de trabalho está autenticada. Se você estiver tentando usar um conjunto diferente para fazer login na Miro, a tentativa de login pode falhar, pois o provedor de identidade transferirá seu conjunto principal de credenciais e haverá uma incompatibilidade. Por exemplo, isso pode acontecer se você for o admin do logon único e testar o procedimento de login com credenciais de usuário diferentes.

## Como alternativa, você pode testar na Miro

1. Conclua as etapas acima para configurar as suas configurações de logon único.
2. Clique no botão **Testar a configuração de logon único**.
3. Revise os resultados:
   1. Se não houver nenhum problema, uma mensagem de confirmação **de que o teste de configuração do logon único foi bem-sucedido** será exibida.
   2. Se forem encontrados problemas, uma mensagem de confirmação **de falha no teste de configuração do logon único** será exibida, seguida por mensagens de erro detalhadas para orientar você sobre o que precisa ser corrigido.

##
