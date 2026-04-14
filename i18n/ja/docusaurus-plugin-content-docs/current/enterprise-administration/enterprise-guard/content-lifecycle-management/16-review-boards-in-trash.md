---
title: "\u30B4\u30DF\u7BB1\u306E\u4E2D\u306E\u30EC\u30D3\u30E5\u30FC\u30DC\u30FC\u30C9"
article_id: 21118388045970
translation_id: 21118388045970
locale: ja
sidebar_position: 16
created_at: '2024-09-02T16:34:18Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

コンテンツエクスプローラー（図1）により、[コンテンツ管理者は](../../../administration/get-started-as-a-miro-admin/02-understand-admin-roles-and-their-privileges.md)ゴミ箱にあるすべてのボードを見ることができます。

![trash_ce.png](images/21358795621010_trash_ce.png)

*図 1：ゴミ箱にボードを表示するコンテンツエクスプローラー*

コンテンツ エクスプローラーでは、次の操作が一つの場所で実施できます。

- ゴミ箱内のボードの表示ボード名、ボードの所有者、ボードが削除された日付、ゴミ箱に残された時間、適用される強制保持ポリシーに従ってボードが保持される日付などの情報を表示します。
- 結果を絞り込み、要件固有の情報を表示します。例えば、チーム、オーナー、機密分類などの一般的な基準に基づいてボードのリストをフィルタリングすることができます。また、trashed from、trashed until、purging from、purging untilのような削除基準に基づいてフィルタリングすることもできます。- 一度に複数の条件に基づいて絞り込むことができます。
- 行の項目をクリックして、ゴミ関連のボード情報を確認してください。スライドアウトパネル（図2）が表示され、ボード名、ボードの所有者、ボードが所属するチーム、ボードが削除された日付、ボードが最後に修正された日付、ボードを削除したユーザー、ボードが強制保持されるまでの日付などの情報を見ることができます。
  ![trash_ce_フライアウト.png](images/21358821122578_trash_ce_flyout.png)
  図 1：スライドアウトパネル

:::note
ゴミ箱のボードを確認するには、[コンテンツ管理者ロールが](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)必要です。コンテンツ管理者になるには、会社の管理者に連絡してください。
:::

## ゴミ箱の中のレビューボード

ゴミ箱にあるボードを確認するには、以下の手順を実行します：

1. **コンテンツ エクスプローラーのページ**を開いている場合は、ステップ 2 に進んでください。
   **コンテンツ エクスプローラー**を開いていない場合：
   a. [Miro の設定](https://miro.com/app/settings)に移動します。
   b. 左側のペインで、**Enterprise Guard の**下の**コンテンツ エクスプローラー** をクリックします。
2. **コンテンツ エクスプローラー]** ページの [**コンテンツのライフサイクル**] で [**ゴミ箱**] をクリックします。
3. **コンテンツエクスプローラー/ゴミ箱**ページで、レビューしたいボードをクリックします。
   画面の右側にスライドアウトパネル（図 3）が表示され、以下の情報が表示されます。
   - ボード名
   - ボードの所有者
   - ボードが所属するチーム
   - ゴミ箱からボードを復元することができます。
   - Delete board permanently ボタンは、ボードを永久に削除することができます。なお、強制保持ポリシーは引き続き適用されます。
   - ボードを削除したユーザー、
   - ボードが強制保持されるまでの日付![trash_ce_flyout.png図](images/21358821122578_trash_ce_flyout.png)3：スライドアウトパネル

## コンテンツ エクスプローラーのボードリストを絞り込み

コンテンツ エクスプローラーが、強制保持中のボードの長いリストを表示し、特定の要件に基づいて結果をカスタマイズしたい場合があるかもしれません。データガバナンス管理者は、様々な基準でボードのリストを絞り込みできるようになり、重要なコンテンツのライフサイクル管理タスクに集中できるようになりました。 [詳細については、「](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)[ゴミ箱のボードの検索、フィルタ、並べ替え」の「ボードのリストをフィルタする](14-search-filter-or-sort-list-of-boards-in-trash.md)」を参照してください。
