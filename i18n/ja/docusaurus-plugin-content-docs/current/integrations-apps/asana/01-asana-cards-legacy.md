---
title: "Asana \u30AB\u30FC\u30C9\uFF08\u30EC\u30AC\u30B7\u30FC\uFF09"
article_id: 360039492573
translation_id: 360039492573
locale: ja
sidebar_position: 1
created_at: '2019-11-25T10:03:42Z'
updated_at: '2025-11-25T16:05:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: asana-cards
---

:::warning
このページは旧式のAsanaインテグレーションについて説明しています。新しいインテグレーションについては、[Asana（ベータ版）ドキュメント](asana)をご参照ください。
:::

**主な機能**

- Asana のタスクを Miro ボードにインポートして、チームの進捗状況を視覚化します
- Asana の絞り込み機能やタスク名を使って、特定のタスクを検索し、Miro から直接インポートできます
- Asana で行ったタスクの変更は、Miro の Asana カードに自動的に同期され、表示されます

> **利用可能なプラン**: Starter、Business、Enterprise プラン。*管理者が Miro チームに対して Asana の使用を承認する必要があります。チームメンバーは、チームレベルでアプリがインストールされている場合のみ、Asana カード アプリを使用できます。*

### Asana カードのインストール方法

1. まず、アクティブな Miro とアクティブな Asana アカウントが必要です。Miro のプロフィールがない場合は、 [こちら](https://miro.com/signup/)からサインアップしてください。
2. Miro マーケットプレイスで[Asana Cards](https://miro.com/marketplace/asana-cards/?backUrl=%2Fmarketplace%2F)*を開き、***アプリを取得**ボタンをクリックします。
   Asana をインストールするチームを選択するよう求められます。チームを選択し、**インストールと承認**をクリックします。
   > ⚠️ 管理者以外のユーザーは、設定で許可されていなければ、このアプリをインストールすることはできません。

![install_Asana_cards.jpg](../../../../../../docs/integrations-apps/asana/images/21020254087442_install%20Asana%20cards.jpg)
*Asana カードの認証*

3. 次に、Asana カードのアプリ設定で**接続**をクリックします。

![connect_Asana_and_Miro.jpg](../../../../../../docs/integrations-apps/asana/images/21020265147410_connect%20Asana%20and%20Miro.jpg)
*チーム設定で Asana カードアプリの設定*
他のチームメンバーは、ボード作成ツールバーに [Asana カード] のアイコンが表示され、そこから自分の Asana アカウントに接続できるようになります。

![Asana_cards_on_the_toolbar.jpg](../../../../../../docs/integrations-apps/asana/images/21020254085010_Asana%20cards%20on%20the%20toolbar.jpg)
*ツールバーの Asana カード*

4. Asana Connect の Asana アカウントへのアクセスを許可します。この時点でアプリにログインしていなければ、Asana の自分のアカウントへのアクセスを許可するよう促されます。

**![grant_permission_to_Asana.jpg](../../../../../../docs/integrations-apps/asana/images/21020254090386_grant%20permission%20to%20Asana.jpg)*****Miro による Asana アカウントへのアクセス許可***

### Asana カードのインポート方法と使用方法

1. Miro を Asana アカウントに接続すると、Miro ボードに Asana カードを自由に追加することができます。ツールバーの**「ツール、メディア、インテグレーション 」**(**+****).**を選択すると、パネルが開きます。「Asana カード」を検索して選択してください。
2. ピッカーは、タスクのフィルタリング機能を提供します。まず、ワークスペースを選択してから、検索条件の「プロジェクト」、「タグ」、「担当者」を使ってカードを絞り込みます。プロジェクトの一覧は作成日順に表示されます。

   > ⚠️ ピッカーには、Asana でアクセス可能なタスクだけが表示されます。もし、Miro ユーザーが権限のないページアクセスしようとすると、権限がないためアクセスできない、というメッセージが表示されます。

   ![Asana_picker.gif](../../../../../../docs/integrations-apps/asana/images/21020254098578_Asana%20picker.gif)
   **ボードに Asana カードをインポート**

Asana でカードを開くには、**ソース**ボタンをクリックします。
![go_to_source.jpg](../../../../../../docs/integrations-apps/asana/images/21020265150226_go%20to%20source.jpg)
**カードのソースボタン**

Asana カードを[カンバン](../../using-miro/advanced-tools/02-columns-formerly-kanban.md)や[ユーザーストーリーマップ](../../using-miro/advanced-tools/07-user-story-mapping.md)のフレームワークにドラッグして簡単に追加できます。

:::warning
MiroではAsanaカードを作成または編集することはまだできませんが、Asana側で加えた変更はすべてMiroで同期されます（カードの更新に若干の遅延があることがありますのでご注意ください）。
:::

![Asana_cards_and_kanban.gif](../../../../../../docs/integrations-apps/asana/images/21020254093074_Asana%20cards%20and%20kanban.gif)
*Asanaカードをカンバンに追加*

### カードの色を変更

カードの色を変更するには、カードをクリックして、コンテキストメニューから**塗りつぶしの色**を選択します。カードを複製すると、新しい色が適用されます。![asana_card_color.png](../../../../../../docs/integrations-apps/asana/images/21020254100242_asana_card_color.png)
*カードの塗りつぶしの色を変更*

### Asana カードのアンインストール方法

Asana カードをチームレベルでアンインストールするには、チーム設定 **> アプリ & インテグレーション > Asana カード**を開き、下にスクロールして**チームに対してアンインストールする**をクリックします。

**個人レベルでアプリをアンインストールする場合は、****アンインストールする**をクリックしてください。

![uninstall_Asna_Cards.jpg](../../../../../../docs/integrations-apps/asana/images/21020265153426_uninstall%20Asna%20Cards.jpg)
*Asana カードのアンインストール*

### よくある質問

1. *Asana カードのために許可リストに入れておく IP はどれですか？*
   *-* 18.203.61.162, 54.220.74.201, 54.216.81.236, 54.73.153.141, 52.215.228.26, 52.16.47.17, 54.217.180.21。
