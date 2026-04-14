---
title: "\u30ED\u30B0\u30A4\u30F3\u3067\u304D\u307E\u305B\u3093"
article_id: 360020993079
translation_id: 360020993079
locale: ja
sidebar_position: 9
created_at: '2021-04-09T06:31:47Z'
updated_at: '2025-11-25T16:04:24Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Miro プロフィールにログインする際に問題が発生した場合は、このガイドの手順を実行してください。

## メールおよび / またはパスワードの問題

メールアドレス / パスワードが機能しません

以下の 2 つのソリューションを試してみてください。

1. ログインに使用するメールアドレス / パスワードに入力ミスがないことを再確認します。
2. 入力した資格情報が正しい場合は、[パスワードをリセット](../../managing-your-profile/05-how-to-change-your-password.md)してください。
3. メールアドレスまたはパスワードに & " < > などの記号が含まれている場合**、**[サポートチームにご連絡](https://help.miro.com/hc/requests/new?)ください。

:::warning
メールとパスワードの入力を 10 回間違えると、**プロフィールがロックされます**のでご注意ください。まず[プロフィールをロック解除](../../tools/troubleshooting/14-profile-lockout.md)してから、パスワードをリセットする必要があるかもしれません。
:::

パスワードをリセットできません

パスワードリセットのメールが届かない場合、以下の 3 つの理由が考えられます。

1.**メールアドレスが正しくない**
送信したメールにタイプミスがないことを確認します。入力ミスがあった場合は、リセットリクエストを再送してください。

