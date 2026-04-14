---
title: "\uBCF4\uC720 \uC2DC\uB098\uB9AC\uC624 \uAC1C\uC694"
article_id: 19205103343506
translation_id: 19205103343506
locale: ko-kr
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

## 보유 기간 동안 보드가 휴지통으로 이동됨

**보유 정책이 휴지통 정책보다 우선합니다.** 보유 대상 보드가 보유 기간의 초기 또는 중간 단계에 있을 때 휴지통으로 이동되면, 보드는 휴지통 정책에 설정된 기간 동안 휴지통에 남게 됩니다 (기본 90일). 이 기간이 지나면 보드는 더 이상 휴지통에 나타나지 않습니다. 그러나 보드는 보유 기간이 완료될 때까지 유지되며, 그 후에는 자동으로 삭제됩니다. 그림 1은 이 시나리오를 설명합니다.

![Figure 1: Board is trashed during retention period](images/28839361322130_board_trashed_during_retention_period.png)*그림 1: 보유 기간 동안 보드가 휴지통으로 이동됨*

## 보유 기간이 종료될 때 보드가 휴지통으로 이동됨

**보유 기간이 끝난 후에도 폐기 정책은 여전히 활성 상태로 유지됩니다.** 보유 대상 보드가 보유 기간이 종료될 때 휴지통으로 이동된 경우, 보드는 폐기 정책에 설정된 기간 동안 휴지통에 남아 있게 됩니다 (기본 90일). 이 기간이 지나면 보드는 더 이상 휴지통에 나타나지 않습니다. 보유 기간이 끝난 후, 보드는 수동으로 영구 삭제할 수 있으며 폐기 정책이 끝나면 자동으로 삭제됩니다. 그림 2는 이 시나리오를 보여줍니다.

![Figure 2: Board is trashed when the retention period is ending](images/28839361324434_board_trashed_when_retention_period_is_ending.png)*그림 2: 보유 기간이 끝날 때 보드는 휴지통으로 이동됩니다*

## 보유 기간 동안 팀이 휴지통으로 이동됩니다

**팀이 삭제되면 해당 팀의 모든 보드는 영구적으로 삭제됩니다.** 팀이 휴지통으로 이동되면 보유 정책을 포함한 해당 팀의 모든 보드는 90일 후 영구적으로 삭제됩니다. 관리자가 휴지통에 있는 팀을 수동으로 영구 삭제하면, 보유 중인 보드라도 모든 해당 팀의 보드는 영구적으로 삭제됩니다. 그림 3은 이 시나리오를 보여줍니다.

![Figure 3: Team is trashed during retention period](images/28839393274642_team_trashed_during_retention_period.png)*그림 3: 보유 기간 동안 팀이 휴지통으로 이동됨*
