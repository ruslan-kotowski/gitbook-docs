---
title: "\u30A2\u30D7\u30EA\u7BA1\u7406"
article_id: 4404659741458
translation_id: 4404659741458
locale: ja
sidebar_position: 2
created_at: '2021-08-03T15:46:50Z'
updated_at: '2026-01-29T10:00:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: apps-management
---

組織レベルおよびチームレベルでのアプリとアクセス権限を管理する方法を学びましょう。

> **関連プラン：**Business プラン、Enterprise プラン
> **管理可能なユーザー：**チームの管理者、会社の管理者

### アプリを管理できるユーザー

組織レベルのアプリ管理をできるのは、Enterprise プランの会社の管理者のみです。チームレベルのアプリ管理をできるのは、Business プランと Enterprise プランのチームの管理者と会社の管理者です。

### 組織または特定のチームのアプリを追加する

アプリ管理コントロールから、組織全体または特定のチームのすべてのユーザー向けにアプリを追加して承認します。
**会社**の設定に移動し、**アプリとインテグレーション** > **アプリ** の順に選択します。このセクションでは、会社の管理者はすべてのチームまたは特定のチームのアプリを追加できます。

![apps-access.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803476626_apps-access.png)*会社の設定でのアプリ管理コントロール*

検索バーにアプリ名またはクライアントIDを入力します。ドロップダウンリストからアプリを選択し、**追加** をクリックします。

![add-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780909714_add-app.png)*会社の設定からアプリを追加する*

組織内のすべてのチームのアプリを追加するか、特定のチームを選択することができます。一部のチームにアプリがすでに追加されている場合、対応するタグが表示されます。チームのアプリを再度追加する場合、チームメンバーはアプリを再認証する必要があります。**追加**をクリックして終了します。

![add-apps-where.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780917010_add-apps-where.png)
*Google ドライブアプリをインストールするために誰に対してインストールするかを選択*

すべてのチームにアプリを追加する場合、新しく作成されたすべてのチームに対してアプリが追加されます。

### 事前に追加されたアプリ

一部のアプリはユーザーに事前に追加されています。追加の認証または個別のログインが必要となる場合があります。これらの事前に追加されたアプリには、[Box](../../integrations-apps/more-integrations/05-box-legacy.md)、[Dropbox](../../integrations-apps/more-integrations/06-dropbox.md)、[Google Drive](../../integrations-apps/google/05-google-drive.md)、[OneDrive](../../integrations-apps/microsoft/06-onedrive.md)、[Smartsheet](../../integrations-apps/more-integrations/15-smartsheet-app-for-miro.md)、[Azure Cards](../../integrations-apps/microsoft/03-azure-cards.md)、[Jira Cards](../../integrations-apps/atlassian/03-jira-cards.md)があります。[Brandfetch](https://miro.com/marketplace/brandfetch/)、[Google Images](../../integrations-apps/google/06-google-images.md)、[Slack](../../integrations-apps/more-integrations/14-slack.md)。これらのアプリは、会社の承認済みリストに記載されていない場合、事前に追加されません。会社の管理者であれば、このリストを管理できます。

### 組織のアプリを事前承認する

アプリを追加する場合、同時に事前承認することもできます。アプリが事前追加され、管理者によって事前承認されている場合、組織内のユーザーはすぐに使用することができます。特定のアプリでは、第三者サービスへのログインを個別に必要とする場合があります。

この機能は、Miro Web SDK を使用してビルドされたアプリでのみ使用できます。Miro Web SDK を使用すると、Miro 機能を拡張することができます。これは、Miro ボード内で実行する強力なアプリをビルドするツールボックスです。

### 個々のユーザー管理用のアプリを承認する

デフォルトでは、ユーザーはチームに任意のアプリを追加できます。会社の管理者は、ユーザーのアプリ管理を制限して、チームが特定のアプリだけしか追加できないように設定することができます。

会社の管理者は、**会社**の設定 > **アプリとインテグレーション** > **アプリ** > **アプリの管理** に移動し、**メンバーが以下のリストにあるアプリのみを追加するように制限する**オプションをオンにして、ユーザーの特定のアプリを有効化または制限することができます。

![manage-apps.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780921490_manage-apps.png)*Enterprise プランで承認済みアプリの追加を制限するオプション*

追加が制限されている場合、Enterprise プランのユーザーは承認済みのアプリのみを追加することができます。ユーザー追加のアプリを承認するには、隣のトグルを有効化するか、対応するフィールドにクライアント ID を貼り付けて、内部で開発されたアプリを承認します。

事前に追加されているアプリを制限するには、リストでアプリを見つけ、アプリの横にあるトグルが無効になっていることを確認します。アプリが制限されている場合、Enterprise チーム全体のユーザーはアプリを使用することができません。

組織でアプリが制限されている場合、ユーザーは[会社の管理者にアプリ使用リクエストを送信](03-app-request-flow.md)することができます。

ユーザーは、Enterprise プランに保存されている Miro ボード内のマーケットプレイスで承認済みのアプリを確認することができます。

### チームでのアプリ使用の許可または制限

チームの管理者と会社の管理者は、チームレベルでアプリの使用を管理することもできます。チームメンバーがチームに新しいアプリを追加することを、許可または制限することができます。設定はチームごとに別々に設定されます。

![add-apps-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780928914_add-apps-team.png)*チーム設定のアプリとインテグレーション*

詳細は[Miro のアプリとインテグレーション](../../integrations-apps/integrations-basics)について学ぶ。
