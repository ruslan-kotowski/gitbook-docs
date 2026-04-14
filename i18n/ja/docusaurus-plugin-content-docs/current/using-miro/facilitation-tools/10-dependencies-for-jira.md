---
title: "Jira \u306E\u4F9D\u5B58\u95A2\u4FC2"
article_id: 10649083010834
translation_id: 10649083010834
locale: ja
sidebar_position: 7
created_at: '2023-03-22T10:22:08Z'
updated_at: '2025-11-25T16:22:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

Miro ボード上の[プランナー](../../integrations-apps/atlassian/21-planner-for-jira.md)や Miro ボードのどこにでも Jira カード間の既存の依存関係をマップしたり、新しい依存関係を作成したりすることができます。 それらは Jira で瞬時に同期されます。依存関係アプリを使用することで、プランニングの作業中に、依存関係の特定、視覚化、議論、記録をリアルタイムで行うことができます。

> ****💡**** この機能は現在、[Azure DevOps](08-dependencies-for-azure-devops.md)でも利用可能です。

> **利用可能なプラン:** Business プラン、Enterprise プラン
>
> **利用可能な環境:** デスクトップブラウザー、デスクトップアプリ

## 依存関係の仕組み

依存関係は接続線のレイヤーとして表示され、Jira カード間の関係を示します。

依存関係はボード上で開いた時にだけ見えます。 参加者はさまざまな依存関係のタイプをフィルターして、ブロッカーや関連性を議論できます。

![Dependencies-app.png](../../../../../../docs/using-miro/facilitation-tools/images/13244544218258_Dependencies-app.png)
*プランナー ウィジェット上の Jira カード間でマップされた依存関係*

## 新しい依存関係の作成方法

1. ボード左側の作成ツールバーに移動します。
2. **依存関係**アイコンをクリックします。作成ツールバーに依存関係アイコンがない場合は、**ツール、メディア、インテグレーション**（**+**）から追加します。
3. 依存関係のパネルが開きます。
4. **新しい依存関係**をクリックします。
5. **[1 番目のカード]**をクリックし、ドロップダウンから、もしくは検索して Jira 課題を選択します。
6. Jira インスタンスで利用可能なもの（例：Blocks（ブロック）、Clones（クローン）、Duplicates（重複）、Relates to（関連））に基づいて、 **依存関係タイプ**を選択します。
7. **[2 番目のカード]**をクリックし、ドロップダウンから、もしくは検索して Jira 課題を選択します。
8. **下書きを保存**、または **Jira に保存**を直接クリックします。

:::tip
依存関係の下書きは Miro にのみ保存されます。依存関係の下書きを作成して、プランニング作業中に他の参加者やチームに提案することができます。その下書きは、確認・検討後、Jira に保存、もしくは削除することができます。
:::

![dependencies-entry-point.png](../../../../../../docs/using-miro/facilitation-tools/images/21537435953426_dependencies-entry-point.png)
*新しい依存関係の作成と Jira への保存*

## 依存関係の閲覧と絞り込み方法

1. ボード左側の作成ツールバーに移動します。
2. 依存関係の**アイコン**をクリックします。作成ツールバーに依存関係のアイコンがない場合は、**ツール、メディアおよびインテグレーション** (**+**) から追加する必要があります。
3. 依存関係のパネルが開き、既存の依存関係はボード上に線で表示されます。
4. 依存関係パネルの上部にある**フィルター**アイコンをクリックします。
5. トグルスイッチを使用して、**依存関係のタイプ**と**同期ステータス**でフィルターします。
6. 依存関係が表示される際の条件を制御するために**線を表示**ドロップダウンを使用します。すべてのアクティブな依存関係を表示するには**常に**を選択します。特定のAzureカードまたは依存関係のタイプをクリックしたときのみ依存関係を表示するには、**選択時**を選びます。

点線は下書きの依存関係を示し、実線は Jira に同期された依存関係を示します。線の色は依存関係のタイプを表します。

![Filtering-dependencies.gif](../../../../../../docs/using-miro/facilitation-tools/images/13245295619730_Filtering-dependencies.gif)
*依存関係ビューのフィルタリング**プランナーウィジェット上*

## 依存関係の編集、保存、削除方法

1. ボード左側の作成ツールバーに移動します。
2. 依存関係**アイコンをクリックします。**
3. 依存関係のパネルが開きます。
4. 依存関係の横にある**編集**アイコンをクリックします。

![The_option_to_edit_a_Dependency.jpg](../../../../../../docs/using-miro/facilitation-tools/images/10866625733778_The%20option%20to%20edit%20a%20Dependency.jpg)
*依存関係の編集*

依存関係の**1 番目のカード**と**2 番目のカード**，および**依存関係タイプを変更できます。**

*![Editing_a_dependency.gif](../../../../../../docs/using-miro/facilitation-tools/images/10866808392722_Editing%20a%20dependency.gif)**1 番目のカードと依存関係タイプを変更*

**Jira に保存**をクリックして、依存関係の下書きを Jira に保存し、同期させます。

![Save_to_Jira.png](../../../../../../docs/using-miro/facilitation-tools/images/10868740630034_Save%20to%20Jira.png)
*依存関係の下書きを Jira に保存する*

**下書きに戻す**をクリックして、同期された依存関係を下書きに戻します。

![Revert_to_draft.png](../../../../../../docs/using-miro/facilitation-tools/images/10868741500690_Revert%20to%20draft.png)
*同期された依存関係を Jira で下書きに戻す*

依存関係を削除するには、**ゴミ箱**アイコンをクリックします。
![Delete_dependency.png](../../../../../../docs/using-miro/facilitation-tools/images/10868804195986_Delete%20dependency.png)*依存関係の削除*
