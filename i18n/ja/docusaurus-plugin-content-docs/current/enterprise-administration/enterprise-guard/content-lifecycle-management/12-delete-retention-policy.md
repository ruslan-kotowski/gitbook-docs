---
title: "\u5F37\u5236\u4FDD\u6301\u30DD\u30EA\u30B7\u30FC\u3092\u524A\u9664"
article_id: 19205219887762
translation_id: 19205219887762
locale: ja
sidebar_position: 12
created_at: '2024-05-28T18:02:52Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

強制保持ポリシーを削除すると、該当する強制保持ポリシーが適用されていたボードが解放されます。これらのボードは、制約なしに永久に削除することができます。

:::note
強制保持ポリシーを削除するには、[Data Governance Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)が必要です。データガバナンス管理者の権限をリクエストするには、会社の管理者にご連絡ください。
:::

強制保持ポリシーを削除するには、次の手順を実行してください。

1. [Miro の設定](https://miro.com/app/settings)に移動します。
2. 画面の左ペインで、**Enterprise Guard**の下にある**コンテンツのライフサイクル**をクリックします。
3. **保持**タブをクリックします。
4. 「**強制保持** **ポリシー**」のページで、削除する強制保持ポリシーをクリックします。
   ポリシーに関連する情報を表示するページが表示されます。
5. ページの右上にある **削除** をクリックします。
6. 強制保持ポリシーを削除した場合の影響を確認します。影響を確認するページには、以下の情報が記載されています。
   **概要：**ポリシー名、強制保持期間、範囲などの強制保持ポリシーの設定内容。
   **ポリシー削除の影響：** 強制保持が解除され、制約なしに永久に削除できるボードの数。 強制保持ポリシーはゴミ箱内のボードにも適用され、影響を確認する際の計算対象となります。
7. 強制保持ポリシーを削除するには、**ポリシーを削除** をクリックします。

:::note
ポリシーの作成、更新、削除を行うと、強制保持ポリシーのプロセスが起動し、完了まで最大 24 時間かかることがあります。ただし、ポリシーの名前または説明の更新については、保持ポリシーのプロセスは起動されず、更新は即座に実行されます。
:::
