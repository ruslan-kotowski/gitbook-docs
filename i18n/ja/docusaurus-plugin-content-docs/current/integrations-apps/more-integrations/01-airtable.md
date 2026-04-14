---
title: Airtable
article_id: 360012807619
translation_id: 360012807619
locale: ja
sidebar_position: 1
created_at: '2020-03-24T12:09:00Z'
updated_at: '2025-08-05T07:33:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'ユーザー: すべての Miro ユーザー、有料 Airtable プランのユーザー Miro プラン: すべてのプラン プラットフォーム: ブラウザー'
---

Airtable を使用して、ホワイトボード視覚化の機能を作業に活用しましょう。Miro から Airtable へデータをエクスポートし、Airtable 内で Miro ボードを埋め込んで閲覧、コメント、編集できます。

## Miro ボードから Airtable へデータをエクスポートする

Airtable Sync インテグレーションにより、Miro ボードからデータをエクスポートして Airtable で整理することができます（例: 付箋、カード）。この機能の設定と使用方法について詳しく知るには、[Airtable の公式ドキュメント](https://support.airtable.com/docs/airtable-sync-integration-miro)をご覧ください。

## Miro ボードを Airtable ベースに埋め込む

### Airtable に Miro アプリをインストールする

:::warning
Airtable 用の Miro アプリは**Safari** ブラウザーでは**利用できません**。
:::

Airtable のベース編集者は Miro アプリをインストールできます。そのためには:

1. Airtable のベースを開き、右上にある**拡張機能**をクリックします。

   ![Airtable extensions button in the top right corner.](../../../../../../docs/integrations-apps/more-integrations/images/21017651877394_Airtable%20extensions.jpg)
   *Airtable ベースの右上にある拡張機能ボタン。*
2. **拡張機能を追加**をクリックします。

   ![Add an extension option in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017647938834_add%20an%20extension.jpg)
   *新しい拡張機能を追加するオプション。*
3. Airtable マーケットプレイスで「Miro」を検索し、**Add** をクリックします。

   ![Miro app in Airtable Marketplace.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933714_Miro%20in%20Airtable.jpg)
   *Airtable マーケットプレイスの Miro アプリ。*

### 既存の Miro ボードを Airtable ベースに追加する

Miro アプリが Airtable ベースに追加されたら、拡張パネルに表示される Miro アプリ セクションで**ボードを追加**をクリックします。

![Add a Miro board button in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651876498_add%20a%20Miro%20board.jpg)
*Airtable の Miro アプリを通じて Miro ボードを追加する。*

Miro ボードピッカーが表示されます。ブラウザーで Miro にログインしていない場合は、サインインするか Miro アカウントを作成するように求められます。

ボードを選択した後、ドロップダウン メニューを使用して Airtable 内での表示方法に対する共有権限を設定します。次の 3 つのオプションがあります。

- **全員が閲覧可:**Airtable の誰でも埋め込みボードのコンテンツを[閲覧](../../using-miro/sharing-boards/01-board-access-rights.md)できます。
- **全員がコメント可:**Airtable の誰でも埋め込みボードに[コメントを残す](../../using-miro/sharing-boards/01-board-access-rights.md)ことができます。（注：このオプションは、Miroの[Freeプラン](../../plans-billing/miro-plans/09-free-plan.md)に保存されたボードでは利用できません。)
- **プライベート:**ボードは、Miro側で設定された既存の共有設定に従います。

  > ✏️ Miroの[Enterpriseプラン](../../plans-billing/miro-plans/04-enterprise-plan.md)のユーザーの場合、アクセス設定は組織全体のアクセス管理に従うため、いくつかの共有オプションが制限されている可能性があります。詳しくはこちら：[埋め込みインテグレーションのEnterprise共有ポリシーの管理](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)。

![Sharing settings options when adding a Miro board to Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651879826_board%20access%20in%20Airtable.jpg)
*Airtable に Miro ボードを追加する際の共有設定。*

埋め込まれた Miro ボードは Airtable ベースに表示され、設定された権限に基づいて閲覧、コメント、編集できます。

![Embedded Miro board within an Airtable base.](../../../../../../docs/integrations-apps/more-integrations/images/21017651872402_Miro%20board%20in%20Airtable.jpg)
*Airtable 内に埋め込まれた Miro ボード。*

埋め込まれたボードを別のものに置き換えるには、Airtable の Miro アプリの歯車アイコン（**設定**）をクリックし、**ボードを選択**を選び、Miro ピッカーから別のボードを選んでください。

![Replacing an embedded Miro board in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017647932690_replacing%20a%20board.jpg)
*Airtable で埋め込まれた Miro ボードの交換。*

### Airtable から新しい Miro ボードを作成する

Airtable から直接新しい Miro ボードを作成するには:

1. Airtable 内の Miro アプリ セクションで、**ボードを追加**（既に埋め込まれている場合、**ボードを選択**）をクリックします。
2. Miro ピッカーで、**新しいボード**を作成するオプションを選択します。

![Creating a new Miro board from the picker within Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651880466_add%20a%20new%20board%20to%20Airtable.jpg)
*Airtable のピッカーで新しい Miro ボードを作成。*

新しいボードはあなたの Miro アカウントに作成され、Airtable ベースに埋め込まれます。

### Airtable から Miro ボードを削除する

埋め込まれた Miro ボードを Airtable ベースから削除するには、そのベース内の Miro アプリ拡張機能を削除するか再設定する必要があります。拡張パネルの Miro アプリでドロップダウンメニューをクリックし、拡張機能を削除または管理するオプションを選択します。

![Deleting the Miro app from Airtable extensions panel.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933074_deleting%20the%20app.jpg)
*Airtable の拡張パネルから Miro アプリを削除。*
