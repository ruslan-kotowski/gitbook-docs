---
title: 보드에서 콘텐츠 잠그기
article_id: 4408887253778
translation_id: 4408887253778
locale: ko-kr
sidebar_position: 17
created_at: '2021-10-29T07:59:49Z'
updated_at: '2026-01-06T19:00:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
availability:
  notes: '실행 가능한 사용자: 로그인한 모든 사용자 어떤 플랜이 있나요: Free, Starter, Business, Enterprise,
    Education 어떤 플랫폼: 브라우저, 데스크톱, 모바일'
---

Miro 보드에서 오브젝트를 잠가 실수로 이동, 편집 또는 삭제되지 않도록 방지하세요. 이메일 [을 통해](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) 보드에 초대된 편집자나 [프로젝트](../sharing-boards/16-projects.md) 또는 [팀](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md)의 구성원이라서 접근 권한이 있는 편집자들은 객체를 잠그고 잠금을 해제할 수 있습니다.

추가 보호를 위해, 유료 또는 Education 플랜을 사용하는 보드 소유자와 공동 소유자는 보호 잠금을 사용할 수 있습니다. 이 기능은 보드 소유자 또는 공동 소유자가 잠금한 항목만 잠금 해제할 수 있도록 하여 다른 편집자가 중요한 콘텐츠를 실수로 이동하거나 삭제하지 못하도록 합니다.

:::warning
방문자는 보드의 오브젝트를 잠그거나 잠금 해제할 수 없습니다. [테이블](../advanced-tools/05-grid.md), [칸반 보드](../advanced-tools/02-columns-formerly-kanban.md), [마인드맵](../advanced-tools/03-mind-map.md), [사용자 스토리 맵](../advanced-tools/07-user-story-mapping.md), [스윔레인](../formats/diagramming/01-miro-for-mapping-diagramming.md) 등에 있는 내용도 잠글 수 없습니다.
:::

## 오브젝트 잠금 및 잠금 해제

보드에서 하나 또는 여러 개체를 잠그거나 잠금 해제할 수 있습니다.

객체를 잠그려면, 선택하고 컨텍스트 메뉴에서 **잠금** 아이콘을 클릭하세요. **Ctrl + Shift + L** (*Windows*) 또는 **Cmd + Shift + L** (*Mac*) 단축키를 사용하세요. 모바일에서는 물체를 탭한 후 세로로 배열된 세 점 아이콘 ![icon-main.svg](../../../../../../docs/using-miro/working-on-the-board/images/24005170925074_icon-main.svg) 메뉴를 통해 잠금 옵션에 접근할 수 있습니다.

![한 객체의 컨텍스트 메뉴에서 잠금 옵션입니다.](../../../../../../docs/using-miro/working-on-the-board/images/21016057891346_lock%20in%20Miro.jpg)
*상황에 맞는 메뉴의 잠금 옵션*

여러 오브젝트를 잠그려면 관련된 오브젝트를 선택한 후 컨텍스트 메뉴에서 **잠금** 아이콘을 클릭하거나 단축키를 사용하세요.

오브젝트의 잠금을 해제하려면 컨텍스트 메뉴에서 **잠금** 아이콘을 길게 누르세요. 또한 동일한 단축키를 다시 사용할 수도 있고 오브젝트를 마우스 오른쪽 버튼으로 클릭하고 **잠금 해제**를 선택할 수도 있습니다.

:::note
오브젝트에 보호 잠금이 활성화된 경우, 해당 오브젝트를 잠근 보드 소유자 또는 공동 소유자만 잠금을 해제할 수 있습니다.
:::

![잠금 아이콘을 길게 눌러 객체의 잠금을 해제하기](../../../../../../docs/using-miro/working-on-the-board/images/21016057894418_long%20press%20to%20unlock.jpg)
*아이콘을 길게 눌러 오브젝트 잠금 해제*

### 모든 오브젝트 잠금 해제

보드의 모든 오브젝트를 한 번에 잠금 해제하려면 보드의 빈 영역을 마우스 오른쪽 버튼으로 클릭하고 **모두 잠금 해제**를 선택하세요. 잠긴 객체의 컨텍스트 메뉴에서 세 점 아이콘을 클릭하고 동일한 옵션을 선택할 수도 있습니다.

:::note
보호 잠금 항목은 보드 소유자나 잠금을 설정한 공동 소유자인 경우가 아니면 잠금 해제되지 않습니다.
:::

![보드에서 모든 오브젝트의 잠금을 해제하는 옵션입니다.](../../../../../../docs/using-miro/working-on-the-board/images/21016044523410_unlock%20all.jpg)
*보드의 모든 요소 잠금 해제*

## 보호 잠금 사용

> **설정 기준:** 보드 소유자, [보드 공동 소유자](../sharing-boards/06-co-owners-of-boards-and-spaces.md)

보호 잠금을 사용해 중요한 보드 콘텐츠를 다른 공동 작업자가 잠금을 해제하지 못하도록 하세요.

보호 잠금을 활성화하려면 먼저 항목을 평소처럼 잠그세요. 그런 다음, 컨텍스트 메뉴에 나타나는 방패 아이콘을 클릭합니다. 방패가 활성화되면 보드의 다른 사용자는 오브젝트를 잠금 해제할 수 없습니다. 언제든지 스스로 항목의 잠금을 해제해 보호 잠금을 비활성화할 수 있습니다.

![잠긴 객체에서 보호 잠금 기능을 활성화하는 사용자.](../../../../../../docs/using-miro/working-on-the-board/images/21016044524434_protected%20lock.gif)
*오브젝트에서 보호 잠금 활성화*

### 공동 작업자가 보는 것

보호 잠금이 설정된 객체는 보드의 다른 공동 작업자에게 다르게 나타납니다. 다른 사용자의 경우 오브젝트 잠금 해제 옵션을 사용할 수 없으며, 항목이 보드 소유자에 의해 보호되고 있다는 메시지가 표시됩니다.

![A widget showing that an object is protected by the board owner.](../../../../../../docs/using-miro/working-on-the-board/images/21016057899794_protected%20locked%20for%20users.jpg)
*보호된 오브젝트가 다른 공동 작업자에게 나타나는 방식*
