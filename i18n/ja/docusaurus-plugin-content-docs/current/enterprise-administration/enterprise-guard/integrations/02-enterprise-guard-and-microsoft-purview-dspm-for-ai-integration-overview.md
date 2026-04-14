---
title: "Enterprise Guard \u3068 Microsoft Purview DSPM \u306B\u3088\u308B AI \u30A4\
  \u30F3\u30C6\u30B0\u30EC\u30FC\u30B7\u30E7\u30F3\u6982\u8981\uFF08\u30D9\u30FC\u30BF\
  \u7248\uFF09"
article_id: 28617278171154
translation_id: 28617278171154
locale: ja
sidebar_position: 0
created_at: '2025-08-07T15:17:38Z'
updated_at: '2026-01-12T11:27:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Microsoft Entra ID（旧 Azure AD）をアイデンティティプロバイダーとして利用する組織向けに、Enterprise Guard は AI プロンプトと応答を AI セキュリティとコンプライアンスチームが Microsoft Purview データセキュリティー態勢管理（DSPM）に安全に転送し、それにより単一の信頼できるプラットフォームから生成型 AI の使用を監視、監査、制御することができます。これにより、運用の負担を軽減し、データ漏洩や誤用などのリスクを軽減し、Miro のエンタープライズグレードの AI ガバナンスを強化します。

:::note
ベータ版では、ダイアグラム、マインドマップ、文書、プロトタイプ、付箋、テーブルなどの Miro AI フォーマットをサポートしており、画像は含まれていません。今後のリリースでは、画像のサポートやさらに多くの AI 機能を追加できるよう取り組んでいます。
:::

## **対象者**

この機能は、Miro および Microsoft Entra ID（旧 Azure AD）/Microsoft Purview を管理している Enterprise Guard のお客様向けに、ベータ版で利用可能です。

## **提供内容**

- **一元的な可視化：**Microsoft Purview の AI ハブで Miro AI の使用状況を閲覧
- **監査可能性：**プロンプト（ユーザー入力）と応答（AI 出力）は記録され、レビューのために保存されます。
- **ガバナンスの整合性：**既存の Purview ワークフローを使用して、監視、アラート、強制保持を行います。

## **要件**

### **Miro**

- Enterprise プランで **Enterprise Guard** が有効です。
- あなたは**会社の管理者**です。
- Miro で SSO プロバイダーとして Microsoft **Entra ID** が構成されています。
- **Enterprise インテグレーション** ページへのアクセス（もし見つからない場合は、**会社の管理者**にアクセス許可を依頼してください）。
- この機能をベータで有効にするには、カスタマーサクセス マネージャーにお問い合わせください。

### **Microsoft**

- 有効な **Microsoft Purview** ライセンス。
- **Microsoft Entra ID テナント ID**（Miro SSO で使用される同じテナント；Microsoft 組織/テナントを識別する GUID）。
- テナント全体の管理者承認をアプリケーションに**付与できる**Entra の役割。

## **仕組み**

1. Miro 管理者が Miro の **Enterprise インテグレーション** ページから Microsoft Entra テナントを接続します。
2. これにより、**Miro AI ガバナンス**アプリケーションがあなたの Microsoft テナントにインストールされます（テナント全体の管理者承認を通じて）。
3. ユーザーがそのテナントを通じて Miro にサインインし、Miro AI を使用すると、Miro はプロンプト/レスポンスを Microsoft Purview に転送します。
4. アクティビティーは Microsoft Purview の**DSPM for AI → Activity explorer**（AI アクティビティーを一覧表示する Purview 閲覧画面）に表示されます（取り込み時間を考慮してください）。

## **データの可視性とレイテンシー**

- 記録データ:**AI プロンプトとレスポンス**は、SSO 経由で設定されたテナントにサインインしたユーザーによって Miro で生成されます。
- 表示場所:**Microsoft Purview → DSPM for AI → アクティビティー エクスプローラー**（Purview で AI アクティビティーをリストするビュー）。監査ログでも情報を閲覧できます。
  **注意:**Miro AI の機能を通じて生成されるすべてのテキストベースのプロンプトとレスポンスは、Purview に転送されます。現在、画像コンテンツは Microsoft Purview に転送されていません。
- レイテンシー:AI アクション後、記録は通常**10～30 分以内**に表示されます。

## **既知の制限事項**

- ベータ版は、ダイアグラム、マインドマップ、文書、プロトタイプ、付箋、テーブルなど、Miro AI のフォーマットをサポートしていますが、画像はサポートしていません。今後のリリースで、画像やさらに多くの AI 機能のサポートを追加するべく取り組んでいます。
- Miro では、一度に**1 つの Microsoft Entra テナント ID**を設定できます。
- マルチ IdP またはマルチテナント環境では、**設定されたテナント**を介して Miro にサインインするユーザーのアクティビティー**のみ**が Microsoft Purview に記録されます。

## **セキュリティーとプライバシー**

Miro は AI のプロンプトとレスポンスを **お客様の Microsoft テナント** に転送し、それらを Purview で監視できるようにします。**ガバナンス、強制保持、アクセス制御**は、お客様の Microsoft 環境で管理されます。

##

## **よくある質問**

- **Q:どの Miro AI 機能が記録されていますか？**
  **A:**Miro AI のすべてのテキストベースのプロンプトとレスポンスが Purview に転送されます。現在、画像コンテンツは Microsoft Purview に転送されていません。
- **Q:すべてのユーザーが対象ですか？**
  **A:**設定された Microsoft Entra テナントを使用して Miro に認証するユーザーのみが対象です。
- **Q:Miro からログをエクスポートできますか？**
  **A：**エクスポートや保持には Microsoft Purview を使用します。Miro はアクティビティをお客様の Microsoft テナントに転送し、そこでお客様のポリシーに従って管理されます。
- **Q：セキュリティーとプライバシーはどうですか？**
  **A：**Miro は AI プロンプトと応答を**お客様の Microsoft テナント**に転送し、Purviewで監視できるようにします。**ガバナンス、強制保持、およびアクセス制御**は、お客様の Microsoft 環境で管理されます。

## **サポートとリソース**

- Entra の同意に関する前提条件については、アプリケーションへの**テナント全体の管理者同意の付与**に関する Microsoft のドキュメントを参照してください。
- Enterprise Guard のセットアップ手順については、[このドキュメント](../../enterprise-subscription-management/integrations/03-set-up-microsoft-purview-dspm-for-miro-ai.md)をご覧ください。
