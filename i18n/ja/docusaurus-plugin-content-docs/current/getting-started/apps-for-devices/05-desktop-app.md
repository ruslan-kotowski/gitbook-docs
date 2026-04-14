---
title: "\u30C7\u30B9\u30AF\u30C8\u30C3\u30D7\u30A2\u30D7\u30EA"
article_id: 360017572854
translation_id: 360017572854
locale: ja
sidebar_position: 5
created_at: '2019-02-11T10:15:04Z'
updated_at: '2025-11-25T16:00:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
---

ホーム画面から直接Miroデスクトップアプリを数秒で起動し、集中してボードで作業できます。アプリは、ブラウザー版の基本機能すべてに対応しています。

:::tip
Miroアプリは[こちらのウェブサイト](https://miro.com/apps/)からダウンロードできます。
:::

## Miroデスクトップアプリのダウンロード

### Windows

- Windows 64-bit - [アプリをダウンロード](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.exe)

:::note
Windows 32-bit は廃止され、利用できなくなりました。
:::

### macOS

- Apple シリコンチップ搭載の Mac - [アプリをダウンロード](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro.dmg)
- Intel チップ搭載の Mac - [アプリをダウンロード](https://desktop.miro.com/platforms/darwin/Install-Miro.dmg)

ご利用のプロセッサーの種類を確認するには、以下の手順に従ってください。

1. Mac の左上にある Apple アイコンをクリックします。
2. これにより、ドロップダウン メニューが表示されます。**[この Mac について]** オプションをクリックします。

画面に、プロセッサー情報（インテルまたは Apple シリコン）などが表示されます。

## 複数デバイスに Miro を導入する

Miro の提供する各種インストーラーにより、IT 管理者は数千のマシン上のユーザーに Miro を展開することができます。これには2つの基本的な方法があります: ユーザーごとにインストールする方法や、マシンごとにインストールする方法です。それぞれに、自動更新があるバージョンとないバージョンがあります。自動更新のバージョンは、アプリが公開されるとすぐにユーザーに更新されたバージョンを提供します。一方、自動更新のないバージョンでは、従業員が使用する Miro のバージョンをより詳細に制御できます。

### Windows の場合

#### Miro を Program Files に配置

Miro は Program Files ディレクトリにインストールすることもでき、デバイスの全てのユーザーが利用できるようにしつつ、それぞれのプロフィールを別々に保つことができます。1 台のマシンに 1 度のインストールで済むということは、そのマシンのすべてのユーザーが Miro を利用できるようにしながらも、規模が大きくなればなるほどハードドライブのフットプリントが小さくなるということです。自動アップデートを選択した場合、アップデートをインストールするには管理者権限が必要です。

- Windows MSI 64 ビット 自動アップデート付き - [アプリをダウンロード](https://desktop.miro.com/platforms/win-nsis/Miro-setup.msi)
- Windows MSI 64 ビット 自動アップデートなし - [アプリをダウンロード](https://desktop.miro.com/platforms/win-nsis/Miro-no-updates.msi)

#### 特定のユーザーに Miro をデプロイ

Miro の提供する各種インストーラーにより、IT 管理者はシングルユーザーに Miro を展開することができます。このバージョンは、管理者権限なしで更新でき、選択した特定のユーザーのみにインストールされます。

- Windows MSI 64 bit 自動更新あり - [アプリをダウンロード](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.msi)
- Windows MSI 64 bit 自動更新なし - [アプリをダウンロード](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-no-updates.msi)

### MacOS の場合

- Apple silicon Mac 自動更新なし - [アプリをダウンロード](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro-no-updates.dmg)
- Intel Mac 自動更新なし - [アプリをダウンロード](https://desktop.miro.com/platforms/darwin/Install-Miro-no-updates.dmg)

## アプリのシステム要件

### Windows の場合

|  |  |  |
| --- | --- | --- |
|  | **最低** | **推奨** |
| **CPU** | 3 GHz (2 コア/4 スレッド) | 2.8 GHz (4 コア/8 スレッド) |
| **RAM** | 8 GB | 16 GB（DDR4） |
| **OS** | Microsoft Store からのアプリについては Windows 10 以上 + Microsoft .NET Framework 4.5  （Windows の ARM バージョンはサポートされていませんのでご注意ください） | 最新の OS |
| **ネットワーク** | 8 Mb/s 以上 | 32 Mb/s |

### MacOS の場合

|  |  |  |
| --- | --- | --- |
|  | **最小** | **推奨** |
| **CPU** | 64 ビットインテルまたは Apple M1 |  |
| **OS** | MacOS 12 (Monterey) 以上 | 最新のOS |
| **ネットワーク** | 8 Mb/s 以上 | 32 Mb/s |

アプリは、お持ちのデバイスで複数のインスタンスを実行します。

- メインプロセス
- ウィンドウプロセス（UI レンダラー）
- ハードウェア アクセラレーション
- クラッシュハンドラー
- 開かれたタブごとにプロセスがひとつ増加（各タブにはウェブビューがあるため）

例えば、作業中に 3 つのタブを開くと、Miro.exe のインスタンスが 7 つ表示されます。さらに詳しい情報は、[こちら](https://www.electronjs.org/docs/glossary#process) や [こちら](https://www.chromium.org/developers/design-documents/multi-process-architecture)をご覧ください。

## アプリ固有のショートカット

デスクトップアプリには、追加の[ショートカット](../../using-miro/working-on-the-board/06-shortcuts-and-hotkeys.md)があります。

- **Ctrl + R** *(Windows)* / **Cmd + R** *(Mac)*：タブをリロード
- **Ctrl + W** *(Windows)* / **Cmd + W** *(Mac)*：タブを閉じる
- **Ctrl + Q** *(Windows)* / **Cmd + Q** *(Mac)*：アプリを終了
- **Ctrl + Shift + L** *(Windows)* / **Cmd + Shift + L** *(Mac)*：ボードのリンクをコピー
- **Ctrl + ~** *(Windows)* / **Cmd + ~** *(Mac)*：ズーム

## アプリのアクション

次のテーブルは、Miroデスクトップアプリにおける使用可能な操作がブラウザとは異なる体験になる可能性があることを示しています：

| 操作 | **Win & Mac アプリから**[**Miro アプリ**](https://miro.com/apps/) |
| --- | --- |
| 画像として保存（低、中、高） | ✔ |
| 画像として保存（ベクター） | ✔ |
| PDFとして保存（低） | ✔ |
| PDF として保存（ベクター） | ✔ |
| スプレッドシートへのエクスポート（CSV） | ✔ |
| ビデオチャット | ✔ |
| スプレッドシートからの貼り付け | ✔ |
| Confluence プラグイン | ✔ |

### 利用不可のアクション

以下のアクションは Miro デスクトップアプリでは利用できません:

- 訪問者はログインできません。

  > ✏️ デスクトップアプリにログインできるのは登録済みの Miro ユーザーのみです。
- Sketch からコピー/貼り付けするオプションはありません
- 一部の Jira Server バージョンでは、安全性のために Jira カードの編集ができません。

## スペルチェック

デスクトップ アプリの自動スペルチェック機能をオフにしたい場合は、以下の手順に従ってください。

- Press **Alt** (*Windows のみ*)
- 上部のメイン ナビゲーション バーの **閲覧** をクリックする
- **スペルチェックを表示** ボタンのチェックを外す

Microsoft ストアからダウンロードされたアプリでは、スペルチェックを無効にするオプションが利用できませんのでご注意ください。

## 起こり得る問題とその解決方法

### アプリデータをリセットする方法

問題が発生する場合（特にログインでお困りの際）は、アプリデータを**リセットする**ことで、アプリのメモリーを消去すると役立つことがあります。

:::tip
データをリセットしても問題が解決しない場合は、最新バージョンを[ダウンロード](https://miro.com/apps/)して、アプリを削除して再インストールしてください。
:::

#### Windows の場合

**Alt > ヘルプ**を押し、以下のスクリーンショットに示されているようにアプリケーションデータをリセットしてください。

​​
![reset app data on Windows.png](../../../../../../docs/getting-started/apps-for-devices/images/21016134171922_reset%20app%20data%20on%20Windows.png)
*Windows のデスクトップアプリにおけるアプリデータのリセット*

メニューが見つからない場合、MS Store からダウンロードしたアプリをご使用している可能性があります。この場合、アプリデータをリセットするには、Windows の**設定** > **アプリ** > **アプリと機能** > 一覧で**Miro**を見つけて > **詳細オプション** > **リセット**を選択します。

これですぐに解決しない場合は、次の場所からすべてのアプリファイルを削除してください：**C:\Users\username\AppData\Roaming\RealtimeBoard** および **C:\Users\username\AppData\Local\Programs\RealtimeBoard**

> **✏️** もし **Appdata** フォルダーが非表示の場合は、[こちら](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5)を参照して表示方法を確認してください。

#### MacOS の場合

トップメニューで Miro をクリックし、以下のスクリーンショットに表示されているように**アプリケーション データのリセット** を選択します。

![reset app data on Mac.png](../../../../../../docs/getting-started/apps-for-devices/images/21016120799378_reset%20app%20data%20on%20Mac.png)
*Mac でアプリデータをリセット*

その後、再度アプリにログインして、問題が解決されているか確認してください。

リセットですぐに問題が解決しない場合は、ファインダー ウィンドウを開き、**Command + Shift + G**を押し、**~/Library/Application Support/RealtimeBoard**を貼り付け、アプリファイルをすべて削除してください。

Mac 用 MDM を使用する場合

アプリが読み込めず先に進めないという問題が起こった場合は、設定を確認し、自動更新機能が有効になっていることを確かめてください。 `https://github.com/Squirrel/Squirrel.Mac` には以下の権限が必要です。

- `Application` ディレクトリを読み出し、書き込み、実行する
- `com.electron.realtimeboard.ShipIt` ディレクトリと動作する `~/Application Support/Caches/` の読み取りと書き込みをする。また、temp ディレクトリ `private/var/folders` でも動作。

更新プロセス中に不具合がある場合は、Squirrel は、`~/Application Support/Caches/com.electron.realtimeboard.ShipIt` に `ShipIt_stderr.log` を作成します。問題の詳細情報は、そちらをご覧ください。
Skype と Slack も同様の更新プロセスを使用しているので、設定された MDM をお持ちの場合は、Miro のデスクトップ アプリと同じ設定を適用することができます。

## よくある質問

1. *デスクトップアプリはどこでダウンロードできますか？*
   - [弊社のウェブサイト](https://miro.com/apps/)からダウンロードできます。
2. *ブラウザーで Miro を起動するときにデスクトップアプリを開くポップアップを削除する方法は？*
   ー [この記事](../../using-miro/troubleshooting-technical-questions/technical-guidelines/04-how-to-disable-miro-desktop-app-pop-up-in-your-browser.md)の手順を試してください。
3. *Linux のデスクトップアプリ版はありますか？*
   ー 現時点では、このバージョンはありません。
4. *デスクトップアプリで開かれたボードのリンクをコピーする方法は？*
   ー ボードの**共有**メニューを開き、そこでボードリンクをコピーできます。もう一つの方法として、右上の**ファイル**をクリックし、**ボードリンクをコピー**を選択します。**Ctrl + Shift + L** *(for Windows) /* **Cmd + Shift + L** *(for Mac)*というショートカットも利用できます。
5. *Windows デスクトップアプリで **Alt** を押してもメニューが表示されません。表示方法を教えてください。*
   - Microsoft Store からダウンロードしたアプリではメニューはサポートされていませんので、ご了承ください。Windows の設定でアプリデータをリセットすることができます(**システム > アプリ & 機能 > Miro を見つける > 詳細オプション > リセット**)。また、[オリジナルアプリバージョンをインストール](https://miro.com/apps/)してください。
6. *デスクトップアプリを削除すると、ボードは削除されますか？*
   - いいえ、コンテンツはあなたのMiroのプロフィールに紐付けられています。ブラウザ、[タブレットアプリ](11-tablet-app.md)、[モバイルアプリ](08-mobile-app.md)でもアクセスできます。
