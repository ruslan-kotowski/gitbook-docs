---
title: "Azure DevOps\u306E\u4F9D\u5B58\u95A2\u4FC2"
article_id: 15556757538450
translation_id: 15556757538450
locale: ja
sidebar_position: 6
created_at: '2023-12-05T11:50:18Z'
updated_at: '2025-11-25T15:39:53Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

[プランナー](../../integrations-apps/microsoft/09-planner-for-azure-devops.md)上のAzureカード間、またはMiroボード上の任意の場所に依存関係をマッピングします。依存関係アプリを利用することで、プランニングの作業中に、依存関係の特定、視覚化、議論、記録をチーム間でリアルタイムに行うことができます。

:::note
Azure DevOpsで依存関係を使用するには、まず[Azureインテグレーションをセットアップ](../../integrations-apps/microsoft/03-azure-cards.md)します。
:::

## 依存関係の仕組み

依存関係は接続線のレイヤーとして表示され、Azure カード間の関係を示します。

これらは、ボード上で依存関係を開いたときにのみ表示されます。参加者は、さまざまな依存関係タイプを絞り込んで、ブロッカーと関連性について検討することができます。

![Mapping-dependencies-Azure.pngAzureのマッピングされた](../../../../../../docs/using-miro/facilitation-tools/images/15603398527890_Mapping-dependencies-Azure.png)
*依存関係*

## 依存関係の閲覧と絞り込み方法

:::note
Azure で作成済みの依存関係のみを閲覧およびフィルタリングできます。まもなく、MiroでAzureカード間の依存関係を直接作成および編集できるようになります。
:::

1. ボードの左側にある作成ツールバーに移動します。
2. **依存関係**のアイコンをクリックします作成ツールバーに「依存関係」アイコンがない場合は、**「ツール」→「メディアとインテグレーション」****（+）から**追加する必要があります。
3. Dependencies パネルが開き、既存の依存関係がボード上に線として表示されます。
4. 依存関係パネルの上部にある **[検索条件]** アイコンをクリックします
5. トグルを使用して、以下の方法でフィルタリングします。 **依存関係のタイプ**。
6. **行の表示]**ドロップダウンを使用して、依存関係を表示するタイミングを制御します。すべてのアクティブな依存関係を表示するには、[**常に**] を選択します。特定の Azure カードまたは依存タイプをクリックしたときにのみ依存関係を表示するには、[**選択時**] を選択します。

![Mapping-dependencies-Azure-and-Jira.png](../../../../../../docs/using-miro/facilitation-tools/images/15603699800338_Mapping-dependencies-Azure-and-Jira.png)
*マッピングされた依存関係の*

## 同じボード上の Jira と Azure カード

チームが Azure DevOps と Jira を使用しており、Miro で両方のインテグレーションを設定している場合、1 つのボードで両方のシステムのカードと依存関係を管理することができます。

依存関係は、2 つの Jira カードまたは 2 つの Azure カードをリンクします。依存関係を持つ Azure カードと Jira カードの両方を持つボードで依存関係アプリを開くと、これらのカード間のすべての既存のリンクが表示されます。

1 つのシステムからの依存関係だけをフィルタするには、**[Jira に保存]**および**[Azure に保存**] トグルを使用します。

![Dependencies-mapped-between-Jira-and-Azure-cards.pngJira](../../../../../../docs/using-miro/facilitation-tools/images/15603628660626_Dependencies-mapped-between-Jira-and-Azure-cards.png)
*と Azure の両方の依存関係を単一の Miro ボードにします。*
