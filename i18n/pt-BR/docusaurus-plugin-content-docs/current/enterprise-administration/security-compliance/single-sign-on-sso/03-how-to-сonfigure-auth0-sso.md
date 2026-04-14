---
title: Como configurar o Auth0 SSO
article_id: 360022496573
translation_id: 360022496573
locale: pt-br
sidebar_position: 3
created_at: '2019-05-01T18:33:32Z'
updated_at: '2025-02-26T11:43:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponível para: plano Business, Enterprise Configurado por: Admins da empresa'
---

*É altamente recomendável configurar o recurso em uma janela separada do modo anônimo do seu navegador.* *Dessa forma, você mantém a sessão na janela padrão, permitindo que você desligue a autorização SSO caso algo esteja configurado incorretamente.*

Se você deseja configurar uma instância de teste antes de habilitar o SSO na produção, solicite-o ao seu executivo de conta ou representante de Vendas da Miro . Somente aqueles que configurarem o SSO serão adicionados a esta instância de teste.

## Criando o aplicativo Miro dentro do seu locatário

1. Crie o aplicativo na sua lista **de aplicativos** .
   ![criar_botão_de_aplicação.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017725476370_create%20application%20button.jpg)
   *Seção de aplicativos Auth0*
2. Selecione o tipo de aplicativo **Aplicativos Web regulares** .
   ![lista_de_tipos_de_aplicativos.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017695804818_application%20types%20list.jpg)
   *Lista de tipos de aplicação*
3. Vá até a aba **Configurações** e certifique-se de que as opções listadas estejam selecionadas exatamente como descrito abaixo.
   ![mceclip0.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017725482002_mceclip0.png)


   |  |  |
   | --- | --- |
   | **Método de autenticação de ponto final de token** | PUBLICAR |
   | **URLs de retorno de chamada permitidas** | https://miro.com/sso/saml |
   | **URI de login do aplicativo** | https://miro.com/sso/saml |
   | **Origens permitidas (CORS)** | https://miro.com/ |
   | **Expiração do JWT** | 36000 (Definido por padrão) |
4. Clique em **Mostrar configurações avançadas:**
   ![mceclip1.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017725485074_mceclip1.png)

   e então vá para **Certificados** e Copie seu Certificado de Assinatura x509:
   ![copy_the_certificate.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017695807634_copy%20the%20certificate.jpg)
   *Guia Configurações avançadas no Auth0*
5. Mude para o Miro e abra suas configurações de SSO ( admins do plano Business encontrarão as configurações na aba **Segurança** , admins do plano Enterprise precisarão ir para a aba **Integrações Enterprise** ) e então cole o **Certificado de Assinatura x509** no campo respectivo, conforme mostrado na captura de tela abaixo:
   ![certificado_em_configurações_SSO_Miro.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928761746_certificate%20in%20Miro%20SSO%20settings.jpg)
   *Guia **de segurança** do Miro com configurações SAML*

## Configurando SAML para o aplicativo

1. Volte para a página de configuração do aplicativo Auth0 e escolha a aba **Addons** e o addon **SAML2** :
   ![add-ons_catalog.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017725489682_add-ons%20catalog.jpg)
   *Catálogo de complementos do Auth0*Você verá uma janela pop-up com as configurações da solicitação e **URL de retorno de chamada do aplicativo:
   ![configurações_add-on.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017725490962_add-on%20settings.jpg)***Aba **Configurações** do Addon*
2. Certifique-se de que o **URL** esteja definido como **`https://miro.com/sso/saml`**As **configurações** da solicitação devem ser definidas como o seguinte:

   ```
    "nameIdentifierFormat": "urna:oasis:nomes:tc:SAML:1.1:formato-nameid:endereço-de-email",
    "nomeIdentificadorProbes": [
    "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress"
   ```
3. Mude as guias para **Uso**e copie o**URL de login do provedor de identidade:**![](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017695812626_mceclip2.png)mceclip2.png
   *Campo URL de login do provedor de identidade no Auth0*
4. Mude para o Miro novamente e cole a URL no campo**URL de iniciar sessão do SAML** .
5. Clique em **Salvar** para que as configurações sejam aplicadas ao seu plano Miro .

## Verificando a configuração

Agora você pode retornar ao console do Auth0 e retornar à aba **Configurações** do complemento. Clique em **Depurar** para acionar a tentativa de login.

![depurar.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017695814290_debug.jpg)
*Acionando a tentativa de login*

Isso iniciará a tentativa de login do IdP e permitirá que você veja os resultados.

Em caso de dificuldades, sinta-se à gratuita para [entrar em contato com nossa Team de Suporte](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).

## Testando a configuração do SSO no Miro

1. Conclua as etapas acima para configurar o SSO.
2. Clique no botão **Testar a configuração de SSO**.
3. Revise os resultados:

- Se não houver nenhum problema, uma mensagem de confirmação **de que o teste de configuração do SSO foi bem-sucedido** será exibida.
- Se forem encontrados problemas, uma mensagem de confirmação **de falha no teste de configuração do SSO** será exibida, seguida por mensagens de erro detalhadas para orientar você sobre o que precisa ser corrigido.

![teste-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Testando a configuração do SSO no Miro*
