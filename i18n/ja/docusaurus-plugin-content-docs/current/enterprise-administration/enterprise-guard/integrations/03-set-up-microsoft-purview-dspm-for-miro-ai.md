---
title: "Miro AI\uFF08\u30D9\u30FC\u30BF\u7248\uFF09\u306E Microsoft Purview DSPM \u306E\
  \u8A2D\u5B9A"
article_id: 28698434922386
translation_id: 28698434922386
locale: ja
sidebar_position: 8
created_at: '2025-08-11T19:20:50Z'
updated_at: '2026-01-12T11:28:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

この手順は、Miro AI の Microsoft Purview データセキュリティー態勢管理（DSPM）を設定し、Miro のAIプロンプトと応答をMicrosoft PurviewのAI向けDSPMに表示させるためのものです。設定後にイベントを確認し、インテグレーションを管理する方法を学びます。

## **前提条件**

### **Miro**

- Enterprise Guardが有効化されているEnterprise プラン。
- あなたがCompany Adminであること。
- Microsoft Entra IDがSSOプロバイダーとしてMiroで構成されていること。
- ベータ版でこの機能を有効化するには、お客様担当者に連絡してください。

### **Microsoft**

- DSPM for AI をサポートするアクティブな Microsoft Purview ライセンス。
- Miro の SSO に使用する Microsoft Entra ID テナント ID （Microsoft 組織/テナントを識別する GUID）。
- アプリケーションにテナント全体の管理者承認を与えることができる Entra ロール。

## **Miro でのインテグレーションの設定**

1. Miro で **Enterprise 設定 → Enterprise インテグレーション**を開きます。
2. 下にスクロールして**Microsoft Purview DSPM for AI**をオンに切り替えます。
3. テナント ID ボックスに、**Microsoft Entra テナント ID**を入力します。
4. **接続**をクリックします。
5. プロンプトが表示されたら、**テナント全体の管理者同意**を与えることができるアカウントで Microsoft Entra にサインインします。
6. **Miro AI ガバナンス**アプリケーションの同意内容を確認し、**受け入れる**をクリックします。
7. Miro に戻り、インテグレーションが**接続済み**と表示されていることを確認します。

## **Microsoft Purview でアクティビティーを検証**

1. Miroで、簡単なAIアクションを実行します（例: ボード上の付箋を**要約**）。
2. 取り込みを待つ**時間は最大10〜30分**です。
3. Microsoft Purviewで、**Microsoft Purview → DSPM for AI → アクティビティ エクスプローラー**に移動します（これはAIアクティビティを一覧表示するPurviewビューです）。監査ログにも情報を表示できます。
   メモ: Miro AIの全機能で生成されるテキストベースのプロンプトとレスポンスは全てPurviewに転送されます。現在、画像コンテンツはMicrosoft Purviewに転送されていません。
4. イベントを**最近**でフィルタリングし、Miroからのアクティビティを（例: プロンプトとレスポンス）探します。

## **インテグレーションの管理**

- **切断**: Miro で、**Enterprise integrations → Microsoft Purview for AI → Disconnect** に移動します。
- **テナントの変更**: まず**切断**し、その後、別の**テナントID**を使用して再**接続**します。

## **トラブルシューティング**

- **統合オプションがない**: 組織が**Enterprise Guard**を持ち、アカウントが**Enterprise integrations**にアクセスできることを確認してください。**Company Admin**にアクセス権の付与を依頼してください。
- **テナントIDの不一致または接続エラー**: テナントIDは、Miro の**SSO**に使用されている Microsoft Entra テナントと**正確に一致**している必要があります。
- **同意に失敗またはサインインループ**: **テナント全体の管理者同意**を付与できるアカウントでサインインします（Microsoft の管理者と連携してください）。
- **アクティビティーが表示されない**: ユーザーが**設定されたテナント**を介してMiroにサインインし、テストAIアクションを実行したことを確認します。**10～30分**待ち、**Purviewライセンス**を確認し、**DSPM for AI → Activity Explorer**をチェックします。
- **複数のテナント/IdP**: Miroで設定できるのは**1つのテナント**のみです。他のテナント/IdP用のSSOを介してサインインするユーザーのアクティビティーは**転送されません**。

## **既知の制限事項**

詳細については、[概要ドキュメントの既知の制限事項セクション](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md)を参照してください。
