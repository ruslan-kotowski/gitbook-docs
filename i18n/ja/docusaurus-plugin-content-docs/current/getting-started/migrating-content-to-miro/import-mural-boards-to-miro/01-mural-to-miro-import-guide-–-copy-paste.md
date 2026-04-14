---
title: Mural から Miro へのインポートガイド - コピー＆ペースト
article_id: 22957521683986
translation_id: 22957521683986
locale: ja
sidebar_position: 1
created_at: '2024-11-29T13:36:36Z'
updated_at: '2025-11-25T15:49:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'ユーザーリスト: 編集権限を持つユーザー プラン: Free、Starter、Business、Enterprise、Education プラットフォーム：:
    ブラウザー、デスクトップ、モバイル'
---

Mural のボードから Miro にコンテンツをコピーして貼り付けることで移行できます。このガイドでは、このインポート方法に関するベストプラクティスを提供し、ステップバイステップのプロセスを説明し、Miroに貼り付けられた後のさまざまなオブジェクトの外観と動作について期待できることを詳細に述べています。

## Mural からのインポートに関するガイドライン

これらのガイドラインに従うことで、Mural から Miro へのコンテンツ移行時に最良の結果を達成できます。

構造化されたデータに対しては、Mural マインドマップのような場合、要素間のつながりを壊さないためにも、通常はコピー＆ペースト法が最適です。

:::note
この方法を使用して Miro にコンテンツをインポートするには、Mural コンテンツが Mural でフルライセンスまたは制限付き無料ライセンスの下にある必要があります。
:::

[Mural から Miro へのインポートガイド (PDF)](02-mural-to-miro-import-guide-–-pdf.md)でサポートされていない個別のウィジェットをインポートする場合や、PDF メソッドで高忠実度でインポートできないウィジェットには、コピー貼り付けメソッドも推奨されます。

コピー＆ペースト方法にはいくつかの制限があることに注意してください。特定のスタイリング属性や、URLを介してリンクされたのではなく元々Muralにアップロードされた画像はクリップボードにコピーされないため、Miroに転送されません。

## Mural のコンテンツをコピーして Miro に貼り付ける

以下の手順では、Mural ボードからコンテンツをコピーして Miro ボードに貼り付ける方法を説明します。

**前提条件**

Mural のソースボードと Miro の移動先ボードの両方で編集アクセス権を持っていることを確認してください。

Mural ボードからコンテンツをコピーして Miro ボードに貼り付けるには：

1. Mural でコピーしたいオブジェクトを選択します。
   > 💡 Mural ボード上のすべてのオブジェクトを選択するには、キーボード ショートカット **Ctrl+A**（Windows）または **Cmd+A**（Mac）を使用します。
2. 選択したオブジェクトをコピーするには、キーボードショートカット**Ctrl+C**（Windows）または**Cmd+C**（Mac）を使用します。
   Mural のオブジェクトがクリップボードにコピーされました。
3. Miro で、コンテンツを貼り付けたいボードを開きます。キーボードショートカット **Ctrl+V**（Windows）または **Cmd+V**（Mac）を使用して貼り付けます。

   これで、Mural から Miro にコンテンツをコピー＆ペーストしました。
   > ✏️ Mural から貼り付けたコンテンツは、Miro で手動調整が必要な場合があります。貼り付けた後、特定のスタイルや書式設定の側面が異なって表示されることがあります。

## 貼り付け後のオブジェクトの外観

Mural のオブジェクトは、通常、そのままコピー & ペーストできますが、Miro に移すと元の状態からいくつかの違いが生じることがあります。このセクションでは、一般的なオブジェクトに期待される結果を説明し、適用可能なベストプラクティスを提供します。

### エリア

MuralからMiroへのフレームと図形のコピー

Mural の領域を Miro に貼り付けると、透過率100％の状態でも、透明でありながら目に見える枠線として表示されます。Mural エリアにタイトルがある場合、このタイトルは Miro でフレームタイトルとして表示され、機能します。

