---
title: "ServiceNow \u306B\u3088\u308B\u30BD\u30D5\u30C8\u30A6\u30A7\u30A2\u8CC7\u7523\
  \u7BA1\u7406"
article_id: 360021758459
translation_id: 360021758459
locale: ja
sidebar_position: 3
created_at: '2021-05-20T05:00:32Z'
updated_at: '2025-02-26T11:53:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

ServiceNow と Miro のインテグレーションを利用して、サブスクリプションの使用状況を大規模に分析し、カスタマイズできます。インテグレーションにより、資産管理アプリから非アクティブユーザーのリストを取得し、非アクティブ化することができます。

> **利用可能なプラン：**[Enterprise プラン](../../../plans-billing/miro-plans/04-enterprise-plan.md)
> **設定者：**会社の管理者

## 対応している機能

インテグレーションにより、以下の機能にアクセスできます。

- **サブスクリプションをダウンロードする**
  - ユーザーのサブスクリプション使用状況や、Miro Enterprise サブスクリプションに割り当てられているライセンス数の一覧を取得します。
- **サブスクリプションを回収する**
  - サブスクリプションの使用状況に基づいて、Miro Enterprise プラン内のユーザーを非アクティブ化します。

## 設定手順

### インテグレーション

1. ServiceNow の **SaaS ライセンス** モジュール > **ダイレクトインテグレーション プロフィール**オプションを選択して、**[New]（新規作成）**をクリックします。

   saas_license_module.jpg
   SaaS ライセンス モジュール

   > ✏️**Saas License**モジュールがServiceNowインスタンスに存在しない場合は、以下の に従ってインストールする必要が[titleあります。title](https://docs.servicenow.com/bundle/quebec-it-asset-management/page/product/software-asset-management2/task/request-saas-license-management.html)
2. **Miro Enterprise インテグレーション プロフィール**を検索します。

   Miro_Enterprise_integration_profile.jpg
   Miro Enterprise インテグレーション プロフィールの検索
3. **購読のダウンロード]**と[**購読の回復]**の 2 つのサブフローが定義済みであることがわかります：
   download_subscription_sybflow.jpg
   *サブスクリプションサブフローのダウンロード*

   reclaim.jpg
   *サブスクリプション・サブフローの回収*

### 新しい接続の作成方法

1. 新しい接続を作成するには、**[資格情報と接続]** > **[接続と資格情報エイリアス]** に移動し、**[新規作成]** をクリックします。
   new_alias.jpg
   *新しい接続と資格情報エイリアスを作成するオプション*

**[新規接続と資格情報を作成]** リンクをクリックします。

create_connection.jpg
接続と資格情報エイリアスの作成

**サブスクリプションをダウンロード**するサブフローでは、**クライアント ID** と**クライアント シークレット**を指定する必要があります。

create_connection_modal.jpg
接続と資格情報の作成

2. **Client** IDと **Client Secretを** 取得するには、Miro側で **[Settings] > [Profile settings] > [Your apps]に** 進み、[ **Create new app]を選択します。**

![](../../../../../../../docs/enterprise-administration/enterprise-subscription-management/software-asset-management/images/23921803379090_image.png)*プロフィール設定で新しいアプリを作成*

3. **アプリ名を**設定し、チームを選択し、**Create appをクリックします。**[デベロッパーチームが](../../managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md)必要です。

4. 4. アプリページの **[管理者権限]** セクションで、**[organizations:read]** を選択して、**[アプリをインストールして OAuth トークンを取得]** をクリックします。

5. 5. Enterprise 組織のチームの 1 つを選択し、アプリをインストールします。

6. **クライアント** IDと **クライアントシークレットを**コピーします。

**Reclaim Subscriptions** サブフローでは、**SCIM API**トークンを提供する必要があります。SCIM APIトークンを取得するには、Miroで管理者コンソールにアクセスし、「**Apps and integrations (アプリとインテグレーション)**」 > 「**Enterprise integrations (インテグレーション)** 」 > 「 **SCIM Provisioning (SCIMプロビジョニング)**」の順に進み、「**API Token (API トークン)**」の下にあるトークンをコピーします。

## サブスクリプションの使用状況のカスタマイズ

デフォルトでは、**最終アクティビティーのしきい値**は、60 日間に設定されています。これを変更するには、[Reclamation Rules]（回収ルール）に移動し、Miro のルールを選択します。次に、最終アクティビティーのしきい値を以下のように変更します。

last_activity_treshold.jpg
最終アクティビティーのしきい値

## 起こり得る問題とその解決方法

チームにアプリをインストールしようとすると、「このアプリをインストールできませんでした。このアプリケーションはインストールできません。そのスコープは現在のプランでは使用できません。
- 開発チームは組織レベルのスコープにアクセスできないため、これは開発チームにアプリをインストールする際に予想される動作です。ServiceNow のインテグレーションを有効するにするには、組織レベルのスコープにアクセス可能な Enterprise チームにアプリをインストールします。

install_app_error.jpg
Dev チームにアプリをインストールする際のエラー
