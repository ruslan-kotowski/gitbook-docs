---
title: "\u30E6\u30FC\u30B6\u30FC\u306E\u62DB\u5F85"
article_id: 360017730013
translation_id: 360017730013
locale: ja
sidebar_position: 4
created_at: '2019-02-11T10:08:23Z'
updated_at: '2026-01-06T11:44:43Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
---

所属するチームやボードにユーザーを簡単に招待し、コラボレーションおよび作成を開始しましょう。[招待の設定](02-invitation-settings.md)に応じて、新しいユーザーを招待するオプションは、管理者のみ、またはすべてのメンバーが利用できる場合があります。

:::note
[この記事](../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md)を訪問して、Enterprise プランでのユーザー招待の方法を学んでください。
:::

## メンバーを招待

所属するチームにメンバーを追加するには、いくつかの方法があります。

- ダッシュボードから：右上の**メンバーを招待**をクリックします
  ![invite-members-dashboard.png](../../../../../../docs/administration/user-management/images/25007019083026_invite-members-dashboard.png)
  *ダッシュボードからメンバーを招待するオプション*
- 管理者コンソールから: **全ユーザー**タブを開きます。そこで、すべてのチームメンバーと招待済みユーザーを閲覧できます。

  ![admin-invite-users.png](../../../../../../docs/administration/user-management/images/25007019084178_admin-invite-users.png)
  *管理者コンソールから新しいメンバーを招待するオプション*

  右上の **新規メンバーを招待する**をクリックし、招待者のメールアドレスを入力します。招待画面には最大 500 件のメールアドレスを加えることができます。

  ![invite_modal.jpg](../../../../../../docs/administration/user-management/images/21017416281746_invite%20modal.jpg)
  *招待画面*
- このメニューでは、[**チーム招待リンク**](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)をコピーすることもできます。このリンクにアクセスした人は誰でもあなたのチームに参加できます（[Free](../../plans-billing/miro-plans/09-free-plan.md)、[Starter](../../plans-billing/miro-plans/08-starter-plan.md)、[Education](../../plans-billing/miro-special-pricing/03-education-plan.md)プランで利用可能）。管理者は[招待設定](02-invitation-settings.md)でリンクを有効化または無効化することができます
- Free プランでは、**すべてのユーザー** [**メールでボードに招待された**](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)場合、チームにも招待され、チームメンバーになります
- Starter プランでは、**すべての編集者**[**がメールでボードに招待された**](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)場合にチームメンバーになります。次の通知が表示され、コメント投稿者としてユーザーをチームに追加せずに招待するオプションもあります
  ![only_members_can_edit.jpg](../../../../../../docs/administration/user-management/images/21017429340690_only%20members%20can%20edit.jpg)
  *このプランでは、メンバーのみがボードを編集できる旨の通知*

招待者は招待メールを受信し、すぐに作業に参加することができます。

招待者が Miro に登録されていない場合、招待は30日間有効になります。すぐに承諾しなかった場合は、3日目と7日目にメール通知が届きます。通知メール内のリンクをクリックすると、[サインアップ](../../getting-started/start-here/02-how-to-register-with-miro.md)を勧められます。未登録者が30日以内に招待を承諾しない場合、その招待は失効し、ユーザーは**アクティブなユーザー**リストから削除されます。

登録済みの Miro ユーザーは、招待した後すぐに[ダッシュボード](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md)の左側のサイドバーであなたのチームを見つけることができます。

誤って招待を間違ったメールアドレスに送信したり、入力ミスをしたりして、追加の招待を削除したい場合は、招待されたユーザーの横にある三点リーダーをクリックし、**招待を取り消し**を選択します。

### Starter プランのメンバートライアル

:::note
[Starter プラン](../../plans-billing/miro-plans/08-starter-plan.md)のみ利用可能です。
:::

メンバーをチームに招待する際、すぐに有料ライセンスで追加されず、まず**Free** **メンバー**として追加されます。

招待されたユーザーがチーム内でボードを開いたり、自分のボードやプロジェクトを作成するなどの有料アクションを実行するまで、ユーザーのライセンスは無料のままです。

有料アクションが実行されると、ライセンスは7日間のトライアルに変更され、この時点でライセンスは消費されません。

ユーザーは 7 日間、無料でチームの有料ライセンスの全機能を利用できます。これにより、すぐにコストをかけずにコラボレーションできます。

