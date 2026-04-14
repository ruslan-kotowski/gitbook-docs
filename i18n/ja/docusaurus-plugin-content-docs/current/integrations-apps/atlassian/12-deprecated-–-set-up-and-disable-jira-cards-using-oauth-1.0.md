---
title: 非推奨 – OAuth 1.0 を使用した Jira カードの設定と無効化
article_id: 360019501754
translation_id: 7488397683602
locale: ja
sidebar_position: 14
created_at: '2022-09-05T14:57:29Z'
updated_at: '2025-11-25T16:03:55Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '利用可能なプラン：: Jira Cloud、Jira Server（オンプレミス）、Datacenter（LDAP 保護も適用） 設定者：: プロジェクト管理権限を持つ
    Miro チーム管理者および Jira システム管理者'
---

:::note
次の OAuth1.0 認証方法は、2025 年 7 月 31 日より Miro でサポートされなくなります。OAuth1.0 は[Jira の非推奨の認証プロトコル](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively.)であり、使用しないでください。この変更は、セキュリティーのベストプラクティスに沿って推奨される OAuth2.0 への広範な移行の一環です。ユーザーには、Miro のサービスのサポートと互換性を確保するために、OAuth2.0 への移行を推奨します。
:::

## Jira での Miro の設定

:::warning
技術的な問題が発生した場合、[起こり得る問題と解決方法](https://help.miro.com/hc/articles/360017572654)についての記事をご覧ください。
:::

:::tip
Jira カードについては、[Jira カードの FAQ](https://help.miro.com/hc/articles/360013463739) と [Jira カードの WebHook の設定方法](https://help.miro.com/hc/articles/360017731113)の記事をご覧ください。
:::

Jira Cloud のセットアップ Jira Server と Jira Data Center

:::note
Jira のメニューは、使用している Jira バージョンによって異なる場合がありますが、一般的なフローは同じであるべきです。以下の手順は、[Atlassian サポート](https://confluence.atlassian.com/adminjiraserver071/using-applinks-to-link-to-other-applications-802592232.html)でも確認できます。
:::

### ステップ 1 - アプリケーションリンク

まず、アプリケーションのリンクを作成し、設定します。

1. Go to **Jira の設定** > **プロダクト** > **インテグレーション** > **アプリケーションのリンク** > **リンクの作成
   ![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)***Jira インターフェイスは、Jira のバージョンによって異なる場合があります。*
2. **ダイレクト アプリケーション リンク** を選択し、**アプリケーション URL** フィールドに `https://miro.com/` と入力します。
   重要：URL をこの正確なフォーマットに入力する必要があります。**続行**をクリックします。
   ![mceclip2.png](../../../../../../docs/integrations-apps/atlassian/images/21017004818066_mceclip2.png)
    *リンクの作成*
3. 次のメニューで、**続行** をもう一度クリックするだけです。
4. **レビューリンク**メニューで、URL がまだ正確に`https://miro.com/`であることを再度確認し、お好みの**アプリケーション名**を入力します。スクロールダウンして、一番下の**受信リンクを作成**ボックスにチェックを入れます。*残りのフィールドをスキップ*し、**続行**をクリックします。
   ![mceclip3.png](../../../../../../docs/integrations-apps/atlassian/images/21017004819346_mceclip3.png)  *アプリケーション名フィールドの入力のみ必須です*
5. ここに、Miro の値のフィールドが表示されます。値を取得するには、Miro にログインしてください。
   - チームレベルのインテグレーションには、**[チーム設定](https://help.miro.com/hc/articles/360021841280)** > **アプリとインテグレーション** > **Jira カード** に移動します。
   - 組織レベルのインテグレーションを行うには、[**会社設定**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **アプリ** > **アプリを管理** > **Jiraカード** > **設定**に進みます。
     > まだアプリリストに Jira カードがない場合は、セクションの上までスクロールして、**アプリをインストール**をクリックし、Miro マーケットプレイスからアプリのインストールに進んでください。リストに Jira カードが表示されたら、クリックして開きます。


     プラグインタブが開き、**ステップ 1** が表示されて、必要な値を取得することができます。

     ![Jira_Cards_values.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017515668626_Jira Cards values.jpg)*Jira カードの値*
     値をコピーし、Atlassian **レビューリンク** メニューに追加します。
6. 1 ～ 2 秒間、処理メッセージが表示されます。
   ![mceclip4.png](https://help.miro.com/hc/article_attachments/26579050606610)
    *リンク作成の最終ステップ*

これで、Atlassian 側での手順は完了です。このリンクは、アプリケーション リンクのリストに表示されます。

### ステップ 2 - 接続

Miro の Jira カード設定に戻り、手動で Webhook を作成するか、自動で作成するか、2 つのオプションのどちらかを選択します。手動で選択する場合は、オプションのチェックを外してください。詳細については[こちらの記事](https://help.miro.com/hc/articles/360017731113)をご覧ください。プラグインが大幅に更新された際にリセットする必要がないよう、自動 Webhook を使用することを強くお勧めします。

最後に、Jira の URL を入力し、**接続**をクリックします：

![step_2.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017528650898_step%202.jpg)*Jira カードの接続*

Jira の URL を取得するには、Jira インスタンスのベース URL をコピーしてください。Miro では以下の形式を利用できます：

`https://your-server.example.com/`
[https://your-server.example.com/
https://your-ip-address/](https://your-server.example.com/)[https://your-ip-address/](https://your-server.example.com/)

Jira の URL が受け入れられない場合は、[こちらの記事](https://help.miro.com/hc/articles/360017572654)をご覧ください。また、Miro が Jira に対して十分なアクセス権を持っていることを確認して、[接続を確立](https://help.miro.com/hc/articles/360017572694)できるようにしてください。

これで Miro チームに Jira インスタンスを接続しました。

:::warning
Atlassian は 2024 年 2 月に Jira Server のサポートを終了しましたが、Miro は今後も Jira Server 用の Jira カード インテグレーションをサポートし続けます。
:::

1. `https://your-jira-server/plugins/servlet/applinks/listApplicationLinks`[に移動します。](https://your-jira-server/plugins/servlet/applinks/listApplicationLinks)「アプリケーション リンク」が選択されていない場合、それをクリックします。![jira_server_create_application_links.png](../../../../../../docs/integrations-apps/atlassian/images/21017515683858_jira_server_create_application_links.png)*Jira Server アプリケーションリンク*
2. **リンクを作成**をクリックします。「Atlassian 製品」を選択し、**アプリケーション URL**「https://miro.com」を入力します。**続ける**をクリックしてください。 ![jira_server_create_link.png](../../../../../../docs/integrations-apps/atlassian/images/21017528656274_jira_server_create_link.png)*アプリケーション URL の設定*
3. 「リンクアプリケーション」ダイアログボックスに移動します。**アプリケーション名**（例：Miro Jira カード）を追加し、**アプリケーションタイプ**には「汎用アプリケーション」を選択します。
   "ここからリンクを作成しています:" の下に Jira アプリケーション URL が表示され、「このアプリケーションへのリンク先:」の下には `https://miro.com` が表示されます。**続行** をクリックします。![jira_server_link_applications.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017528658834_jira_server_link_applications.jpg)*アプリケーションのリンク設定*
4. リンクの設定を処理します。完了すると、「アプリケーション リンク」エリアに新しいリンクが Jira サーバーに表示されます。![jira_server_application_links_created.png](../../../../../../docs/integrations-apps/atlassian/images/21017515685522_jira_server_application_links_created.png)*Jira Server で設定されたアプリケーション*
5. 次に、アプリケーションの詳細を設定する必要があります。アプリケーションの詳細を編集するには、アプリケーションの鉛筆アイコンをクリックしてください。
6. 構成ダイアログボックスで、**受信認証**オプションをクリックします。**Consumer Key、Consumer Name、公開鍵**を入力し、必要に応じて説明を追加します。
   - チームレベルのインテグレーションに関する情報は、[**チームの設定**](https://help.miro.com/hc/articles/360021841280) > **アプリとインテグレーション** > **Jira カード** で確認できます。
   - 組織レベルのインテグレーションについては、[**会社設定**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **アプリ** > **アプリの管理** > **Jiraカード** > **設定**でこの情報を利用できます。
     ![jira_server_config_oauth.png](../../../../../../docs/integrations-apps/atlassian/images/21017528687506_jira_server_config_oauth.png)*Jira Server での受信認証詳細の設定*
     ![jira_webhooks_jira_server_config.png](../../../../../../docs/integrations-apps/atlassian/images/21017515686418_jira_webhooks_jira_server_config.png)*Miro での Jira アプリケーションリンクの詳細*
7. 受信認証オプションの最後までスクロールして、**保存**をクリックします。あなたの認証ステータスは現在確認されているはずで、この Jira サーバーは Miro 内で Jira カードと共に使用できるようになりました。Miro 側で「Jira Server」と「OAuth 1.0」を選択してください。![jira_server_welcome_to_jira.png](../../../../../../docs/integrations-apps/atlassian/images/21017515690258_jira_server_welcome_to_jira.png)

### ユーザー認証

インテグレーションが接続されたら、各エンドユーザーは個人の Jira プロフィールを接続して適切なアクセス権を確立する必要があります。これにより、Miro 側の各ユーザーのアクセスが、 *Jira インスタンス側と全く同じになります*。エンドユーザーが Jira カードを初めてインポートまたは編集しようとする場合、個人のユーザー資格情報を使用して Jira へログインするよう求められます。

これでホワイトボードにタスクをカードとして追加することができます。Jira で行われた変更はすべて、ボード上の Jira カードに反映されます。

:::note
ユーザーが Jira 資格情報を持っておらず、カードが追加されたボードへのアクセス権を持っている場合、カードのタイトル、課題の種類、優先度、担当者、Jira カードに表示されるように設定されているすべての属性が表示されます。ただし、許可しない限り、カードを展開して、他の属性を表示したり、カードを編集したりすることはできません。ユーザーが Jira 認証情報を接続しない場合、担当者のアバターは表示されず、カードの一般的な外観も異なるものとなります。
:::

### 複数の Miro チームに Jira の 1 つのインスタンスを使用

カードはチームレベルまたは組織レベルにインストールできます。複数のチームがある場合、組織レベルの設定を活用して、各チームごとに設定手順を繰り返すことを避けることができます。既存のアプリケーション リンクはすべてのチームで使用されます。

チームまたは組織を Jira インスタンスに接続すると、その Miro チームまたは組織に対して Jira WebHook に新しい Webhook が作成されます。Webhook を作成すると、更新リクエストのチャネルを確立します。

組織レベルの設定を指定すると、すでに接続されているチームは現在の設定を保持します。ただし、いつでも組織レベルの設定に切り替えることができます。

さらに、必要であれば、チームは組織単位の設定を上書きして、別の Jira インスタンスに接続することができます。

複数のチームレベルの接続をデフォルトの組織レベルの接続に移行したいという Enterprise のお客様は、アカウントチームにお問い合わせください。

:::warning
複数のチームを個別に接続する場合は、各チームの Webhook に固有の名前を付けることをお勧めします。Jira Webhook ページに移動して、新しく作成された各 Webhook を編集します。
:::

複数の Jira インスタンスを 1 つの Miro チームに接続することはサポートされていません。

## プラグインの無効化

チームレベルのインテグレーションを行うには、**チームの設定** > **アプリとインテグレーション** > **Jira カード** に移動します。次に**チームから削除**を選択します。

組織レベルのインテグレーションで Jira アプリの使用を制限するには、**会社の設定** > **アプリ** > **アプリの管理** > **Jira カード** に移動します。その後、トグルをオフの位置に移動します。

:::warning
組織内で Jira を無効化すると、すべての Enterprise チームのユーザーが Jira カードを使用できなくなります。アプリ管理と制限について詳しく知りたい場合は、[アプリ管理](https://help.miro.com/hc/articles/4404659741458)をご覧ください。
:::

**詳細情報：**[Jiraカードの使い方](https://help.miro.com/hc/articles/360017572434)を参照してください。
