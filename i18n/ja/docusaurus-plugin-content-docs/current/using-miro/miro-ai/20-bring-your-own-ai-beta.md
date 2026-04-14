---
title: "\u6301\u3061\u8FBC\u307FAI\uFF08\u30D9\u30FC\u30BF\u7248\uFF09"
article_id: 21885197978642
translation_id: 21885197978642
locale: ja
sidebar_position: 20
created_at: '2024-10-09T18:45:40Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: ai-generate-image
---

Bring Your Own AI (BYOAI)は、Miro AIの一部の機能で、Miro AIの代わりに独自のAIプロバイダーを使用することを可能にします。

> **利用可能なプラン：**Enterprise
> **利用可能な環境：**デスクトップ

BYOAIでAIプロバイダーをMiroに接続し、[GPTに依存するAI機能を](18-miro-ai-reference.md)活用することができます。画像生成など、BYOAIがサポートしていないMiro AIの機能は、オプションで無効にすることができます。詳しくは、Bring Your Own AI以外のAI機能を無効にするをご覧ください。

現在、BYOAIはOpenAIとAzure OpenAIをサポートしています。

:::note
BYOAIはGPTによるMiro AI機能のみをサポートしています。どのMiro AI機能がGPTを搭載しているかについては、[Miro AIの概要を](18-miro-ai-reference.md)ご覧ください。
:::

## 持ち込みAIの設定方法

> **利用可能なプラン：**会社の管理者

以下の手順では、Open AIおよびAzure OpenAIのBYOAI（Bring Your Own AI）の設定方法を説明します。

### オープンAI

以下の手順に従ってください。

1. 管理者設定で、**アプリとインテグレーションを**選択します。
2. **Enterpriseインテグレーションでは**、**Bring your own AIで** **OpenAIを**選択します。
3. **APIキーには**、OpenAIのキーを入力します。
   > ⚠️ 最もセキュリティーを高めるため、APIキーをコピー＆ペーストしてください。
4. **接続を**選択します。
5. 組織でMiro AIが有効になっていることを確認してください。
   詳細はこちらBring Your Own AIのためのMiro AIの有効化をご覧ください。

   OpenAIでBYOAIの設定が完了しました。

:::note
Miroは一方向ストレージシステムを使用して、APIキーを安全に保存し暗号化します。キーが更新され、安全に保存された後、Miroも管理者もAPIキーを取得することができます。
:::

### Azure OpenAI

以下の手順に従ってください。

1. 管理者設定で、**アプリとインテグレーションを**選択します。
2. **Enterpriseインテグレーションでは**、**Bring your own AIで** **Azure OpenAIを**選択します。
3. Azure API キー、デプロイメント名、デプロイメント URL を入力します。
   > ⚠️ 最もセキュリティーを高めるため、APIキーをコピー＆ペーストしてください。デプロイがGPT-4oを使用していることを確認してください。
4. **接続を**選択します。
5. 組織でMiro AIが有効になっていることを確認してください。
   詳細はこちらBring Your Own AIのためのMiro AIの有効化をご覧ください。

   Azure OpenAIを使ったBYOAIのセットアップが完了しました。

:::note
Miroは一方向ストレージシステムを使用して、APIキーを安全に保存し暗号化します。キーが更新され、安全に保存された後、Miroも管理者もAPIキーを取得することができます。
:::

### Miro AIを有効にしてBring Your Own AIを実現

Open AIまたはAzure Open AIを接続したら、組織でMiro AIが有効になっていることを確認します。

以下の手順に従ってください。

1. 管理者設定で、**機能アクセスを**選択します。
2. **機能の有効化**]で、**Miro AIについて**以下のオプションのいずれかを選択します：
   - **全員が使用可**
   - **特定のチームが使用可**
3. (オプション）**Enable Miro AI Beta Featuresを**オンに切り替えます。

   組織でMiro AIが有効になりました。

:::note
デフォルトでは、Miro AIを有効にすると、すべてのMiro AI機能が利用可能になります。AIプロバイダによってサポートされていないMiro AI機能を無効にするには、Miroサポートに連絡してください。詳しくは、Bring Your Own AI以外のAI機能を無効にするをご覧ください。
:::

## Bring Your Own AIが搭載されていないAI機能の無効化

デフォルトでは、Miro AIを有効にすると、すべてのMiro AI機能が利用可能になります。BYOAI（Bring Your Own AI）は、GPTを活用するLLM機能のみをサポートします。BYOAIがAIプロバイダーがサポートするLLM機能のみを使用するようにするには、オプションでLLM以外のMiro AI機能を無効にすることができます。

LLM以外のMiro AI機能を無効にするには、Miroカスタマーサクセスマネージャーまたは[Miroサポートに](../tools/troubleshooting/06-contacting-miro-support.md)お問い合わせください。

詳細はこちら[Miro AIの概要を](18-miro-ai-reference.md)ご覧ください。

## よくある質問

**BYOAIを利用した場合のAI出力は誰が行うのですか？**

BYOAIでは、AIプロバイダーと設定した品質で、AIによる出力をコントロールすることができます。

**独自のAIプロバイダーを活用することで、入力モデレーションにどのような影響がありますか？**

BYOAIでは、MiroはAIプロバイダーが出力を生成する前にコンテンツをフィルタリングしません。モデレーションを有効にしたい場合は、プロバイダーによって入力モデレーションが有効になっているかどうかを確認し、カスタマーサクセスマネージャーまたは[Miroサポートに](../tools/troubleshooting/06-contacting-miro-support.md)ご連絡ください。

**BYOAIがAIのクレジット消費に与える影響とは？**

BYOAIでは、MiroのAI機能を実行するために、独自のAIプロバイダーからトークンを消費します。MiroのAIクレジットも消費し続けます。詳細については、[EnterpriseプランのMiro AIクレジットを](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/03-miro-ai-credits-for-enterprise-plans.md)ご覧ください。

**APIキーの有効期限が切れたり、トークンを使い切ったりした場合はどうなりますか？**

管理者としてはエラーメッセージが表示され、エンドユーザーはBYOAIを利用したAI機能を利用できなくなります。

**AIプロバイダーとのインテグレーションで問題が発生した場合、どのようにサポートを受けることができますか？**

カスタマー・サクセス・マネージャーまたはカスタマー・サポートにお問い合わせください。AIプロバイダーにも相談されることをお勧めします。

**BYOAIを使用した場合、Miroは何らかの入力や出力を使用するのでしょうか？**

いいえ、データの入出力はプロバイダーとの契約に従います。
