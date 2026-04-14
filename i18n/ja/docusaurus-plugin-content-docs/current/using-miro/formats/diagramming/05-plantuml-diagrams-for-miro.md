---
title: Miro の PlantUML ダイアグラム
article_id: 7004940386578
translation_id: 7004940386578
locale: ja
sidebar_position: 5
created_at: '2022-08-05T14:09:39Z'
updated_at: '2025-06-02T10:44:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: plantuml-diagrams
availability:
  notes: '人々：: 全ユーザー プラン：: すべてのプラン プラットフォーム：: ブラウザー、デスクトップ'
---

Miro の PlantUML アプリを使用すると、コードベースのダイアグラムを直接 Miro ボードに作成・埋め込むことができます。このインテグレーションにより、Miro 環境を離れることなく、テキストベースの説明からダイアグラムを生成することで、ワークフローが効率化されます。

## PlantUML アプリをインストールする

PlantUML アプリをインストールして、Miro のボードでダイアグラムの作成を開始できます。アプリは、Miro マーケットプレイスまたは Miro ボードの作成ツールバーから直接利用できます。

1. 作成ツールバーで**ツール、メディア、インテグレーション**（**+**）を選択します。**ツール、メディア、インテグレーション**パネルが開きます。
2. **ツール**タブで、**PlantUML Diagrams** を検索して選択します。**PlantUML Diagrams** パネルが開きます。
3. プロンプトが表示されたら、Miro のチームを選択し、**インストールして承認** をクリックしてインストールを完了します。

:::warning
管理者以外のユーザーは、チーム設定で許可されていない場合はアプリをインストールできません。
:::

[Miro マーケットプレイス](http://miro.com/marketplace)から、または[このリンク](https://miro.com/marketplace/plantUML/)からアプリを直接インストールすることもできます。

## Miro のボードにダイアグラムを作成して追加する

PlantUML アプリがインストールされると、作成ツールバーで見つけることができます。以下の手順に従って、ダイアグラムを作成し、追加してください。

![PlantUML Diagrams app on the Creation toolbar](../../../../../../../docs/using-miro/formats/diagramming/images/21537438798994_plantuml-entry-point.png)
*作成ツールバーの PlantUML Diagrams アプリ*

1. 作成ツールバーから PlantUML アプリを開きます。
2. エディターに PlantUML コードを入力してください。アプリには、始めるためのデフォルトのサンプルが含まれています。コードを入力または変更すると、右パネルのダイアグラムプレビューが自動的に更新されます。

![PlantUML ダイアグラムの変更](../../../../../../../docs/using-miro/formats/diagramming/images/21017043137938_PlantUML%20diagram.gif)
*ダイアグラムの変更*

3. コードエディター パネルのサイズは、必要に応じて右端をドラッグして調整します。

![PlantUMLエディターの幅を変更](../../../../../../../docs/using-miro/formats/diagramming/images/21017013630226_change%20the%20width%20of%20editor.gif)
*コードエディターのサイズ変更*

4. ダイアグラムが準備できたら、**ボードに追加**（またはそれに類似した名前のボタン）をクリックします。このアクションはダイアグラムの画像を作成し、Miro ボードに配置します。

![Adding a PlantUML diagram to the board](../../../../../../../docs/using-miro/formats/diagramming/images/21017013631250_add%20PlantUML%20diagram%20to%20board.gif)
*ボードにダイアグラムを追加*

ダイアグラムをボードに追加した後、画像をダウンロードするか、[ボードをコラボレーターと共有](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md)することができます。

## 既存のダイアグラムを編集

あなたの Miro ボードにある PlantUML ダイアグラムを編集することができます。ダイアグラムを修正するには:

1. ボード上のダイアグラムをクリックして選択します。
2. 作成ツールバーの **PlantUML** アイコンをクリックします。PlantUML エディターが開き、ダイアグラムのコードが表示されます。
3. コードに変更を加えてください。
4. **[ダイアグラムを更新]** をクリックします。Miro ボードに戻ると、ダイアグラムは変更内容で更新されます。

![Miro ボードから PlantUML ダイアグラムを編集](../../../../../../../docs/using-miro/formats/diagramming/images/21017013632530_diagrams_editing_plantuml_diagrams.gif)
*Miro から直接ダイアグラムを編集*

## 追加情報

PlantUML の構文や機能の詳細については、[公式の PlantUML ドキュメント](https://plantuml.com/)を参照してください。アプリパネルの左下隅にあるリンクからも PlantUML ドキュメントに素早くアクセスすることができます。
