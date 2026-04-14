---
title: Como configurar o OKTA SSO
article_id: 360023901054
translation_id: 360023901054
locale: pt-br
sidebar_position: 7
created_at: '2019-05-31T11:32:41Z'
updated_at: '2025-11-25T16:05:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Disponível para: planos Enterprise e Business** Configurado por: Admins
    da empresa'
---

> *💡 É altamente recomendável configurar o SSO em uma janela separada do modo anônimo do seu navegador.* Dessa forma, você mantém a sessão na janela padrão, permitindo que você desative a autorização SSO caso algo esteja mal configurado.

[Se você quiser configurar uma instância de teste antes de ativar o SSO na produção, entre em contato com a equipe de suporte para assistência.](https://help.miro.com/hc/requests/new?referer=help-center-article) Somente aqueles que configurarem o SSO serão adicionados a esta instância de teste.

> **⚠️ Veja nosso artigo principal sobre SSO** [**aqui**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **para regras, recursos suportados e configuração opcional no Miro .**

## Configurando o Okta

### Adicionando e configurando o aplicativo

Clique na aba **Aplicativos** e escolha **Catálogo de Aplicativos do Navegador**:

![procurar_catálogo_de_aplicativos.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928758930_browse%20app%20catalog.jpg)
*Seção de aplicativos no Okta*

Encontre nosso aplicativo pré-configurado para fácil configuração e clique em **Adicionar** :

![Miro_pre-configured_app.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928759570_Miro%20pre-configured%20app.jpg)
*Miro no catálogo do aplicativo Okta*

Dê ao aplicativo na sua galeria o etiqueta que você preferir (outras etapas são opcionais) e clique em **Avançar** para alternar para a guia **Opções de logon** :

![configurações_gerais.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928760466_general%20settings.jpg)
*Configurações gerais do aplicativo Miro*

Nas **Opções de Login,** todos os valores esperados já estão preenchidos e nenhum dado adicional é necessário.

:::warning
Você pode adicionar valores personalizados se preferir, mas certifique-se de que o **Estado de retransmissão padrão** seja mantido *vazio*: nossos aplicativos autônomos empregam redirecionamento para o navegador do usuário final durante o procedimento de autenticação e geram valores de RelayState exclusivos para isso. Se você usar um valor Padrão, o Okta substituirá nossos dados e seus usuários só poderão acessar a versão do navegador do Miro, mas não nenhum aplicativo independente (desktop, tablet, celular).
:::

![opções_de_sinalização.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016941715730_sign-on%20options.jpg)
*Métodos de login*

Clique para **finalizar**. Você poderá voltar e editar quaisquer campos mais tarde, se necessário.

### Formato do nome de usuário

:::tip
O **formato de nome de usuário do aplicativo** é definido por padrão como **Nome de usuário Okta,** o que é aceitável se seu nome de usuário estiver no formato de e-mail. Como alternativa, defina o nome de usuário como **e-mail.**
:::

:::warning
O e-mail é o ID principal pelo qual o usuário é reconhecido no Miro e não deve ser atualizado no Okta, a menos que você tenha o SCIM habilitado. Se você não usa o SCIM, mas precisa atualizar os endereços dos seus usuários finais, entre em contato com nossa [time de Suporte](https://help.miro.com/hc/requests/new?).
:::

### Configurando fotos de perfil (opcional)

Configurar um atributo personalizado como ProfilePicture pode ser considerado um processo separado. Siga este [guia](https://drive.google.com/file/d/1go4BJWzFpQS5R04WdN1Q4O5Dy93k4wGp/view) para configurar o atributo no Okta e, em seguida, [habilitar o requisito ProfilePicture](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) no Miro .

## Configurando o Miro

Role para baixo até **Certificados de assinatura SAML** para obter os metadados do IDP. Se você não tiver nenhum certificado emitido, primeiro crie um.

Depois disso, clique em **Ações** e escolha **Exibir metadados do IdP** , assim:

![view_Idp_metadata.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928761234_view%20Idp%20metadata.jpg)
*Obtendo os metadados do IdP*

Você será direcionado para uma aba separada que contém todas as informações. Copie o certificado da linha que começa com &lt;ds:X509Certificate&gt; e cole-o nas configurações do Miro SSO em Campo**Certificado x509** .

![certificado_em_configurações_SSO_Miro.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928761746_certificate%20in%20Miro%20SSO%20settings.jpg)
*Certificado chave x509 nas configurações do Miro SSO*

Volte para a página de metadados e copie a URL da linha**SingleSignOnService**após**Location=**e cole-a em **SAML iniciar sessão-in URL**.

Está tudo pronto!

Como etapa final das configurações do Miro , adicione seus domínios e [verifique-os](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Você também pode configurar [as configurações opcionais](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

Se você encontrar algum problema, por favor, verifique [nossa lista de casos comuns e como resolvê-los.](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)

## Testando a configuração do SSO no Miro

1. Conclua as etapas acima para configurar o SSO.
2. Clique no botão **Testar a configuração de SSO**.
3. Revise os resultados:

- Se não houver nenhum problema, uma mensagem de confirmação **de que o teste de configuração do SSO foi bem-sucedido** será exibida.
- Se forem encontrados problemas, uma mensagem de confirmação **de falha no teste de configuração do SSO** será exibida, seguida por mensagens de erro detalhadas para orientar você sobre o que precisa ser corrigido.

![teste-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Testando a configuração do SSO no Miro*
