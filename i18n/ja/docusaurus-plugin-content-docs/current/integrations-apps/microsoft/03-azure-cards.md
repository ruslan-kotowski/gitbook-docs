---
title: Azure カード
article_id: 360033799934
translation_id: 360033799934
locale: ja
sidebar_position: 4
created_at: '2019-08-13T10:01:30Z'
updated_at: '2025-11-25T16:05:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: azure-cards
availability:
  notes: 'ユーザー: 全ユーザー プラン：: Business、Enterprise プラットフォーム：: ブラウザー、デスクトップ、モバイル'
---

Azure カードを使うと、Azure ボード（Azure DevOps サービスの一部で、旧 VSTS - クラウド ソリューション）から作業項目を Miro ボードにインポートすることができます。リモートでのふりかえり、ストーリーサイジング、バックログの優先順位付け、ストーリーマッピング、その他のチーム活動において欠かせない存在となるでしょう。Miro のカンバンやユーザー ストーリー マッピングのフレームワークで使用することもできます。

Azure カードは、Azure ボードと直接統合することで、さまざまなチームアクティビティのためのシームレスなワークフロー管理を実現し、Miro の体験を強化します。

## 主な機能

Azure カードのインテグレーションは、いくつかの主要な機能を提供します。

- アプリ内の Azure ボードの作業項目ピッカーを活用して、Azure カードをインポートします。これには、様々な並び替え機能が含まれます。
- このアプリ内ピッカーで、Azure ボードの作業項目を検索します。
- 自動化された読みやすいカード表示がズームインやズームアウトする際に変わります

:::note
Azure カードが常に更新されるようにカードポーリングを設定しましょう。これにより、[webhook](../atlassian/14-how-to-set-up-webhooks-for-jira-data-center.md) が失敗しても、ユーザーは常にカードの更新を受け取ることができます。
:::

## Azure カードのインテグレーションを設定する

設定には以下の 2 段階が必要です。

1. このアプリはすべてのチームに対して組織レベルで追加するか、特定のチームに対してチームレベルで追加する必要があります。
2. アプリが追加された後、Azure カードをインポートするために、インテグレーションを個人レベルで接続し、認証する必要があります。

このプロセスには、Miro と Azure DevOps の両方で特定の管理者権限が必要です。

:::note
Miro で Azure カードを正常に設定するには、**Azure 管理者と Miro 管理者が同じアカウントである必要があります**。

Azure カードを追加するには、Miro のチームまたは会社の管理者権限**と**、Azure Boards のプロジェクトコレクション管理者グループ権限が必要ですが、接続完了後にそれらの権限をダウングレードすることができます。ただし、管理者を削除することはできず、Azure プロジェクトへのアクセス権を引き続き保持する必要があります。
:::

### 組織またはチームに Azure カードを追加する

Miroの会社管理者はすべてのチームにAzureカードを追加でき、チーム管理者は自分が管理する特定のチームに追加できます。このステップにより、Azure カードアプリの接続が可能になります。

:::note
Azure カードをチーム単位で連携するには、チームの管理者であることが必要です。
:::

1. **プロフィール設定** に移動します（メインメニューのハンバーガーアイコンをクリックして **プロフィール設定** を選択するか、ダッシュボードから右上にある自分のアバターをクリックして **設定** を選択します）。
2. **アプリ** をクリックし、右側の **アプリを追加** タブに移動します。
3. 「Azure カード」と入力して、ドロップダウンリストから選択します。**追加**をクリックします。
4. 次のダイアログボックスで、**すべてのチーム** または **特定のチーム**（必要に応じてチームを選択）を選択し、**次のステップ** をクリックします。
5. 「Azure カードを確認して追加」画面で、**追加** をクリックします。アプリが会社またはチームに追加されます。
6. **「アプリを管理」**タブに移動し、Azure カードを検索して、**「承認」**をクリックします。これでアプリが会社またはチームレベルで承認されるようになりました。
7. 次に、Azure 組織を Miro に接続します。アプリパネルから、**アプリを管理**に移動します。
8. アプリリストで「Azure Cards」を検索し、**設定**をクリックします。
9. Azure カードの設定パネルで、**Azure インスタンス**の URL を追加し、**接続**をクリックします。Microsoft Azure のログイン資格情報を入力してください。
10. 認証ダイアログボックスで、**Accept**（受諾）をクリックして、Azure を Miro に接続を完了します。