2.**メールがまだ Miro に登録されていない**
この場合は、パスワードリセットのリンクがメールアドレスに送信されません。[登録ページ](https://miro.com/signup/)で新しいプロフィールを登録してください。メールアドレスが登録されている場合、その旨メッセージが表示されます。
![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)

3.**メール配信に問題がある**

- **スパム、プロモーション、迷惑メール、ソーシャル**、**アップデート**のフォルダーを開き、リセットリクエストのメールがあるか確認してください。
- ファイアウォールがメールの受信トレイへの配信を妨げている可能性もあります。

  *システム管理者*に連絡し、Miro のドメインとサブドメイン：[miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) および [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/) を許可リストに追加し、Miro のメール送信システムの IP アドレスをユーザー側の許可リストに追加してもらえるよう依頼してください。

  専用 IP アドレスは次の通りです：198.2.178.132、198.2.178.117、198.2.128.203、198.2.178.252、198.2.178.205許可リストへの登録が必要なメーラーの詳細については、[こちらの記事](../../tools/troubleshooting/02-allowlist-miro-mailers.md)をご覧ください。

パスワードをリセットしてもログインできません

まだプロフィールにアクセスできない場合：

1. 新しいパスワードを入力したことを確認してください。
2. ブラウザーの非公開（シークレット）モードにログインするか、別のブラウザーを試してみてください。

1 つのメールでログインしても、リダイレクトされてもう 1 つ別のメールでログインしたことになります

この問題は、別の認証方法でログインしているために発生しているようです（Google、Slack、Office 365、Apple ID、Facebook）。

![new-sing-in-third-party.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)
*ログインページ上の別のログインオプション*

別のメールアドレスで登録した Miro プロフィールに、Google/Office 365 などのメールアドレスをリンクしてしまっている可能性があります。その場合は、以下の手順を試してください。

1. 間違ったメールアドレスの関連付けを削除するには、**[プロフィール設定]** > **[インテグレーション]** に移動し、Google/Office 365 などの隣の **[ログアウト]** をクリックします。
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Google ログインとの関連付けの削除*
2. ログアウト後、メールで再度ログインします。

:::note
Miro プロフィールのメールアドレスと一致する Google、Office 365、Slack のメールアドレスとの接続を設定すれば、問題を防ぐことができます。
:::

## SSO のログインが機能しません

こちらの記事をご覧ください：[「SSO ログインで発生する可能性のある問題」](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md)

## ログイン時に読み込み中が無限に続く

Miro の資格情報を入力後、読み込み中が無限に続く場合、以下の手順を実行することをお勧めします：

1. **別のブラウザー**でログインする。
2. ブラウザーの**非公開（シークレット）モードを使ってログインする。**シークレットモードや別のブラウザーで問題が繰り返されなければ、ブラウザーのキャッシュをクリアします。

   Chrome のキャッシュをクリアする方法

   1.`https://miro.com/` に移動し、Chrome の**開発者ツール**（*Mac の場合*は **Command + Option + J**、*Windows の場合*は **Ctrl+ Shift + J** ）を開きます。
   2.**[アプリケーション] > [ストレージ]** タブを選択します。**[サイトデータを消去]** という青ボタンが表示されます。  ボタンをクリックし、Chrome ブラウザーに保存された Miro のデータを削除し、新しい作業セッションを開始することができます。
   ![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
   *Chrome 内のサイトデータを消去するオプション*
3. **VPN** を使用している場合は、トグルをオフかオンにします。
4. Miro をブロックする可能性のあるファイアウォールやプロキシーを会社が使用していないか、IT 部門に確認してください。[こちらの手順](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)を実行して、**Miro を許可リストに追加**するか、バイパスを提供してください。
5. インターネットの接続を確認します。ネットワーク帯域幅が最低 8 Mb/s に達していない場合、**別のネットワーク、できれば****より高速なもの**に切り替えます。
6. 利用可能なモバイルスポットあれば、**モバイルホットスポットに接続**してみてください。次に、元のネットワークに再度接続してください。
7. それでも問題が解決しなければ、[リクエストを送信](https://miro.com/contact/recover/)し、[ブラウザーのコンソールログをサポートに送信してください。](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md)

## Miro デスクトップアプリでログインする際の問題

1. デスクトップアプリで Miro にアクセスできない場合は、ブラウザーを使ってログインしてください。それでもログインできない場合は、上記の手順を実行してください。ブラウザーで Miro にアクセスできる場合は、以下のステップを実行します。
2. アプリケーション データをリセットします。

アプリデータを Windows でリセットする方法

アプリケーション データをリセットするには、以下のスクリーンショットに表示されているように 、**[Alt] > [ヘルプ]** キーを押してください：

​![reset_app_data_on_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725434514_reset%20app%20data%20on%20Windows.jpg)
*Windows 用デスクトップアプリのアプリデータの再設定*

MS Store からダウンロードしたアプリをご使用の場合は、メニューが見つからないこともあります。その場合、アプリデータをリセットするには、Windows を開き **[設定]** > **[アプリ]** > **[アプリと機能]** > リストから **[Miro]** > **[詳細オプション]** > **[リセット]** を選択します。

この手順ですぐにリセットできない場合、**C:\Users\username\AppData\Roaming\RealtimeBoard** および **C:\Users\username\AppData\Local\RealtimeBoard** からすべてのアプリファイルを削除してください。

> **✏️** **アプリデータ**のフォルダーが非表示になっている場合は、[こちら](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5)の表示させる方法をご覧ください。

アプリデータを Mac でリセットする方法

トップメニューで Miro をクリックし、以下のスクリーンショットに表示されているように、**[アプリケーション データのリセット]** を選択します。

![reset_app_data_on_Mac.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
*Mac 上でアプリデータをリセットする*

その後、再度アプリにログインして、問題が解決されているか確認してください。

リセットですぐに問題が解決しない場合は、ファインダー ウィンドウを開き、**Command + Shift + G** を押し、**~/Library/Application Support/RealtimeBoard** 貼り付け、アプリファイルをすべて削除してください。

3. 問題が解決しない場合は、[Miro のウェブサイトから](https://miro.com/apps/)ダウンロードしたアプリの最新バージョンをご使用になっているか、確認してください。

## Google/Office 365/Slack などでのログイン

Google/Office/Slack などでログインできません

1. 標準の資格情報（メールとパスワード）を使って Miro にログインします。パスワードを忘れたか、なくしてしまった場合、[パスワードをリセット](../../managing-your-profile/05-how-to-change-your-password.md)します。
2. **[プロフィールの設定]** > **[インテグレーション]** へ移動し、Google、Office 365 などの隣りにある **[ログアウト]** をクリックして接続を再設定します。
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Google ログインとの関連付けの削除*

Google/Office/Slack などからデスクトップアプリにログインできません

これらのトラブルシューティングの手順を試してください。

Google/Office 365 などから Miro にログインしていましたが、メールサービスを変更しました。どうやったらログインできるでしょうか？

新規サービスの資格情報（メールとパスワード）を使って Miro にログインします。パスワードを忘れたか、なくしてしまった場合、[パスワードをリセット](../../managing-your-profile/05-how-to-change-your-password.md)します。

## タブレット / モバイルでログインする際の問題

1. ブラウザーバージョンにログインできるか確認してください。ログインできない場合は、こちらのトラブルシューティングのステップを実行することをお勧めします。
2. ブラウザーでログインできる場合は、デバイスの認証データが破損している可能性があります。**[アプリ設定] > [ストレージ] > [ストレージを削除]** へ移動するか、デバイスに Miro のアプリを再インストールしてください。

## トラブルシューティングのヒント

上記で問題が解決しない場合は、**別のブラウザー**または**シークレットモード**を使って Miro にログインしてください。ブラウザーのシークレット モードで問題がない場合は、ブラウザーのキャッシュと Cookie をクリアし、標準モードで Miro にログインします。

Chrome のキャッシュをクリアする方法

1.`https://miro.com/` に移動し、Chrome の**開発者ツール**（*Mac の場合*は **Command + Option + J**、*Windows の場合*は **Ctrl+ Shift + J** ）を開きます。
2.**[アプリケーション] > [ストレージ]** タブを選択します。**[サイトデータを消去]** という青ボタンが表示されます。  ボタンをクリックし、Chrome ブラウザーに保存された Miro のデータを削除し、新しい作業セッションを開始することができます。

![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
*Chrome 内のサイトデータを消去するオプション*

問題が解決しない場合は、[Miro サポートにご連絡](https://miro.com/contact/recover/)ください。問題を詳細にご説明ください。

:::note
Miro 登録の際に問題が発生した場合は、こちらの[承認コードに関する不具合](../../tools/troubleshooting/12-issues-with-confirmation-code-or-password-reset-emails.md)をご覧ください。
:::
