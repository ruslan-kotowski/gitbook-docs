---
title: 서드파티 앱에 임베드된 보드의 사용자 권한
article_id: 4411883577618
translation_id: 4411883577618
locale: ko-kr
sidebar_position: 1
created_at: '2021-12-08T10:13:42Z'
updated_at: '2025-11-25T16:07:55Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: '사용자: 보드 소유자, 보드 공동 소유자 플랜: 모든 플랜 플랫폼: 브라우저, 데스크톱 앱'
---

Miro는 [Microsoft Teams](../microsoft), [Confluence](../atlassian/01-miro-for-confluence.md), Notion, Google Meet 같은 서드파티 환경에서 보드를 쉽게 협업할 수 있도록 여러 통합을 제공합니다. 다른 지원되는 앱은 [Miro 마켓플레이스](https://miro.com/marketplace/category/embed-miro/)에서 확인할 수 있습니다. 보드를 임베드할 때, 사용자의 액세스 수준을 다르게 설정하고 이러한 권한을 Miro 내에서 관리할 수 있습니다.

## 임베드 액세스 이해

외부 앱에서 보드를 공유할 때, Miro 접근 권한과 관계없이, 해당 앱 내의 사용자에게 일회성 협업을 위해 보기를 제공할 수 있습니다. 이 사용자들은 앱 내에서 보드에 액세스하기 위해 Miro 프로필이 필요하지 않습니다. 이를 통해 Miro에 등록되지 않은 앱 사용자에게 보드를 공개하지 않고도 특정 보드 액세스 권한을 설정할 수 있습니다.

최대한의 보안을 위해, 일회성 협업(예: 워크숍) 외부에서는 이 방법을 사용하지 않는 것이 좋으며, 조직에서 필요한 사람들에게 적절히 Miro 액세스를 할당하는 것을 권장합니다.

![embed_Miro_in_Zoom.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020254296722_embed%20Miro%20in%20Zoom.gif) *보드 임베드에 대한 액세스 권한 설정*

보드는 임베드된 앱 내에서만 액세스할 수 있습니다. 앱 내에서 보드 임베드를 위해 설정한 액세스 수준은 앱 외부의 보드 공유 설정에 영향을 미치지 않습니다. 예를 들어, [비공개 보드](../../using-miro/sharing-boards/15-make-a-miro-board-private.md)가 Microsoft Teams 채널에 "누구나 보기 가능" 액세스로 임베드된 경우, 해당 Microsoft Teams 채널의 사용자는 Miro에 로그인하지 않고도 보드를 볼 수 있습니다. 동일한 사용자가 Microsoft Teams 채널 밖에서 보드 링크를 따라 보드에 액세스하려고 시도하면, 액세스할 수 없습니다.

그러나 Miro 측의 보드 공유 설정이 외부 앱에서 설정한 액세스 수준보다 우선합니다. 예를 들어, 보드가 [Miro 측에서 공개적으로 공유](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)되면, 보드를 비공개로 임베드했더라도 Microsoft Teams의 모든 사용자가 사용 가능합니다.

## 임베드 액세스 관리 및 취소

지원 외부 앱에 임베드된 보드의 액세스를 쉽게 추적하고, 관리하며 취소할 수 있습니다.

임베드된 보드의 액세스를 관리하고 취소하려면:

1. **공유** 버튼을 클릭하여 Miro 보드의 공유 설정을 엽니다.
2. **공유 설정**을 선택합니다.
3. **임베드** 탭을 엽니다.
4. 보드가 임베드된 외부 애플리케이션, 통합 이름, 임베드된 일시와 사람, 앱 내의 보드 액세스 설정을 모두 확인할 수 있습니다.
5. 앱 내에서 보드에 대한 액세스를 취소하려면, 앱 옆의 **액세스 취소**를 클릭하세요. 이 작업은 되돌릴 수 없음을 유의하세요.

ol

![remove_an_access_link.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020265344914_remove%20an%20access%20link.gif)
*액세스 링크 제거*

임베드 액세스가 취소된 후, 보드 액세스는 앱 내에서 제한됩니다. 보드가 Miro 측에서 공유되면 여전히 앱 내에서 액세스할 수 있음을 유의하세요. 예를 들어:

- 애플리케이션 내에서 보드를 **편집**할 수 있고 동일한 보드가 Miro 측에서 [공개적으로 공유](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)되어 **보기**가 가능하다면, 앱 내에서는 여전히 누구나 보드를 **보기**할 수 있습니다.
- 보드가 비공개 상태이며 [다른 사용자에게 이메일로만 공유](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)된 경우, 임베드된 보드는 앱 내에서 액세스하려면 **로그인**이 필요합니다.

## 임베드 규칙 및 제한 사항

보드를 임베드할 때 다음 규칙 및 제한 사항에 유의하세요:

- 보드가 [비활성 상태](../../using-miro/tools/troubleshooting/15-the-board-is-locked.md)이거나 보기에 대한 전용 액세스만 있는 경우, 보드를 임베드할 수 없습니다.
- [Free 팀](../../plans-billing/miro-plans/09-free-plan.md)에 저장된 보드는 댓글 액세스로 임베드할 수 없습니다.
- [Enterprise 플랜](../../plans-billing/miro-plans/04-enterprise-plan.md) 사용자에게는 액세스 설정이 조직 전체의 액세스 제어를 따르며 일부 공유 옵션이 제한될 수 있습니다. 자세히 알아보기: [임베드 통합을 위한 Enterprise 공유 정책 관리하기](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- 일부 이전 링크의 경우, 액세스 수준과 애플리케이션만 볼 수 있으며, 보드를 누가 생성했는지 또는 언제 임베드되었는지는 볼 수 없습니다.
- Enterprise 조직 내에서 외부 앱에 Miro 보드 임베드 기능을 제한하고 싶다면, [임베드 통합을 위한 Enterprise 공유 정책 관리하기](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)를 참조하세요.
- 모바일 및 태블릿 기기에서는 아직 임베드된 보드 액세스 링크 관리를 지원하지 않습니다.

[제한된 무료 라이선스 사용자를 위한 임베드된 보드 액세스](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)에 대해 자세히 알아보세요.
