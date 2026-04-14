---
title: "\u30D6\u30E9\u30A6\u30B6\u30FC\u3067 Miro \u30C7\u30B9\u30AF\u30C8\u30C3\u30D7\
  \u30A2\u30D7\u30EA\u306E\u30DD\u30C3\u30D7\u30A2\u30C3\u30D7\u3092\u7121\u52B9\u5316\
  \u3059\u308B\u65B9\u6CD5"
article_id: 360019244239
translation_id: 360019244239
locale: ja
sidebar_position: 5
created_at: '2021-01-29T12:48:31Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

[Miro デスクトップアプリ](../../../getting-started/apps-for-devices/05-desktop-app.md)をお使いのデバイスにインストールしている場合、ブラウザーで Miro ボードを開くと、アプリでボードを開くよう勧めるポップアップが表示されます。

browser_pop-up.jpg
Miro デスクトップアプリの利用を勧めるブラウザーのポップアップ メッセージ

このポップアップを無効化したい場合は、以下の手順に従って設定を行います。

- Mac ユーザーの場合
- Windows ユーザーの場合
- Safari ブラウザーの場合

### Mac ユーザーの場合

**ステップ 1**コンピュータから Desktop アプリを削除（アンインストール）します。

**ステップ 2。**ブラウザの「常にMiroアプリでURLを開く」設定をロールバックします。Chrome と Firefox で設定をロールバックする手順を以下に示します。

*Chrome の場合：*

1. まず始めに、すべての Chrome と Miro のウィンドウを閉じます（Windows の場合、**C****md + Q** でブラウザーを終了します）。
2. Mac で Finder を開きます > **Command + Shift + G** を押します > 検索ボックスに次のパスを入力します：**~/Library/Application Support/Google/Chrome**Chrome の Profile フォルダーを開いて、Preferences ファイルを見つけます。

   このファイルを含む複数のフォルダーが存在する場合は、次の手順に従ってください：

   - Google Chrome のプロフィール フォルダーにプロフィールファイルが 1 つしかない場合は、**Default** フォルダーの中の **Preferences** ファイルを開いて検索します
   - Google Chrome に複数の Profile フォルダーがある場合、すべての **Profile X**（**X** は Profile の識別番号です）フォルダーの **Preferences** ファイルを開いて検索します
   - もし、Default、Guest Profile、Profile X フォルダーがあれば、そのすべてのフォルダーの **Preferences** ファイルを開いて検索します
3. **Preferences** ファイルをテキストエディターで開きます。
4. **`https://miro.com":\{"miroapp":true\}`** を検索します。
5. **`https://miro.com":\{"miroapp":true\}`** を削除します。
6. 変更を保存します。
7. Chrome ブラウザーを再起動します。

複数の Google プロフィールを使用している場合、すべてのカタログの Preference ファイルを編集する必要があります。これを実行するには、ステップ 2 で示した手順に従い、**~/Library/Application Support/Google/Chrome** を開き、**Profile 1、Profile 2、Profile X** フォルダーにある **Preference** ファイルをすべて変更します。

*Firefox の場合：*

1. ブラウザーの設定を開きます。
2. **「一般」**セクションで**「アプリケーション」**までスクロールダウンします。
3. **miroapp** を見つけ、ドロップダウンメニューでオプションを選択して、**「Miro を使用する」**（デフォルト）を**「常に確認する」**に変更します。

### Windows ユーザーの場合

**ステップ 1**コンピュータから Desktop アプリを削除（アンインストール）します。

**ステップ 2：[このリンクから](https://desktop.miro.com/platforms/Miro_DeleteAppSchema.reg)入手できるスクリプトを使用して、Windowsレジストリ *から値をクリアします。これが完了すると、ブラウザーのポップアップは表示されないはずです。まだポップアップが表示される場合は、ステップ 3 を実行します。***

**ステップ 3。**ブラウザの「常にMiroアプリでURLを開く」設定をロールバックします。Chrome と Firefox で設定をロールバックする手順を以下に示します。

*Chrome の場合：*

1. まず始めに、すべての Chrome と Miro のウィンドウを閉じます。
2. *PC >* **Users > \{current_user\} > AppData > Local > Google > Chrome > UserData > Default > Preferences** に**移動**します。
3. **Preferences** ファイルをテキストエディターで開きます。
4. **`https://miro.com":\{"miroapp":true\}`** を検索します。
5. **`https://miro.com":\{"miroapp":true\}`** を削除します。
6. 変更を保存します。
7. Chrome ブラウザーを再起動します。

複数の Google プロフィールを使用している場合、すべてのカタログの Preference ファイルを編集する必要があります。これを実行するには、**PC >** **Users > \{current_user\} > AppData > Local > Google > Chrome > UserData** に移動し、**Profile 1、Profile 2、Profile X** フォルダーにある **Preference** ファイルをすべて変更します。

*Firefox の場合：*

1. ブラウザーの設定を開きます。
2. **「一般」**セクションで**「アプリケーション」**までスクロールダウンします。
3. **miroapp** を見つけ、ドロップダウンメニューでオプションを選択して、**「Miro を使用する」**（デフォルト）を**「常に確認する」**に変更します。

### Safari ブラウザーの場合

Safari で表示されるポップアップを無効化するには、お使いのデバイスから Miro デスクトップアプリを削除します。
