---
title: Confluence 用の Miro
article_id: 360020712594
translation_id: 7636394663570
locale: ja
sidebar_position: 3
created_at: '2022-09-14T18:02:14Z'
updated_at: '2026-03-12T09:15:24Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: '利用可能なプラン：: すべての Miro プラン、Confluence Cloud（Miro への埋め込み）、Confluence Cloud/Server/DC（Confluence
    への埋め込み） 実行可能なユーザー：: Confluence 管理者'
---

Miro と Confluence は、2 方向同期で連携するため、どこからでも双方のプラットフォームから最新のコンテンツを確認できます。

## Miro と Confluence の連携方法

Miro ボードと Confluence ドキュメントを埋め込み、インスタント同期で変更を把握できます。該当するユーザーが常に適切な情報にアクセスできるように、埋め込みデータのアクセスレベルを設定することができます。

Confluence 文書を Miro ボードに埋め込む

Miro ボードを Confluence 文書に埋め込む

## Miro ボードに Confluence ドキュメントを埋め込む

Miro ボードにリンクを貼り付けるだけで、Miro に Confluence ドキュメントを埋め込むことができます。**ただし、Miro に Confluence ドキュメントを埋め込むには Confluence Cloud が必要です。**

初めて Confluence リンクを Miro ボードに貼り付けると、それは[Miro スマートリンク](https://help.miro.com/hc/articles/360017730993)として表示されます。Confluence リンクを初めて貼り付ける際には、Confluence へのアクセスを許可するために**接続**をクリックする必要があります。

:::warning
セキュリティー上の理由から、Miro の公開ボードには Confluence リンクの詳細は表示されず、ユーザーは非公開ボードで Confluence リンクのタイトルのみを表示できます。ユーザーが Confluence アカウントを認証したときのみ、ページのタイトルが表示されます。その後、Confluence ドキュメントを展開して編集できるようになります（提供されたアクセス権限に応じて）。
:::

![Connect_Confluence.png](https://help.miro.com/hc/article_attachments/21019705195922)*Miro で Confluence ページをリンク*

Confluence が承認されると、ボードにアクセスしたユーザーは、ドキュメントのタイトル、プロバイダーのアイコン、リンク先を表示できるようになります。 ユーザーは、Miro スマートリンクを全画面モードに拡大することもできます。

:::tip
Miro スマートリンクのタイトルは URL から抽出されます。Confluence ドキュメントのタイトルを編集する場合、Miro スマートリンクに更新されたタイトルを表示するには、リンクをもう一度貼り付ける必要があります。
:::

![Connected_Confluence_card.png](https://help.miro.com/hc/article_attachments/21019694106642)*Miro スマートリンクとしてリンクされた Confluence ページ*

ユーザーが [展開] アイコンをクリックすると、Miro 内のドキュメントを表示、編集する前に、自分の Confluence アカウントを認証するように求められます。

![Expanded_Confluence_card.png](https://help.miro.com/hc/article_attachments/21019705177490)*展開した Confluence ドキュメント*

## Confluence ドキュメントに Miro ボードを埋め込む

Miro ボードを Confluence 文書に埋め込むには、Confluence 用 Miro プラグイン または Atlassian Smart Links を直接使用します。これらは Confluence クラウド、サーバー、または DC で実行できます。

### ステップ 1： Miro プラグインを設定する

まず、[Miro for Confluence アプリ](https://marketplace.atlassian.com/apps/1217530/miro-for-confluence?tab=reviews&hosting=cloud) を Atlassian マーケットプレイスからインストールします。

**Miro for Confluence アプリのインストール方法**

> **設定者**：Confluence 管理者

1. 管理者として Confluence インスタンスにログインします。
2. 管理者のドロップダウンをクリックし、**アドオン（アプリ）**を選択します
3. **新しいアプリを探す**または**新しいアドオンを探す**を選択します
4. **Miro for Confluence** を検索
5. **アプリを取得** をクリック

![Miro_for_Confluence.png](https://help.miro.com/hc/article_attachments/21019705183122)*Confluence 用 Miro アプリ*

アプリが正常にインストールされたことを示す以下のメッセージが表示されます：

![success_message.jpg](https://help.miro.com/hc/article_attachments/22250034904338)
*アプリが正常にインストールされました*

### ステップ 2：Confluence ページにボードを埋め込む

Confluence ページに Miro ボードを埋め込むには 3 つの方法があります。

1. Confluence ドキュメントで直接 **/miro** と入力する。
   ![Typing_miro_on_the_doc.png](https://help.miro.com/hc/article_attachments/22250025101202)
   *Confluence ページに /miro と入力して、ボードを埋め込む*
2. アプリツールバーから Miro を検索する。Confluence ドキュメントから**挿入** をクリックし、アプリ一覧から **Miro** を選択します。
   ![Miro_plugin.jpg](https://help.miro.com/hc/article_attachments/22250025110290)
   *アプリリストから Miro を選択してボードを埋め込み*
3. Atlassian スマートリンクを使用して、Confluence に Miro のリンクを直接貼り付けます。

### ステップ 3：ボードピッカーからボードを選択する

ボードピッカーが開きます。ドロップダウンから埋め込みたいボードを選択するか、ボードを検索します。 ユーザーには、Miro で利用可能なボードだけが表示され、編集権限がある場合にのみボードを埋め込むことができます。

![Board_picker.png](https://help.miro.com/hc/article_attachments/21019705190162)*ボードピッカーから埋め込むボードを選択*

埋め込みボードの**開始ビュー**を選択します。

![Set-the-starting-view-for-your-embed.png](https://help.miro.com/hc/article_attachments/21019705211922)*埋め込まれた Miro ボードの開始ビューを設定*

**すべての訪問者**用の Confluence ページのアクセスレベルを選択します。

- **閲覧可能:** Confluence ページの訪問者全員がボードを閲覧できます。
- **アクセス要件:** Miro でボードへのアクセス権限を持っている人にのみ閲覧が制限されます。

![Access-level-for-embed.png](https://help.miro.com/hc/article_attachments/21019694119954)*Confluence ページ上の Miro ボードへのアクセスレベルの設定*

### ステップ 4：ボードを埋め込む

[**ボードの埋め込み**] をクリックすると、Miro のボードが iFrame として Confluence のページに挿入されます。ユーザーはボードを閲覧し、ナビゲートすることができます。

:::note
Enterprise プランで Miro をお使いの場合、アクセス権限は組織全体のアクセス設定に準ずるため、一部の権限が制限される可能性があります。詳しくは、[Enterprise プランでの埋め込まれたボードの管理](https://help.miro.com/hc/articles/4405088016274)をご覧ください。
:::

![Miro-board-embedded-in-confluence.png](https://help.miro.com/hc/article_attachments/21029914963218)*Confluence ページに埋め込まれた Miro ボード*

Miro ロゴをクリックして Miro のボードを直接開くこともできます。

![Open-embedded-board-in-miro.png](https://help.miro.com/hc/article_attachments/21029914965010)
*Miroでボードを開くオプション*

#### **ConfluenceクラウドとConfluenceサーバーのユーザーエクスペリエンス**

埋め込みボードの画面サイズメニューは、ConfluenceクラウドとConfluenceサーバーで異なります。

Confluenceクラウドでは、**全幅表示**オプションを設定できる以下の画面サイズメニューが表示されます。

![Go-full-width-Miro-board-confluence.png](https://help.miro.com/hc/article_attachments/21029914965522)
*Confluenceブラウザでの画面サイズメニュー*

Confluenceサーバーでは、画面サイズの小、中、大（**S/M/L**）を選択できるオプションを含むメニューが表示されます。

![Miro_in_Confluence_Server.jpg](https://help.miro.com/hc/article_attachments/21019694126610)*Confluence アプリの画面サイズメニュー*

## Atlassian スマートリンクで Miro ボードを埋め込む

Atlassian スマートリンク機能を使って、アプリをインストールすることなく、Miro ボードを Confluence に埋め込むこともできます。

Confluence ページに移動し、ボードのリンクを貼り付けるか、**/link** と入力して挿入します。初めてこの機能を使用する場合は、Miro のチームを接続するよう求められます。**連携してプレビュー**をクリックし、Miro で認証を行い、埋め込むボードがあるチームを選択します。

:::note
Miro と Atlassian アカウントを連携後、埋め込まれた Miro ボードのプレビューで作業できるのは、Miro 側で埋め込みボードへのアクセス権があるユーザーのみですのでご注意ください。Confluence ユーザー全員がボードのプレビューを利用できるようにしたい場合は、Miro アプリをご利用ください。
:::

![install_Atllassian_links.jpg](https://help.miro.com/hc/article_attachments/22250034923154)
*埋め込むボードのあるチームを選択*

Miro のボードのリンクを Confluence ページに貼り付けると、自動的にウィジェットに変換されます。リンクをクリックすると、表示オプションを確認できます。Miro ボードを **URL**、**インライン**テキスト、**カード**、**埋め込み** のいずれかで表示することができます。

![Confluence_widget.png](https://help.miro.com/hc/article_attachments/21019705194130)*Confluence 上の Miro ボードのウィジェット*

ボードを埋め込みとして表示する選択をした場合は、ボードの端をドラッグすることで埋め込みサイズを変更できます。

![changing_embed_size.gif](https://help.miro.com/hc/article_attachments/22250025121554)
*Confluence で Miro の埋め込みサイズを変更*

:::warning
ご利用のブラウザーでサードパーティーのクッキーがブロックされている場合、埋め込みボードを表示する際に予期せぬ問題が発生する可能性があります。
:::

## Confluence 用 Miro アプリの無効化

アプリを無効化するには、**マーケットプレイス** > **アプリの管理** > **Confluence Cloud 用 Miro** > **アンインストール**に移動します。

*![Uninstall_Confluence_plugin.jpg](https://help.miro.com/hc/article_attachments/22250034931858)*
*インストールされた Atlassian アプリリストにある Confluence 用 Miro アプリ*

## Confluence における移行とボードへの影響

オンプレミスからクラウドへのインスタンス移行、またはクラウド間の移行の場合でも、Miro プラグインには専用の移行手順は必要ありません。Confluence は iFrame を通して Miro ボードを表示します。これは URL に基づいた埋め込みであり、Confluence はボードのリンクのみを保存し、ボード自体は Miro 内に保持されます。
