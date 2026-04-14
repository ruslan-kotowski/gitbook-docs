---
title: サードパーティーの認証を使用した OAuth 2.0 参照による Jira オンプレミス
article_id: 26726425696530
translation_id: 26751148570386
locale: ja
sidebar_position: 11
created_at: '2025-05-16T09:09:20Z'
updated_at: '2025-11-25T15:51:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '実行可能なユーザー：: 会社の管理者 利用可能なプラン：: エンタープライズ'
---

この記事では、Miro と Jira を統合するために、OAuth 2.0 を使用してサードパーティ認証サーバーを利用する技術詳細を提供しています。

接続の設定方法を学ぶには、[サードパーティー認証サーバーを介した OAuth 2.0 で Jira オンプレミスに接続する方法](https://help.miro.com/hc/articles/25692796700306)をご覧ください。

## Jira における Miro とのインテグレーションは、オンプレミス認証と OAuth 2.0 を使用してどのように機能するか

次のグラフは、Miro とオンプレミスの Jira 認証サーバー間の通信フローを示しています。

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*API ゲートウェイを介したオンプレミス認証サーバーを使用した Miro と Jira のインテグレーション*

## 構成パラメーター

Miro と Jira の間で OAuth 2.0 を利用してサードパーティーの認証サーバーを用いた認証フローを構成するには、以下のパラメーターを指定する必要があります。

- **認証サーバー**
  - 認証リクエスト URL
  - トークンリクエスト URL
  - スコープ
- **認証アプリの設定**
  - クライアント ID
  - クライアント シークレット
- **Jira インスタンス**
  - Jira 公開 URL
  - Jira ベース URL; 内部 URL

:::note
Miro は、認証サーバーが登録済みアプリを検証するためのリダイレクト URL を提供します。
:::

**詳細情報：**[サードパーティの認証サーバーを使用した OAuth 2.0 での Jira オンプレミスへの接続](https://help.miro.com/hc/articles/25692796700306)を参照してください。

## Miro とオンプレミス認証サーバー間のユーザー認証リクエスト

Miro と Jira の統合でサードパーティー認証サーバーを使用する場合、次のグラフはユーザー認証要求フローを示しています。

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*ユーザー認証要求*

### 認証リクエスト

```
https://{authorization_URL}?
    response_type=code&
    client_id={CLIENT_ID}&
    redirect_uri={Miro Redirect URI}&
    scope=範囲&
    state={state}
```

ユーザーは、構成においてキーと値のペアとして認可リクエストにパラメーターを追加できます。

### トークンリクエスト

```
curl --request POST \\
    --url '{token request URL}' \
    --header 'content-type: application/x-www-form-urlencoded' \\
    --data grant_type=authorization_code \
    --data 'client_id={CLIENT_ID}' \\
    --data 'client_secret={CLIENT_SECRET}' \
    --data 'code={取得した承認コード}' \
    --data 'redirect_uri={Miro Redirect URI}' \
```

Miro が認証コードを受け取った後、Miro は状態を提供し、トークンペアを要求します。

### トークンの更新交換

```
curl --request POST \
    --url '{token request URL}' \\
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=refresh_token \
    --data 'client_id={CLIENT_ID}' \
    --data 'refresh_token={current valid refresh token}' \
```

リフレッシュトークン操作が有効であることを確認し、APIへのオフラインアクセスを有効にします。

### Jira API リクエスト

```
curl --request GET \
    --url {Jira Public URL}/rest/api/{apiversion}/... \
    --header 'authorization:Bearer {accessToken}' \
    --header 'content-type: application/json'
```

各リクエストは、提供された Jira の公開 URL をベース URL として使用し、ユーザーアクセス トークンをベアラートークンとして使用します。
