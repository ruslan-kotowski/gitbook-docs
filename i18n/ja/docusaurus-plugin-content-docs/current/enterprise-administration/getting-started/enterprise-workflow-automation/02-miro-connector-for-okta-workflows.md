---
title: "Okta Workflows \u7528 Miro \u30B3\u30CD\u30AF\u30BF\u30FC"
article_id: 8264504421394
translation_id: 8264504421394
locale: ja
sidebar_position: 1
created_at: '2022-10-25T14:04:07Z'
updated_at: '2025-02-26T12:20:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: okta-workflows
---

Okta Workflows ダッシュボードから、Miro 管理コネクターを利用するには、Okta Workflows 用の Miro コネクターを設定します。

[管理者コネクターとユーザーコネクターの詳細については、Set up workflow automation for Okta Workflows（Okta Workflows ワークフロー自動化セットアップ）をご覧ください。](03-set-up-miro-connectors-for-okta-workflows.md)

> **利用可能なプラン：** Enterprise
> **実行可能なユーザー：**会社の管理者

## Miro の設定

### アクセストークンの生成

1. Miro Enterpriseの設定ページで、[**Apps and integrations (アプリとインテグレーション)**] >**[Enterprise Integrations (エンタープライズインテグレーション)**] に進み、**Okta Workflowsまで**スクロールダウンします。

2. 2. トグルをクリックして、**Okta Workflows** の設定を有効にします。

![okta-workflows-turn-on.pngMiro](images/24938335989778_okta-workflows-turn-on.png)
*Enterpriseインテグレーション設定のワークフロー*

3. 3. **[コピー]** をクリックしてアクセストークンをコピーします。

4. 4. 新しいアクセストークンを生成するには、**[Generate new token]（新しいトークンを生成する）**をクリックします。

![okta-workflows-enablement.pngアクセストークン](images/24938360557970_okta-workflows-enablement.png)

:::warning
他の会社の管理者がこのトグルをすでに有効にしている場合、アクセストークンをコピーすることはできません。インテグレーションの無効化のみが設定可能です。
:::

:::warning
インテグレーションは、ユーザー数が最も多いチームと結び付けられます。別のチームを選択することはできません。ただし、インテグレーションは、Enterprise プラン内のすべてのチームに適用され、インテグレーションに関連するイベントは、全プランの監視ログに表示されます。
:::

## Okta Workflows の設定

### 新しい接続の作成

1. 1. Okta Workflows ダッシュボードで、**[接続]** に移動します。

2. 2. **[+ 新規接続]** ボタンをクリックします。

3. 3. **新規接続**ダイアログで、**Miro 管理者**コネクターを選択します。

![Miro-Administrator-connection.pngMiro](images/21019791315602_Miro-Administrator-connection.png)
*管理コネクタ*

4. 4. ダイアログの入力欄に**組織 ID** と**アクセストークン**をコピー&ペーストします。

5. **[作成]** をクリックします。

![Paste-org-ID-and-access-token-click-create.png](images/21019791318930_Paste-org-ID-and-access-token-click-create.png)
*新しいコネクタの*

6. 新しく作成した接続を確立したら、Okta Workflows の作成を開始できます。