![タイトル、100%の透明な背景と枠線のあるミューラル領域。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*背景と枠が100%透明なMuralの自由形式エリアにタイトルを付けます*

![Mural から Miro に貼り付けた領域。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mural から Miro への貼り付けエリア*

### コネクター

Mural のコネクターをコピー＆ペーストで Miro のコネクターとして使用する。

コネクターラベルの垂直位置と水平位置は、中央揃えで Miro に貼り付けられます。Miro は、コネクターラベルの位置を中央にのみサポートしています。

コネクターのタイプについて、Miro は*実線*、*点線*、および*破線*をサポートしています。Mural にはさらに、*ゆるやかに点線を引いた*コネクタータイプも含まれています。Miro では、Mural から貼り付けられたコネクターの種類を次のようにマップします: *solid* は *solid* に、Mural の *loosely dashed* タイプは Miro の *dashed* タイプにマップされます。他の直接的な一致（点線対点線のようなもの）も保持されます。

Miro は、Mural の各タイプのコネクター曲線をサポートしていますが、Miro 内での表示が少し異なる場合があります。

![ミューラル コネクターカーブ](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*ミューラルコネクター曲線*

![Miro のコネクター曲線。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Miro コネクター カーブ*

### GIF と画像

Mural に URL から追加された GIF と画像を Miro にコピー&ペーストできます。

:::note
デバイスから直接アップロードされた、または Mural のツールバーから追加された GIF や画像は、この方法では Miro へコピー貼り付けすることはできません。
:::

### マインドマップ

Muralからコピーされたマインドマップを、ルートノード、各子ノード、およびそれらのテキストを含めてMiroのマインドマップとして利用する。

親ノードのスタイルはほとんど保持されます。ただし、図形の半径が異なる場合があり、テキストのフォントサイズは Mural から Miro へ移行する際に保持されません。

Muralからの子ノードはMiroのテキストノードとして貼り付けられ、そのスタイルは保持されません。

マインドマップのコネクターの色や太さも異なる場合があります。

![Mural にコピーされたマインドマップ。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)
*Mural にコピーされたマインドマップ*

![Mural から Miro にコピーされたマインドマップ。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Miro にコピーされたマインドマップ*

Mural のマインドマップで複数のノードレベルがある場合、Miro に貼り付けるとノードの順序が変わることがあります。

![Mural のマインドマップ、複数のノードレベルがあります。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*複数のノードレベルを持つ Mural のマインドマップ*

![MuralからMiroにコピーされた複数のノードレベルを持つマインドマップ。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mural から Miro へ、複数のノードレベルを持つマインドマップをコピー＆ペースト*

:::tip
Mural から Miro にコピーされたマインドマップは、元のスケールが失われる可能性があります。マインドマップを貼り付けた後、Miro ボードで手動で拡大することができます。
:::

### 図形

Mural から貼り付けた図形は、通常 Miro の図形として貼り付けられます。Miro は Mural のほとんどの図形を直接サポートしています。

ただし、Mural には Miro には直接対応するものがない16種類の特定の図形が含まれています。これらの図形は Miro に四角形として貼り付けられます。

![Mural から Miro にコピーして貼り付けると長方形として表示されるすべての 16 の図形。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mural から Miro にコピー & ペーストする16の図形は長方形として貼り付けられます*

### 付箋

Mural の付箋を Miro の付箋として貼り付ける。

Miro は付箋の色と不透明度レベルを、Miro で使用可能な最も近いものに合わせます。

Mural の付箋を Miro にコピー＆ペーストする際、次のような違いが生じる場合があります。

- Mural の丸い付箋は Miro の四角い付箋として貼り付けられます。
- 付箋内のリストはインタラクティブなリストとしては保持されませんが、個々の項目は Miro の付箋内で別々の行に表示されます。
- テキストのフォントサイズは保持されません。Miroの付箋はコンテンツと付箋のサイズに基づいてフォントサイズを自動的に設定します。
- Mural で付箋に適用された回転は、貼り付け時に保持されません。

![Mural にコピーされた付箋。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mural でコピーされた付箋*

![MuralからMiroにコピー＆ペーストされた付箋。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Miro にコピーされた付箋*

### テーブル

Mural からのテーブルは Miro のテーブルとして貼り付けられます。

Mural から Miro にテーブルをコピー＆ペーストする際に、次のような違いが生じる場合があります。これらの項目のそれぞれについて、Miroで貼り付け後に手動で設定を復元することが一般的です。

- Mural で他のオブジェクト（エリア、図形、画像など）の上に配置されたテーブルは、Miro に貼り付けられたときに、それらのオブジェクトの後ろに部分的に隠されることがあります。レイヤーを調整する必要があるかもしれません（最前面に移動）。
- 枠線の色は無視され、枠線は灰色で貼り付けられます。
- 背景の不透明度は無視されます。Mural の透明なセルは Miro では白いセルとして貼り付けられます。ただし、背景色自体が（透過でない場合）一般的に保持されます。
- テキストフォントファミリーは無視され、テキストは Miro のデフォルトテーブルフォント（RobertPro）で貼り付けられます。
- 表セル内での太字や斜体などのインラインテキスト書式は無視されます。

![Muralにコピーされた混合フォーマットの表](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*書式設定が混在した表を Mural にコピー*

![MuralからMiroにコピーされた混合フォーマットのテーブル。](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Miro にコピー＆ペーストされた混在する書式設定の表*

### テキスト

Mural のテキストオブジェクトが Miro のテキストオブジェクトとして貼り付けられます。元の Mural フォントファミリーは保持されていません。Miro は、Mural フォントファミリーを Miro で利用可能な最も近いフォントにマップし、Miro ボード上で最適な結果が得られるように貼り付けたテキストのスケールを調整します。
