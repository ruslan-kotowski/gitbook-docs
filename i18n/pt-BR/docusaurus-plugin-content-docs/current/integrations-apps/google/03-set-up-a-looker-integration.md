---
title: "Configurar a integra\xE7\xE3o do Looker"
article_id: 25112862440978
translation_id: 25112862440978
locale: pt-br
sidebar_position: 4
created_at: '2025-03-05T14:00:46Z'
updated_at: '2025-06-04T08:30:26Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: looker
---

:::note
Para documentos administrativos abrangentes com detalhes e mais informações sobre a integração Miro + Looker, consulte a [documentação administrativa do Looker](https://docs.google.com/document/d/1AUCQWRwDICLygwVmwSxXpz7RmRivPit0EIKgBMIkT6A/edit?usp=sharing).
:::

Para configurar uma integração do **Looker** com a Miro, você deve registrar o aplicativo OAuth no Looker.

## Pré-requisitos

- Certifique-se de que um **Admin da empresa** tenha aprovado o Looker para a sua organização Miro.

## Registrar aplicativo OAuth no Looker

1. No **Looker Marketplace**, encontre e selecione a **extensão API Explorer**.
2. Selecione **Instalar**.
3. Vá para **Início** > **Aplicações** > **Extensão de API**.
4. Encontre e selecione **Registrar OAuth App**.
5. Selecione **Executar**.
6. Um menu é aberto onde você pode adicionar dados de solicitação.
   Adicione os seguintes valores:
   - **client_guid**: `15609152-a12a-4fa1-b364-337e7896d25d`
   - **corpo**:

   ```
   Texto: {
     "redirect_uri": "https://integrations.miro.com/api/contenthub/public/oauth/callback"
     "nome_exibido": a Miro
     Descrição Integração Miro Looker
     "ativado": true,
     "group_id": ""
   }
   ```
7. Selecione **Entendo que este endpoint da API mudará os dados**.
8. Selecione **Executar**.
9. Uma execução bem-sucedida retorna o corpo com um código de resposta **HTTP 200**.
   - 💡 Se o corpo retornado incluir `"enabled":false`, execute a API de Atualização do App OAuth com os mesmos valores do passo 6.

Você configurou com sucesso uma integração do Looker com a Miro.

## Mais informações

- Veja a [Referência da API Looker](https://developers.looker.com/api/explorer/4.0/methods/Auth/register_oauth_client_app) (Externo).
