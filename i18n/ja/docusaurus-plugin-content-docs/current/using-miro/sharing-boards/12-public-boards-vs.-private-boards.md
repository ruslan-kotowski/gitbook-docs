---
title: 公開ボードと非公開ボード
article_id: 360011114519
translation_id: 360011114519
locale: ja
sidebar_position: 12
created_at: '2019-12-26T20:14:13Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
availability:
  notes: '実行可能なユーザー：: ボード所有者 どのプラットフォーム：: ブラウザー、デスクトップ、モバイル'
---

Miro は、ボードにさまざまなアクセスレベルを設定することができます。この記事を読んで、非公開と公開ボードが互いにどう異なるかをご覧ください。

## 非公開ボードとは何ですか？

> **利用可能なプラン：**Starter、Business、Enterprise、Education

非公開ボードにはボード所有者のみがアクセスでき、他の誰とも共有されません。[デフォルトの共有設定](11-default-sharing-settings.md)に応じて、有料プランで作成されたすべてのボードは、[共有](03-sharing-boards-and-inviting-collaborators.md)されるまで、所有者が共有するか、チームで自動的に共有されるまで、非公開に設定することができます。有料チームまたは Education チームで非公開ボードを作成する方法は[こちら](15-make-a-miro-board-private.md)でご覧ください。

[Free プラン](../../plans-billing/miro-plans/09-free-plan.md)では、*作成されたすべてのボードは、明示的に共有されなくてもチームがアクセスできます*。Free プランのボードの**共有**ウィンドウは、デフォルトでチーム全体が利用できることをユーザーに知らせます。[チーム設定](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md)の**アクティブなユーザー**タブでチームメンバーを確認できます。

![Screenshot_background_template__4__2_.jpg](images/22250060619282_Screenshot%20background%20template%20%204%20(2).jpg)
*無料プランでのボードの共有設定*

## 公開ボードとは何ですか？

> **利用可能なプラン：**Free、Starter、Business、Enterprise、Education

公開ボードは、ボードリンクがある人なら誰でもアクセス可能なボードです。ボードを公開するには、次の手順を行ってください。

1. ボードの右上隅にある **共有** ボタンをクリックします。
2. **リンクを知っている人は誰でも**の横にある**閲覧可 / コメント可 / 編集可**を選択します。
3. ボードリンクをコピーして、他のユーザーと共有しましょう。設定された権限に応じて、ボードの閲覧、コメント、編集ができるようになります。ボードは未登録のユーザーも利用できるようになりますのでご注意ください。

![public_sharing.gif](../../../../../../docs/using-miro/sharing-boards/images/21016967259154_public%20sharing.gif)
*ボードを公開にする設定*

:::note
ボードを公開して共有すること以外に、Miro は、メールでコラボレーターを招待するか、Team/会社/スペースへのアクセスを有効にすることができます。[ボードの共有とコラボレーターの招待](03-sharing-boards-and-inviting-collaborators.md)の記事で詳細を確認しましょう。
:::

## 共有ボードを非公開に設定する

> **利用可能：** Starter、Business、Enterprise、Education のプラン

ボードを非公開にするには、[さまざまなアクセスレベル](01-board-access-rights.md)での共有を停止してください：チーム、会社（Enterprise プランの場合）、公開、スペース、および特定のユーザーとの共有を**共有**ダイアログの**共有設定**で選択解除します。あなた（所有者）のみが表示されるまで、各ユーザーを削除する必要があります。

ボードの**所有者ではなく**、[チーム](03-sharing-boards-and-inviting-collaborators.md)または[スペース](../spaces/01-spaces.md)経由でボードにアクセスする場合は、[自分のメールアドレスをボードに招待](03-sharing-boards-and-inviting-collaborators.md)してください。それ以外の場合、チーム / スペースへのアクセスを削除するとすぐに、ボードへの**アクセスを失います**。

[無料プラン](../../plans-billing/miro-plans/09-free-plan.md)では、チームとのボードの共有を停止できないことにご注意ください。

**詳細情報：**[Miro のボードを非公開にする](15-make-a-miro-board-private.md)を参照してください。

![set_a_board_to_private.gif](../../../../../../docs/using-miro/sharing-boards/images/21016967257490_set%20a%20board%20to%20private.gif)
*共有ボードを非公開に設定する*

## よくある質問

Free プランにダウングレードした後にボードがロックされたのはなぜですか？

Free プランでは、ボードを非公開にすることはできません。ボードをチームと共有して、ロック解除してください。記事[「ボードがロックされています」](../tools/troubleshooting/15-the-board-is-locked.md)で詳細を確認してください。

ボードを非公開にするためにアップグレードするオプションがあるのを見ました。ボードはデフォルトで公開されていますか？

Free プランでは、デフォルトでチーム全体と共有されます。これは、Free チーム内でボードが「チームで共有されている」ことにのみ関連しています。

自分の公開ボードはオンラインで検索できますか？

Miro は、公開ボードが Google や Bing のような検索エンジンにインデックスされないよう努めています。しかし、こうしたボードは、リンクがあれば誰でも開くことができ、意図しないユーザーにもリンクが共有される可能性があります。ご利用中の Miro プランによっては、[公開ボードにパスワードを設定](13-password-protection-for-public-boards.md)してセキュリティーを強化することができます。

私は、無料チームと有料チームのメンバーです。ボードを無料チームから有料チームに移動して非公開にすることはできますか？

はい、[ボードを移動する](../managing-boards/04-how-to-move-a-board.md)ことができます。

公開ボードは複製できますか？

はい、[ボードのコンテンツ設定](14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)でこれが許可されている場合は可能です。

ボードを公開して共有する場合、ボードリンクからボードにアクセスするユーザーの利用料金を支払う必要はありますか？

いいえ、ビジターはボードに無料でアクセスすることができます。[ボードを公開して共有する](08-collaboration-with-visitors.md)方法を学びましょう。