トライアル中に、新しいメンバーは管理者コンソール内の**すべてのユーザー**セクションでフルメンバーに昇格したり、ゲストに変更したりできます。

トライアル終了（7 日間）までにアクションが取られない場合、トライアルメンバーは有料メンバーになります。トライアル終了後にトライアルメンバーを**フルチームメンバー**として追加したくない場合は、トライアル期間中いつでも[削除](08-remove-users.md)するか、ゲストユーザー（招待されたボードの閲覧やコメントができる）に変更できます。

メンバートライアルは、新規メンバー登録時に 1 回限り利用可能です。トライアルを使用した後で再追加されたメンバーは、そのまま有料ライセンスを使用します。

Starter プランが[Business プランにアップグレード](https://help.miro.com/hc/articles/360011780620-How-to-Change-Your-Plan#h_8315f4f8-9f5b-4665-b271-e438aedaf289)されると、すべてのトライアルメンバーはアップグレードの時点でフルメンバーに変換されます。

新しいライセンスの費用は、現在のサブスクリプション期間の残り時間（精度は1日）で**日割り計算される**ため、新しいライセンスの更新日は常に既存のライセンスと一致します。サブスクリプション期間中に空きライセンスがあり、新規メンバーを追加する場合、料金は発生しません。日割りの料金システムの詳細については、[請求とお支払い](../../plans-billing/billing-and-payments/04-miro-billing.md)の記事をご覧ください。

## ゲストの招待

メンバーとしてチームに追加せずに、メールでユーザーとボードを共有することができます。こうしたユーザーは、チーム設定でゲストとして表示されます。

:::warning
ゲストは[Freeプラン](../../plans-billing/miro-plans/09-free-plan.md)では利用できません。
:::

:::note
Business プランでは[招待設定](02-invitation-settings.md)でゲスト招待オプションが制限される場合があります。
:::

Starter および Education プランでは、閲覧またはコメントのアクセス権限のみを持つゲストを招待できます。

Business プランでは、閲覧者、コメント投稿者、または編集者としてゲストをボードに招待できます。

そのようなユーザーは**ゲスト**として管理者コンソールにリストされます。管理者はメンバーに変更するまたはチームから削除する / 招待を取り消すことができます。

ゲストはチーム内で自身のボードを作成することはできず、[チーム共有ボード](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)やプロジェクトにアクセスすることができません。チームへの参加をリクエストした場合、通知は管理者に送信されます。

:::note
メンバーをゲストに変換する方法は[こちらのページ](../../using-miro/sharing-boards/07-collaboration-with-guests.md)をご覧ください。
:::

## ビジターの招待

ボードをビジターと共有することも可能です。このようなユーザーはチームに追加されず、登録ユーザーでなくても公開ボードを閲覧 / コメント / 編集ができます。このオプションは、すべての有料プランで利用可能です。詳細は[ビジターとのコラボレーション](../../using-miro/sharing-boards/08-collaboration-with-visitors.md)を参照してください。

:::note
メンバー、ゲスト、ビジターの違いは[こちらのページ](../../using-miro/sharing-boards/07-collaboration-with-guests.md)で確認できます。
:::

## よくある質問

1. *招待者に、送信した招待メールが届きません。どのようにしてチームにアクセスできますか？*
   - ユーザーに Miro に登録してもらうか、Miro のプロフィールがある場合はログインするように依頼してください。そうすれば、[ダッシュボード](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md)の左側のサイドバーからチームを見つけることができます。
2. *Miro チームに招待されていますが、ログインしても表示されません。どのようにすればチームにアクセスできますか？*
   - [ダッシュボード](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md)の左側サイドバーでチームを探して切り替えてください。チームがない場合は、チームに招待された同じメールアドレスで Miro にログインしていることを確認してください。
3. *ダッシュボードに「メンバーを招待する」ボタンがありません。なぜですか？*
   - 管理者は[招待設定](02-invitation-settings.md)で新しいメンバーを招待するオプションを制限しています。このオプションは、Enterprise プランのチームの管理者に制限される場合がありますので注意してください。
4. *Miro に登録せずにユーザーを招待することができますか？*
   - はい、未登録のユーザーと[公開リンクを介してボードを](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)無料で共有できます。
5. *誤って新たに有料メンバーを招待してしまった場合はどうすればよいですか？*
   - [こちらの手順をお試しください](../../plans-billing/billing-and-payments/04-miro-billing.md)。
