---
title: OAuth 2.0 を使用して Jira データセンターに接続する
article_id: 25753304280466
translation_id: 26513369505042
locale: ja
sidebar_position: 8
created_at: '2025-05-06T09:05:00Z'
updated_at: '2025-05-21T09:27:26Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '実行可能なユーザー：: Jira システム管理者権限を持つ会社の管理者 利用可能なプラン：: エンタープライズ 利用可能なプラットフォーム：:
    ブラウザー、デスクトップ'
---

:::note
OAuth 2.0 を使用した Jira Data Center への接続は、組織レベルでのみ有効です。
:::

## 前提条件

- 以下の権限を確認してください:
  - Jira システム管理者権限
  - Miro 会社の管理者役割
- Jira データセンターで OAuth 2.0 アプリケーション リンクを作成します。方法については、外部の [Atlassian Jira applications Support](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Create%20an%20incoming%20link%20using%20application%20links) をご覧ください。
  - プロンプトが表示されたら、以下のリダイレクトURLを使用してください。
    https://integrations.miro.com/api/external-auth/oauth2/callback
  - 自動 Webhook を使用するには、**管理者**をスコープとして選択してください。

## Miro を OAuth 2.0 を使用して Jira Data Center に接続する

1. Miro のダッシュボードで右上の自分のアバターを選択し、(Enterprise) **管理コンソール**、または(Starter および Business) **設定**に進みます。
2. 左側のサイドバーで、**アプリとインテグレーション ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **アプリ** > **アプリの管理** タブに移動します。
3. **以下のリストのアプリのみを許可する**が有効になっていることを確認します。
4. **アプリ**列で、**Jira カード**を選択し、**設定**を選択します。
5. **新しい接続を追加**を選択します。
6. **Jira セットアップ** で、**Jira データセンター** を選択します。
7. **認証方法**で、**OAuth 2.0**を選択します。
8. **Jira URL** には、Jira インスタンスの URL を入力します。
9. (オプション) 組織内のすべてのチームにおいて、この接続をデフォルト接続にするには、**デフォルトに設定**をクリックします。
10. Jira の**クライアント ID**を入力してください。
    **詳細情報**:(外部) [受信リンクを設定](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application) を参照してください。
11. Jira **クライアント シークレット**を入力します。
    **詳細情報**:[外部リンクの設定](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application) を参照してください。
12. スコープを選択
    **管理者**または**システム管理者**を選択して自動 Webhook を使用します。
13. （オプション）Jira から Miro へのリアルタイム更新を受け取るには、**Webhook を自動的に作成する**にチェックを入れてください。
    > オプションで、後から手動で Webhook を追加することもできます。
14. **接続** を選択します。
    > ユーザーが Jira 関連のアクションを初めて試みると、認証を求められます。再認証する必要はありません。

## 次は何ですか？

接続されている Jira インスタンスを表示および管理するには、**管理コンソール** | **設定** > **アプリとインテグレーション ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)**  > **アプリを管理** に移動します。次に、**アプリ**の列で、**Jira カード**の**設定**を選択します。

チームをデフォルトの Jira インスタンスに接続する方法については、[組織内のチームをデフォルトの Jira 設定に接続する方法](https://help.miro.com/hc/articles/26438407676434)をご覧ください。

## よくある質問

**スコープとして管理者を選択すると、全ユーザーが Jira で管理者権限を持つ必要がありますか？**

いいえ。管理者スコープは、Miro でユーザーが持つことができる最も高いスコープを意味します。範囲は、Jira の権限に応じて、ユーザーごとに制限されています。

**チームレベルで Jira データセンターを OAuth 2.0 で接続できますか？**

いいえ。組織レベルのみです。
