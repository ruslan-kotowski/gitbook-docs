---
title: プロフィールを削除する方法
article_id: 360017571354
translation_id: 360017571354
locale: ja
sidebar_position: 7
created_at: '2019-02-11T10:08:54Z'
updated_at: '2026-01-07T13:30:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
availability:
  notes: '設定者：: プロフィールの所有者'
---

Miro からプロフィールを削除すると、ユーザー情報がシステムから削除されます。プロフィールとチームは、異なるものですのでご注意ください。

- プロフィールは、ユーザーの登録とメールアドレスにリンクされたデータを表します
- チームとは、他のチームメンバーと一緒に、メンバーがコンテンツを作成してボードを保存できるスペースのことです。

すべてのプロフィールは、複数のチームに関連付けることができます。チームを削除したい場合は、[こちら](../../administration/team-management/06-delete-and-restore-teams.md)でその方法を確認してください。
:::warning
プロフィールの削除は取り消すことは**できません**。
:::

:::warning
プロフィールの削除は、利用中のサブスクリプションはキャンセルされませんのでご注意ください。更新を停止するには、[設定でサブスクリプションをキャンセル](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md)してください。
:::

### プロフィールを削除する方法

1. [プロフィール設定](https://miro.com/app/settings/user-profile/)を開きます。

2. 2. ページの下部までスクロールし、**[プロフィールを削除する]** を選択します。

Delete_profile.png
プロフィールを削除

3.3. この時点で、削除する前にボードの[バックアップ](../import-and-export/export/05-how-to-save-board-backup.md)を保存するか、[エクスポート](../import-and-export/export/03-how-to-export-your-board.md)することをお勧めします。

![プロフィール削除確認メッセージ.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017429125778_profile%20removal%20modal.jpg)*プロフィール削除確認メッセージ*

4.5. その後すぐに、確認リンクが記載されたメールが届きます。リンクをクリックして終了します。**[プロフィールを削除する]** をクリックする際には、ブラウザーで Miro プロフィールにログインしていないと、プロフィールの削除は正常に完了しないのでご注意ください。

Profile_deletion_email.jpg
プロフィールを削除するための確認メール

### プロフィールの削除後のコンテンツ

プロフィールを削除すると同時にボードは削除されます。

プロフィールを削除したユーザーがチームの唯一の管理者である場合は、コンテンツは*完全に*削除されます。管理者権限は、一番最初にチームに招待されたメンバーに付与されます。

チームに他の管理者がいる場合は、コンテンツは削除され、管理者の 1 人に再度割り当てられます。そして、その管理者は、[90 日以内であればボードを復元](../managing-boards/08-how-to-restore-a-deleted-board.md)できるようになります（有料ユーザーはゴミ箱から、また無料ユーザーはリンクから復元することができます）。

### よくある質問

1. *[シングルサインオン（SSO](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)）でMiroにログインした場合、プロファイルを削除できますか？*
   — はい、可能です。[ただし、組織が SCIM を使用している場合は、メールが SCIM 経由で Miro に提供されている限り、プロフィールはすぐに再作成されます。](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)

    を選択します
2. *Miroプロフィールにリンクされているメールアドレスを変更するにはどうすればよいですか？*
   - このガイドをご利用ください：メールアドレスの変更方法

    を選択します
3. *確認リンクが記載されたメールが届きません。*どうすればよいですか？
   - 以下の手順をお試しください：

- **スパム、プロモーション、****迷惑メール、ソーシャル**、**アップデート**のフォルダーを開き、Miro の確認メールを探してみてください。
- 受信トレイがいっぱいかどうかをみて、メールの受信トレイのメモリーの上限を超えていないことを確認してください。上限に達している場合は、新しいメールを受信するために、既存のメールの一部を削除する必要があります。メールを削除した後、再度プロフィールの削除をリクエストしてください。
- ファイアウォールがメールの受信トレイへの配信を妨げている可能性があります。次のドメインとサブドメインを許可リストに登録してもらえるよう、システム管理者に依頼してください。miro.com*、*./span>*miro.com*、mirostatic.com*、*.mirostatic.com[、](http://miro.com/)realtimeboard.com*、*.[realtimeboard.com](http://miro.com/) 。 許可リストに必要なメーラーの詳細情報についてはこちらの記事をご覧ください。
- どの方法でも解決しない場合は、Miro のサポートにご報告[ください](../tools/troubleshooting/06-contacting-miro-support.md)
