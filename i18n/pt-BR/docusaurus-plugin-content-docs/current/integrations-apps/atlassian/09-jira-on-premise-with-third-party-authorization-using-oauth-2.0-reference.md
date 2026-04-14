---
title: Jira on-premise com autorização de terceiros usando uma referência OAuth 2.0
article_id: 26726425696530
translation_id: 26751178919186
locale: pt-br
sidebar_position: 11
created_at: '2025-05-16T09:09:32Z'
updated_at: '2025-11-25T15:51:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Quem pode fazer isso: Admins da empresa Quais planos: Enterprise'
---

Este artigo fornece detalhes técnicos para usar um servidor de autorização de terceiros com OAuth 2.0 para integrar o Jira com a Miro.

Para saber como configurar uma conexão, consulte [Conectar ao Jira on-premise com servidores de autorização de terceiros usando OAuth 2.0](https://help.miro.com/hc/articles/25692796700306).

## Como a integração do Jira com a Miro funciona usando autorização local e OAuth 2.0

O gráfico a seguir mostra o fluxo de comunicação entre a Miro e um servidor de autorização Jira local.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Integração da Miro com o Jira usando um servidor de autorização on-premise via um gateway de API*

## Parâmetros de configuração

Para configurar o fluxo de autorização entre a Miro e o Jira usando um servidor de autorização de terceiros com OAuth 2.0, você deve especificar os seguintes parâmetros:

- **Servidor de autorização**
  - URL de solicitação de autorização
  - URL de solicitação de token
  - Escopo
- **Configuração do aplicativo de autorização**
  - ID do cliente
  - Segredo do cliente
- **Instância do Jira**
  - URL pública do Jira
  - URL base do Jira; URL interna

:::note
A Miro fornece a URL de redirecionamento que o servidor de autorização valida em relação ao aplicativo registrado.
:::

**Mais informações:** Veja [Conectar ao Jira on-premise com servidores de autorização de terceiros usando OAuth 2.0](https://help.miro.com/hc/articles/25692796700306).

## Solicitações de autorização de usuário entre a Miro e o servidor de autorização local

Para uma integração entre Miro e Jira usando um servidor de autorização de terceiros, o gráfico a seguir mostra o fluxo de solicitação de autorização do usuário.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Solicitação de autorização do usuário*

### Solicitação de autorização

```
https://{authorization_URL}?
    response_type=código&
    client_id={CLIENT_ID}&
    redirect_uri={URI de redirecionamento da Miro}&
    scope={scope}&
    status={state}
```

O usuário pode adicionar parâmetros à solicitação de autorização como pares de chave-valor na configuração.

### Solicitação de token

```
curl --request POST \
    --url '{URL de solicitação de token}' \
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=código_de_autorização \
    --data 'client_id={CLIENT_ID}' \
    --data 'client_secret={CLIENT_SECRET}' \
    --data 'code={Código de Autorização Obtido}' \
    --dados 'uri_de_redirecionamento={URI de redirecionamento da Miro}' \
```

Após a Miro receber o código de autorização, a Miro fornece o status e solicita um par de tokens.

### Atualizar a troca de tokens

```
curl --request POST \\
    --url '{URL de solicitação de token}' \
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=refresh_token \
    --dados 'client_id={CLIENT_ID}' \
    --data 'refresh_token={token de atualização atual válido}' \
```

Certifique-se de que a operação de refresh token esteja habilitada; ative o acesso offline às APIs.

### Solicitações de API do Jira

```
curl --request GET \
    --url {Jira Public URL}/rest/api/{apiversion}/... \
    --header 'autorização: Portador {accessToken}' \
    --header 'content-type: application/json'
```

Cada solicitação usa o URL público do Jira fornecido como o URL base, e o token de acesso do usuário como o token ao portador.