### 特定のチームにカスタムの Azure Cards 設定を適用する

特定のチームに対して、グローバルな会社レベルの設定とは異なる設定が必要な場合、チーム管理者はチーム**アプリとインテグレーション**エリアでこれを設定できます。

1. プロフィール設定ページから、**チーム**をクリックします。
2. カスタム設定を適用したいチームをクリックします。
3. チームパネルで、**アプリとインテグレーション**をクリックします。
4. **Azure カード**を見つけ、クリックします。
5. アプリ設定パネルで、右側のドロップダウンから**カスタム設定を適用**を選択し、カスタム設定したい Azure アカウントに接続します。
6. Microsoft アカウントで Azure DevOps 上の Miro を認証: 「Microsoft アカウント」の横にある **接続** をクリックして Microsoft アカウントにログインし、Miro で使用できるようにします。
7. **Azure 組織 URL** を入力し（Azure DevOps からコピーできます）、**接続** をクリックします。Miro は、インスタンスのパーソナライズされた URL または、インスタンス名で終わる一般的な`https://dev.azure.com/`アドレスのどちらかを受け入れます。
   ![特定のチーム用にカスタム Azure Cards 設定を適用する方法を示すアニメーション。](https://help.miro.com/hc/article_attachments/21017042730130)
   *特定のチームにカスタム Azure カード設定を追加する*

### Azure カードを利用するには、個人の Azure アカウントをリンクしてください。

Miro の管理者がアプリをインストールして承認した後、Azure カードを使用したい各チームメンバーは、自分の Azure アカウントへの接続を個別に承認する必要があります。これにより、カードピッカーがパーソナライズされ、ユーザーがアクセスできるすべての Azure の作業項目をインポートできるようになります。

作成ツールバーで Azure カードのアイコンを見つけることができます。アイコンが表示されない場合は、検索する必要があるかもしれません。

1. 作成バーで、**ツール、メディア、インテグレーション**（**+**）を選択します。
   **ツール、メディア、インテグレーション**パネルが開きます。
2. **ツール**タブで、Azure カードを検索して選択します。

アカウントをリンクするには:

1. ツールバーの Azure Cards アイコンをクリックします。ポップアップが表示され、**承認**を求められます。
2. **認証**ボタンをクリックし、**次へ**をクリックします。[チーム設定] > [アプリとインテグレーション] ページに移動します。
3. アプリ設定パネルを使用して、Microsoft アカウントを Miro に接続し、使用したい Azure インスタンスを指定します。この URL は Azure DevOps からコピーできます。Miro は、インスタンスのパーソナライズされた URL またはインスタンスの名前で終わる一般的な `https://dev.azure.com/` アドレスを受け入れます。
   ![Miro アプリ設定で Azure 組織 URL を指定する。](../../../../../../docs/integrations-apps/microsoft/images/21017013107730_org%20URL.jpg)

:::note
初期のチームまたは会社レベルの設定を行えるのはチーム管理者のみであることにご注意ください。管理者設定の際に Azure 組織 URL のための **接続** ボタンが表示されない場合は、 [チームの管理者権限を有している](../../administration/user-management/06-how-to-manage-admin-roles.md) ことを確認してください。
:::

## Azure の作業項目を Miro ボードにインポートする

Azure Cards アプリを設定し、個人アカウントを接続したら、接続されたチームに関連付けられた Miro の任意のボードに Azure の作業項目をインポートできます。この方法を行うには 2 つの主要な方法があります。

- Azure の作業項目の URL をコピーして、Miro ボードに直接貼り付けます。このアイテムは自動的に Azure カードに変換されます。
- Azure カード ピッカーを使用:ツールバーの **Azure Cards** アイコンをクリックしてピッカーを開きます。

  ![Azure Cards picker interface in Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017013109010_Azure%20cards%20picker.jpg)*Azure カードピッカー*

  ピッカーはすべての項目の検索に対応しており、タイトル、タイプ、ステータスなどでカードを見つけることができます。Microsoft の[キーワード検索](https://docs.microsoft.com/azure/devops/project/search/get-started-search?view=azure-devops#start-your-search-with-a-keyword)機能を活用することもできます。

  ![Animation showing search functionality within the Azure Cards picker.](../../../../../../docs/integrations-apps/microsoft/images/21017013114002_Azure%20Cards%20picker.gif)*ピッカーで Azure カードを検索*

  プロジェクト、担当者、種別、エリア、ステータスでカードをフィルターでき、Miro 内で Azure の作業項目を高度にフィルターすることができます。

  ![Filtering options within the Azure Cards picker.](../../../../../../docs/integrations-apps/microsoft/images/21017013116306_filter.jpg)*ピッカーで Azure カードを絞り込む*

  Azure の元の作業項目に移動するには、ボード上のカードを選択して、そのコンテキストメニューで **ソース** ボタンをクリックしてください。

  ![Source button on an Azure Card linking to the item in Azure DevOps.](../../../../../../docs/integrations-apps/microsoft/images/21017042632338_card%20spurce.jpg)*カードのソース ボタン*

  Azure カードはスタンドアロンのボードウィジェットとして、またはインタラクティブな[カンバン](../../using-miro/advanced-tools/02-columns-formerly-kanban.md)や[ユーザーストーリー マップ](../../using-miro/advanced-tools/07-user-story-mapping.md)のフレームワークのコンポーネントとして使用できます。Azure カードをドラッグして、これらのフレームワークに追加することができます。

  ![Animation showing Azure Cards being used within a Miro Kanban board.](../../../../../../docs/integrations-apps/microsoft/images/21017042632850_Azure%20cards%20and%20kanban.gif)*カンバンでの Azure カードの操作*

## Miro で Azure カードを直接作成および編集

Miro と Azure DevOps の双方向インテグレーションにより、チームは Miro ボードから直接新しい Azure 作業項目を作成したり、既存の項目を編集したりすることができます。既存の Miro カードや付箋を Azure カードに変換することもできます。

### 新しい Azure カードを作成する

Miro から新しい Azure の作業項目を作成するには：

1. 作成ツールバーで**Azure カード**を選択し、ピッカーの右上にある**作業項目の作成**を選択します。
2. カードフィールドに入力し、プロジェクト、項目の種類、担当者を選択して**作成**をクリックします。新規アイテムは、Azure DevOps ディレクトリーおよび Miro ボードにも作成されます。

![Animation showing the process of creating a new Azure Card from Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017042635282_create%20an%20Azure%20Card.gif)*Miro で Azure カードを作成*

### Miro カードや付箋を Azure カードに変換

既存の Miro カードまたは付箋を Azure カードに変換するには：

1. ボード上の付箋またはカードを選択します。
2. オブジェクトのコンテキストメニューで、変換オプション（通常は Azure DevOps のアイコンまたは "Azure 作業項目に変換"）をクリックします。
3. ダイアログでカードのパラメーター（プロジェクトや項目タイプなど）を設定し、**変換**をクリックします。付箋 / カードのテキストはカードのタイトルに変換されます。

> **💡** 付箋や Miro カードを Azure カードに一括変換することで時間を節約できます。クリックしながらドラッグして変換したいオブジェクトをすべて選択し、コンテキストメニューで**Azure の作業項目に変換**を選択します。

![Converting a Miro sticky note into an Azure Card.](../../../../../../docs/integrations-apps/microsoft/images/21017013125650_convert%20a%20sticky%20into%20an%20Azure%20Card.jpg)*付箋を Azure カードに変換*

### Azure カードを編集

Miro で Azure カードを編集するオプションは、ツール間を切り替える手間を省きます。カードを編集するには：

1. Miro ボードで Azure カードをクリックします。
2. カードのコンテキストメニューの **ペンアイコン（編集）** をクリックします。ポップアップウィンドウが開き、項目のフィールドを編集できるようになります。
3. **更新** をクリックして変更を保存します。変更は Azure DevOps にも反映されます。

![Editing an Azure Card's details directly within Miro.](https://help.miro.com/hc/article_attachments/21017042712978)*Miro で Azure カードを編集するオプション*

### Azure カードの色を変更

ボード上の Azure カードの外観をカスタマイズするには、

カードの塗りつぶしの色を変更するには、カードをクリックして、コンテキストメニューから**塗りつぶす色**を選択します。カードを複製すると、コピーしたカードはすべて同じ塗りつぶしの色になります。

## Azure カードのインテグレーションをアンインストールする

Azure カードのインテグレーションが不要になった場合は、アンインストールすることができます。チームレベルでアンインストールするには、チームの管理者権限が必要です。

1. **チームの設定 > [アプリとインテグレーション] > [Azure カード]**に移動します。
2. 下にスクロールし、**チームに対してアンインストールする** をクリックします。
3. Azure カードを個人アカウントのみでアンインストールするには、**アンインストールする** をクリックします。

![Options to uninstall Azure Cards for the team or for an individual user.](../../../../../../docs/integrations-apps/microsoft/images/21017042628370_uninstall%20Azure%20cards.jpg)*アプリをチーム全体または個別にアンインストールします*

## サポートされている Azure カードフィールド

Miro の Azure カードでサポートされているフィールドは次のとおりです。

- タイトル
- プロジェクト
- 種類
- 状態
- 説明（編集はサポートされていません）
- 親 WI
- 担当者
- 優先度
- ストーリーポイント
- エリア
- イテレーション
- 受け入れ基準

カスタムフィールドはサポートされていません。

## Azureカードのトラブルシューティング

Azure カードのインテグレーションに問題が発生した場合は、以下の一般的な問題と解決策をご参照ください。

URL が無効です

設定された URL が正しくありません。スペルと書式設定を確認してください。たとえば、Azure 組織のアドレスは、スラッシュで終わる必要があります。

Azure 組織の URL にアクセスできません

設定した URL が存在しません。既存の URL を入力するか、スペルを確認してください。また、次のことを確認してください:

- 組織で第三者認証の受け入れが許可されていることを確認してください：「**組織の設定 > ポリシー（セキュリティ）** **>**」で「OAuth を介したサードパーティー アプリケーションのアクセス」が有効になっていることを確認します。
- Azure 組織が非公開ネットワーク上にあるか、会社のファイアウォールが外部ネットワークへの接続をブロックしています。ファイアウォールと VPN の設定に必要な変更をおこない、miro.com*、*.miro.com、mirostatic.com*、*.mirostatic.com、realtimeboard.com*、*.realtimeboard.com、*static.miro-apps.com ドメインを許可リストに追加してください。プロキシを使用する場合は、アクセスを許可するように逆設定してください。設定の**Azure DevOps URL**フィールドには、必ずアクセス可能なアドレスを入力してください（入力されたアドレスは、制限された Azure DevOps の実際のアドレスとは異なる場合があります）。プロキシサーバーのタイムアウト値を長くすることもできます。
- インテグレーションへのリクエストはすべて、Amazon のロードバランサーを通過するので、Miro から特定のネットワーク情報を提供することはできません。

サービスフック サブスクリプションを作成できませんでした

現在 Azure にログインしているユーザーには、必要な権限がありません。Azure インスタンスの代理として Miro に接続される Azure ユーザーは、これらの REST API メソッドへのアクセス権を持っていなければなりません。

- [*サービスフック サブスクリプションを作成する*](https://docs.microsoft.com/rest/api/azure/devops/hooks/subscriptions/create?view=azure-devops-rest-6.0)（「*vso.serviceendpoint_manage」*[スコープ](https://docs.microsoft.com/azure/devops/integrate/get-started/authentication/oauth?view=azure-devops#scopes)が必要です）
- [*プロジェクトに関するメタデータを受信する（この情報は、サブスクリプション イベントの作業項目を正しく指定するために使用される）*](https://docs.microsoft.com/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-6.0)
- *インテグレーションを使用するすべてのユーザーがアクセスできるようにするためには、以下のメソッドも必要です。*
  - [*アイテムを取得*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/get%20work%20item?view=azure-devops-rest-6.0)
  - [*アイテムを表示*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/list?view=azure-devops-rest-6.0)
  - [*項目の種類を取得する*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/get?view=azure-devops-rest-6.0)
  - [*項目タイプをリストにする*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/list?view=azure-devops-rest-6.0)

ユーザー **username@microsoft.com** は、指定された Azure 組織 URL のどのプロジェクトにもアクセスできません。

使用されている Azure 組織のどのプロジェクトへのアクセス権も有していません。カードをインポートするには、Azure ボード側でのアクセス権が必要です。Azure 組織の所有者に連絡し、Azure 組織に招待するよう依頼してください。[こちらの記事](https://docs.microsoft.com/azure/devops/organizations/security/look-up-organization-owner?view=azure-devops)を読んで、組織の所有者の名前を確認する方法を知ることができます。

サービスフック サブスクリプションを作成できませんでした。ユーザー **username@microsoft.com** は、組織の所有者ではありません。この手順を設定するには、組織の所有者に依頼してください。

Miro 内で Azure カードを設定するためには、Azure 組織の所有者であり、かつ Miro 会社の管理者である必要があります。

認証の有効期限が切れています。チームの設定でインテグレーションを再接続してください。

Azure 認証の有効期限が切れています。"個人レベル"の「Azure カードを使用するために個人の Azure アカウントを接続する」セクションに記載されている手順に従って、インテグレーションを再接続してください。

作業中のカードが予期しない挙動を示しています。

このような挙動は、Azure 組織のカードが同期されなかった場合に発生することがあります。例えば、他のボードからカードをコピーしたり、チーム間を移動させたボードで作業したりしている場合などです。この問題を解決するには、ボードに Azure アイテムを追加し直します。

返された作業項目数が、サイズ制限の 200 件を超えています。返される項目数を減らすためにクエリを変更してください。

このエラーメッセージは、ボードにカードとして追加するタスクを一度に多く選択しすぎた場合に表示されます。検索バーを使用して、表示されるタスクの数を制限してください。その時点では、ピッカーを開いてもフィルターは適用されず、過去 3 か月間のすべてのタスクが表示されます。ピッカーが 200 件以上のタスクを表示しようとすると、毎回このエラーメッセージが表示されます。

Miro の設定で、Azure 組織を Miro と接続しようとすると、**Connect** ボタンが表示されません。

チームの管理者権限を持っていることを確認してください。チームの設定で**アクティブなユーザー**タブに移動し、必要に応じて[自分をチーム管理者に昇格させます](../../administration/user-management/06-how-to-manage-admin-roles.md)。これは、管理者による Azure 組織接続の初期設定に適用されます。

:::note
その他の問題が発生した場合は、[Miro サポート](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)にご連絡ください。
:::

## Azure Cards よくある質問

Azure カードのインテグレーションに関する一般的な質問への回答をご紹介します。

Azure カードの許可リストに設定すべき IP を教えてください。

Azure カードのインテグレーションを正しく機能させるためには、特にネットワークが制限された環境では、次の IP アドレスを許可リストに追加する必要があります。

- 18.203.61.162
- 54.220.74.201
- 54.216.81.236
- 54.73.153.141
- 52.215.228.26
- 52.16.47.17
- 54.217.180.21

Azure カードアプリとの接続を解除してからアプリをアンインストールすると、既存の Azure カードはどうなりますか？

カードのデータは失われずに Miro のボードに残りますが、Azure との同期は停止し、ソースボタンが表示されなくなります。
