---
title: 콘텐츠 관리자 권한
article_id: 360012777280
translation_id: 360012777280
locale: ko-kr
sidebar_position: 13
created_at: '2020-03-26T12:31:39Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-admin-permissions
availability:
  notes: '사용 가능 대상: Enterprise 플랜'
---

콘텐츠 관리자 권한을 통해 Enterprise 구독 내에서 모든 콘텐츠를 감독할 수 있습니다. 콘텐츠 관리자는 보드, 스페이스, 섹션, 템플릿에 대한 접근을 원활하게 관리하고 사용하지 않는 보드, 스페이스, 섹션을 삭제하여 대시보드를 정리할 수 있습니다.

### 콘텐츠 관리자 역할 할당 방법

1. [설정](https://miro.com/app/settings/user-profile/)으로 이동합니다.
2. **사용자** 아래에서 **관리자 역할**을 클릭합니다.
3. **콘텐츠 관리자** 역할 옆에 있는 세 점 아이콘(**…**)을 클릭하고, 드롭다운 메뉴에서 **역할 할당**을 선택합니다.
4. 콘텐츠 관리자 권한을 부여할 사용자들을 선택합니다. 사용자를 최대 50명까지 선택할 수 있습니다.
5. **할당** 버튼을 클릭하여 선택을 확인합니다.
6. 콘텐츠 관리자 역할이 할당된 모든 사용자를 보려면, 세 점 아이콘(**…**)을 다시 클릭하고 **사용자 보기**를 선택하세요. 또는 **콘텐츠 관리자 막대**를 클릭하면 사용자 목록을 확인할 수 있습니다.

콘텐츠 관리자에게 할당된 권한을 보려면, **콘텐츠 관리자** 막대를 클릭하고, **권한** 탭으로 전환한 후, 모든 **콘텐츠** 권한을 확인하세요.

## 보드 및 스페이스 관리

콘텐츠 관리자가 보드와 스페이스에서 가지는 권한에 대한 자세한 정보는 [관리자 역할 문서의 콘텐츠 관리 섹션](../../administration/get-started-as-a-miro-admin/02-understand-admin-roles-and-their-privileges.md)을 참조하세요.

또한, 콘텐츠 관리자는 다음을 수행할 수 있습니다:

- 공유 대화 상자를 열어 보드 공유 설정을 관리합니다 ([사용자의 접근 권한을 제거 및 변경](../../using-miro/sharing-boards/01-board-access-rights.md), 보드를 [팀](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)/사용자/[회사](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)/[공개적으로](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) 공유).
- 보드 세부정보 변경 (이름, 설명, 표지)
- 보드를 [스페이스로 이동](../../using-miro/spaces/01-spaces.md)
- 보드를 섹션으로 이동
- [보드를 삭제](../../using-miro/managing-boards/07-how-to-delete-a-board.md)
- [보드 백업을 다운로드](../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)
- [보드 콘텐츠 설정](../../using-miro/sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md) 구성
- 고급 보드 공유 권한을 [구성](../../using-miro/sharing-boards/02-who-can-share-a-miro-board.md)
- 공개 보드의 [비밀번호를 생성한 사용자를 보고](../../using-miro/sharing-boards/13-password-protection-for-public-boards.md), 공개적으로 공유된 보드에 대한 비밀번호를 설정, 변경 또는 제거
- [휴지통](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md)에서 보드를 복원

콘텐츠 관리자와 팀 콘텐츠 관리자는 보드 소유자가 멤버로 있는 다른 팀으로 보드를 이동할 수 있습니다. 보드 소유자가 대상 팀의 멤버가 아닌 경우, 소유권을 멤버에게 [이전할 수](../../using-miro/managing-boards/05-how-to-transfer-board-ownership.md) 있습니다.

대시보드에서 보드가 보이지 않는 경우, 해당 보드가 공유되지 않았다는 의미입니다. 하지만 여전히 찾을 수 있습니다. 대시보드에서 보드 이름, 보드 소유자, 위치(팀)를 기준으로 [검색](../../getting-started/start-here/miro-dashboard/03-how-to-search-in-miro.md)할 수 있습니다. 공유되지 않은 보드는 이름 옆에 자물쇠 아이콘이 표시됩니다. 보드를 관리하려면 오른쪽 상단의 세 점 아이콘을 클릭하세요.

직접 링크나 검색 결과에서 보드를 열려고 할 때, **보드에 접근할 수 없음** 메시지가 표시됩니다. 하단에서는 **보드 세부정보 보기** 및 **접근 권한 관리** 옵션을 볼 수 있습니다.

:::note
**회원이 아닌** **비공개** 스페이스의 설정은 변경할 수 없으며, 스페이스 목록에서도 볼 수 없습니다. 비공개 스페이스의 설정을 변경해야 하는 경우, 스페이스 소유자에게 접근 권한을 요청하거나 [Miro의 공개 API](https://developers.miro.com/reference/enterprise-update-project-settings)를 사용하세요. 대시보드에서 *보이는* 스페이스의 설정은 변경할 수 있습니다*.*
:::

## 템플릿 관리

템플릿의 공유 설정([개인, 팀 또는 회사](../../getting-started/start-here/your-first-board/02-custom-templates.md))을 변경하거나, 템플릿 상세 정보(이름, 설명 및 대표 이미지)를 편집하거나, 템플릿을 완전히 삭제할 수 있습니다.

**맞춤 설정 템플릿 관리 방법**

1. 대시보드로 이동하여 오른쪽 위에 있는 **템플릿 탐색**을 클릭하세요.
2. 왼쪽 탐색 메뉴에서 **맞춤 설정 템플릿**으로 이동하고 **[회사 이름] 템플릿** 또는 **개인용**을 클릭하세요.
3. 편집할 템플릿 위에 마우스를 올리고 세 점 아이콘을 클릭합니다.
4. 템플릿을 삭제하려면 **삭제**를 클릭합니다.
5. 다른 템플릿 세부 정보를 관리하려면 **편집**을 클릭합니다.
6. 보드가 열립니다. 보드 메뉴에서 템플릿 이름을 클릭합니다.
7. **템플릿 이름**과 **설명**을 추가하거나 수정하고, 표지 이미지의 **미리보기 영역 선택**을 선택하며, 공유 설정을 **개인**, **팀** 또는 **회사**로 변경합니다.
8. **변경 사항 저장**을 클릭합니다.
