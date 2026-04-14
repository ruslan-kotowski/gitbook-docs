---
title: '보드 변경 이력: 버전'
article_id: 360021668819
translation_id: 360021668819
locale: ko-kr
sidebar_position: 12
created_at: '2021-05-17T11:56:55Z'
updated_at: '2026-01-06T19:02:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: activity-list
availability:
  notes: '실행 가능한 사용자: 보드 소유자, 공동 소유자, 보드가 위치한 팀의 멤버인 보드 편집자 보드 콘텐츠 복사가 허용된 경우
    해당 플랜: Starter, Business, Enterprise, Education 사용 가능 환경: 브라우저, 데스크톱, 태블릿 앱'
---

Miro 보드의 모든 버전은 보드 변경 이력에 자동으로 저장됩니다. 언제든지 변경 사항을 검토하고 복구할 수 있습니다.

### 주요 기능

- 보드는 변경 사항이 있을 경우뿐만 아니라 각 협업 세션이 끝날 때마다 백업됩니다.
- 저장된 보드 변경 이력 버전은 *90일* 동안 보관됩니다.
- 원본 보드는 *변경되지* 않습니다. 복원된 버전은 *별도의* 보드로 생성되며 기본적으로 제목은 날짜로 지정됩니다.

:::warning
때때로 예기치 않은 네트워크 문제가 보드 백업을 방해할 수 있습니다. 원활한 백업을 위해 인터넷 연결이 안정적인지 확인하세요.
:::

### 보드의 이전 버전 복원하기

이전 버전을 복원하려면:

1. 보드 바에서 세로로 된 **세 점 아이콘**을 선택합니다.
   **메인** 메뉴가 열립니다.
2. **보드** > **변경 이력**을 선택합니다.
   **변경 이력** 패널이 열립니다. **활동** 탭이 기본적으로 열려 있습니다.
3. **버전**을 선택합니다.
4. 버전을 선택합니다.
   **별도의 보드로 복원** 모달이 열립니다.
5. (선택 사항) 화면의 지침을 따릅니다.
6. **복원**을 선택합니다.

### 이전 보드 버전 복원의 제한 또는 비활성화

- 이 기능은 [보드 소유자](../sharing-boards/01-board-access-rights.md)와 공동 소유자에게 제공되며, 보드가 위치한 팀에 속한 [편집자](../sharing-boards/01-board-access-rights.md)도 사용할 수 있도록 활성화할 수 있습니다.
- 해당 기능은 [보드 콘텐츠 설정](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)에 따라 달라집니다. 팀 멤버가 보드 콘텐츠를 복사할 수 있도록 보드 소유자가 허용해야만 멤버가 이 옵션을 사용할 수 있습니다. 보드 **공유** 버튼 > **공유 설정** > **권한**에서 이를 구성할 수 있습니다.
- [콘텐츠 관리자 권한](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)은 [Enterprise 플랜](../../plans-billing/miro-plans/04-enterprise-plan.md)에서 활성화되면, 회사 관리자가 **버전**을 콘텐츠 설정에서 비활성화된 상태에서도 [보드 소유권을 자신에게 다시 할당함으로써](../sharing-boards/01-board-access-rights.md) 접근할 수 있도록 합니다.

이 옵션을 사용할 권한이 없으면 **버전** 탭에 해당 메시지가 표시됩니다. 보드 소유자에게 문의해 기능을 활성화하세요.

## 자주 묻는 질문

**최근에 [팀을 업그레이드](../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md)했습니다. 팀이 Free 플랜을 사용하고 있을 때 만든 보드의 버전을 복원할 수 있나요?**

네, 업그레이드 후에는 Free 플랜을 사용하던 시기에 생성된 버전을 복원할 수 있습니다.

**보드 변경 이력에 버전이 없습니다. 왜죠?**

[무료 팀](../../plans-billing/miro-plans/09-free-plan.md)에서는 이 기능이 지원되지 않는다는 점을 유의하세요. 또한, 본인이 보드에서 버전을 복원할 수 있는 역할을 가지고 있는지 확인하세요. [보드 소유자](../sharing-boards/01-board-access-rights.md), [공동 소유자](../sharing-boards/06-co-owners-of-boards-and-spaces.md) 또는 [편집자](../sharing-boards/01-board-access-rights.md)이며 보드가 위치한 팀의 구성원이어야 합니다. 또한 보드 소유자/공동 소유자가 팀 구성원이 보드 콘텐츠를 복사할 수 있도록 허용해야 합니다.
삭제한 오브젝트를 복원할 수도 있습니다. [이 가이드](../working-on-the-board/18-restoring-board-content.md)를 확인하세요.
