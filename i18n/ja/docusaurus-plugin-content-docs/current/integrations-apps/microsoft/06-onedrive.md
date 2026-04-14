---
title: OneDrive
article_id: 360017731273
translation_id: 360017731273
locale: ja
sidebar_position: 7
created_at: '2019-02-11T10:14:03Z'
updated_at: '2025-01-13T13:02:45Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-drive-onedrive
---

OneDrive とのインテグレーション機能により、Microsoft Office と Office 365 の各ドキュメント（Word、Excel、PDF、画像、プレゼンテーションなど）を活用してボードを豊かにすることができます。

> **利用可能なソフトウェア：**ブラウザー版、[デスクトップアプリ](../../getting-started/apps-for-devices/05-desktop-app.md)

### プラグインをインストールする

チームレベルでプラグインをインストールし、OneDrive アカウントを Miro に接続すれば、インテグレーション機能を使い始めることができます。

[OneDriveを](../integrations-basics/04-how-to-install-apps.md)探し、**Get appをクリックします。**次に、プラグインをインストールしたいチームを選択し、「**インストール＆承認**」をクリックします。

:::warning
管理者以外のユーザーは、**アプリとインテグレーション**設定で許可されていなければ、このアプリをインストールすることができません。
:::

install_OneDrive.jpg
チームを選択して OneDrive プラグインをインストールする

ボードからアプリをインストールすることもできます。以下の手順に従ってください。

1. 作成バーで、**ツール、メディア、インテグレーション** **（+）を**選択します。**ツール、メディア、インテグレーション」**パネルが開きます。
2. **ツール]**タブで検索し、[アップロード]を選択します。
   **アップロードメニューが**開きます。

![アップロードエントリーポイント.png](../../../../../../docs/integrations-apps/microsoft/images/21537454978706_uploads-entry-point.png)
*作成ツールバーのOneDriveアイコン*

Miro から OneDrive に接続するには、**アップロード** メニューの [OneDrive] を選択します。Microsoft のログインページにリダイレクトされるので、ログイン ID とパスワードを入力して認証します。

[プロフィールのインテグレーション ページ](https://miro.com/app/account/profile/integrations/)で、**OneDrive** を見つけて**、**[接続] をクリックすることもできます。

connect_OneDrive.jpg
OneDrive と Miro を接続

### ファイルの追加方法

作成ツールバーの**アップロードボタンを**クリックし、**OneDriveを**選択します。ボードに追加するファイルを選択して、**[開く]** をクリックします。

**OneDrive for Business** を利用していれば、ドキュメントをダブルクリックするだけで、ボード上でドキュメントを閲覧できます。ボード上のポップアップウィンドウにドキュメントが表示され、OneDrive と同じようにドキュメントを閲覧できます。

Miro ボードから、直接 OneDrive にアクセスして、ドキュメントを編集することができます。

file_source_.jpg
ソースボタンを使って OneDrive のファイルを開く

### ファイルの更新方法

Miro ボード上のファイルを更新するには、コンテキストメニューの各ボタンをクリックします。

update_OneDrive_file.jpg
Miro ボード上の OneDrive ドキュメントの更新

新しいデータが表示されるまでに時間がかかる場合があります。

### プラグインの無効化

チームのプラグインをアンインストールするには、チームの設定を開き、**アプリとインテグレーション**のセクションで One Drive を見つけ、**[チームに対してアンインストールする]** をクリックします。

uninstall_OneDrive.jpg
チームの設定から OneDrive をアンインストールする

Miro から OneDrive との接続を解除するには、[プロフィールのインテグレーション ページ](https://miro.com/app/account/profile/integrations/)を開き、**OneDrive** を見つけて、**[ログアウトする]** をクリックします。

log_out_from_OneDrive.jpg
Miro から OneDrive との接続を解除する

### よくある質問

1. *Miroは共有ファイルをアップロードできますか？*
   - いや、それは無理です。Miro が使用する MS One Drive のファイルピッカーは、共有フォルダーに対応していません。
2. *「OneDrive アカウントを認証してください」というエラーメッセージが表示されます。*解決方法を教えてください。/em>
   - プラグインをアンインストールし、[プロファイル](https://miro.com/app/account/profile/integrations/)設定でOneDriveアカウントを切断してください。次に、インテグレーション機能を再度インストールして接続します。
