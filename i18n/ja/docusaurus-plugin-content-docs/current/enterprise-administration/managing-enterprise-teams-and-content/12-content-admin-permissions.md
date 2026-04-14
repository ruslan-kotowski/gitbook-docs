---
title: コンテンツ管理者権限
article_id: 360012777280
translation_id: 360012777280
locale: ja
sidebar_position: 13
created_at: '2020-03-26T12:31:39Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-admin-permissions
availability:
  notes: '利用可能なプラン：: Enterprise プラン'
---

コンテンツ管理者権限を利用すると、Enterprise サブスクリプション内のすべてのコンテンツを監督できます。コンテンツ管理者として、ボード、スペース、セクション、テンプレートへのアクセスをシームレスに管理し、未使用のボード、スペース、セクションを削除してダッシュボードを整理することができます。

### コンテンツ管理者の役割を割り当てる方法

1. [設定](https://miro.com/app/settings/user-profile/)に移動します。
2. **ユーザー**の下にある**管理者の役割**をクリックします。
3. **コンテンツ管理者**の役割の横にある三点リーダー（**…**）をクリックし、ドロップダウンメニューから**役割を割り当てる**を選択します。
4. コンテンツ管理者の権限を付与したいユーザーを選択します。最大 50 人のユーザーを選択できます。
5. **割り当てる**ボタンをクリックして選択を確定します。
6. コンテンツ管理者の役割が割り当てられているすべてのユーザーを閲覧するには、もう一度三点リーダー (**…**) をクリックし、「**ユーザーを表示**」を選択します。または、**コンテンツ管理者バー**をクリックして、ユーザーのリストを表示することもできます。

コンテンツ管理者に割り当てられた権限を確認するには、**コンテンツ管理者**バーをクリックし、**権限**タブに切り替えて、すべての**コンテンツ**権限をスクロールダウンしてご覧ください。

## ボードとスペースの管理

コンテンツ管理者がボードとスペースで持つ権限の詳細については、[管理者役割ドキュメントのコンテンツ管理セクション](../../administration/get-started-as-a-miro-admin/02-understand-admin-roles-and-their-privileges.md)をご覧ください。

さらに、コンテンツ管理者は以下のことができます：

- 共有ダイアログを開いてボードの共有設定を管理する（[ユーザーのアクセスを削除または変更する](../../using-miro/sharing-boards/01-board-access-rights.md)、ボードを[チーム](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)／ユーザー／[会社](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)／[公開](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)で共有する）
- ボードの詳細（名称、概要、カバー）を変更する
- ボードを[スペース](../../using-miro/spaces/01-spaces.md)に移動させる
- ボードをセクションに移動させる
- [ボードを削除する](../../using-miro/managing-boards/07-how-to-delete-a-board.md)
- [ボードのバックアップをダウンロードする](../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)
- [ボードのコンテンツ設定を構成する](../../using-miro/sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)
- 高度なボード共有権限を[設定する](../../using-miro/sharing-boards/02-who-can-share-a-miro-board.md)
- 公開ボードのパスワードを[作成したユーザーを確認し](../../using-miro/sharing-boards/13-password-protection-for-public-boards.md)、公開ボードのパスワードを設定、変更、削除する
- ゴミ箱から任意のボードを[復元する](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md)。

コンテンツ管理者とチームコンテンツ管理者は、ボード所有者がメンバーである別のチームにボードを移動できます。もしボード所有者が対象チームのメンバーでない場合は、所有権をメンバーに[移行](../../using-miro/managing-boards/05-how-to-transfer-board-ownership.md)することができます。

ダッシュボードでボードが表示されない場合、それはボードが自分と共有されていないことを意味します。ただし、ダッシュボードでボード名、ボードの所有者、または場所（チーム）で[検索](../../getting-started/start-here/miro-dashboard/03-how-to-search-in-miro.md)して見つけることができます。自分と共有されていないボードには、ボード名の横にロックアイコンが表示されます。ボードを管理するには、右上にある三点リーダーをクリックします。

直接リンクや検索結果からボードを開こうとすると、**「ボードにアクセスできません」**というメッセージが表示されます。下部には、**ボードの詳細を見る** と **アクセス権限を管理する** のオプションが表示されます。

:::note
**非公開**スペースで、あなたが**メンバーではない**スペースの設定を変更することはできず、スペースリストにも表示されません。非公開スペースの設定を変更する必要がある場合は、スペースの所有者にアクセスを依頼するか、[Miro の公開 API](https://developers.miro.com/reference/enterprise-update-project-settings)を利用してください。ダッシュボードに*表示される*スペースの設定は変更可能です*。*
:::

## テンプレートの管理

テンプレートの共有設定（[個人、チーム、会社](../../getting-started/start-here/your-first-board/02-custom-templates.md)）を変更したり、テンプレートの詳細（名前、説明、カバー画像）を編集したり、テンプレートを完全に削除することができます。

**カスタムテンプレートの管理方法**

1. ダッシュボードに移動し、右上の**テンプレートを探す**をクリックします。
2. 左ナビゲーションの**カスタムテンプレート**に移動し、**[会社名] テンプレート**または**個人用**をクリックします。
3. 編集したいテンプレートにカーソルを合わせて、三点リーダー（...）をクリックします。
4. テンプレートを削除するには、**削除**をクリックします。
5. 他のテンプレート詳細を管理するには、**編集**をクリックします。
6. ボードが開きます。ボードメニューのテンプレート名をクリックします。
7. **テンプレート名**や**説明**を追加または編集し、カバー画像の**プレビューエリアを選択**し、共有設定を**個人用**、**チーム**または**会社**に変更します。
8. **変更を保存**をクリックします。
