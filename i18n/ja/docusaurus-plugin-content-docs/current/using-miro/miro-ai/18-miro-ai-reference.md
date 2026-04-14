---
title: Miro AIリファレンス
article_id: 20970362792210
translation_id: 20970362792210
locale: ja
sidebar_position: 18
created_at: '2024-08-26T09:34:26Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: '対象者: すべてのユーザー 対応プラン: Free、Starter、Business、Enterprise、Education 対応プラットフォーム:
    ブラウザー、デスクトップ、モバイル'
---

この参考記事では、Miro AI の機能について説明します。

## Miro AI モデル

モデルは一般的にプロバイダーのインフラ、または Microsoft の Azure AI サービスや AWS Bedrock 上でホストされています。AWS マーケットプレイスを通じて Miro を利用する顧客の場合、すべてのモデルは AWS Bedrock 上でホストされます。

### AI を活用した作成と反復

| **Miro AI 機能** | **説明** | **モデル** |
| --- | --- | --- |
| 会話ダイジェスト | Miro ボード上の長いコメントスレッドを要約する機能です。 | GPT 4o-mini |
| ダイアグラム作成 - フローチャート | ユーザーのプロンプトと選択したボードの内容からフローチャートを作成します。 | GPT-4o |
| ダイアグラムを編集 - フローチャート | ユーザーのプロンプトと選択されたボード上のコンテンツからフローチャートを編集します。 | GPT-4o |
| ダイアグラムを作成 - マインドマップ | ユーザーのプロンプトと選択されたボード上のコンテンツからマインドマップを作成します。 | GPT 4o-mini |
| 図の編集 - マインドマップ | ユーザーのプロンプトと選択したボード内容からマインドマップを編集します。 | GPT-4o |
| 図の作成 - ERD | ユーザーのプロンプトからエンティティ関係図（ERD）を作成します。**AIで作成**オプション。 | GPT 4o-mini |
| ダイアグラムを編集 - ERD | ユーザーのプロンプトと選択したボードのコンテンツからERDを編集します。 | GPT-4o |
| ダイアグラムをデジタル化する | 手書きダイアグラムの画像をMiro内で完全に編集可能なダイアグラムに変換します。 | Claude 3.7 Sonnet (AWS Bedrock) |
| Doc を作成 | ユーザーのプロンプトと選択されたボード上のコンテンツから Miro Doc を作成します。**AI で作成**オプションです。 | GPT-4o |
| Doc を編集 | ユーザーのプロンプトと選択されたボード上のコンテンツから Miro Doc を編集します。 | GPT-4o |
| 画像を作成 | ボード上のオブジェクトをコンテキストとして、ユーザーのプロンプトから画像を作成します。**AI で作成**オプション。 | Segmind Stable Diffusion 1B (SSD-1B) + StabilityAI Diffusion XL Refiner 1.0 |
| 画像を編集 | ボード上のオブジェクトをコンテキストとして、ユーザーのプロンプトから画像を編集します。**AIで作成**オプションです。 | GPT-4o |
| 画像をプロトタイプに変換 | スケッチやプロトタイプの画像を編集可能なMiroのプロトタイプに変換します。 | Miro自社モデル + Claude 3.7 Sonnet |
| 画像の代替テキスト | 画像の説明文を生成します。AI クレジットは消費しません。 | Miro 独自モデル |
| 付箋を作成 | ユーザーのプロンプトと選択したボード上のコンテンツから Miro 付箋を作成します。 | GPT-4o |
| 付箋を編集 | ユーザーのボードと選択したボードコンテンツから付箋を編集します。 | GPT-4o |
| 付箋をキャプチャ | 物理的な付箋の画像を Miro の付箋に変換します。 | Miro 独自モデル |
| プロトタイプを作成 | ユーザーのプロンプトと選択されたボードのコンテンツからMiroプロトタイプを作成します。 | GPT-4o + Claude 4.5 Sonnet + GPT 4o-mini + Gemini 2.5 Flash Image（nano-banana） |
| プロトタイプ画面を編集 | ユーザーのプロンプトと選択されたボードのコンテンツからMiroプロトタイプ画面を編集します。 | Claude 4.5 Sonnet + Gemini 2.5 Flash Image（nano-banana） |
| 背景を削除 | 画像から背景を削除します。 | Miro独自モデル |
| スマート図形 | 鉛筆で描いた図を線、図形、または付箋に変換します。 | Miro独自モデル |
| テーブルを作成 | ユーザーのプロンプトと選択されたボード上のコンテンツから Miro テーブルを作成します。 | Claude 3.7 Sonnet |
| テーブルを編集 | ユーザーのプロンプトと選択されたボード上のコンテンツから Miro テーブルを編集します。 | Claude 3.7 Sonnet |

