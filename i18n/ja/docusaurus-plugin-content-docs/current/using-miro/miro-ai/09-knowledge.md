---
title: ナレッジ
article_id: 29737566936850
translation_id: 29737566936850
locale: ja
sidebar_position: 9
created_at: '2025-09-25T08:24:51Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: sticky-notes
availability:
  notes: '実行可能なユーザー: チームメンバー 対象プラン: Business, Enterprise 対応プラットフォーム: ブラウザー、デスクトップ、モバイル'
---

Miroにおけるナレッジは、Glean、Microsoft Copilot (ベータ版)、Miro Insightsなどのプロバイダーと統合され、会社の知識をキャンバス上で直接アクセスでき、活用可能にします。

ナレッジにより、チームは内部情報やウェブ検索結果をシームレスに取得し、開発を速めるためのキャンバスとしてMiroを利用できます。

既に使用中のナレッジシステムを接続し、会社の知識を文書、テーブル、付箋、スライドなどのフォーマットに簡単に変換します。

ナレッジはウェブ検索を含む以下のインテグレーションをサポートします。

- [Amazon Q](../../integrations-apps/amazon-web-services-aws/03-amazon-q-beta.md)（ベータ版）
- [Gemini Enterprise](../../integrations-apps/google/01-gemini-enterprise-integration.md)（ベータ版）
- [Glean](../../integrations-apps/glean/01-glean-for-miro.md)
- [Microsoft Copilot](../../integrations-apps/microsoft/01-microsoft-copilot-integration.md)（ベータ版）
- [Miro Insights](../tools/use-miro-insights/02-use-miro-insights-on-the-canvas.md)

会社の管理者は、各インテグレーションをチームのために有効化および承認する必要があります。

:::note
Microsoft Copilot や Gemini Enterprise など、一部のインテグレーションには、それぞれのプロバイダーでの有料ライセンスが必要です。
:::

特定の知識インテグレーションの詳細を知るには、[インテグレーション & アプリ](../../integrations-apps)を参照してください。

## 主な機能

- **ナレッジインテグレーション**
  Miro は、[Glean](../../integrations-apps/glean/01-glean-for-miro.md)、[Microsoft Copilot](../../integrations-apps/microsoft/01-microsoft-copilot-integration.md)（ベータ版）、[Amazon Q](../../integrations-apps/amazon-web-services-aws/03-amazon-q-beta.md)（ベータ版）、Miro Insights などの主要プロバイダーと連携し、自社の知識を直接キャンバスに呼び出して活用できます。
- **企業ナレッジをプロンプトに活用**
  取得したナレッジをコンテキストとして、[Miro AI](01-miro-ai-overview.md)に促し、アイデア出しから創造プロセスを迅速化できます。
- **複数のアクセスポイント**
  Miro では、[サイドキック](07-sidekicks.md)や[フロー](04-flows-overview.md)などの複数のエントリーポイントでナレッジが利用可能であり、ワークフローの各段階において最も関連性の高いコンテンツを指定することができます。

:::note
管理者は、ナレッジと Miro AI の権限、ウェブ検索機能、およびコンプライアンスを確保するためのフォーマット作成を管理することができます。
:::

## ナレッジを使用して会社の情報を取得する

以下のいずれかのエントリーポイントからナレッジにアクセスできます。

:::note
ナレッジプロバイダーを初めて接続する際には、認証が求められます。
:::

- [**サイドキック**](06-sidekicks-overview.md)
  作成バーの上にある**サイドキック**をクリックします。**サイドキック**パネルが開きます。プロンプトボックスで**ナレッジ**をクリックします。ナレッジプロバイダーを接続するか、オンの位置に切り替えます。
  ![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)*サイドキックパネルでナレッジプロバイダーを選択し、Miroで企業のナレッジを取得します。*
  サイドキックのプロンプトを書きます。必要に応じてキャンバス上のオブジェクトを選択して文脈を追加することができます。プロンプトを実行すると、選択したプロバイダーがナレッジを活用します。

  > 💡 Knowledgeを活用して、キャンバス上でタスクを支援するカスタムAIエージェントとしての専門的なサイドキックを作成しましょう。
- [**Docs**](04-flows-overview.md) **in Flows**
  Docのコンテキストメニューから、**AIで編集**をクリックします。**サイドキック**パネルが開きます。プロンプトボックスで**Knowledge**をクリックします。知識プロバイダーを接続または選択します。プロンプトを実行すると、選択したプロバイダーをKnowledgeが活用します。
- [**AIインストラクションブロック**](05-flows.md) **内のフロー**
  AIインストラクションブロック内で、**知識ベースを選択** をクリックします。ナレッジプロバイダーに接続または選択します。AIインストラクションを実行すると、選択したプロバイダーを活用してナレッジを取得します。
- **単独チャット**
  Miroの単独チャットアプリでKnowledgeリソースにアクセスできます。
  - 作成バーの上で**サイドキック**をクリックします。**サイドキック**パネルが開きます。**Hey \{あなたの名前\}**の上で下向きのキャレットをクリックし、**もっとサイドキックを探す**をクリックします。**Knowledge**タブをクリックします。
  - 作成バーで**ツール、メディア、インテグレーション**を選択します。Knowledgeプロバイダーを検索して選択します。例えば、**Gemini**。チャットパネルが開きます。
