---
title: Como configurar o AWS SSO
article_id: 360014798100
translation_id: 360014798100
locale: pt-br
sidebar_position: 4
created_at: '2020-07-01T20:03:44Z'
updated_at: '2025-02-26T11:33:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Disponível para: planos Enterprise e Business** Configurado por: Admins
    da empresa'
---

> *💡 É altamente recomendável configurar o SSO em uma janela separada do modo anônimo do seu navegador.* Dessa forma, você mantém a sessão na janela padrão, permitindo que você desative a autorização SSO caso algo esteja mal configurado.

Se você deseja configurar uma instância de teste antes de habilitar o SSO na produção, solicite-o ao seu executivo de conta ou representante de Vendas . Somente aqueles que configurarem o SSO serão adicionados a esta instância de teste.

> **⚠️ Veja nosso artigo principal sobre SSO** [**aqui**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **para regras, recursos suportados e configuração opcional no Miro .**

## Pré-requisitos

Você precisará do seguinte para configurar o acesso SSO da AWS com o Miro:

1. Acesso ao console do AWS SSO com permissões do IAM para gerenciar aplicativos
2. Permissões de admin em nível de empresa no plano Enterprise ou Business da Miro

## Instruções de configuração

1. Na página Configurar SSO da AWS, adicione um novo aplicativo e procure por **Miro**.  Ao adicionar o aplicativo Miro , o nome de exibição e a descrição podem ser atualizados.
   *![application_catalog.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016120652050_application%20catalog.jpg)
   Catálogo de aplicativos AWS SSO*
2. Faça login no painel do Miro em uma janela diferente do navegador. Recomendamos uma janela anônima separada do navegador.
3. No canto superior direito, clique no ícone do seu perfil e vá para **Configurações**. No painel esquerdo, certifique-se de que a time correta esteja selecionada no menu suspenso no canto superior esquerdo.
4. No painel esquerdo, vá para **Integrações Enterprise** (usuários do plano Business precisam ir para **Segurança**) e ative a opção **Ativar SSO/SAML** . Insira o seguinte valor para **URL de iniciar sessão SAML** do AWS SSO.

![application_configuration_page.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016134037522_application%20configuration%20page.jpg)
*Página de configuração do aplicativo AWS SSO*

5. Baixe o arquivo de metadados SAML do AWS SSO e copie e cole o Certificado X509 na **Chave do Certificado x509**. Sua configuração no Miro agora deve ser semelhante à configuração abaixo.

![Configurações_SSO_Miro.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016134038802_Miro%20SSO%20settings.jpg)
*Configurações do Miro SSO*

6. Na configuração do Miro SSO , insira o nome de domínio do e-mail da sua empresa no valor para **Domínios**. Certifique-se de ter adicionado pelo menos um Domínio da Empresa.
7. Clique em **Salvar** para salvar as alterações.
8. Retorne ao seu aplicativo para o Miro no console da Web do AWS SSO . Em Metadados do aplicativo, verifique se os seguintes valores foram inseridos. Eles devem ser extraídos automaticamente se você pesquisou e adicionou o aplicativo Miro em vez de criar um aplicativo personalizado.
9. |  |  |
   | --- | --- |
   | **Campo** | **Valor** |
   | URL do aplicativo ACS | https://miro.com/sso/saml |
   | Público-alvo do aplicativo SAML | https://miro.com/ |
10. Selecione **Salvar alterações**.
11. [Atribua um usuário](https://docs.aws.amazon.com/singlesignon/latest/userguide/assignuserstoapp.html) ao aplicativo em Usuários atribuídos do aplicativo no console do AWS SSO .

E isso é tudo! Sua configuração de SSO agora está concluída.

Se você também deseja habilitar o provisionamento automático para Miro, confira [este artigo](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

## teste

Use a seção a seguir para verificar a integração do SSO . Antes da verificação, certifique-se de que o usuário que está realizando a verificação esteja desconectado do AWS SSO e do Miro antes de executar as etapas abaixo. Os usuários não poderão fazer login usando SSO , a menos que o usuário exista no seu diretório, seja membro do seu plano Enterprise ou Business no Miro e usuário atribuído ao aplicativo.

### Verificando o SSO iniciado pelo IdP a partir do AWS SSO

1. Acesse o portal do usuário final do AWS SSO usando as credenciais de um usuário atribuído ao aplicativo Miro .
2. Na lista de aplicativos, escolha o aplicativo Miro para iniciar um login no Miro.
3. Se o login for bem-sucedido, você será conectado ao painel do Miro .

### Verificando o SSO iniciado pelo provedor de Serviço do Miro

1. Acesse [https://miro.com/login/](https://Miro.com/login/)e escolha **Entrar com SSO**. Em seguida, insira seu e-mail de trabalho.
2. Você será redirecionado para o portal do AWS SSO , onde digitará as credenciais de um usuário atribuído ao aplicativo no console do AWS SSO .
3. Você será conectado ao painel do Miro se o login for bem-sucedido.

### Alternativamente, você pode testar no Miro

1. Conclua as etapas acima para configurar o SSO.
2. Clique no botão **Testar a configuração de SSO**.
3. Revise os resultados:
   1. Se não houver nenhum problema, uma mensagem de confirmação **de que o teste de configuração do SSO foi bem-sucedido** será exibida.
   2. Se forem encontrados problemas, uma mensagem de confirmação **de falha no teste de configuração do SSO** será exibida, seguida por mensagens de erro detalhadas para orientar você sobre o que precisa ser corrigido.![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)*Teste a configuração SSO do Miro*

## Solução de problemas

Para solução de problemas gerais, consulte o [Guia de solução de problemas do AWS SSO](http://docs.aws.amazon.com/singlesignon/latest/userguide/troubleshooting.html).