### AI 搭載サイドキック

|  |  |  |
| --- | --- | --- |
| **Miro AI 機能** | **説明** | **モデル** |
| AI サイドキック - アジャイルコーチ | ふりかえりにおける重要なテーマを特定し、次のステップを提案します。 | GPT-4o |
| AI サイドキック - プロダクトリーダー | フレーム、付箋、またはテキストにコメントとしてフィードバックや提案を行う。また、解決策のアイデアを付箋として提供します。 | GPT-4o |
| AI サイドキック - プロダクトマーケティングアライアンス | フレーム、付箋、またはテキストにコメントとしてフィードバックや提案を行います。 | GPT-4o |

### AI を活用したクラスター化

| **Miro AI 機能** | **説明** | **モデル** |
| --- | --- | --- |
| キーワードによる付箋のクラスター化 | キーワードで付箋を分類し、各グループにタイトルを付けます。 | Claude 3.5 Haiku + Amazon Nova Micro |
| 感情による付箋のクラスター化 | 意見や視点のような感情で付箋を分類し、ポジティブ、中立、ネガティブのグループにまとめます。 | Claude 3.5 Haiku |

### AI によるテキスト編集

以下の表は、Miro AI によって強化されたテキスト編集を示しています。

|  |  |  |
| --- | --- | --- |
| **Miro AI 機能** | **説明** | **モデル** |
| 語調を変更する | 選択した文面の語調を、「親近感、プロフェッショナル、ビジネス、快活・大らか」などに変更します。 | GPT-5 nano |
| スペルと文法を修正する | 選択した文章のスペルと文法を修正します。 | GPT-5 |
| 読みやすく書き換え | 選択したテキストをわかりやすい文章に書き換えます。 | GPT-5 Chat |
| 文章を短くする | 選択した文面を伝達内容はそのままに、短く明瞭にまとめます。 | GPT-5 mini |
| 翻訳 | 選択されたテキストを英語、スペイン語、ドイツ語、フランス語、日本語、ポルトガル語、韓国語、ポーランド語、イタリア語、トルコ語、アラビア語、ロシア語、デンマーク語、フィンランド語、ノルウェー語、オランダ語、スウェーデン語、タイ語に翻訳します。単一または複数のオブジェクトを同時に翻訳できます。 | GPT-5 mini |

### AI を活用したマインドマップ

| **Miro AI 機能** | **説明** | **モデル** |
| --- | --- | --- |
| マインドマップを生成 | 選択したルートノードからマインドマップを生成します。 | GPT 4o-mini |
| マインドマップ - アイデアで拡張 | 選択したルートノードまたはチャイルドノードからアイデアを生成します。 | GPT 4o-mini |
| マインドマップ - トピックを拡大 | 選択したルートノードまたは子ノードからトピックを生成します。 | GPT 4o-mini |
| マインドマップ - 質問を拡大 | 選択したルートノードまたは子ノードから質問を生成します。 | GPT 4o-mini |

### AI 搭載スライド

Miroスライドでは、以下のモデルを使用しています:

- Amazon Titan
- Claude 4 Sonnet
- Claude 3.7 Sonnet
- Claude 3.5 Sonnet
- GPT-5
- GPT-4o
- Stable Diffusion 3.5 Large
- Stability Image Core

### Miro Insights

