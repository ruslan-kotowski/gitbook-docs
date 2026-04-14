---
title: Amazon Q（ベータ版）
article_id: 31347586131346
translation_id: 31347586131346
locale: ja
sidebar_position: 3
created_at: '2025-11-25T13:35:45Z'
updated_at: '2025-12-29T15:25:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: '操作できるユーザー：: ボードの所有者、ボードの共同所有者、ボード編集者、チームメンバー、チームの管理者、ユーザーの管理者、コンテンツ管理者、（セットアップ）会社の管理者、Amazon
    Q 管理者 対象プラン：: Business、Enterprise 対象プラットフォーム：: ブラウザー、デスクトップ'
---

Amazon Q インテグレーションにより、チームは企業知識を Miro AI プラットフォームにサイドキックやフローを通じて取り込むことができます。エンタープライズインテリジェンスはMiroの中で直接提供され、視覚化されます。

:::note
Amazon Q のインテグレーションは Miro AI プラットフォームでのみ利用できます。[ここで登録](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb)してアクセスを取得してください。 Miro AI プラットフォームがあなたの組織で有効化されたときに通知が届きます。
:::

企業の知識はしばしば Slack、Confluence、Salesforce、Google Drive など多数のツールや内部リポジトリに散在しており、プロダクトマネージャーや技術リーダー、テクノロジーチームが重要な詳細を探し、インサイトを一致させるために貴重な時間を費やすことを余儀なくされています。

以下の Miro および Miro AI の機能は Amazon Q インテグレーションをサポートしています：

- [**フロー**](../../using-miro/miro-ai/04-flows-overview.md)
  分散した情報を明確な成果物に変えるワークフローを視覚化し、チームがどのように洞察を行動に移すかを自動化および標準化するのを支援します。
- [**サイドキック**](../../using-miro/miro-ai/06-sidekicks-overview.md)
  ボードのコンテンツや企業データを吟味するAIエージェントと連携して作業し、新しいアーティファクトを生成したり、即時の洞察を提供したり、アイデア出し、ドキュメント化、デザインを加速させたりします。

## Amazon Q インテグレーションの設定

[ここのリンク](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb)からサインアップを確認し、Miro AIプラットフォームが貴社向けに有効化されていることの確認を受けた後、次の2つの手順を完了してください。

Amazon Q インテグレーションを Miro と設定するには、まず Miro を Amazon Q Business にデータアクセサーとして追加し、その後 Ama…ンを Miro の管理者コンソールに接続する必要があります。

### Amazon Q BusinessにMiroをデータアクセサーとして追加する

1. Amazon Q Business コンソールで、ナビゲーションペインの**アプリケーション**をクリックします。
2. データアクセサーを追加したいアプリケーションをクリックします。
3. ナビゲーションペインの**データアクセサー**をクリックします。
4. **データアクセサーを追加**をクリックします。
5. **データアクセサー**の下で、**Miro** に対してプラス (**+**) アイコンをクリックします。
6. **外部 ID**には、Miro の組織 ID を追加します。
   Miro の組織 ID を取得するには、Miro の管理者コンソールにアクセスしてください。ブラウザの URL バーから組織 ID をコピーしてください。
   ![](../../../../../../docs/integrations-apps/amazon-web-services-aws/images/31367058137746_image.png)
   *管理者コンソールで組織 ID を確認できます。ID はブラウザの URL バーからコピー可能です。*
7. **データ アクセサーを追加**をクリックします。
8. 次の詳細をメモしてください。それぞれの値は Miro 管理者コンソールで設定を完了するために必要です。
   - アプリケーション ID
   - IdC アプリケーション ARN
   - レトリーバー ID
   - アプリケーション リージョン
   - IdC アプリケーション リージョン

### Amazon Q インデックスを Miro の管理者コンソールに接続する

1. Miro で、**管理コンソール** > **アプリとインテグレーション** > **アプリ** >**アプリを追加** に進みます。
2. Amazon Q を検索して探します。

   > ✏️ 名前で Amazon Q が見つからない場合は、次のクライアント ID を使用して検索してください: `1601842442647206821`。
3. アプリのプロフィールで、**すべてのチーム** または **特定のチーム** のいずれかを選択してアプリを追加します。
4. 権限ページを確認します。

   > ✏️ Amazon Q アプリは Miro によって開発および管理されており、特定の権限は必要ありません。
5. **追加** をクリックします。
6. **アプリ** > **アプリの管理** に進みます。
7. Amazon Q を検索して見つけます。
8. **設定** をクリックします。
9. Amazon Q のデータアクセス詳細を追加します。Amazon Q Business に Miro をデータアクセスとして追加するの最終ステップを参照してください。
10. **保存** をクリックします。
    設定が適用されます。
