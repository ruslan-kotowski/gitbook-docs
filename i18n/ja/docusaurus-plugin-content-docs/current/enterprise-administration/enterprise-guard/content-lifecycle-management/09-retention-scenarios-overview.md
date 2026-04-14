---
title: "\u5F37\u5236\u4FDD\u6301\u306E\u30B7\u30CA\u30EA\u30AA\u6982\u8981"
article_id: 19205103343506
translation_id: 19205103343506
locale: ja
sidebar_position: 9
created_at: '2024-05-28T17:58:22Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

## ボードが強制保持期間中にゴミ箱に移動

**強制保持ポリシーはゴミ箱ポリシーより優先されます。**強制保持期間中にあるボードがその保持期間の初期または中間段階でゴミ箱に移動された場合、ボードはゴミ箱ポリシーで設定された期間（デフォルトで90日間）ゴミ箱に残ります。この期間が過ぎると、ボードはゴミ箱に表示されなくなります。ただし、ボードは強制保持期間が終了するまで保持され、その後は自動的に消去されます。図 1 はこのシナリオを示しています。

![Figure 1: Board is trashed during retention period](images/21019694932370_board_trashed_during_retention_period.png)*図 1：強制保持期間中にボードがゴミ箱に移動されました*

## 強制保持期間が終了する際にボードがゴミ箱に移動されます

**ゴミ箱ポリシーは、強制保持期間終了後も有効です。**強制保持期間終了時に保持中のボードがゴミ箱に移動された場合、ボードはゴミ箱ポリシーで設定された期間（デフォルト 90 日間）ゴミ箱に残ります。この期間が過ぎると、ボードはゴミ箱に表示されなくなります。強制保持期間が終了した後、ボードは手動で永久に削除することができ、ゴミ箱ポリシーが終了した後、自動的に消去されます。図 2 はこのシナリオを示しています。

![Figure 2: Board is trashed when the retention period is ending](images/21019706062226_board_trashed_when_retention_period_is_ending.png)*図 2：強制保持期間が終了する際にボードがゴミ箱に移動される*

## 強制保持期間中にチームが削除された場合

**チームが削除されると、そのチームに属するすべてのボードが永久に削除されます。**チームがゴミ箱に移動されると、強制保持ポリシーが適用されるボードも含め、そのチームに属するすべてのボードは 90 日後に永久に削除されます。消去されたチームが管理者によって手動で永久削除された場合、同じ結果が適用され、そのチームに属するすべてのボードは、強制保持中であっても永久に削除されます。図 3 はこのシナリオを示しています。

![Figure 3: Team is trashed during retention period](images/21019694939922_team_trashed_during_retention_period.png)*図 3：強制保持期間中にチームが削除された場合*
