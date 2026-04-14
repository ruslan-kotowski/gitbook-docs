---
title: Como configurar o OneLogin SSO
article_id: 360022547134
translation_id: 360022547134
locale: pt-br
sidebar_position: 8
created_at: '2019-05-07T13:32:16Z'
updated_at: '2025-02-26T11:22:04Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Disponível para: planos Enterprise e Business** Configurado por: Admins
    da empresa'
---

> *💡 É altamente recomendável configurar o SSO em uma janela separada do modo anônimo do seu navegador.* Dessa forma, você mantém a sessão na janela padrão, permitindo que você desative a autorização SSO caso algo esteja mal configurado.

Se você deseja configurar uma instância de teste antes de habilitar o SSO na produção, solicite-o ao seu executivo de conta ou representante de Vendas . Somente aqueles que configurarem o SSO serão adicionados a esta instância de teste.

> **⚠️ Veja nosso artigo principal sobre SSO** [**aqui**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **para regras, recursos suportados e configuração opcional no Miro .**

## Configurando o Onelogin

### Adicionando e configurando o aplicativo

A configuração do OneLogin no Miro é simples, pois o OneLogin tem um aplicativo Miro funcional pré-configurado no catálogo **de aplicativos** .

![Miro_em_OneLogin_apps.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017429898130_Miro%20in%20OneLogin%20apps.jpg)
*Miro no catálogo de aplicativos OneLogin*

Clique no botão **Salvar** .

![botão_salvar.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017429899538_save%20button.jpg)
*Guia de configuração do aplicativo no OneLogin*

## Configurando o Miro

Após salvar a configuração, você será direcionado diretamente para as configurações do aplicativo. Mude para a aba **SSO** para obter seu **URL de login** e **certificado x509**.

![sso_tab.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017416854674_sso%20tab.jpg)
*Guia SSO*

Abaixo você verá uma lista de URLs. Copiar URL **do ponto de extremidade SAML 2.0 (HTTP)** :

![Ponto de extremidade SAML.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017416855698_SAML%20endpoint.jpg)

e ***cole-*** o **no campo URL de login SAML** do Miro :

![URL_de_entrada.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017429902354_sign-in%20URL.jpg)
*Campo **de URL de login** do Miro SAML*

Volte para a guia SSO do aplicativo OneLogin e clique em **Exibir detalhes** para copiar o **certificado x509**.

![ver_detalhes.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017416856722_view%20details.jpg)
*Botão Ver detalhes*

![copy_certificate.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017429903634_copy%20certificate.jpg)
*Copiando **certificado x509***

Cole o certificado no campo Certificado Miro **x509** .

![certificado_em_configurações_SSO_Miro.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016928761746_certificate%20in%20Miro%20SSO%20settings.jpg)
*Campo de **certificado x509** nas configurações do Miro SSO*

Como etapa final das configurações do Miro , adicione seus domínios e [verifique-os](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Você também pode configurar [as configurações opcionais](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

Está tudo pronto e agora seus usuários poderão se autenticar no Miro via SSO!

Se você encontrar algum problema, por favor, verifique [nossa lista de casos comuns e como resolvê-los.](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)

## Testando a configuração do SSO no Miro

1. Conclua as etapas acima para configurar o SSO.
2. Clique no botão **Testar a configuração de SSO**.
3. Revise os resultados:

- Se não houver nenhum problema, uma mensagem de confirmação **de que o teste de configuração do SSO foi bem-sucedido** será exibida.
- Se forem encontrados problemas, uma mensagem de confirmação **de falha no teste de configuração do SSO** será exibida, seguida por mensagens de erro detalhadas para orientar você sobre o que precisa ser corrigido.

![teste-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Testando a configuração do SSO no Miro*
