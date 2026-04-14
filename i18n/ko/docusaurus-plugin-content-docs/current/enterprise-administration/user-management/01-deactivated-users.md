---
title: "\uBE44\uD65C\uC131\uD654\uB41C \uC0AC\uC6A9\uC790"
article_id: 360025025894
translation_id: 360025025894
locale: ko-kr
sidebar_position: 1
created_at: '2019-06-19T22:16:18Z'
updated_at: '2026-02-19T10:44:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-deactivation
---

Miro의 고급 사용자 관리는 회사 관리자가 사용자를 삭제하지 않고 비활성화할 수 있도록 합니다. 비활성화된 사용자는 플랜 디렉토리에 남아 있으면서 언제든지 다시 활성화할 수 있습니다.

> **사용 가능 대상**: [Enterprise 플랜](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **설정 가능한 사용자:** 회사 관리자

## 규칙

- 비활성화된 사용자는 Enterprise 계정 및 기능에 접속할 수 없습니다.
- 비활성화된 사용자 차단 설정을 활성화한 경우, 관리되는 사용자를 비활성화하면 그 사용자는 [Miro에 로그인을 할 수 없습니다.](02-block-deactivated-users.md)
- 비활성화된 사용자는 회사의 SSO(통합 로그인) 옵션을 통해 더 이상 로그인할 수 없으며, 일반 인증 방법으로 돌아갑니다.
- 비활성화된 사용자가 생성한 공유 보드와 스페이스는 *다른 사람에게* 재할당되지 않으며, 공동 작업자가 계속 접근할 수 있습니다 (비활성화 시, 사용자를 팀에서 제거한 경우에는 보드가 팀 관리자에게 재할당됩니다. 이는 보통 [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) 작업에 관련됩니다).
- 비활성화된 사용자에게 모든 [알림](../../using-miro/managing-your-profile/02-miro-notifications.md)이 차단됩니다.
- 다른 사용자는 비활성화된 사용자와 보드 및 스페이스를 공유할 수 없습니다.
- 비활성화된 사용자는 귀하의 Enterprise 구독에서 팀에 추가될 수 없습니다. 회사 관리자는 회원으로 초대하면 비활성화된 사용자를 재활성화할 수 있습니다. [더 알아보기](05-manage-user-invitations-on-enterprise-plan.md).
- 비활성화된 사용자는 요금이 청구되지 않으며, 이들의 라이선스는 다른 활성 사용자에게 적용할 수 있습니다.
- 비활성화된 사용자에 대해 다음 속성은 업데이트할 수 없습니다:

|  |
| --- |
| `userName` |
| `userType` |
| `roles.value` |

## 사용자 비활성화

언제든지 사용자를 비활성화할 수 있습니다. 사용자를 비활성화하면, 해당 사용자는 **활성화** 상태에서 **비활성화** 상태로 변경되며 라이선스를 더 이상 소모하지 않습니다. 이 변경 사항은 **사용자** 설정의 활성화 및 비활성화 사용자 목록에도 반영됩니다.

사용자를 비활성화하려면:

1. **회사** 설정을 엽니다.
2. **사용자** 메뉴에서 **모든 사용자**를 선택합니다.
3. 비활성화하려는 사용자 오른쪽의 **세 점 아이콘** (**...**)을 클릭합니다.
4. **비활성화**를 클릭하세요.
   ![deactivate-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921781594002_deactivate-users.png)
   *Enterprise 플랜에서 사용자를 비활성화하는 옵션*

   사용자를 일괄로 비활성화할 수도 있습니다. 왼쪽의 체크박스를 선택해서 여러 사용자를 선택하거나 필터를 적용하여 최대 50명의 필터된 사용자를 한 번에 선택한 후 **일괄** 작업에서 **비활성화**를 선택하세요.
5. 사용자의 보드, [템플릿](../../getting-started/start-here/your-first-board/02-custom-templates.md), [스페이스](../../using-miro/spaces/01-spaces.md)를 이전하고 싶다면 **사용자 콘텐츠 재할당** 확인란을 선택하세요. 선택한 사용자에게 콘텐츠가 있었던 각 팀에 대해 새로운 소유자를 선택해야 합니다. 사용자 콘텐츠 재할당은 실행 취소할 수 없습니다.
   ![deactivate-reassign-content.png](../../../../../../docs/enterprise-administration/user-management/images/23921804187154_deactivate-reassign-content.png)
   *사용자 비활성화 시 콘텐츠를 재할당할 수 있는 옵션*
6. **비활성화**를 선택하세요.

사용자를 비활성화해도 Miro에서 해당 사용자의 데이터는 삭제되지 않습니다. 사용자가 보유하고 있던 권한은 그대로 유지되며, 사용자가 다시 활성화되면 복원됩니다.

:::note
참고: 회사 관리자를 비활성화하려면 먼저 회사 관리자 권한을 해제해야 합니다.
:::

:::note
사용자를 비활성화하는 동안 **팀에는 최소한 한 명의 관리자**가 있어야 한다는 알림이 표시되면, 해당 사용자는 Enterprise 팀 또는 여러 팀의 *유일한* 관리자임을 의미합니다. 이를 해결하려면 [해당 팀에 본인을 초대하고](05-manage-user-invitations-on-enterprise-plan.md) [팀 관리자 권한을 부여하십시오](../../administration/user-management/06-how-to-manage-admin-roles.md). 해당 사용자가 속한 팀의 수에 대한 정보를 확인하려면 팀 수를 클릭하세요.
:::

:::note
회사에서 [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) 솔루션을 사용하는 경우, ID 공급자를 통해 사용자 비활성화를 진행할 수 있습니다. SCIM에 의해 사용자가 비활성화되면 해당 사용자의 콘텐츠는 재할당되지 않으며, 재할당 옵션은 이 시나리오에서 UI에서만 지원됩니다.
:::

### 게스트 자동 비활성화

이메일로 초대받은 게스트(원래 보드에 초대된 사용자)의 경우, [자동 비활성화](03-invitation-settings-on-enterprise-plan.md)를 활성화할 수 있습니다.

## 사용자 재활성화

사용자를 재활성화하려면 다음과 같이 하세요:

1. **회사** 설정을 엽니다.
2. 사용자 메뉴 항목 아래에서 **모든 사용자**를 선택한 다음 **비활성화된 사용자** 탭을 클릭합니다**.**
3. 다시 활성화할 사용자의 오른쪽에 있는 **세 점 아이콘**(...)을 클릭합니다.
4. **다시 활성화**를 선택합니다.
5. 필요한 경우 사용자를 팀에 추가합니다.
6. **다시 활성화**를 확인합니다.

![reactivate-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921804191762_reactivate-users.png)
*사용자 다시 활성화*

사용자를 재활성화할 경우:

- 사용자는 즉시 로그인할 수 있습니다
- 비활성화 이전에 생성한 공유 보드, 팀 보드 및 개인 보드에 액세스할 수 있습니다 (보드가 재할당되지 않은 경우)

:::note
참고: 사용자를 재활성화할 수 있는 사람은 회사 관리자뿐입니다.
:::

### 사용자 영구 삭제

비활성화된 사용자를 영구적으로 삭제하려면:

1. **회사** 설정을 엽니다.
2. **사용자** > **모든 사용자**를 메뉴에서 클릭합니다.
3. **비활성화된 사용자** 탭을 선택합니다.
4. 삭제할 사용자의 오른쪽에 있는 **세 점** (**...**) 아이콘을 클릭합니다.
5. **삭제**를 선택합니다.
   ![delete-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921781612562_delete-users.png)
   *비활성화된 사용자 삭제*
6. 사용자의 콘텐츠를 재배정할지 제거할지 선택하세요. 새로운 소유자를 선택한 후 **사용자 삭제**를 클릭하거나 **사용자 및 콘텐츠 삭제**를 선택합니다.

일괄 작업을 사용하여 사용자 삭제도 가능합니다:

1. 비활성화된 사용자 탭에서 삭제하려는 사용자 옆의 체크박스를 클릭합니다.
2. **회사에서 삭제** 버튼을 상단에서 클릭합니다.

:::note
참고: 삭제 후, 사용자는 새 사용자를 [추가할 권한이 있는](05-manage-user-invitations-on-enterprise-plan.md) 사람들에 의해 멤버로 또는 보드에 게스트로 초대될 수 있습니다.
:::
