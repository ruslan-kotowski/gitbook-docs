---
title: Como configurar o Google SSO
article_id: 4716499382546
translation_id: 4716499382546
locale: pt-br
sidebar_position: 6
created_at: '2022-03-18T18:12:44Z'
updated_at: '2025-11-25T16:08:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponível para: plano Business, Enterprise Configurado por: Admins da empresa'
---

:::tip
É altamente recomendável configurar o SSO em uma janela separada do modo anônimo do seu navegador. Dessa forma, você mantém a sessão na janela padrão, permitindo que você desative a autorização SSO caso algo esteja mal configurado.
:::

Configurar o Miro na sua organização está mais fácil do que nunca com o aplicativo de integração que o Google criou dentro do Console de admin do Google Workspace. Este aplicativo permite que você configure o Google SSO para uso com o Miro, bem como [o provisionamento de usuário do SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md).

Este artigo se concentra na configuração do Google SSO para uso com o Miro.

Se você deseja configurar uma instância de teste antes de habilitar o SSO na produção, solicite-o ao seu executivo de conta ou representante de Vendas . Somente aqueles que configurarem o SSO serão adicionados a esta instância de teste.

:::tip
Consulte o [SSO](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)  Miro SSO para obter regras, recursos suportados e configurações opcionais.
:::

Leia mais sobre [como configurar o Google SSO com o Miro](https://support.google.com/a/answer/14100608#zippy=%2Cstep-set-up-google-as-saml-identity-provider) na Central de ajuda do Google.

## Configurando o Google SSO para Miro usando SAML

A configuração do Google SSO para autenticação no Miro pode ser concluída em quatro etapas:

1. Configurando o Google como provedor de identidade SAML
2. Configurando o Miro como provedor de serviços SAML
3. Ativando o Miro para usuários
4. Testando autenticação

Configurando o Google como provedor de identidade SAML

1. No Console de admin do Google Workspace, clique em **Aplicativos > Aplicativos da Web e móveis**
2. No painel Aplicativos, clique no menu suspenso **Adicionar aplicativo** , escolha “Pesquisar aplicativos” e digite “Miro”
3. Escolha “Miro Web (SAML)” e clique em **Selecionar**
4. Em “Detalhes do Provedor de Identidade do Google”, na Opção 2, verifique se “URL SSO ”, “ID da entidade” e “Certificado” estão todos preenchidos e clique em **Continuar.** Você copiará esses valores mais tarde ao configurar o Miro
5. Em “Detalhes do provedor de Serviço ”, adicione os seguintes valores:
   **URL do ACS:** https://miro.com/sso/saml
   **ID da entidade:** https://miro.com
   **URL inicial:** em branco
   **Resposta assinada:** deixar desmarcado
   **Nome ID: E-MAIL**
6. Clique **em Continuar**
7. Em “Mapeamento de atributos” em “Atributos do diretório do Google”, escolha **Nome**e, em seguida, **Sobrenome**, certificando-se de que eles mapeiam para os atributos do aplicativo
8. Clique em **Concluir**. Agora você verá seu aplicativo da Miro adicionado ao Google Workspace
   ![google_sso_configuring_google_settings.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017515989394_google_sso_configuring_google_settings.gif)*Configurando o provedor de identidade SAML do Google*

Configurando o Miro como provedor de serviços SAML

1. Abra uma aba anônima no seu navegador e faça login no painel do Miro (miro.com/app/ painel)
2. Clique no seu avatar no canto superior direito e clique em **Configurações**
3. Nas configurações da sua empresa, clique em **Autenticação.** Se você for um cliente do plano Business , essa configuração estará em **Segurança**.
4. Clique no botão de alternância para “Ativar SSO para configurar o provisionamento SCIM”
5. Você será levado para a seção Autenticação das configurações da empresa. Clique no botão de alternância **SSO/SAML** . Você será solicitado a clicar em **Ativar** para habilitar o SSO para sua organização
6. Para o **URL de iniciar sessão SAML**, volte ao Console de admin do Google Workspace e, no aplicativo da Miro, clique em **BAIXAR METADADOS.** Este painel oferece a opção de copiar os valores necessários
7. Em **URL do SSO**, clique no botão **Copiar** . Volte para o Miro e cole o valor em **URL de iniciar sessão SAML**
8. Repita este processo para **o Certificado Key x.509** usando o Certificado no Google
9. Adicione as informações do seu **domínio** . Certifique-se de que você já [configurou e verificou seu domínio](../../canvas-25-admin-features/domain-control/01-domain-control.md)
10. Clique em **Salvar![google_sso_configurando_miro_authentication.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017515990802_google_sso_configuring_miro_authentication.png)***Configurando as definições de autenticação SSO no Miro*

Ativando o Miro para usuários

1. Retornar ao Console de admin do Google Workspace
2. Se necessário, clique em **Aplicativos da Web e móveis** no menu Aplicativos e selecione **Miro**
3. Clique em **Acesso do usuário**
4. Clique em **ON para todos** e clique em **Salvar![google_sso_ligando_miro.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528995474_google_sso_turning_on_miro.gif)***Ativando o aplicativo da Miro para todos os usuários*

Se você quiser ativar o Miro para unidades organizacionais específicas, clique primeiro no grupo em Unidades Organizacionais e depois clique em **SOBRE.** Pode ser necessário clicar **em SUBSTITUIR** ou **HERDAR** adicionalmente.

Testando autenticação

1. No Console de admin do Google Workspace, inicie o aplicativo da Miro , se necessário
2. Na seção Miro , clique em **TESTAR LOGIN SAML**
3. Uma nova guia deve aparecer com as opções de login do Google SSO
   .GIF
4. Para testar a autenticação no Miro , abra uma nova aba anônima e inicie o painel do Miro (miro.com/app/ painel)
5. Você deverá ver uma página de login. Clique em **Entrar com Login Único** e faça login com as credenciais da sua conta.
   ![google_sso_testing_authentication.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528996882_google_sso_testing_authentication.gif)*Testando a autenticação SSO do Google com o Miro*

Alternativamente, você pode testar no Miro:

1. Conclua as etapas acima para configurar o SSO.
2. Clique no botão **Testar a configuração de SSO**.
3. Revise os resultados:
   1. Se não houver nenhum problema, uma mensagem de confirmação **de que o teste de configuração do SSO foi bem-sucedido** será exibida.
   2. Se forem encontrados problemas, uma mensagem de confirmação **de falha no teste de configuração do SSO** será exibida, seguida por mensagens de erro detalhadas para orientar você sobre o que precisa ser corrigido.![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)*Teste a configuração SSO do Miro*

> **⚠️** Se você já configurou o SSO para sua organização e precisa reconfigurá-lo, é altamente recomendável **desativar** o SSO no Miro antes de continuar no Google admin Console; caso contrário, você poderá ficar bloqueado do Miro. Para evitar um bloqueio, crie um usuário 'quebre o vidro' com um e-mail com um domínio fora do domínio listado nas configurações de SSO , como acmebreaktheglass@gmail.com. Caso contrário, você pode entrar em contato com o suporte e eles podem desabilitar o SSO para toda a organização.

Se você quiser configurar o provisionamento de usuário com o Google, as instruções podem ser encontradas no artigo “[Configurando o provisionamento automatizado com o Google](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md)”.
