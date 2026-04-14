---
title: Gemini Enterprise インテグレーション（ベータ版）
article_id: 32304596526482
translation_id: 32304596526482
locale: ja
sidebar_position: 1
created_at: '2026-01-05T10:38:04Z'
updated_at: '2026-02-17T09:38:53Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: '実施可能な人: 会社の管理者 対象プラン: Business, Enterprise プラットフォーム: ブラウザ、デスクトップ'
---

会社の管理者として、Miro組織内のチームでGemini Enterpriseインテグレーションを有効化し、設定することができます。

Gemini Enterpriseインテグレーションにより、MiroでGemini Enterpriseを[知識](../../using-miro/miro-ai/09-knowledge.md)リソースとして接続できます。例えば、サイドキックやフローに企業インテリジェンスを提供するためにGemini Enterpriseを使用することができます。

また、Gemini EnterpriseをMiroの[単独のチャット](../../using-miro/miro-ai/09-knowledge.md)アプリに接続することもできます。

Gemini Enterpriseインテグレーションを使用するには、次のステップに従ってください:

1. Gemini Enterpriseアプリを有効にします。
   1. 会社の管理者として、**管理コンソール**にアクセスします。
   2. **アプリ＆インテグレーション** > **アプリ** > **アプリを追加**へ進みます。
   3. **Gemini Enterprise**を検索し、見つけます。
      アプリ名で見つからない場合、以下のクライアントIDで検索してください：`2392210303456548729`。
   4. アプリの**プロフィール**で、**\{Team name\}内のすべてのチーム**または**特定のチーム**でアプリを追加するかを選択します。
   5. **追加**をクリックします。
2. Gemini Enterprise アプリを設定します。
   1. **管理コンソール**で、**アプリとインテグレーション** >**アプリ**に移動します。
   2. Gemini Enterprise の**許可**がオンになっていることを確認し、**設定**をクリックします。
   3. Gemini Enterprise の構成詳細を追加します。
      Project ID の確認方法については、（外部）[Project ID を確認する](https://support.google.com/googleapi/answer/7014113?hl=en)をご覧ください。
      App ID を取得するには、Gemini Enterprise の「Apps」に移動し、ID 列の値を使用します。
      ![](images/33222285664274_image (2).png)
      *Miro で使用するための Gemini Enterprise アプリを構成します。*

      > ✏️ **Project ID** と **App ID** は必須です。他のフィールドはオプションです。
   4. **保存** をクリックします。

:::note
メンバーが Gemini Enterprise を[ナレッジ](../../using-miro/miro-ai/09-knowledge.md)リソースとして最初に接続する際に、認証が求められます。メンバーは Gemini Enterprise ライセンスを持っている必要があります。
:::
