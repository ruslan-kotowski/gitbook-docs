---
title: Como configurar webhooks para o Jira Data Center
article_id: 360017731113
translation_id: 14537528239378
locale: pt-br
sidebar_position: 15
created_at: '2023-10-19T15:31:20Z'
updated_at: '2026-01-14T09:25:32Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Pessoas: Admins de Sistema do Jira Planos: Todos os planos da Miro (para
    integração com Jira Server/Data Center via OAuth 1.0) Plataformas: Navegador,
    aplicativo para desktop (para procedimentos de configuração)'
---

Para garantir que seus [cartões do Jira](https://help.miro.com/hc/articles/360017572434) em um board da Miro fiquem atualizados, a Miro deve receber mensagens do Jira sempre que ocorrerem alterações nos dados. Esses eventos do Jira são transmitidos para a Miro via um Webhook.

Este guia fornece duas maneiras de criar Webhooks para Jira Server e Jira Data Center usando OAuth 1.0 e OAuth2.0.

## Criar um Webhook automaticamente

Ao [configurar a integração dos seus cartões do Jira](https://help.miro.com/hc/articles/360019501754), se você estiver conectando ao Jira Server ou Jira Data Center, pode deixar ativa a opção **Criar um webhook automaticamente**. Este é o método recomendado.

:::note
A criação automática do webhook requer que você esteja logado no Jira como admin do sistema Jira.
:::

![jira-webhooks-server-config.png](../../../../../../docs/integrations-apps/atlassian/images/21304245707026_jira-webhooks-server-config.png)
*Configurações dos cartões do Jira, Passo 2: "Criar um webhook automaticamente**"** está ativada*

Depois que o webhook for criado automaticamente, é uma boa prática acessar a página de WebHooks do Jira e editar o webhook para dar a ele um nome único. Isso é especialmente importante se você planeja conectar vários times Miro à sua instância do Jira.

:::note
Para conexões OAuth2.0, a conexão do lado da Miro é configurada no nível da empresa. Um webhook é criado para todos os times Miro.
:::

:::note
Para conexões OAuth 1.0 no nível de time Miro, um webhook é criado por time. No nível da empresa Miro, um único webhook é criado para todos os times.
:::

## Criar um webhook manualmente

Se você preferir ou precisar criar o webhook manualmente, siga estas etapas.

**Obtenha a URL do webhook na Miro**

1. Nas configurações de Cartões do Jira na Miro (Passo 2, ao conectar ao Jira Server/Data Center), desmarque a opção para **Criar um webhook automaticamente**.
2. Copie e cole o **URL do Jira** da sua organização e clique em **Conectar e salvar configurações.**
   ![jira-webhooks-configure-jira-url-cropped.png](../../../../../../docs/integrations-apps/atlassian/images/21304245708818_jira-webhooks-configure-jira-url-cropped.png)
   *Configurações do Cartão do Jira, Passo 2: "Criar um webhook automaticamente" está desabilitado*
3. Permita que a integração se conecte ao Jira quando solicitado.
4. Após esses passos, a Miro fornecerá o **URL do Webhook**:
   ![webhook_URL.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016928565010_webhook%20URL.jpg)*URL do Webhook fornecido pela Miro*

:::note
Caso você não seja um admin do Jira, por favor, copie o **URL do Webhook** fornecido pela Miro e envie para o admin do Jira da sua organização para que ele possa criar o webhook no Jira usando as instruções abaixo.
:::

**Crie o webhook no Jira**

Abaixo estão os passos para criar um Webhook no Jira usando a URL obtida na Miro. Você também pode se referir à documentação oficial da Atlassian para o [Jira Server](https://developer.atlassian.com/server/jira/platform/webhooks/) e para a [Jira Cloud](https://developer.atlassian.com/cloud/jira/platform/webhooks/) (embora este artigo se concentre no Server/Data Center).

1. Para acessar a página de **WebHooks** no Jira, vá até **Administração do Jira** > **Sistema** > **Avançado >** **WebHooks** (o caminho exato pode variar ligeiramente dependendo da versão do Jira que você estiver usando). Alternativamente, você também pode usar um link direto anexando `/plugins/servlet/webhooks` à URL da sua instância do Jira (por exemplo, `https://NomeDaSuaInstanciaJira/plugins/servlet/webhooks`).
2. Clique em **Criar um WebHook** no canto superior direito da página de WebHooks.
3. Insira um **Nome** descritivo para o WebHook (por exemplo, "Webhook de Integração Miro").
4. Defina o status do WebHook como **Ativado**.
5. Cole a **URL do Webhook** copiada das configurações do Miro no campo URL.
   ![system_webhooks.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941532050_system%20webhooks.jpg)
   *Configuração de Webhooks do sistema no Jira*
6. Na seção **Eventos**, em **Questão**, selecione os eventos **atualizado** e **excluído**.
7. Clique em **Criar** para salvar o webhook.
   ![Jira_Webhook_settings.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941533074_Jira%20Webhook%20settings.jpg)
   *Configurações de evento do Webhook do Jira*
8. Após o webhook ser criado no Jira, volte para o **Passo 2** nas configurações do cartão do Jira na Miro, certifique-se de que sua **URL do Jira** está preenchida corretamente e clique em **Conectar**.

Agora o webhook está criado e configurado. Os cartões do Jira em seus boards na Miro serão atualizados automaticamente quando houver mudanças no Jira.
