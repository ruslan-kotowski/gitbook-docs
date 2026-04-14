---
title: "\uC0AC\uC6A9\uC790 \uC81C\uAC70"
article_id: 360017571234
translation_id: 360017571234
locale: ko-kr
sidebar_position: 8
created_at: '2019-02-11T10:08:26Z'
updated_at: '2025-11-25T15:58:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-management
---

관리자가 사용자를 제거하면 팀 콘텐츠에 대해 해당 사용자의 액세스를 제한할 수 있고 해당 사용자의 콘텐츠 소유권을 가져오거나 삭제할 수 있습니다.

> **해당 대상:** Free, Starter, Business, Education
> **설정 권한을 가진 사용자:** 팀 관리자, 회사 관리자

### 사용자 삭제하기

팀에서 멤버 또는 [게스트](../../using-miro/sharing-boards/07-collaboration-with-guests.md)를 삭제하려면 **팀** 설정으로 이동합니다. 대시보드에서 설정으로 이동하려면 팀 이름을 클릭하고 드롭다운 메뉴에서 **사용자**를 선택합니다.

![Miro_팀_설정으로_이동.jpg](images/21574837067922_get%20to%20Miro%20team%20settings.jpg)*팀 설정으로 이동하기*

**사용자** 탭에서 사용자 옆에 있는 세 점 아이콘을 클릭하고 **팀에서 삭제**를 선택합니다.

:::note
사용자 삭제 옵션이 표시되지 않으면 아래 안내된 내용을 확인하세요.
:::

![멤버_삭제.jpg](images/21574826241298_delete%20a%20member.jpg)*팀 멤버 삭제하기*

삭제 대상인 사용자가 팀에서 만든 일부 보드, [프로젝트](../../using-miro/sharing-boards/16-projects.md), [템플릿](../../getting-started/start-here/your-first-board/04-templates.md)의 소유자인 경우, 이러한 공유 또는 비공개 콘텐츠의 소유권을 팀원 중 한 명(Free 및 Education 플랜의 경우 관리자 중 한 명)에게 이전할지 또는 소유권을 삭제할지 여부를 선택할 수 있습니다. 소유자를 변경하려면 x자 모양 아이콘을 클릭합니다. 사용자 및 콘텐츠 삭제를 선택하더라도 관리자는 90일 이내에 [보드를 복원](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md)할 수 있습니다.

:::note
Business 플랜에서는 팀 관리자에게 소유권 이전을 선택하면 자동으로 관리자 중 한 명에게 콘텐츠가 다시 할당됩니다.
:::

![사용자_삭제_화면.jpg](../../../../../../docs/administration/user-management/images/21017515322002_delete%20user%20modal.jpg)*사용자 제거 과정에서 보드 소유권 변경하기*

유료 플랜에서는 사용자를 일괄 삭제할 수도 있습니다. 여러 사용자를 선택하고 **일괄 작업**에서 **팀에서 삭제**를 선택합니다.

![사용자_일괄_삭제.jpg](images/21574826243986_bulk%20delete%20users.jpg)*여러 사용자 일괄 삭제하기*

삭제된 사용자는 별도 알림 없이 팀 프로젝트에 대한 모든 액세스 권한을 즉시 잃게 됩니다. 단, 삭제된 사용자가 특정 보드의 공개 링크를 저장한 경우 해당 [공개 링크를 통해 공유된 팀 보드](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)에는 액세스할 수 있습니다.

팀 멤버를 제거하면 상단에 현재 사용 가능한 라이선스 수를 나타내는 알림이 표시됩니다. 새 팀 멤버를 초대할 수도 있고, 결제 설정으로 이동해 팀의 라이선스 수를 줄일 수도 있습니다.

![활성_사용자_메시지.jpg](images/21574826244754_Active%20users%20message.jpg)*사용자 제거 후 해제된 라이선스에 대한 메시지*

팀 규모를 줄이면 사용하지 않은 시간에 해당하는 금액이 구독 잔액에 크레딧으로 적용됩니다. 요금 일할 계산 시스템에 대해 자세히 알아보려면 [청구 및 결제](../../plans-billing/billing-and-payments/04-miro-billing.md) 문서를 참고하세요.

### Business 플랜에서 사용자 삭제하기

사용자를 제거하고 빈 라이선스를 해제하려면 **회사 설정** > **활성 사용자** 섹션을 열고 사용자 메뉴에서 **삭제**를 선택합니다. 사용자의 콘텐츠 소유권을 이전할지 아니면 사용자의 모든 리소스를 제거할지 결정하고 **확인**을 클릭합니다. 사용자의 콘텐츠 이전을 선택하면 해당 콘텐츠가 위치한 팀의 관리자에게 다시 할당됩니다.

![Business_플랜_사용자_삭제.png](images/21574826247314_Delete-user-Business-Plan.png)
*Business 플랜 구독에서 사용자 제거하기*

[풀 라이선스](../../enterprise-administration/user-management/11-user-access-levels-on-enterprise-plan.md)를 보유한 사용자를 제거하면 상단에 현재 사용 가능한 라이선스 수를 나타내는 알림이 표시됩니다. 빈 라이선스를 사용할 풀 멤버를 초대할 계획이 없는 경우 **결제** 설정 > **팀 규모 변경**에서 팀 규모를 줄일 수 있습니다.

![Business_플랜_사용자_제거_알림.png](images/21574826248338_Seats-removed-notification-Business-Plan.png)
*풀 멤버 제거 후 해제된 라이선스에 대한 메시지*

:::note
사용자를 삭제하려고 할 때 **팀에는 관리자가 한 명 이상이어야 합니다**라는 알림이 표시되면 삭제하려는 사용자가 구독 내에서 팀의 유일한 관리자라는 의미입니다. 이 문제를 해결하려면 [해당 팀에 자신을 초대](01-invite-users.md)하고 [자신에게 팀 관리자 권한을 부여](06-how-to-manage-admin-roles.md)합니다. 각 사용자의 팀 수를 클릭해 해당 사용자가 속한 팀을 확인할 수 있습니다.
:::

### 자주 묻는 질문

1. *사용자 삭제 옵션이 없습니다. 이유가 무엇인가요?*
   - 멤버 제거 옵션은 관리자만 사용할 수 있습니다. 설정에 옵션이 표시되지 않으면 관리자에게 사용자 삭제를 요청하세요. 현 관리자의 이메일은 **활성 사용자** 목록에서 찾을 수 있습니다. 또한 사용자에게 자신을 [관리자로 승격](06-how-to-manage-admin-roles.md)하도록 요청할 수도 있습니다.
   ![팀_설정의_팀_관리자.jpg](images/21574826249874_Team%20admin%20in%20team%20settings.jpg)*팀 설정 > 활성 사용자에 있는 팀 관리자*
2. *Miro 관리자가 퇴사했습니다. 어떻게 제거할 수 있나요?*
   - 다음 문서를 확인하세요. [Miro 관리자가 퇴사한 경우](07-my-miro-admin-left-the-company.md)
3. *빈 라이선스는 어떻게 제거하나요?*
   - 빈 라이선스를 삭제하려면 [이 가이드](../../plans-billing/billing-and-payments/04-miro-billing.md)를 따르세요.
