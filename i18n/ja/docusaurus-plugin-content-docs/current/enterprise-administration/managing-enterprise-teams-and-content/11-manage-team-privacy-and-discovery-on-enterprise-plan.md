---
title: Enterprise プランのチームのプライバシーと公開の管理
article_id: 360011821219
translation_id: 360011821219
locale: ja
sidebar_position: 12
created_at: '2020-02-07T12:46:14Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: sharing-settings
availability:
  notes: '利用可能なプラン：: Enterprise 設定者：: 会社の管理者'
---

大規模な組織で作業していると、コンテンツやユーザーが複数のチームに分散していることがよくあります。サブスクリプションのメンバーが関連するチームを表示し、参加できるようにすることで、誰もが必要な情報にアクセスできるようにします。

### チームの公開

**チームの公開設定とは、組織のメンバーがどのようにチームを検索して参加できるかをコントロールする、チームレベルの設定です。**チームの公開設定を管理するには、[**会社設定] > [チーム]**に進み、設定を変更したいチームをクリックします。次に**「設定」**タブを選択します。

![チーム管理リスト.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921803038994_team-management-list.png) *会社設定内のチームリスト*

> [⚠️](../../administration/user-management/02-invitation-settings.md) チームの管理者がユーザーをチームに招待することを許可されている場合、会社の管理者とチームの管理者は、チームの公開を設定することができます（チームに参加するユーザーリクエストも受け取ることができます）。

チームの公開には以下の 3 つの段階があります。

- **非表示**—メンバーがチームに招待されない限り、チームを検索することはできません
- 承認によるメンバーの参加ーチームが表示され、メンバーは参加をリクエストすることができます
- **メンバーに公開**ーチームが表示され、メンバーはすぐに参加することができます

チームが [ドメイン許可リストの制限](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)を設定している場合、メールドメインがチームの許可リストに登録されているユーザのみが、そのチームを発見し、参加申請することができます。この設定により、チームの検出可能性は、チームレベルで設定されたドメイン制限に従うようになります。

> [ジャストインタイム プロビジョニング](../user-management/13-user-provisioning-on-enterprise-plan.md))を使用してチームの公開機能を有効化すると、既存のユーザーには新規登録ユーザー向けに設定されたデフォルトチームも表示され、参加できるようになります。

![チームの公開設定.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780537234_team-management-discovery-settings.png)
*チームの公開設定*

チームの公開は、メンバーがサブスクリプションで他のユーザーを表示する方法には影響しません。したがって、チームのプライバシーによって却下されない限り、メンバーは設定で他のユーザーの詳細リストを表示することができます。/span>

ダッシュボードの左上にあるTeamsメニューを開き、![icon-zoom-in.svg](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921803048338_icon-zoom-in.svg) **Join teamを**選択すると、Enterpriseプランのメンバーは参加できるチームを見つけることができます。各チームのセキュリティー設定に応じて、「**参加する**」または「**参加を依頼する**」オプションが付いたチームのリストが表示されます。

![チーム管理-join.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780544914_team-management-join.png) *発見可能なチームのリスト*

### チームのプライバシー

**チームのプライバシ**ーとは、チームとユーザーの両方の表示を設定する会社レベルの機能のことです。**会社の** 設定＞**セキュリティー** ＞**共有の** 「**チームのプライバシー**」セクションにあります。

![team-management-privacy.pngチームの](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780547218_team-management-privacy.png)
*プライバシー設定*

- チームのプライバシーが無効になっていると、サブスクリプションのメンバーは、設定のユーザーの詳細リストと公開可能なチームのリストを表示することができます。メンバー全員が関連するコンテンツを見つけ、他のユーザーとコラボレーションして、知識の共有、透明性を促し、作業の重複を削減できるようにするのが、Enterprise プランのサブスクリプションのデフォルトの状態です。/span>
- チームのプライバシーが有効になっている場合、サブスクリプションのメンバーは、招待されたチームと、こうしたチームの他のユーザーのみを表示することができます。別のチームで異なるクライアントと作業する際に、交流しないようにすることができます。チームのプライバシーを有効にすると、ワンクリックで会社全体とボードを共有/span>することはできません。

### 共同作業するチームのプライバシーとチームの公開

チームのプライバシーは、チームレベルで設定された公開よりも優先順位が高くなります。チームの公開設定が有効ではない旨の通知が表示されます。チームのプライバシーを無効化しても、そのオプションを管理することはできます。

> ️️[✏️](../user-management/13-user-provisioning-on-enterprise-plan.md) チームのプライバシー設定とチームの公開設定は両方とも、サブスクリプション内のメンバーの体験に影響し、ユーザーがサブスクリプション自体に参加する方法には影響しません。
