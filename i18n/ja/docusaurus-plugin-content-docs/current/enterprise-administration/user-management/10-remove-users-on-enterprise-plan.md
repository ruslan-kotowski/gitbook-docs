---
title: "Enterprise \u30D7\u30E9\u30F3\u306E\u30E6\u30FC\u30B6\u30FC\u306E\u524A\u9664"
article_id: 360017730193
translation_id: 360017730193
locale: ja
sidebar_position: 10
created_at: '2019-02-11T10:09:21Z'
updated_at: '2025-11-04T11:30:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-management
---

Miro の高度なユーザー管理により、管理者はすべてのユーザーを一か所で簡単にフィルタリングし、管理することができます。管理者は、いつでも余分なユーザーを削除することができます。

> **利用可能なプラン：**Enterprise

### チームユーザーを削除する方法

Enterpriseサブスクリプションの特定のチームからユーザーを削除するには、ダッシュボードのチーム名にカーソルを合わせてチーム設定を開き、**チームメンバーの**アイコンをクリックします。

**ユーザー]**タブが開きます。削除したいチームメンバーを見つけて、**三点**リーダー（**...**）メニューから**「チームから削除**」を選択します。

![チームからのユーザー削除.png](../../../../../../docs/enterprise-administration/user-management/images/23921781390482_delete-users-from-team.png)

チームユーザーを削除する

チームからユーザーを削除しても、Enterprise 組織からは完全に削除されず、ライセンスも解放されない点にご注意ください。組織（会社）からユーザーを削除するには、こちらの手順に従って手続きをしてください。

また、複数のユーザーを選択して（最大で 50 件）、まとめて削除することもできます。

### 会社からユーザーを削除する方法

:::warning
ユーザーを削除する前に、[[非アクティブ化したユーザーをブロックする]](02-block-deactivated-users.md) の設定が有効になっているかを確認してください。削除されたユーザーは、非アクティブ化したユーザーとは扱いが異なります。
:::

Enterprise プランからユーザーを完全に削除するには、まず、[[会社](01-deactivated-users.md)の設定] の**[アクティブなユーザー]** セクション**で、**削除するユーザーを非アクティブ化します。その後、**「Deactivated users** 」タブを開き、 ユーザーの行にある**三点**リーダー（**...**）メニューから**「Delete」を** 選択します 。

また、最大 50 件のユーザーをまとめて選択し、一度に削除することもできます。

削除するユーザーが、Enterprise プランで作成されたボード / [テンプレート](../../getting-started/start-here/your-first-board/04-templates.md) / [プロジェクト](../../using-miro/sharing-boards/16-projects.md)の所有者である場合、コンテンツの所有権を再割り当てするユーザーを管理者または非管理者の中から選ぶことができます。**[ユーザーとコンテンツを削除]** を選択すると、ユーザーのコンテンツは削除されます。管理者は削除後 90 日以内であれば、[削除されたボードを復元](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md)することができます。

削除されたユーザーは、ご利用のプランのアセットへのすべてのアクセス権が（通知なしで）すぐに失われます。ただし、[公開リンクで](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)共有されたボードへのリンクをユーザーが保存していた場合、そのボードへのアクセスは維持されますので、ご注意ください。

Enterprise サブスクリプションからマネージドユーザーを削除する場合、そのユーザーはドメイン管理設定で[未確認](../canvas-25-admin-features/domain-control/01-domain-control.md)としてカウントされます。
