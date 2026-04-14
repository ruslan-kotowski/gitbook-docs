---
title: "Looker \u30A4\u30F3\u30C6\u30B0\u30EC\u30FC\u30B7\u30E7\u30F3\u3092\u8A2D\u5B9A\
  \u3059\u308B"
article_id: 25112862440978
translation_id: 25112862440978
locale: ja
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
Miro + Looker 統合に関する包括的な管理者向けドキュメントの詳細情報については、[Looker 管理ドキュメント](https://docs.google.com/document/d/1AUCQWRwDICLygwVmwSxXpz7RmRivPit0EIKgBMIkT6A/edit?usp=sharing)をご覧ください。
:::

**Looker** と Miro のインテグレーションを設定するには、Looker で OAuth アプリを登録する必要があります。

## 前提条件

- **会社の管理者**が Miro 組織の Looker を承認していることを確認してください。

## Looker に OAuth アプリを登録

1. **Looker Marketplace** で、**API Explorer 拡張機能**を見つけて選択します。
2. **インストール**を選択。
3. **ホーム** > **アプリケーション** > **API 拡張機能** に移動します。
4. **OAuth アプリを登録**を見つけて選択します。
5. **実行**を選択します。
6. メニューが開き、リクエストデータを追加できます。
   以下の値を追加してください。
   - **client_guid**:`15609152-a12a-4fa1-b364-337e7896d25d`
   -**本体**:

   ```
   {
     "redirect_uri": "https://integrations.miro.com/api/contenthub/public/oauth/callback"
     表示名Miro
     説明Miro Looker インテグレーション
     "有効": true,
     "group_id": ""
   }
   ```
7. **API エンドポイントがデータを変更することを理解しました**を選択してください。
8. **実行**を選択します。
9. 成功すると、**HTTP 200**のレスポンスコードが含まれたボディが返されます。
   - 💡 返された本文に`"enabled":false`が含まれている場合は、ステップ6と同じ値でOAuthアプリAPIを更新してください。

これで Miro と Looker の統合が成功しました。

## 詳細はこちら

- [Looker API リファレンス](https://developers.looker.com/api/explorer/4.0/methods/Auth/register_oauth_client_app)（外部）。
