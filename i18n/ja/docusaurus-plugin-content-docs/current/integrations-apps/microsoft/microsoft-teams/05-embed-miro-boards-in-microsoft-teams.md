---
title: "Microsoft Teams\u3078\u306EMiro\u30DC\u30FC\u30C9\u306E\u57CB\u3081\u8FBC\u307F"
article_id: 360017572514
translation_id: 360017572514
locale: ja
sidebar_position: 5
created_at: '2019-02-11T10:13:30Z'
updated_at: '2025-04-24T13:52:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ms-teams
---

Microsoft Teams チャネルに Miro を埋め込み、チームメンバーとの共有をシームレスにしましょう。Miro のボードが手近にあれば、チーム全体の共通認識を確実にします。

:::note
Microsoft Teams MeetingsにMiroボードを埋め込む方法を確認してください：[Miro for Microsoft Teams Meetings (管理者ガイド)](01-miro-for-microsoft-teams-admin-guide.md)、[Miro for Microsoft Teams Meetings (ユーザーガイド)](02-miro-for-microsoft-teams-user-guide.md)。
:::

> **利用可能なプラン：**すべての Miro プラン

### プラグインをインストールする

まず、**Microsoft Teams ストア** で **Miro** を検索するか、[直接リンク](https://teams.microsoft.com/l/app/8216e453-3db5-48ee-a3d6-5122f505c8a3)をたどってください。

:::warning
なお、Microsoft Teams 側のテナント管理者は、Teams のサードパーティー アプリのカタログで Miro のアプリを有効にする必要があります。 Miro が承認されない限り、Microsoft Teams ストアのアプリには表示されることはありません。
:::

[**追加**] をクリックしてプラグインをインストールします。

Miro_plugin_installation.jpg
Miro のプラグイン インストール

Miro のプラグインをインストールすると、チャットにリダイレクトされます。そこで Miro の通知受信の設定ができます。詳細は、[こちらの記事](10-miro-notifications-in-microsoft-teams.md)をご覧ください。

追加設定をしなくても、その時点で Microsoft Teams チャネルに Miro のボードの埋め込み開始が可能です。

### Microsoft Teams チャネルにボードを埋め込む

> **設定者：**ボードが所在するチームのメンバーである[ボード所有者](../../../using-miro/sharing-boards/01-board-access-rights.md)と[ボード編集者](../../../using-miro/sharing-boards/01-board-access-rights.md)

新しいタブを作成することで、 Microsoft Teams チャネルにボードを埋め込むことができます。プラスアイコンをクリックしてください。さまざまなアプリがリストされたピッカーが表示されます。アプリのリストから Miro を検索し、選択します。同じブラウザー上、またはデスクトップ アプリ内の Miro で認証がされていない場合、ログインが必要です。**[Get Started]**（始める） をクリックしてログインするか、[Miro で登録](../../../getting-started/start-here/02-how-to-register-with-miro.md)してください。

embed_in_MS_teams.gif
Miro プロフィールの認証を促すモーダルウィンドウ

認証されると、Miro のボードでピッカーが表示されます。ピッカーには、Miro 側でアクセスできるボードが表示されます。なお、Miro と Microsoft Teams ではそれぞれ異なるメールアドレスでの認証が可能です。

Microsoft チーム チャンネルに追加したいボードを選択してください。

![MS_teams_embed_picker.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734978322_MS%20teams%20embed%20picker.jpg)
Miro のボードを使用したピッカー

チームメンバーであるボード所有者とボード編集者のみが Miro のボードを埋め込むことができることにご注意ください。必要なアクセスレベルを持たないボードを選択すると、警告メッセージが表示されます。

unable_to_embed_boards.jpg
ボードの埋め込みを許可するアクセスレベルがないことを警告するメッセージ

次に、会議参加者のアクセス権限を設定し、ボードへのアクセス権を付与または制限することができます。以下のアクセス権タイプから選択できます。

- **全員が編集可**（ログイン不要）
- **全員がコメント可**（ログイン不要）
- **全員が閲覧可**（ログイン不要）
- **非公開**

sharing_level.jpg
埋め込みボードのアクセス設定

> ️ Miro でボード設定された共有設定は、Microsoft チーム内のボードアクセスも定義することになりますのでご注意ください。ボードが Miro で全員に公開されている場合は、Microsoft Teams でボードを非公開/span>として埋め込んでいても、Teams 内の誰もが利用できます**。**また、Miro 側のボードが非公開で、Teams に全員が閲覧 / コメント / 編集可で埋め込む場合は、Miro 上でのボードアクセスには影響を与えません。/span>詳細はこちらをご覧ください。

> ️✏️ [Enterprise プラン](../../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md)の Miro ユーザーの場合、アクセス設定は組織全体のアクセス管理に準ずるので、共有オプションの一部は制限されている可能性があります。さらに詳しい情報：[インテグレーションの埋め込みに関する Enterprise 共有ポリシーの管理](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)

> **⚠️ [無料チーム](../../../plans-billing/miro-plans/09-free-plan.md)のボードを埋め込む場合は、全員がコメント可のオプションはありません。**

ボードが埋め込まれるとすぐに使用を開始できます。

Miro_embed_in_MS_teams.jpg
Microsoft チーム チャンネルに埋め込まれたボード

> *✏️ ️*️Microsoft Teams のモバイルアプリで Miro を使用する Microsoft Teams のユーザーは、設定された権限に応じて、ボードの閲覧やコメントができます。ボードを編集するためには、ユーザー インターフェイスを最適化した Miro の[モバイル ネイティブアプリ](../../../getting-started/apps-for-devices/08-mobile-app.md)をインストールすることをお勧めします。

Miro_in_MS_Team_on_mobile.jpg
**モバイル MS Teams 上の Miro ボード — [Open in the app]（アプリで開く）をタップして、Miro のモバイル ネイティブアプリをインストール**

### よくある質問

1. *Microsoft Teams に埋め込まれたボードを閲覧するには、各チームメンバーに Miro のプロフィールが必要ですか？*
   **ー ボードを埋め込む際に、全員が閲覧 / コメント / 編集可を選択すると、登録されていないユーザーもボードを閲覧やコメントをすることができます。**また、Miro 側でボードが[公開共有](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)されている場合は、Microsoft Teams 内の全員が利用することができます。
2. *ボードの埋め込み後、MS Teams でボードのアクセスを変更できるのは誰ですか？（例：「全員が閲覧可」から「非公開」への変更）*
   ー 加えられたボードへのアクセスを変更することはできません。そのボードを加えた本人でも変更できません。ただし、タブで **[設定]** をクリックして、同じタブで別の（もしくは同じ）ボードを選択し、そのボードで別のアクセスレベルを選択することは誰にでも可能です。
3. *メールを 2 つ Miro に登録しており、2 番目の Miro プロフィールから Miro ボードを埋め込みたいのですが、*Miro プロフィールを切り替える方法を教えてください。
   ー Miro に認証されたユーザーのボードは、同じブラウザー内でピッカーに表示されます。別のブラウザーのタブで Miro を開き、ログアウトしてから、2 番目の Miro プロフィールにログインします。
   Microsoft Teams のデスクトップアプリを使用する場合は、アプリからログアウトします。すると、アプリ内の Miro からもログアウトされることになります。次にアプリにログインし、[ボードの埋め込み](#h_5af20ae6-78c0-4e6c-ab20-e4968c89c97f)をしてください。Miro のログイン画面が表示され、別の Miro プロフィールでログインすることができます。
