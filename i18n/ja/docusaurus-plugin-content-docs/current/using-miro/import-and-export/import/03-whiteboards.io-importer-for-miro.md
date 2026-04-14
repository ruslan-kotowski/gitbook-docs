---
title: "\u30DB\u30EF\u30A4\u30C8\u30DC\u30FC\u30C9.io Miro\u7528\u30A4\u30F3\u30DD\
  \u30FC\u30BF\u30FC"
article_id: 20624350720402
translation_id: 20624350720402
locale: ja
sidebar_position: 3
created_at: '2024-08-07T16:30:40Z'
updated_at: '2026-01-19T14:08:30Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
---

ServiceRocketのWhiteboards.io Importer for Miroは、Miroからのデータのインポートを合理化するために設計されたユーザーフレンドリーなソリューションです。 [ホワイトボード.io](https://whiteboards.io/) アプリから [Miro](https://miro.com/app/dashboard/).ホワイトボードで作成したバックアップを素早く簡単にアップロードできます。

今すぐインポーターにアクセスしましょう。訪問[https://www.servicerocket.com/miro/whiteboards-io-miro-migration をご覧ください。](https://www.servicerocket.com/miro/whiteboards-io-miro-migration) をご覧ください。

## **Whiteboards.ioからのボードのエクスポート**

1. ログイン [ホワイトボード.io](https://whiteboards.io/).
2. メインページで、警告ステータスメッセージのボードのエクスポートをクリックします。

*警告ステータスメッセージから、ボードのエクスポートをクリックしてください。*

3. 次に、以下のステップを実行してボードをエクスポートします。

*ボードをエクスポートする際に設定が正しいことを確認します。*

1. 1. .json形式のみを選択してください。
   2. メディア（画像、ビデオ、その他のファイル）を含めるのチェックを外します。
   3. Export をクリックして設定を確認し、ボードをエクスポートします。

4. .zipファイルが正常に生成されます。

## **Whiteboards.ioボードのMiroへのインポート**

1. Miroボードを開いてください。
2. ツールバーの「その他のアプリ」をクリックし、ホワイトボード.io Miro Importer を選択または検索します。
3. ファイルを選択] をクリックし、[Whiteboards.io] から生成された (.zip) ファイルをアップロードします。 [ホワイトボード.io](http://whiteboards.io/)アプリから生成された (.zip) ファイルをアップロードします。
4. 次に、インポートしたいボードを選択し、インポートをクリックします。
5. インポートが完了すると、システムはボードのステータスをCOMPLETEDと表示します。
6. アプリを閉じ、Miroのメインページに戻ります。アプリは選択したボードをチームアカウントにインポートします。

## **Miroにおけるホワイトボード.ioのデータマッピング**

データマッピングは、あるアプリケーションから別のアプリケーションへの移行中に、データの整合性、一貫性、スキーマの違いを維持するために不可欠です。以下の表は、同等の用語、データ構造、フィールド名、フォーマットなどをすべてリストアップしたものです。

|  |  |  |
| --- | --- | --- |
| **ホワイトボード.io** | **Miro** | メモ |
| テキスト | [テキスト](https://developers.miro.com/docs/text-1) | 該当なし |
| 図形 | [図形](https://developers.miro.com/docs/shape-1) | - ハートの図形は雲の図形としてインポートされます。 - paperTape図形は、flowchart_input_outputフローチャート図形としてインポートされます。 - アイコンは画像としてインポートされます。 |
| カード | [付箋](https://developers.miro.com/docs/stickynote-1) | - カードに変換すると、フォントのフォーマットが失われます。 - カードの色が失われ、アライメントが崩れます。 - 付箋の大きさは異なる場合があります。 |
| ライン | [コネクター](https://developers.miro.com/docs/connector_intro) | 該当なし |
| フレーム | [フレーム](https://developers.miro.com/docs/frame-1) | フレームの子オブジェクトを親フレームにリンクすることはできません。 |
| 無料ドロー | [画像](https://developers.miro.com/docs/image-1)(.svg) | 該当なし |
| コメント | 該当なし | Miroにはこれをマッピングする方法はありません。 |
| ファイル | [ファイル](../../troubleshooting-technical-questions/technical-guidelines/03-supported-file-formats.md) | ファイルの種類とファイル形式   - 画像 - 表とスプレッドシート - テキスト文書 - プレゼンテーション |
| 画像 | [画像](https://developers.miro.com/docs/image-1) | 該当なし |
| iFrameの埋め込み | [埋め込み](https://developers.miro.com/docs/embed-2) | 該当なし |
| カードテーブル | [カードと](https://developers.miro.com/docs/card-1) [フレーム](https://developers.miro.com/docs/frame-1) | カラム名とスイムレーン名を除きます。 |
| マインドマップ | [マインドマップ](https://developers.miro.com/docs/mind-maps)(実験) | ボーダーカラーには対応していません。 |
| ギットハブカード | [カード](https://developers.miro.com/docs/card-1) | 該当なし |
| Jira カード | Jira Issue URL を含むテキスト | 該当なし |
