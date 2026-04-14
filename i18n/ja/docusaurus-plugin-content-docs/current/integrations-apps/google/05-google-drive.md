---
title: "Google \u30C9\u30E9\u30A4\u30D6"
article_id: 360017731253
translation_id: 360017731253
locale: ja
sidebar_position: 6
created_at: '2019-02-11T10:14:01Z'
updated_at: '2025-01-13T14:51:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-drive-onedrive
---

**Google ドライブ**を使うと、オンラインで安全にファイルを保存し、どこからでもアクセスでき、他のメンバーとコラボレーションできます。Google ドライブとのインテグレーションを利用すれば、タスクに集中し、ドキュメントをボード上でより簡単に管理できるようになります。

Google_Drive_on_the_Upload_menu.jpg

> **管理** 者は、管理者以外のユーザーによるアプリのインストールを制限することができます。
> ブラウザ版、[デスクトップアプリ](../../getting-started/apps-for-devices/05-desktop-app.md)（フル機能、ファイル編集**可能**）、[タブレットアプリ](../../getting-started/apps-for-devices/11-tablet-app.md)、[モバイルアプリ](../../getting-started/apps-for-devices/08-mobile-app.md)（機能制限、編集不可）

### Google ドライブの有効化

Google ドライブからファイルの追加を開始するには、プラグインをインストールし、Google ドライブを Miro に接続する必要があります。

[Miro のマーケットプレイス](https://miro.com/marketplace/google-drive/?backUrl=%2Fmarketplace%2F)からアプリをインストールします。「 **アプリを入手**」をクリックすると、プラグインをインストールするチームを選択する画面が表示されます。![install_Google_Drive.jpg](../../../../../../docs/integrations-apps/google/images/21016134562450_install%20Google%20Drive.jpg)*Google Driveプラグインをインストールする際のチームの選択*

ボードからプラグインをインストールすることもできます。作成バーで、**ツール、メディア、インテグレーション****（+）を**選択します。パネルが開きます。**ツール]**タブで[Googleドライブ]を検索します。**アップロード]**を選択し、[**Googleドライブ]**を選択します。

Google_Drive_on_the_toolbar.jpg

次に、Google ドライブを Miro に接続しますが、簡単な方法が 2 つあります。

1.   プロフィール設定からボードバーで、ハンバーガーアイコンを選択します。サイドバーが開きます。アバターを選択し、[**設定]を**選択します。プロフィールの設定が新しいウィンドウで開きます。**インテグレーション」** タブを選択します。**Googleドライブの**場合は、「**接続**」を選択します。

![connect_Google_Drive.jpg](../../../../../../docs/integrations-apps/google/images/21016121228306_connect%20Google%20Drive.jpg)*インテグレーションページのGoogle Drive*

2. 2. ツールバーの **[アップロード]** メニューにある **[Google ドライブ]** をクリックし、ボード内で Miro のプロフィールと Google ドライブをリンクします。

![Google_Drive_on_the_Upload_menu.jpg](../../../../../../docs/integrations-apps/google/images/21016121222546_Google%20Drive%20on%20the%20Upload%20menu.jpg)*ツールバーのGoogle Driveアイコン*

必要な Google アカウントの認証を確認し、アプリのファイルへのアクセスを **[続行]** します。

permissions.jpg
Google ドライブへのアクセス権限

これらは Google ドライブに対する一般的なアクセス権限です。

—**Google ドライブのすべてのファイルの表示、ダウンロード** —ボード上の Google ドライブファイルのピッカーに表示。この権限で、Google ドライブから Miro へのドキュメントのインポートが可能

—**このアプリで使用する Google ドライブ上の特定のファイルのみの参照、編集、作成、削除** —この権限で、Miro ボードの Google ドライブへの保存が可能