お客様のフィードバックを統合するために、[Miro Insights](https://help.miro.com/hc/articles/25438311770770)はGPT-4oを使用しています。

### AWSマーケットプレイスのお客様

**AWS マーケットプレイスモデル**

| **Miro AI 機能** | **モデル** |
| --- | --- |
| 会話ダイジェスト | Claude Haiku 3.7 (AWS Bedrock) |
| 図作成 – フローチャート | Claude Sonnet 3.7 (AWS Bedrock) |
| 図編集 – フローチャート | Claude Sonnet 3.7 (AWS Bedrock) |
| マインドマップを作成 | Claude Sonnet 3.7 (AWS Bedrock) |
| マインドマップを編集 | Claude Sonnet 3.7 (AWS Bedrock) |
| ERD を作成 | Claude Sonnet 3.7 (AWS Bedrock) |
| ダイアグラムを編集 – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| ドキュメントを作成 | Claude Sonnet 3.7 (AWS Bedrock) |
| ドキュメントを編集 | Claude Sonnet 3.7 (AWS Bedrock) |
| 付箋の作成 | Claude Sonnet 3.7 (AWS Bedrock) |
| 付箋の編集 | Claude Sonnet 3.7 (AWS Bedrock) |
| 付箋キャプチャー | Claude Sonnet 3.7 (AWS Bedrock) + Miro 独自モデル |
| 画像を作成 | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| 画像を編集 | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| 画像の代替テキスト | Claude Sonnet 3.7 (AWS Bedrock) |
| プロトタイプを作成する | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| プロトタイプ画面を編集する | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| 画像をプロトタイプに変換する | Claude Sonnet 3.7 + Miro専用モデル |
| テーブルを作成 | Claude Sonnet 3.7（AWS Bedrock） |
| テーブルを編集 | Claude Sonnet 3.7（AWS Bedrock） |
| ダイアグラムをデジタル化 | Claude Sonnet 3.7（AWS Bedrock） |
| キーワードによる付箋のクラスター化 | Claude Sonnet 3.7 (AWS Bedrock) + Miro 独自モデル |
| 感情による付箋のクラスター化 | Miro 独自モデル |
| AI 搭載サイドキック | Claude Sonnet 3.7 (AWS Bedrock) |
| AI駆動のテキスト編集 | Claude Sonnet 3.7 (AWS Bedrock) |
| AI駆動のマインドマップ | Claude Sonnet 3.7 (AWS Bedrock) |

## モデルを選択する

以下は、[モデル選択](10-select-your-own-model-beta.md)で使用可能なモデルを示しています。これは、[フロー](04-flows-overview.md)とサイドキックで利用可能です。

### 大規模言語モデル

**Claude**

- Claude 3.7 Sonnet
- Claude Sonnet 4

**OpenAI**

- GPT-4o
- GPT-4o ミニ
- OpenAI o4-mini
- GPT-5
- GPT-5 ミニ
- GPT-4.1
- GPT-4.1 ミニ

### 画像モデル

**Stability AI**

- Stable Image Core
- Stable Image Ultra
- Stable Diffusion 3.5 Large

**Amazon**

- Amazon Titan 画像ジェネレーター
- Amazon Nova キャンバス

**Google**

- Gemini 2.5 フラッシュ画像 (Nano Banana)
- Vertex AI イメージジェン 3
- Vertex AI イメージジェン 3 高速版
- Vertex AI イメージジェン 4

## Miro AI クレジットとアドオン

Miro は、アカウントごとに毎月一定数の AI クレジットを割り当てます。クレジットの割当数はプランによって異なります。この割当は毎月1日にリセットされます。

各AIアクションを実行するごとにAIクレジットを消費します。ほとんどのAIアクションは1つのアクションにつき1つのクレジットを消費しますが、一部の機能ではより多くのクレジットを消費する場合があります。

AI クレジット数を増やしたい場合は、オプションとして Miro AI クレジット アドオンのサブスクリプションを購入できます。詳細は、[Miro AI クレジットと AI アドオン](../../plans-billing/billing-and-payments/03-miro-ai-credits.md)を参照してください。

## Miro AI プライバシーとセキュリティー

2025年2月3日以降、Miro は Free プランのユーザーからAI機能の改善を目的として、AIのインタラクションデータを収集します。これにより、AI サマリーやダイアグラム、AI サイドキックなどの Miro AI 機能が向上します。

Miro が AI インタラクションをどのように利用して Miro AI を改善しているか、またデータの設定方法については、[Miro AI の品質改善](19-miro-ai-quality-improvements.md)をご覧ください。
