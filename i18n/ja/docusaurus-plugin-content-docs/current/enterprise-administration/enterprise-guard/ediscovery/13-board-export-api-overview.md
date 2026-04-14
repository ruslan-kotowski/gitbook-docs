---
title: "\u30DC\u30FC\u30C9\u30A8\u30AF\u30B9\u30DD\u30FC\u30C8API\u306E\u6982\u8981"
article_id: 17774560667794
translation_id: 17774560667794
locale: ja
sidebar_position: 12
created_at: '2024-03-19T12:52:09Z'
updated_at: '2025-07-09T17:32:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: discovery-board-export
---

[eDiscovery APIにより](https://developers.miro.com/reference/enterprise-create-board-export)、Enterpriseプランのお客様はMiroからボードデータをエクスポートし、手動でレビューしたり、法律、コンプライアンス、セキュリティーを目的とした専用ツールに取り込んだりすることができます。

ボードエクスポートAPIは、指定されたフォーマットSVG、PDF、またはHTMLでのボードコンテンツのエクスポートを含む、ジョブ実行時のボードデータのスナップショットを含むZIPファイル、すべてのコメント投稿者の記録を含むJSONファイル、ボードを閲覧または修正したすべてのユーザーのリストを含むJSONファイル、該当する場合、ボードに関連付けられたTalktrackウェブカメラ映像のビデオ記録、およびボードマタデータを含むJSONを提供します。大きなボードの場合、PDFフォーマットでエクスポートすると、ボード全体を描いた複数のPDFファイルが作成されます。

非同期APIデザインには、ステータスのようなボードエクスポートジョブに関する情報を取得するためのエンドポイントが含まれています。

:::note
Enterpriseプランの場合、一度に実行できるボードのエクスポートジョブは1つだけです。Enterprise Guardのお客様であれば、最大5つのボードエクスポートジョブを同時に実行し、エクスポート速度を大幅に向上させることができます。
:::

## ユースケース

一般的なeDiscoveryのユースケースには、以下のようなものがあります：

- **eDiscovery（電子証拠開示）：**電子的に保存された情報を特定、収集、保存し、法的問題で使用するために検討するプロセス。
- **情報アーカイブ：**組織が長期保管や記録保持の目的で、元のシステムの外部にデータを保持する慣行。コンテンツとメタデータは、アーカイブの索引付けと検索、およびコンプライアンス上の懸念事項の積極的な監視に役立ちます。
