---
title: "CA Agile Central\uFF08Rally\uFF09"
article_id: 360017731133
translation_id: 360017731133
locale: ja
sidebar_position: 4
created_at: '2019-02-11T10:13:34Z'
updated_at: '2025-11-25T16:02:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: rally-cards
---

CA の業界をリードするアジャイル ソフトウェアと手法を直接ボード上で活用しましょう。CA Agile Central の機能を扱いやすいカードに変換し、バックログの優先順位付け、ストーリーのマッピング、他のチームの活動を視覚化することで、チームが一貫して高品質なプロジェクトを迅速に開発することを可能にします。

> **利用可能なプラン：**[Enterprise プラン](../../plans-billing/miro-plans/04-enterprise-plan.md)

## CA Agile の接続

CA Agile の認証は、OAuth 2.0 プロトコル（認証コード付与）により行われ、すべてのリクエストは SSL を介して行われます。Miro のデータと CA Agile Central アカウントの接続には、ユーザープロフィール レベルとチームレベルの 2 つがあります。

CA Agile への接続は、次のように一方通行のみです。CA Agile --> MiroMiro のボードにカードをインポートし、カードの編集セクションで後述するSource（ソース）ボタンを介してカードを編集することができます。Miro で CA Agile カードを直接編集することはできません。

### チームレベル

> **設定者：**チームの管理者

:::warning
Miro のチームごとに、異なる Rally ユーザーアカウントを使用して、同じ Rally インスタンスを接続する必要があります。
:::

