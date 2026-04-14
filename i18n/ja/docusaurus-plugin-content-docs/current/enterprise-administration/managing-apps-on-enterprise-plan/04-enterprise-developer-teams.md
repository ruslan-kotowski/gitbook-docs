---
title: "Enterprise Developer \u30C1\u30FC\u30E0"
article_id: 4766759572114
translation_id: 4766759572114
locale: ja
sidebar_position: 4
created_at: '2022-03-22T14:13:15Z'
updated_at: '2025-04-29T13:25:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: developer-teams
---

Enterprise サブスクリプション内で Developer チームを設定するオプションを満たすと、Enterprise アカウントでカスタムアプリを簡単かつ安全に作成することができます。

> **利用可能なプラン：**[Enterprise プラン](../../plans-billing/miro-plans/04-enterprise-plan.md)
> 設定者：**会社の管理者
> 他のMiroプランのユーザーは、[この](https://developers.miro.com/docs/rest-api-build-your-first-hello-world-app#step-1-create-a-developer-team-in-miro)ページから開発者チームを作成できます。**

### Developer チーム作成

Developer チームを設定するには、[**会社の設定**] > [**チーム**] を開き、右上にある [**新しいチームの作成]** をクリックします。

次のポップアップでチーム名を挿入し、[チーム権限のレベルを選択します。デフォルトの権限設定を設定するか、チームを選択してチーム権限をコピーすることができます (詳細](../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)は、[権限とデフォルトの設定] を参照してください)。 **Developer teamに**チェックを入れ、承認を確認し、**Create teamを**クリックします。

![create-dev-team.png。](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803173266_create-dev-team.png)
Developer チーム作成

### Enterprise Developer チームの権限

Enterprise Developer チームに安全にアプリを作成でき、Enterprise サブスクリプションの一部でありつつ Enterprise セキュリティ機能すべてが提供され、

Enterprise Developer チームはボードが無制限で、メンバーの制限はありません。

チームで作成されたボードには、組織内の他のチームと差別化するためにウォーターマークが表示されます。

チームには、Enterprise プランのユーザーを構成する標準的な設定があります。チームメンバーが新規ユーザーを招待することを許可 / 禁止、チーム / 会社 / 公開リンクとのボードの共有、ボードの移動、許可されたドメインの制限などを設定することができます。詳細については、[こちらの記事](../managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md)をご覧ください。

### アプリの作成とインストール

> 設定者：**チームの管理者
> チーム内でアプリを開発するために開発者を招待したい場合は、必ず[チームの管理者に権限を与えて](../../administration/user-management/06-how-to-manage-admin-roles.md)ください。**

[Enterprise Developer チームを使用して、Miro Enterprise で新しいアプリを作成するには、](../../using-miro/managing-your-profile/01-profile-settings.md)**[**プロフィール設定**] > [アプリ] を選択し、****利用規約に同意し、[**新しいアプリの作成] をクリックします。

![プロファイル-新規アプリ作成.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780634770_profile-create-new-app.png)
プロフィール設定のアプリ

:::tip
Developerチームのダッシュボードの右上にある**Build an appを**クリックしてもページに移動できます。
:::

![dev-team-build-an-app.png。](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780641298_dev-team-build-an-app.png)
新しいカスタムアプリをビルドするオプション

**アプリ名を挿入し、アプリの Developer チームを選択し、[**アプリの作成] をクリックします。

create_a_new_app.jpg
Enterprise Developer チームの新しいアプリの作成

**アプリページでスクロールダウンし、アプリに付与するアクセス範囲を選択し、**[アプリのインストール] をクリックし、OAuth トークンを取得します。

app_permissions.jpg
アプリの権限

アプリをインストールするときに、Enterprise 組織からチーム (Developer チームと異なります) を選択し、[**インストールと認証**] をクリックします。アクセストークンは、次の手順で表示されます。

installing_the_app.jpg
アプリのインストール方法

### Developer チームを削除する

Enterprise 組織内の他のチームと同様に、開発者チームを削除することができますが、まず、そのチームで作成されたアプリをすべて削除する必要があります。アプリを削除したら、次の場所に移動します。 [**チーム**](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md)に移動し、チーム名をクリックし、[**Profile]**タブを選択し、[**Delete team]**を選択します。

:::warning
Enterprise 開発者チームを削除すると、そのチームに紐づけられたトークンは無効になりますのでご注意ください。
:::

![削除-開発チーム.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803181586_delete-dev-team.png)*Enterprise Developer チームの削除*
