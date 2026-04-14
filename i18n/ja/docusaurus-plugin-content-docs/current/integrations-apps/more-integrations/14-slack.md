---
title: Slack
article_id: 360017572494
translation_id: 360017572494
locale: ja
sidebar_position: 15
created_at: '2019-02-11T10:13:25Z'
updated_at: '2025-02-26T12:10:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
---

ボードの新しいコメントやメンション、プロフィールに関連するその他の変更内容に関して、Slack から通知を受け取り、Slack 内で Miro のボードを簡単に共有すると、ボードのリンクが自動的に展開されます。この記事では、Slack を Miro に接続し、素晴らしい機能の全てにアクセスする方法をお伝えします。

:::note
Slack チャンネルに投稿された Miro のボードへのリンクをクリックすると、Slack の一部のユーザーに対して、Slack 経由で Miro にシームレスに登録することが推奨されます。現在この機能はベータ版であり、Slack が管理しています。Slack のワークスペースに Miro のアプリケーションをインストールする必要はありません。
ワークスペースの管理者には、Slack のワークスペースの設定（アプリ管理設定 > Slack の設定でサインイン）で、Slack 機能を使ったサインインを完全に無効にできるオプションがあります。/span>ベータ期間の開始時から 、Enterprise Grid Org とそのワークスペース が除外されています。
:::

:::note
Slack アプリに関するお問合せは、[slack_integration_support@miro.com までご連絡いただくか、](mailto:slack_integration_support@miro.com)[Miro サポートへのお問合せ方法](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)をご覧ください。
:::

## アプリの有効化

ユーザーは自分のプロフィールに対して Slack アプリのインテグレーションを設定します。インテグレーションを有効にするには、Miro の[プロフィール設定](../../using-miro/managing-your-profile/01-profile-settings.md)を開きます。

getting_to_profile_settings.jpg
[Miro のダッシュボードからプロフィール設定へアクセス](https://miro.com/app/dashboard/)

**インテグレーション** タブに切り替え、**Miro（Slack App）**を検索し、**[接続する]** をクリックします。

connect_Slack.jpg
Slack アプリの接続

別のオプションとして、[通知タブ](https://miro.com/app/account/profile/notifications/)で有効にすることもできます。

connect_Slack_from_notifications.jpg
通知ページで Slack アプリを有効化

リダイレクトされるので、Slack で承認します。資格情報を入力して、Slack にサインインしてください。

authorize_Slack.jpg
ワークスペースへの Miro のアクセス権を許可

## 通知の設定

通知を受けたいイベントを選択して、受け取ったフィードをカスタマイズします。

以下のイベントをチェックすることができます。

- 招待者の登録
- チームまたはボードへのアクセス権のリクエスト
- 誰かプロジェクトに自分を招待したとき
- ボードが自分と共有されたとき
- 自分のボード上での新しいコメントやボード上での自分のコメントへの返信があったとき
- 誰かがコメントで自分を @メンション、また返信したとき

[通知ページ](https://miro.com/app/account/profile/notifications/)を開き、環境設定をします。

notification_settings.jpg
通知設定

なお、通知が届くのは、*通知者が送信を決定した場合にのみ*ということもありますので、ご留意ください。

## Slack の通知への対応

ボードへのアクセス権がリクエストされた場合、Slack で認証することができます。オプションを選択し、ボタンをクリックします。

react_in_Slack.jpg
Slack チャンネルのボードへのアクセス権の付与

## ボードのリンクの展開

Miro Slack アプリの最新バージョンでは、ボード名、詳細情報、ボードのサムネイルを追加すると、Miro のボードへのリンクが展開されます。

unfurl_a_board_link.jpg
*/span>Slack チャンネルのボード名、詳細情報、サムネイル*

Slack のインテグレーションを再インストールして、その機能へのアクセス権を得ることができます。Miro の**プロフィール設定 > **インテグレーション****に移動して、**Miro のフィード（Slack アプリ）**の隣のログアウトをクリックします。次に、接続をクリックして、再認証します。

> ️✏️ 再認証するには、Slack ワークスペースの管理者から承認を受ける必要があります。

ボードのサムネイルを設定するには、Miro のボードにアクセスし、ボード左上にあるタイトルをクリックして、ボード情報カードを開きます。ポップアップ ウィンドウで、左上の画像をクリックし、デバイスから画像をアップロードするか、ボードからセクションを選択します。ボードのリンクを共有すると、サムネイルが Slack に表示されます。

change_board_thumbnail.gif
ボードのサムネイルを設定

## Slack からボードを共有

Slack でボードのリンクを投稿すると、ボードへのアクセス権がないユーザーを示す通知が表示されます。Slack 経由でボードに容易にそのユーザー招待することができます。 リンクを知っている人なら誰でも閲覧 / コメント追加できるよう、自由に[ボードを公開](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)してください。

share_from_Slack.jpg
/span>Slack から Miro ボードを共有/em>

>  オプションが利用できない場合は、設定でアプリを再インストールするか、Slack マーケットプレイスでプラグインの更新を管理者に依頼してください。

## Slack からボードを作成

Miro のショートカットを使用して、Slack 内からボードを作成することができます。Miro を検索して、**ボードの作成**を選択します。

Miro_shortcut.jpg
Slack からボードを作成

ボードのタイトルを入力して、Miro のチームを選択し、ショート メッセージを追加して、Slack 内の新規作成ボードへのリンクと一緒に送信します。

create_board_modal.jpg
/span>Slack での新規ボードのパラメーターを設定

ボードを作成すると、ボードのリンクと一緒に、チャンネル／会話にメッセージが送信されます。

new_board_message.jpg
Slack 内から新規ボードを作成した後、メッセージが投稿されます。

一部のチャンネルメンバーに新規作成ボードへのアクセス権がない場合、[Slack 内からボードを共有](#h_007785b5-df52-43e2-9eb0-ccb53b795955)するよう推奨されます。

## アプリの無効化

インテグレーションを無効にするには、**プロフィールの設定 > インテグレーション**に移動して、**ログアウトを**クリックします。

Slack_log_out.jpg
Miro のフィードの無効化

Slack からアプリを完全に削除するには、Slack の **Miro** のチャンネル設定を開き、**設定**をクリックします。

Miro_Slack_configuration.jpg
Slack 用 Miro アプリの設定

Miro のアプリ設定ページにリダイレクトされます。下にスクロールし、認証されたユーザーリストで自分の名前を検索し、**[取り消し]** をクリックします。

revoke_access.jpg
Slack への Miro のアクセス権の無効化

ワークスペースの管理者には、*ワークスペース全体*からアプリを削除するオプションも表示されます。

remove_app.jpg
Slack からアプリを削除

## よくある質問や不具合

*1.  ユーザーがMiroをSlackに追加した場合、Miroは彼らのSlackチャンネルを読むことができますか？*
- いいえ、Miroはワークスペースのパブリックチャンネルに関する基本的な情報を見るだけです。つまり、Miro はチャンネル名リストを読み取ることができますが、チャンネル メッセージを読み取ることはできません。

2. *Miro Feed for Slackに接続しようとすると、「Something went wrong」というメッセージが表示されます。*
- お使いのブラウザがMiro.comドメインからのポップアップを許可しているかどうかご確認ください。アプリの権限を求める別のページがあるかもしれません。/span>

3. 3. *Miro-Slack の通知が届かず、Slack に Miro のアプリを再インストールしても解決しません。*解決方法を教えてください。
- Miro側でMiroとSlackを再接続してみてください**（プロフィール設定[>インテグレーション](https://miro.com/app/account/profile/integrations/)**）。