Google ドライブ アプリケーションは、ドライブ上で作成されたファイルのみを管理します（ボードへのリンクなど）。  Miro は Google ドライブ内のコンテンツを管理することはできません。インテグレーションの実施には、**Google ドライブ API v3** を使用しています。この API では、書き込み権限がフルディスクのアクセス権限とは別にリクエストできないように、スコープをグループ化しています。詳しくは Google の記事、[「Google API のスコープ」](https://developers.google.com/identity/protocols/googlescopes)でアクセス権限をご確認ください。

Miro にリンクしている Google アカウントの変更が必要な場合は、**[プロフィールの設定]** > **[インテグレーション]** へ移動し、**Google ドライブ**の隣りの **[ログアウト]** をクリックして別のアカウントにリンクしてください。

![Google_Drive_log_out_in_settings.jpg](../../../../../../docs/integrations-apps/google/images/21016121230610_Google%20Drive%20log%20out%20in%20settings.jpg)*プロフィール設定のGoogleドライブ接続*

### Google ドライブと共有ドライブからのファイルの追加

> **利用可能なソフトウェア：**ブラウザー版、[デスクトップアプリ](../../getting-started/apps-for-devices/05-desktop-app.md)、[タブレットアプリ](../../getting-started/apps-for-devices/11-tablet-app.md)、[モバイルアプリ](../../getting-started/apps-for-devices/08-mobile-app.md)（機能に制限あり）

:::warning
Miro のボードにアクセスできるすべてのユーザーは、Google 側で制限されている場合でも、インポートされたドキュメントを取り出せます。ファイルを保護するには、ドキュメントへのアクセスを制限すべきユーザーとボード共有をしないでください。
:::

Google ドライブからファイルを追加するには、以下の手順を実行します。

1. ドキュメントの URL を直接ボードに貼り付けます（URL を[図形](../../using-miro/essential-tools/11-shapes.md)や[付箋](../../using-miro/essential-tools/14-sticky-notes.md)に貼り付けた場合、ドキュメントはボードに埋め込まれず、リンクが単なるテキストとして追加されるだけなのでご注意ください）。⚠️ Google スプレッドシートから特定のシートのリンクをコピーして、Miro ボードに貼り付けても、貼り付けたスプレッドシートは、Miro 上では最初のページから始まります。または

   あるいは
2. ツールバーの **[アップロード]** ボタン（上のスクリーンショットに表示）をクリックし、**Google ドライブ**を選択すると、ピッカーメニューが表示されます。追加したいすべてのドキュメントを選び、**[Select]** （選択）をクリックします。検索バーを使って Google ドライブ上のドキュメントを検索することもできます。

> [モバイルアプリ](../../getting-started/apps-for-devices/08-mobile-app.md)でボードに Google ドライブのドキュメントを追加するには、[Upload]（アップロード）メニューを使ってドキュメントの URL を貼り付けます。

![Googleドライブ内のファイル選択.gif](../../../../../../docs/integrations-apps/google/images/21016121231122_select%20a%20file%20in%20Google%20Drive.gif)*Googleドライブ内のドキュメントの選択*

**共有ドライブ**からドキュメントを追加 —タブに切り替えてファイルを選択します。

![チームドライブ.jpg](../../../../../../docs/integrations-apps/google/images/21016134572434_team%20drive.jpg)*Googleドライブピッカーのチームドライブ*

### Google ドキュメントの編集

> **利用可能なソフトウェア：**ブラウザー版、[デスクトップアプリ](../../getting-started/apps-for-devices/05-desktop-app.md)

Google ドキュメント、スプレッドシートおよびスライドをボードに直接埋め込んで、移動、サイズ変更、またドキュメントのページのスワイプができます。

ドキュメントをクリックすると、ページを切り替え、ページを **[ピン留め]**、**[ページを抽出]**、コンテンツを **[編集]**、**[再読み込み]**、**[更新]**、**[ソース]** への移動を実行するためのコンテキストメニューが表示されます。

ドキュメントの編集を開始するには、コンテキストメニューのペンのアイコンをクリックするか、ドキュメントをダブルクリックします。ドキュメントはポップアップ内で開き、Google ドライブ上と同様に編集できます。**[閉じる]** または グレーのエリアをクリックし、編集を終了します。すべての変更は自動的に保存され、ボード上と Google ドキュメント内で表示されます。

![google_drive_edit_docs.gif](../../../../../../docs/integrations-apps/google/images/21016121248274_google_drive_edit_docs.gif)*埋め込み Google ドキュメントの編集*

必要に応じて、**ソース**ボタンをクリックし、次のタブでドキュメントを開いて編集することもできます。

Google ドライブで直接編集した場合（特にオフラインで作業した場合）は、コンテキストメニューの **[更新]** ボタンを使って、ボードに埋め込まれたものを更新してください。ボードに埋め込まれた Google ドライブのファイルは、Miro 上で編集されない限り、自動的に更新されることはありません。

![更新ボタン.jpg](../../../../../../docs/integrations-apps/google/images/21016121232274_update%20button.jpg)*更新ボタン*

### アクセス権の管理

Google ドライブと Miro のアクセス権は*個別に*設定されていますので、ご注意ください。つまり、ユーザーが Google ドキュメントを編集できるようにするには、そのユーザーと Google ドライブで*編集者*の権限付きでドキュメントを共有し、さらに[ボードに*編集者*として招待](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)する必要があります。

Google でドキュメントの編集者権限を与えても、ボードに[閲覧またはコメント権限](../../using-miro/sharing-boards/01-board-access-rights.md)のみで招待した場合、ドキュメントの編集モードを有効にすることはできません。逆の場合も同様に、編集者としてボードに招待しても、Google ドライブでドキュメントを共有しなければ、Google はこのユーザーにドキュメントの編集許可を与えません。

コラボレーションの成功に必要なアクセスレベルが、ご自身とチームメンバーに付与されていることをご確認ください。

### ボードの Google ドライブへの保存

> **設定者：**ボード所有者

ボードバーで縦の三点リーダーを選択します。**メイン**メニューが開きます。**ボード** > **エクスポート** > **Googleドライブに保存を**選択します。

Google ドライブで保存したボードをクリックできるようになります。クリックすると別のブラウザータブでボードが開きます。ボードは、Google ドライブで削除しても、Miro では引き続き利用できます。ただし、Miro でボードを削除すると、Google ドライブからのアクセスはできなくなります。/span>

:::warning
ボード所有者でない場合は、以下のエラーメッセージが表示されます。
:::

![Google_Drive_error.jpg](../../../../../../docs/integrations-apps/google/images/21016121236882_Google%20Drive%20error.jpg)*保存権不足のエラーメッセージ*

### プラグインの削除

チームのプラグインを削除するには、チーム設定の **[アプリとインテグレーション]** セクションでプラグインをみつけ、**[チームから削除]** をクリックします。

![アンインストール_Google_Drive_app.jpg](../../../../../../docs/integrations-apps/google/images/21016134575122_uninstall%20Google%20Drive%20app.jpg)*Googleドライブのアンインストール*

Miro と Google ドライブのリンクを解除するには、プロフィールの設定の**インテグレーション**のページを開き、Google ドライブのアイコンの横にある **[ログアウト]** をクリックします。

![Google_Drive_log_out_in_settings.jpg](../../../../../../docs/integrations-apps/google/images/21016121230610_Google%20Drive%20log%20out%20in%20settings.jpg)*MiroからのGoogle Driveの切断*

### ボードに埋め込まれた Google ドライブのファイルでは利用できない機能

**一般**

- Google ドライブの開始ページ
- フォルダー間のファイルの移動
- 共有
- ヘルプ検索

**Google プレゼンテーション**

- プレゼンテーション モード

### 起こり得る問題とその解決方法

**アップロードできませんというエラー**

**「このファイルをアップロードすることはできません。このファイルをアップロードする権限がないか、ファイルが削除されたようです。**アクセス権を確認して再度お試しください」というエラーメッセージが、Google ドライブのファイルを Miro ボードにアップロードしようとするときに表示されたら、Google 管理者に、Drive SDK API で Google ドライブへのアクセス許可をユーザーに与えるよう依頼してください。

1. [Google 管理コンソール](https://admin.google.com/)にログインします。
2. **[ホーム] > [アプリ] > [Google Workspace]** をクリックします。**[ドライブとドキュメント]** が**オン（すべてのユーザー）**になっていることを確認してください。
3. **[ドライブとドキュメント] > [機能とアプリケーション]** をクリックします。**[Drive SDK]** のセクションで、**「Drive SDK API 経由での Google ドライブへのアクセスをユーザーに許可する」**が**オン**になっていることを確認します。

unable_to_upload.png
アップロードができない場合の警告メッセージ

**認証に関する問題**

Google ドライブと Miro をリンクできない場合、次の権限がGoogle ドライブにリンクする際 Miro に与えられていることを確認します。**「Google ドライブのすべてのファイルの表示、ダウンロード」**、「このアプリで使用する Google ドライブ上の特定のファイルのみの参照、編集、作成、削除」。この権限を付与するには、Miro の [プロフィールの設定] > [インテグレーション] をクリックし、Google ドライブとのリンクを解除し、再度設定し直します。

Permissions.png
Miro の Google ドライブアカウントへのアクセス権限

### よくある質問

1. *埋め込みファイルをGoogle Driveで開くことはできますか？*
   - はい、ドキュメントを選択し、コンテキストメニューの **ソース**ボタンをクリックします。
2. *Miroボードの内容をGoogle Driveのファイルに貼り付けることはできますか？*
   [- ボードの内容をテキストまたは画像としてコピー](../../using-miro/working-on-the-board/09-copy-as-text-or-as-an-image.md)し、Google Driveのファイルに貼り付けることができます。
