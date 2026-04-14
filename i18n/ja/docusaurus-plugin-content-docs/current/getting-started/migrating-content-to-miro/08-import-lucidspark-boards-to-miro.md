---
title: Lucidspark のボードを Miro にインポートする
article_id: 9549014537490
translation_id: 9549014537490
locale: ja
sidebar_position: 7
created_at: '2023-01-12T09:05:07Z'
updated_at: '2026-01-19T14:30:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'ユーザー: Lucidspark と Miro の両方のボードを編集できるユーザー プラン: Free、Starter、Business、Education、Enterprise
    プラットフォーム: ブラウザ、デスクトップ'
---

Lucidspark のコンテンツを Miro にシームレスに移行し、より優れたコラボレーションを実現します。このガイドでは、ボードをインポートする方法と、そのプロセス中に期待されることを説明します。

> **警告:** インポートしたコンテンツの編集は一方向です。Miro で行った変更は Lucidspark に同期されません。

> **注:** Free または制限付きライセンスの Lucidspark ボードを移行することができます。

## Lucidspark ボードを PDF エクスポートでインポートする方法

以下の手順に従って、PDF エクスポート方法を使用し、Lucidspark のボードを Miro にインポートしてください。

1. Miro にインポートしたい **Lucidspark** のコンテンツを PDF としてエクスポートしてください。
2. Miro **ホーム** ダッシュボードで、**+ 新規作成** をクリックします。
3. **インポート** を選択し、次に **Lucidspark からインポート** を選びます。
   **Lucidspark からインポート** モーダルが開き、複数の Lucidspark PDF をバルクインポートできます。
4. モーダルに表示される画面上の指示に従ってください。
5. **ボードをインポート** を選択します。
6. インポートしたコンテンツを確認し、必要な調整を行います。Lucidspark と Miro には似たような機能がありますが、スタイルや書式のオプションには違いがあります。オブジェクトがどのように変換されるかについては、[Miro における Lucidspark オブジェクトの表れ方（PDF一括インポート法）](#lucidspark-object-mapping-bulk-import)をご参照ください。

## 別の方法: コンテンツのコピー＆ペースト

少量のコンテンツには、Lucidspark ボードから直接要素をコピーし、それを Miro ボードにペーストするというより迅速な方法が利用できます。

> **注意:** Lucidspark と Miro の両方のボードの編集権限を持つユーザーであれば、Lucidspark からコンテンツをコピーして Miro に貼り付けることができます。この方法でオブジェクトがどのように変換されるかの詳細は、[Lucidspark オブジェクトの Miro での表示（コピー/ペースト法）](#lucidspark-object-mapping-copy-paste)を参照してください。

## Lucidspark オブジェクトの Miro での表示（コピー/ペースト法）

この表は、Lucidspark からコンテンツを直接コピーして Miro に貼り付ける際にオブジェクトがどのように変換されるかを包括的に比較しています。

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Azure カード | Azure カードは Miro カードとして移行されます： 1. Miro で Azure インテグレーションを設定します。 2. Miro カードを[Azure カード](../../integrations-apps/microsoft/03-azure-cards.md)に変換します。 |
| コラボレーターと共有 | 🟠 手動で再作成できます |
| コメント | 🟠 手動で再作成できます |
| 接続線＆区切り線 | 接続線 |
| コンテナ | 図形 |
| ファイルおよび URL からのドキュメント | 🟠 手動で再作成可能 |
| URL からのドキュメント（PDF） | 埋め込みドキュメント |
| 図形の描写 | 画像 |
| ダイナミックテーブル | テーブル |
| 絵文字 | 画像 |
| フレーム | フレーム |
| ツールバーからの GIF | 画像 |
| ファイルからの GIF | 画像 |
| URL からの GIF | GIF |
| 画像 | 画像 |
| Jira カード | Jira カードは Miro カードとして移行されます：  1. Miro で Jira インテグレーションを設定 2. Miro カードを[Jira カード](../../integrations-apps/atlassian/03-jira-cards.md)に変換します。 |
| Lucid カード | カード |
| マインドマップ | マインドマップ |
| 図形 | 図形 |
| 付箋 | 付箋 |
| テーブル | テーブル |
| テキスト | テキスト |
| タイムライン | 🟠 手動で再作成可能 |
| 動画およびその他のURL | プレビュー |

## Lucidspark オブジェクトの Miro での表示（PDF 一括インポート メソッド）

この表は、PDFを使ってコンテンツを一括インポートした後の Lucidspark と Miro のオブジェクトの違いを包括的に比較したものです。

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Azure カード | 画像 |
| コラボレーターと共有 | 🟠 手動で再作成可能 |
| コメント | 🟠 手動で再作成可能 |
| 接続線＆区切り線 | コネクター |
| コンテナ | 図形 |
| ドキュメント | 🟠 手動で再作成可能 |
| 図を描く | 線 |
| 動的テーブル | 図形とコネクター |
| 絵文字 | 画像 |
| フレーム | フレームと図形 |
| GIF | 画像 |
| 画像 | 画像 |
| Jira カード | 図形 |
| Lucid カード | 図形 |
| マインドマップ | 図形とコネクター |
| 図形 | 図形 |
| 付箋 | 付箋 |
| テーブル | テーブル・図形とコネクター |
| テキスト | テキスト |
| タイムライン | 図形とコネクタ |
| ビデオと他のURL | 🟠 手動で再作成可能 |

## インポートの制限

Lucidspark と Miro は類似した機能を提供しますが、コンテンツをインポートする際には以下の相違点と制限に注意してください:

- Miro のテキストボックスは、スペースを含めて最大 6,000 文字まで入力できます。それ以上のテキストはカットされます。
- 色とスタイルは、Miro において最も近いものが適用されます。
- Lucidspark の不透明度は、インポート時に正確には抽出されません。
- Miro の付箋は、回転、色パレットの調整、及び Lucidspark で適用されたテキストの箇条書きには対応していません。

## ヘルプの利用

> **注:** Lucidspark の移行に関するご質問やサポートについては、[Miro サポート](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)にお問い合わせいただくか、Miro のお客様担当者に直接ご連絡ください。