チームレベルで接続を確立するには、チームの管理者が、[Miro マーケットプレイス](https://miro.com/marketplace/)で **CA Agile** アプリを検索し、チームにインストールする必要があります。[**アプリを取得**] をクリックしてから、チームを選択して、[**インストールして承認**] をクリックします。

![install_Rally_for_a_team.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416392594_install%20Rally%20for%20a%20team.jpg)
*チームに Rally をインストール*

ボード内からアプリをインストールすることもできます。

1. [作成] バーで [**ツール、メディア、インテグレーション**（**+**）] を選択します。[**ツール、メディア、インテグレーション**] パネルが開きます。
2. [**ツール**] タブで、[CA Agile] を検索して選択します。
   [**CA Agile**] パネルが開きます。

![ca-agile-entry-point.png](../../../../../../docs/integrations-apps/more-integrations/images/21537455155858_ca-agile-entry-point.png)
*ボードからアプリをインストール*

次に、**チームの設定 > [アプリとインテグレーション]** を開き、そこからインテグレーションと [**接続する**] を選択します。Rally で認証されていない場合、Rally アカウントにログインするよう促されます。

![connect_Rally.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416393874_connect%20Rally.jpg)
*チームレベルでのインテグレーションを接続*

この設定中に、Rally 側で Webhook が作成され、インポートされたカードの最新情報が Miro に送信されるようになります。

チームレベルでインテグレーションが設定されている場合、チームメンバーであれば誰でも、他の参加者がボードにインポートした Rally カードやカードの現在の状態を確認できます。

なお、チームレベルでインテグレーションの設定で使用される Rally アカウントには、カードのインポートが行われるすべての Rally プロジェクトへのアクセスが必要です。もし、この Rally アカウントでアクセスできない Rally プロジェクトがある場合、そのプロジェクトからインポートされたカードはボード上で更新されず、チームユーザー全員にフリーズした状態で表示されます。

### プロフィールレベル

> **設定者：**各ユーザー

:::warning
インテグレーションを接続する前に、別のブラウザータブで Rally にログインしてください。
:::

ユーザーがボード上の Rally カードをインポートするオプションが必要な場合、プロフィールレベルでインテグレーションを設定することも必要となります。Miro のプロフィールでインテグレーションと接続するには、[[プロフィールの設定]](https://miro.com/app/account/profile/) を開き、**[インテグレーション]** に切り替え、**CA Agile Central（Rally）** を検索して、**[接続する]** をクリックします。

![connect_Rally_on_profile_level.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017429433746_connect%20Rally%20on%20profile%20level.jpg)
*プロフィールレベルでインテグレーションを接続*

プロフィールレベルの接続が確立されると、ユーザーは、ツールバー上の Rally アイコンを使用して Rally ライブラリーピッカーを開くことができます。そこでは、プロフィールレベルでインテグレーションの設定に使用される Rally アカウントで利用可能な Rally の要素（ユーザーストーリー、タスク、不具合）のすべてを確認できます。つまり、Rally ピッカーを使えば、ユーザーは Rally で利用可能な項目だけインポートすることができるようになります。

## ボードへの CA Agile カードの追加

ボードにカードを追加するには、タスクの URL アドレスをコピーしてボードに貼り付けるだけです（通常の[ショートカットの組み合わせ](https://help.realtimeboard.com/support/solutions/articles/1000206698-shortcuts-hotkeys)も使えます）。

タスクをフィルターにかける、またはカードを一括で追加するには、作成ツールバーで [**CA Agile**] を選択します。。

CA Agile Central ピッカーが表示され、プロジェクト、タイプ、イテレーション、リリースなどの検索フィルターを設定できるようになります。1 つまたは複数を選択し、**[エクスポート]** をクリックします。

![Rally_picker.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416397714_Rally%20picker.jpg)
*CA Agile Central ピッカー*

タスクは自動的にボードに追加されます。タスク名が長い場合、カードの下側をドラッグすると全体が表示されます。

*![Rally_cards_on_the_board.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416398482_Rally%20cards%20on%20the%20board.jpg)
ボード上の Rally カード*。

> Miro の Rally インテグレーションでは、Miro で Rally カードを作成または直接編集することはできません。

## カードの編集

カードのコンテンツを編集するには、カードのソースリンクをクリックしてください。

![Rally_card_source.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416398866_Rally%20card%20source.jpg)
*カード上の編集アイコン*。

ソースタスクは新しいタブで開かれ、編集できるようになります。変更内容はすべて、カードに即座に反映されます。

## インテグレーションの無効化

Rally イテレーションへの接続を解除するには、**チームの設定 > [アプリとインテグレーション]** でインテグレーションを **[無効化]** し、**[チームに対してアンインストールする]** をクリックします。

![uninstall_Rally.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017429436562_uninstall%20Rally.jpg)
*インテグレーションを無効化するオプション*

## 発生する可能性のある問題と解決方法

1. *Miro-Rally ピッカーに、自分のプロジェクトの一部が表示されません*
   — Miro の Rally インテグレーションでは、[Rally SDK ピッカー](https://rally1.rallydev.com/docs/saas/apps/2.1/doc/index.html#!/api/Rally.ui.picker.project.ProjectPicker)を使用してデータを入力しますが、これは「公開」状態のプロジェクトでのみ機能し、残念ながらカスタマイズできません。Miro 側でプロジェクトを表示するには、プロジェクトの状態を [公開] に変更してください。
2. *カードや一部のカードのフィールドの更新が Miro に反映されません*— 複数の Miro のチームと Rally カードのインテグレーションを使用している場合、すべてのチームが*異なる* Rally ユーザーアカウントを使用して、Rally インスタンスに接続されていることを確認してください。接続用の認証情報が別の Miro チームですでに使用されているため、選択したチームの更新に問題が発生している可能性があります。必要に応じて、別の Rally ユーザーの認証情報を使用してインテグレーションを再接続してください。
3. *Miro で Rally ピッカーを開こうとしても、読み込みが終了しません*— 以下のトラブル シューティング手順をお試しください。

   1.サブスクリプション メニューを開きます（`https://rally1.rallydev.com/#/subscription`）。

   2.[**アクション**] メニューのドロップダウンをクリックし、[**編集**] を選択します。

   3.**CORS Allowed Origins**（許可オリジン） フィールドが表示されるまでスクロールダウンします。

   4.フィールドに `https://miro.com,https://*.miro.com` （[https://miro.com](http://miro.com)）を入力します。

   5.[**保存して閉じる**] をクリックします。
