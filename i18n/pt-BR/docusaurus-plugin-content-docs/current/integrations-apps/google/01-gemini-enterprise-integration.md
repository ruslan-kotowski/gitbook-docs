---
title: Integração Gemini Enterprise (Beta)
article_id: 32304596526482
translation_id: 32304596526482
locale: pt-br
sidebar_position: 1
created_at: '2026-01-05T10:38:04Z'
updated_at: '2026-02-17T09:38:53Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: 'Quem pode fazer: Admins da empresa Quais planos: Business, Enterprise Quais
    plataformas: Navegador, Desktop'
---

Como Admin da empresa, você pode habilitar e configurar a integração Gemini Enterprise para times em sua organização Miro.

A integração Gemini Enterprise permite conectar o Gemini Enterprise como um recurso de [Conhecimento](../../using-miro/miro-ai/09-knowledge.md) na Miro. Por exemplo, use o Gemini Enterprise para fornecer inteligência empresarial aos Assistentes de IA e fluxos.

Você também pode conectar o Gemini Enterprise ao aplicativo de [chat independente](../../using-miro/miro-ai/09-knowledge.md) na Miro.

Para usar a integração Gemini Enterprise, siga estas etapas:

1. Ativar o aplicativo Gemini Enterprise.
   1. Como Admin da empresa, vá para **Admin Console**.
   2. Vá para **Apps & integrations** > **Apps** > **Add apps**.
   3. Procure e encontre o **Gemini Enterprise**.
      Se você não conseguir encontrar o aplicativo pelo nome, busque pelo seguinte ID do cliente: `2392210303456548729`.
   4. No perfil do aplicativo, selecione se deseja adicionar o aplicativo para **Todos os times em \{Team name\}** ou selecione **Em** **times específicos**.
   5. Clique em **Add**.
2. Configure o aplicativo Gemini Enterprise.
   1. No **Admin Console**, vá para **Apps & integrations** > **Apps**.
   2. Para o Gemini Enterprise, certifique-se de que **Permitido** esteja ativado. Em seguida, clique em **Configurações**.
   3. Adicione os detalhes da configuração do Gemini Enterprise.
      Para saber como encontrar o Project ID, consulte (Externo) [Localizar o Project ID](https://support.google.com/googleapi/answer/7014113?hl=en).
      Para obter o App ID, vá para Gemini Enterprise > Apps e use o valor na coluna ID.
      ![](images/33222239058066_image (2).png)
      *Configure o app Gemini Enterprise para uso na Miro.*

      > ✏️ **Project ID** e **App ID** são obrigatórios. Os outros campos são opcionais.
   4. Clique em **Salvar**.

:::note
Quando um membro do time conecta o Gemini Enterprise como um recurso de [Conhecimento](../../using-miro/miro-ai/09-knowledge.md) pela primeira vez, o membro é solicitado a autenticar. O membro do time deve ter uma licença do Gemini Enterprise.
:::
