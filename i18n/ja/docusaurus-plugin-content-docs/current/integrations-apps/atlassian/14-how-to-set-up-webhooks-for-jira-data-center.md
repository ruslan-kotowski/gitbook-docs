---
title: Jira Data Center の Webhook の設定方法
article_id: 360017731113
translation_id: 8531824016018
locale: ja
sidebar_position: 15
created_at: '2022-11-11T17:33:20Z'
updated_at: '2026-01-14T09:25:34Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '対象: Jira システム管理者 プラン: すべての Miro プラン（Jira Server/Data Center 統合には OAuth 1.0
    が必要） プラットフォーム: ブラウザ、デスクトップアプリ（セットアップ手順用）'
---

Miro ボード上の[Jira カード](https://help.miro.com/hc/articles/360017572434)が常に最新の状態を保つために、Jira からデータが変更されるたびに Miro にメッセージが送信される必要があります。これらの Jira イベントは、Webhook を介して Miro に送信されます。

このガイドは、OAuth 1.0 と OAuth2.0 を使用して Jira Server と Jira Data Center 用の Webhook を作成する 2 つの方法を提供します。

## Webhook を自動的に作成する

[Jira カードのインテグレーションを設定する場合](https://help.miro.com/hc/articles/360019501754)、Jira Server または Jira Data Center に接続する際は、**Webhook を自動的に作成する**オプションを有効のままにできます。これは推奨メソッドです。

:::note
Webhook の自動作成には、Jira のシステム管理者としてログインしている必要があります。
:::

![jira-webhooks-server-config.png](../../../../../../docs/integrations-apps/atlassian/images/21304245707026_jira-webhooks-server-config.png)
*Jira カードの設定、ステップ 2：「Webhook を自動的に作成する**」**が有効になっています*

Webhook が自動で作成された後、この Webhook に一意な名前を付けるために Jira WebHooks ページにアクセスして編集することをお勧めします。特にいくつかの Miro チームを Jira インスタンスに接続する予定がある場合には重要です。

:::note
OAuth2.0 接続では、Miro 側の接続は会社レベルで設定されます。すべての Miro チームに対して一つの Webhook が作成されます。
:::

:::note
Miro チームレベルでの OAuth 1.0 接続では、チームごとに Webhook が作成されます。Miro 会社レベルでは、すべてのチームに対して一つの Webhook が作成されます。
:::

## Webhook を手動で作成する

Webhook を手動で作成することを希望する場合、または必要がある場合は、以下の手順に従ってください。

**Miro から Webhook URL を取得します**

1. Miro の Jira カード設定 (Jira Server/Data Center 接続時のステップ 2) で、**Webhook を自動的に作成する** オプションのチェックを外します。
2. 組織の**Jira URL**をコピー & ペーストし、**接続して設定を保存**をクリックします。
   ![jira-webhooks-configure-jira-url-cropped.png](../../../../../../docs/integrations-apps/atlassian/images/21304245708818_jira-webhooks-configure-jira-url-cropped.png)
   *Jira カード設定、ステップ 2：「Webhook を自動的に作成する」が無効になっている*
3. Jira で接続を許可してください。
4. これらのステップの後、Miro が **Webhook URL** を提供します。
   ![webhook_URL.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016928565010_webhook%20URL.jpg)*Miro によって提供された Webhook URL*

:::note
もしあなたが Jira システム管理者でない場合、Miro によって提供された **Webhook URL** をコピーして、Jira システム管理者に送り、以下の手順で Jira 側に Webhook を作成してもらってください。
:::

**Jira での Webhook 作成**

以下は、Miroから取得したURLを使用してJiraにWebhookを作成する手順です。[Jira Server](https://developer.atlassian.com/server/jira/platform/webhooks/)および[Jira Cloud](https://developer.atlassian.com/cloud/jira/platform/webhooks/)の公式 Atlassian ドキュメントも参照できますが、この文書はサーバーやデータセンターに重点を置いています。

1. Jiraで**WebHooks**ページに移動するには、**Jira管理** > **システム** > **詳細** > **WebHooks**と進みます（Jiraのバージョンによって正確なパスは若干異なることがあります）。また、`/plugins/servlet/webhooks`をJiraインスタンスのURLに追加して直接リンクを使用できることが多いです（例：`https://YourJiraInstanceName/plugins/servlet/webhooks`）。
2. **WebHookの作成**をWebHooksページの右上隅でクリックします。
3. Webhookの説明的な**名前**を入力します（例：「MiroインテグレーションWebhook」）。
4. Webhookのステータスを**有効**に設定します。
5. Miro の設定からコピーした**WebHook URL**を URL フィールドに貼り付けます。
   ![system_webhooks.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941532050_system%20webhooks.jpg)
   *Jiraのシステム Webhook 設定*
6. **イベント**セクションの**課題**の下で、**更新済み**と**削除済み**のイベントを選択します。
7. **作成**をクリックして、Webhook を保存します。
   ![Jira_Webhook_settings.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941533074_Jira%20Webhook%20settings.jpg)
   *Jira WebHook イベント設定*
8. Jira で Webhook を作成した後、Miro の Jira カード設定の**ステップ 2**に戻り、**Jira URL**が正しく入力されていることを確認し、**接続**をクリックします。

これで、Webhook が作成および設定されました。Miro のボード上の Jira カードは、Jira で変更が行われると自動的に更新されます。
