---
title: Conectar ao Jira Data Center usando OAuth 2.0
article_id: 25753304280466
translation_id: 26513421903378
locale: pt-br
sidebar_position: 8
created_at: '2025-05-06T09:05:20Z'
updated_at: '2025-05-21T09:27:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Quem pode fazer isso: Admins da empresa com permissões de administrador
    do sistema Jira Quais planos: Enterprise Quais plataformas: Navegador, Desktop'
---

:::note
A conexão com o Jira Data Center usando OAuth 2.0 só é habilitada no nível da organização.
:::

## Pré-requisitos

- Você deve ter as seguintes permissões:
  - Permissões de administrador do sistema Jira
  - Função de Admin da empresa da Miro
- Crie um link de aplicativo OAuth 2.0 no Jira Data Center. Para saber como, consulte (Externo) [Suporte para aplicações Atlassian Jira](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Create%20an%20incoming%20link%20using%20application%20links).
  - Quando solicitado, use o seguinte URL de redirecionamento:
    https://integrations.miro.com/api/external-auth/oauth2/callback
  - Para usar webhooks automáticos, certifique-se de selecionar **admin** para seu escopo.

## Conectar a Miro ao Jira Data Center usando OAuth 2.0

1. No seu painel da Miro, selecione seu avatar no canto superior direito e vá para (Enterprise) **console de admin**, ou(Starter e Business) **Configurações**.
2. Na barra lateral esquerda, vá para **Aplicativos e integrações ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Aplicativos** > guia **Gerenciar aplicativos** .
3. Certifique-se de que **Permitir apenas aplicativos da lista abaixo** esteja habilitada.
4. Na coluna **Aplicativo**, para **cartões do Jira**, selecione **Configurações.**
5. Selecione **Adicionar nova conexão**.
6. Em **Configuração do Jira**, selecione **Jira Data Center**.
7. Em **Método de autenticação**, selecione **OAuth 2.0**.
8. Para **URL do Jira**, insira o URL da sua instância do Jira.
9. (Opcional) Para tornar esta conexão a conexão padrão para todos os times da sua organização, clique em **Definir como padrão**.
10. Insira o **ID do cliente** do Jira.
    **Mais informações**: Veja (externo) [Configurar um link de entrada](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
11. Insira o **segredo do cliente** do Jira.
    **Mais informações**: Veja (externo) [Configurar um link de entrada](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
12. Escolha seu escopo.
    Para usar os webhooks automáticos, escolha **admin** ou **admin do sistema**.
13. (Opcional) Para receber atualizações em tempo real do Jira na Miro, marque **Criar Webhook automaticamente**.
    > ✏️ Se preferir, você pode adicionar o Webhook manualmente em outro momento.
14. Selecione **Conectar**.
    > ✏️ Na primeira vez que um usuário tentar realizar uma ação relacionada ao Jira, ele precisará se autenticar. Não é necessário se autenticar novamente.

## E depois?

Para visualizar e gerenciar suas instâncias conectadas do Jira, vá para **Console de admin** | **Configurações** > **Aplicativos e integrações ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Gerenciar aplicativos**. Na coluna **Aplicativo**, para **cartões do Jira**, selecione **Configurações**.

Para aprender como conectar seus times à instância padrão do Jira, veja [Conectar times da organização às configurações padrão do Jira.](https://help.miro.com/hc/articles/26438407676434)

## Perguntas frequentes

**Ao selecionar Admin como escopo, todos os usuários devem ter privilégios de admin no Jira?**

Não. O escopo de admin indica que esse é o nível máximo de acesso que um usuário pode ter na Miro. Cada usuário tem seu escopo, com base nas permissões que ele tiver no Jira.

**Posso conectar o Jira Data Center ao OAuth 2.0 no nível do time?**

Não, somente no nível da organização.
