---
title: "Jira \uC885\uC18D\uC131"
article_id: 10649083010834
translation_id: 10649083010834
locale: ko-kr
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

플래너 [또는 Miro 보드 어디에서나](../../integrations-apps/atlassian/21-planner-for-jira.md) Jira 카드 간의 기존 종속성을 맵핑하거나 새로 만들고, 이는 Jira에서 즉시 동기화됩니다. 종속성 앱을 사용하면 계획 연습 동안 팀 간의 종속성을 실시간으로 식별, 시각화, 논의 및 기록할 수 있습니다.

> ****💡**** 이 기능은 이제 [Azure DevOps](08-dependencies-for-azure-devops.md)에서 사용할 수 있습니다.

> **사용 가능 대상:** Business 플랜, Enterprise 플랜
>
> **사용 가능 환경:** 데스크톱 브라우저, 데스크톱 앱

## 종속성 작동 방식

종속성은 연결선의 레이어로 나타나며, Jira 카드 간의 관계를 보여줍니다.

종속성은 보드에서 열었을 때만 보입니다. 참여자는 다양한 종속성 유형을 필터링하여 방해 요소와 관계를 논의할 수 있습니다.

![Dependencies-app.png](../../../../../../docs/using-miro/facilitation-tools/images/13244544218258_Dependencies-app.png)
*플래너 위젯에서 Jira 카드 간의 종속성 매핑*

## 새로운 종속성 생성 방법

1. 보드의 왼쪽에 있는 작성 툴바로 이동합니다.
2. 아이콘 **Dependencies**를 클릭합니다. Dependencies 아이콘이 작성 툴바에 없으면 **도구, 미디어 및 통합**(**+**)에서 추가해야 합니다.
3. Dependencies 패널이 열립니다.
4. 아이콘 **새로운 종속성**을 클릭합니다.
5. 아이콘 **첫 번째 카드** 를 클릭하고 드롭다운이나 검색을 통해 Jira 이슈를 선택합니다.
6. Jira 인스턴스에서 사용할 수 있는 **종속성 유형**을 선택합니다 (예: 차단, 복제, 중복 또는 관련 있음).
7. **두 번째 카드** 를 클릭하고 드롭다운 또는 검색을 통해 Jira 이슈를 선택합니다.
8. **초안 저장**, 또는 **직접 Jira에 저장**을 클릭합니다.

:::tip
초안 종속성은 Miro에만 저장됩니다. 초안 종속성을 생성하여 플래닝 단계에서 다른 참여자와 팀에 제안할 수 있습니다. 검토 및 논의가 완료되면 이를 Jira에 저장하거나 삭제할 수 있습니다.
:::

![dependencies-entry-point.png](../../../../../../docs/using-miro/facilitation-tools/images/21537435953426_dependencies-entry-point.png)
*새로운 종속성을 생성하고 Jira에 저장하기*

## 종속성 보기 및 필터링 방법

1. 보드 왼쪽에 있는 작성 툴바로 이동합니다.
2. **Dependencies** 아이콘을 클릭하세요. Dependencies 아이콘이 작성 툴바에 없으면 **툴, 미디어 및 통합** (**+**)에서 추가해야 합니다.
3. Dependencies 패널이 열리면, 기존의 모든 의존 관계들이 보드 상의 선으로 나타납니다.
4. **필터** 아이콘을 Dependencies 패널 상단에서 클릭하세요.
5. 토글을 사용해 **종속성 유형**과 **동기화 상태**로 필터링합니다.
6. **선 표시** 드롭다운을 사용해 종속성이 표시될 때를 제어합니다. 모든 활성 종속성을 보려면 **항상**을 선택하세요. 특정 Azure 카드나 종속성 유형을 클릭할 때만 종속성을 보려면 **선택 시**를 선택하세요.

점선은 초안 종속성을 나타내고, 실선은 Jira에 동기화된 종속성을 나타냅니다. 선의 색상은 종속성 유형을 나타냅니다.

![Filtering-dependencies.gif](../../../../../../docs/using-miro/facilitation-tools/images/13245295619730_Filtering-dependencies.gif)
*플래너 위젯에서 종속성 보기 필터링*

## 종속성 편집, 저장, 되돌리기 또는 삭제하는 방법

1. 보드의 왼쪽 작성 툴바로 이동합니다.
2. **종속성** 아이콘을 클릭합니다.
3. 종속성 패널이 열립니다.
4. **편집** 아이콘을 종속성 옆에서 클릭합니다.

![The_option_to_edit_a_Dependency.jpg](../../../../../../docs/using-miro/facilitation-tools/images/10866625733778_The%20option%20to%20edit%20a%20Dependency.jpg)
*종속성 편집*

종속성의 **첫 번째 카드**와 **두 번째 카드**, 그리고 **종속성 유형**을 변경할 수 있습니다.

*![Editing_a_dependency.gif](../../../../../../docs/using-miro/facilitation-tools/images/10866808392722_Editing%20a%20dependency.gif)**첫 번째 카드와 종속성 유형 변경*

**Save to Jira**를 클릭하여 초안 의존성을 Jira에 저장하고 동기화합니다.

![Save_to_Jira.png](../../../../../../docs/using-miro/facilitation-tools/images/10868740630034_Save%20to%20Jira.png)
*초안 의존성을 Jira에 저장*

동기화된 의존성을 초안으로 되돌리려면 **Revert to draft**를 클릭합니다.

![Revert_to_draft.png](../../../../../../docs/using-miro/facilitation-tools/images/10868741500690_Revert%20to%20draft.png)
*Jira에서 동기화된 의존성을 초안으로 되돌리기*

**휴지통** 아이콘을 클릭하여 종속성을 삭제합니다.
![Delete_dependency.png](../../../../../../docs/using-miro/facilitation-tools/images/10868804195986_Delete%20dependency.png)*종속성 삭제*
