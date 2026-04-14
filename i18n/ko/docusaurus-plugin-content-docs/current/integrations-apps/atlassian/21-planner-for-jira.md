---
title: "Jira\uC6A9 \uD50C\uB798\uB108"
article_id: 10648975837970
translation_id: 31352799344018
locale: ko-kr
sidebar_position: 22
created_at: '2025-11-25T16:20:27Z'
updated_at: '2026-02-09T13:21:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Jira용 플래너를 사용하면 퍼실리테이터와 팀이 Miro 보드에서 계획 이벤트를 실행하고 참가할 수 있으며, 실시간으로 Jira 보드에 업데이트를 동기화할 수 있어 수작업 시간을 절약할 수 있습니다.

> **사용 가능 대상:** Business 플랜, Enterprise 플랜

Program Increments (PI), Big Room, 로드맵 및 스프린트와 같은 팀 및 회사 계획 이벤트 동안 개발 팀은 서로 주고받으며 조율합니다.

:::tip
플래너는 이제 [Azure DevOps](https://help.miro.com/hc/articles/15280547945618)에서도 사용할 수 있습니다.
:::

## Jira 플래너 만드는 방법

1. 보드의 왼쪽에 있는 [작성 툴바](https://help.miro.com/hc/articles/360017730553-Toolbars) 로 이동하세요.
2. **더 많은 앱**(**+**)을 클릭하고 ‘플래너’를 검색하세요.
3. **플래너**를 클릭하여 앱을 실행하세요.
4. 커서가 보드에 나타납니다. 빈 플래너를 배치하려는 위치를 클릭하세요.
5. **Jira 보드** 드롭다운을 클릭하고 플래너에 연결할 보드를 선택하세요. 아직 Miro에서 Jira 계정이 인증되지 않은 경우, 로그인을 요청받게 됩니다.
6. 첫 번째 **컬럼** 필드는 *컬럼 유형*입니다. Jira 보드를 선택한 후 컬럼 유형은 기본적으로 **상태**로 설정되며 최대 3개의 컬럼이 표시됩니다. 첫 번째 **컬럼** 필드를 클릭하여 드롭다운에서 다른 컬럼 유형을 선택하세요 (Sprint, 상태, 우선순위, 수정 버전, 컴포넌트, 또는 맞춤형 필드를 선택할 수 있습니다).
7. 두 번째 **열** 필드를 사용해 플래너를 정교화하세요. 예를 들어, 열 필드로 '스프린트'를 선택한 경우, 표시할 스프린트를 선택할 수 있습니다.
8. **스윔레인**을 열뿐만 아니라 플래너에 추가하여 두 번째 Jira 필드를 기준으로 작업을 더 체계적으로 정리하세요 (스프린트, 상태, 우선순위, 수정 버전, 구성 요소 또는 맞춤형 필드를 선택할 수 있습니다).

:::note
현재 플래너는 하나의 Jira 보드만 지원합니다. 하지만, 하나의 Miro 보드에 여러 개의 플래너를 생성할 수 있습니다.
:::

![Creating-a-planner-widget.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696033042_Creating-a-planner-widget.gif)*플래너 만들기*

## 플래너 사용 방법

Jira 카드를 열 간에 드래그하여 업데이트하세요. 예를 들어, 백로그에서 플래너 안의 스프린트로 Jira 카드를 드래그하면, Miro와 Jira 모두에서 업데이트됩니다.

![Dragging-stories-between-columns-planning-widget.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696028306_Dragging-stories-between-columns-planning-widget.gif)*스프린트 간에 Jira 카드 이동*

**스윔레인**에 사용할 필드를 선택하여 작업을 행과 열로 나눌 수 있습니다. 스윔레인 간에 카드를 이동하면 관련된 Jira 이슈의 *열* 및 *스윔레인* 필드가 업데이트됩니다.

![Choosing-a-swimlane.png](../../../../../../docs/integrations-apps/atlassian/images/21017725756946_Choosing-a-swimlane.png)*스윔레인에 사용할 필드 선택*

기본적으로 플래너는 백로그에 있는 모든 이슈를 표시합니다. 현재 스프린트에 집중하려면 우측 상단에서 필터 아이콘을 선택하고 **스프린트**를 체크합니다. 그런 다음 **스프린트** 필터를 선택하고 **활성 스프린트로 필터링**을 활성화합니다. **적용**을 선택하여 스프린트 필터를 적용합니다.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*활성 스프린트로 이슈를 필터링합니다.*

또한 **이슈 유형** 드롭다운을 사용하여 플래너에 표시할 이슈 유형을 선택할 수 있습니다. 예를 들어, Story로만 필터링할 수 있습니다.

![Filtering-by-issue-type-planning-widget.png](../../../../../../docs/integrations-apps/atlassian/images/21017725749138_Filtering-by-issue-type-planning-widget.png)*이슈 유형별 필터링*

참여자들은 Jira 카드에 댓글을 달아 진행 중인 논의와 메모를 추적할 수 있습니다.

![Commenting_on_a_story.png](../../../../../../docs/integrations-apps/atlassian/images/21017696024594_Commenting%20on%20a%20story.png)*플래너에서 Jira 카드에 댓글 달기*

:::note
Miro 카드, 스티커 메모 및 기타 객체는 플래너 안에 배치할 수 없습니다.
:::

## 작업 수용량 및 작업량

읽기 쉬운 컬럼으로 스토리 포인트 총계를 시각화함으로써 스프린트 및 PI 계획 시 정보에 기반한 우선순위 결정을 내릴 수 있습니다. 팀의 효율성을 높이고 최적의 작업 배분을 보장하세요.

### Jira 카드에서 스토리 포인트 필드 활성화하기

1. 보드 왼쪽에 있는 [작성 툴바](https://help.miro.com/hc/articles/360017730553-Toolbars#Creation_toolbar)로 이동합니다.
2. **앱 추가** (**+**)를 클릭하고 ‘Jira 카드’를 검색합니다.
3. **Jira 카드**를 클릭하여 앱을 실행합니다.
4. **카드 설정**을 클릭합니다.
5. 아래로 스크롤하고, **스토리 포인트**를 활성화합니다.

![Enabling-Story-Points-for-Jira-Cards.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696030866_Enabling-Story-Points-for-Jira-Cards.gif)
*Jira 카드에 스토리 포인트 활성화*

### 용량과 로드 사용하기

스토리 포인트를 활성화한 후에는 새 플래너를 생성하거나 기존 플래너를 보드에서 새로 고칠 수 있습니다. 보드에 있는 적어도 하나의 이슈에 스토리 포인트가 할당된 경우, 플래너의 각 컬럼 상단에서 **용량** 및 **로드** 필드를 즉시 확인할 수 있습니다.

![Balancing-Capacity-and-Load.gif](../../../../../../docs/integrations-apps/atlassian/images/21017725755794_Balancing-Capacity-and-Load.gif)*용량과 로드를 균형 맞추기*

### 용량과 로드 이해하기

**용량**: 플래너의 각 칼럼 용량을 수동으로 입력하세요. 용량이 적재량보다 작을 경우, 팀의 용량을 초과했음을 알리는 빨간색으로 표시됩니다. 이 시각적 신호는 업무 부하를 균형 있게 유지하기 위해 이슈를 재배치할 것을 고려하게 만듭니다.

**적재량**: 이는 특정 칼럼 내 모든 카드의 스토리 포인트 합계를 나타냅니다. 스토리 포인트가 없는 카드는 계산 시 0으로 간주됩니다.

## Jira 구성

플래너를 설정하려면, 이슈를 가져올 Jira 보드를 선택하세요. 이는 Jira 스크럼이나 칸반 보드에서 가져올 수 있습니다.

플래너를 만들 때, 컬럼과 행(스윔레인)으로 사용할 Jira 필드를 선택할 수 있습니다. 포함 가능한 필드는 다음과 같습니다:

- 스프린트
- 상태
- 버전 수정
- 요소
- 우선순위
- 담당자
- 단일값 드롭다운 선택을 갖는 커스텀 필드
- 다중값 드롭다운 선택을 갖는 커스텀 필드

현재, 다른 Jira 필드나 날짜 관련 필드는 지원하지 않습니다.

스프린트 옵션은 Jira의 이슈 편집 화면에서 스프린트 필드가 사용 가능한 경우에만 나타납니다. 이는 일반적으로 Jira 서버/데이터 센터에는 미리 설정되어 있지만, 클라우드의 경우 스프린트 필드를 수동으로 추가해야 하는 경우가 많습니다. [이슈 화면 구성 방법](https://support.atlassian.com/jira-cloud-administration/docs/configure-issue-screens/)에 대해 자세히 알아보세요.

:::note
종료된 스프린트는 플래너에 표시할 수 없습니다.
:::

### 커스텀 JQL을 사용하여 플래너 만드는 방법

커스텀 JQL을 사용해 플래너를 만들려면 JQL 쿼리를 사용해 Jira 보드를 먼저 만드세요. Jira 보드를 만든 후, 위의 플래너 만들기 지침을 따르세요. 5단계에 도달했을 때, 사용자 지정 JQL 쿼리를 사용해 만든 Jira 보드를 선택하는 것을 잊지 마세요.

## 플래너 동기화

### Miro에서 Jira로

커스텀 필드 간에 카드를 드래그하면 Jira가 자동으로 업데이트됩니다. 이 작업은 몇 초 정도 걸릴 수 있습니다.

### Jira에서 Miro로

Jira에서 스프린트를 변경하면 플래너 컨텍스트 메뉴에 **업데이트 가능** 알림이 표시됩니다. Jira에서 변경을 수행한 후 몇 초 후에 나타날 수 있습니다.

플래너를 클릭해 컨텍스트 메뉴를 열고, 최신 변경 사항을 동기화하기 위해 **Jira와 동기화** 아이콘을 클릭하세요.

![Sync-planning-widget-with-jira.png](../../../../../../docs/integrations-apps/atlassian/images/21017696029970_Sync-planning-widget-with-jira.png)*Jira에서 Miro로 업데이트 동기화*

## 종속성 매핑

참여자는 플래너에서 작업 간의 의존성을 시각적으로 매핑할 수 있습니다. [Jira의 의존성](https://help.miro.com/hc/articles/10649083010834)에 대해 더 알아보세요.
