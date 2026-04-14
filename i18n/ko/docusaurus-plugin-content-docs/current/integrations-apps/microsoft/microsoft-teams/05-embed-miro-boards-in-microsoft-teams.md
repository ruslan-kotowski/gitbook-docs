---
title: "Microsoft Teams\uC5D0 Miro \uBCF4\uB4DC \uC784\uBCA0\uB4DC\uD558\uAE30"
article_id: 360017572514
translation_id: 360017572514
locale: ko-kr
sidebar_position: 5
created_at: '2019-02-11T10:13:30Z'
updated_at: '2025-04-24T13:52:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ms-teams
---

Miro 보드를 Microsoft Teams 채널에 임베드하고 팀 멤버와 원활하게 공유하세요. Miro 보드를 유지하고 팀 전체가 동일한 페이지에 있는지 확인하세요.

:::note
Microsoft Teams를 통해 Miro 알림을 받으려면 [이 가이드를](10-miro-notifications-in-microsoft-teams.md) 확인하세요.
:::

:::note
Miro 보드를 Microsoft 팀 회의에 임베드하는 방법을 확인하세요. [Microsoft Teams 회의용 Miro(관리자 가이드)](01-miro-for-microsoft-teams-admin-guide.md), [Microsoft Teams 회의용 Miro(사용자 가이드)](02-miro-for-microsoft-teams-user-guide.md).
:::

> **사용 가능:** 모든 Miro 플랜

### 플러그인 설치하기

먼저 **Microsoft Teams 스토어에서** **Miro를** 찾거나 [직접 링크를](https://teams.microsoft.com/l/app/8216e453-3db5-48ee-a3d6-5122f505c8a3) 따라가세요.

:::warning
Microsoft Teams 측에서 테넌트 관리자가 팀에 타사 앱 카탈로그 내에서 Miro 앱을 활성화해야 한다는 점에 유의하세요. Miro가 승인되지 않으면 Microsoft Teams Store의 앱에 표시되지 않습니다.
:::

추가를 클릭해 플러그인을 **설치하세요.**

![Miro_plugin_installation.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790725266_Miro%20plugin%20installation.jpg)
*Miro 플러그인 설치*

Miro 플러그인을 설치하면 채팅으로 리디렉션되며 Miro 알림을 받을 수 있습니다. 더 많은 정보를 보려면 [이 문서를](10-miro-notifications-in-microsoft-teams.md) 확인하세요.

그러나 그 시점에서 추가 구성 없이 Miro 보드를 Microsoft Teams 채널에 이미 임베드할 수 있습니다.

### Microsoft Teams 채널에 보드 임베드하기

> **설정 기준:** 보드가 위치한 팀의 멤버인 [보드 소유자](../../../using-miro/sharing-boards/01-board-access-rights.md) 및 [보드 편집자](../../../using-miro/sharing-boards/01-board-access-rights.md)

새 탭을 만들어 보드를 Microsoft 팀 채널에 임베드할 수 있습니다. 더하기 아이콘을 클릭하세요. 다양한 앱이 있는 선택기를 받게 됩니다. 앱 목록에서 Miro를 찾아 선택하세요. 동일한 브라우저나 데스크톱 앱에서 Miro에 인증되지 않은 경우 로그인해야 합니다. **시작하기를 클릭하고** [Miro에](../../../getting-started/start-here/02-how-to-register-with-miro.md) 로그인하거나 가입하세요.

![embed_in_MS_teams.gif](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734975122_embed%20in%20MS%20teams.gif)
*Miro 프로필을 인증하라는 메시지 표시 모드*

승인되면 Miro 보드가 있는 선택기가 표시되며, 선택기는 Miro 측에서 액세스할 수 있는 보드를 표시합니다. 다른 이메일로 Miro 및 Microsoft Teams에서 인증될 수 있습니다.

Microsoft 팀 채널에 추가하려는 보드를 누우세요.

![MS_teams_embed_picker.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734978322_MS%20teams%20embed%20picker.jpg)
*Miro 보드 선택*

팀 멤버인 보드 소유자와 보드 편집자만 Miro 보드를 임베드할 수 있습니다. 필요한 액세스 수준이 없는 보드를 선택하면 경고 메시지가 표시됩니다.

![unable_to_embed_boards.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790732690_unable%20to%20embed%20boards.jpg)
*액세스 레벨이 보드를 임베드할 수 없다는 경고 메시지*

다음으로 나머지 회의 참여자의 권한을 설정하고 보드에 대한 액세스를 제공하거나 제한할 수 있습니다. 다음 권한 유형 중에서 선택할 수 있습니다.

- **모든 사용자가 편집** 가능(로그인 필요 없음)
- **모든 사용자가 댓글을 달 수** 있음(로그인 필요 없음)
- **모든 사용자가 볼 수** 있음(로그인 필요 없음)
- **비공개**

![sharing_level.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790733586_sharing%20level.jpg)
*임베디드 보드 설정 액세스*

:::note
Miro에서 보드에 설정된 공유 설정으로 Microsoft 팀 내에서 보드 액세스를 정의할 수도 있습니다. 보드가 Miro에서 공개적으로 공유되면 보드를 **비공개로** 임베드했더라도 Microsoft Teams의 모든 사용자가 사용할 수 있습니다. 그러나 보드가 Miro 측에서 [비공개이고](../../../using-miro/sharing-boards/15-make-a-miro-board-private.md) **모든 사용자가 보기/댓글/편집** 액세스 권한을 가지고 임베드하면 Miro의 보드 액세스는 영향을 받지 않습니다. [자세히 알아보세요](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).
:::

:::note
[Enterprise 플랜](../../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md) Miro 사용자의 경우 액세스 설정이 조직 전체의 액세스 제어를 따르며 일부 공유 옵션이 제한될 수 있음을 암시합니다. 자세히 알아보기: [임베드 통합을 위한 Enterprise 공유 정책 관리하기](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)
:::

:::warning
무료 [팀에](../../../plans-billing/miro-plans/09-free-plan.md) 있는 보드를 임베드하면 **누구나 댓글** 작성 가능 옵션이 지원되지 않습니다.
:::

보드가 임베드되면 즉시 상호 작용을 시작할 수 있습니다.

![Miro_embed_in_MS_teams.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734972562_Miro%20embed%20in%20MS%20teams.jpg)
*Microsoft 팀 채널에 보드 임베디드*

:::note
Microsoft 팀 모바일 앱에서 Miro를 사용하는 Microsoft 팀 사용자는 설정된 권한에 따라 보드를 *보고 댓글을 달* 수 있습니다. 보드를 편집하는 경우 사용자 인터페이스를 최적화한 기본 [모바일](../../../getting-started/apps-for-devices/08-mobile-app.md) 앱을 설치하라는 메시지가 표시됩니다.
:::

![Miro_in_MS_Team_on_mobile.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734976146_Miro%20in%20MS%20Team%20on%20mobile.jpg)
*모바일 버전의 MS Teams에서 Miro 보드 - **앱에서 열기를** 눌러 Miro 기본 모바일 앱을 설치하세요.*

### 자주 묻는 질문

1. *Microsoft Teams에서 임베디드 보드를 보려면 각 팀 멤버가 Miro 프로필이 있어야 하나요?*
   - 보드를 포함할 때 **모든 사용자가 볼 수 있음/댓글을 달 수 있음/편집 옵션을** 선택하면 등록되지 않은 사용자도 보드를 보거나 댓글을 달 수 있습니다. 또한 보드가 Miro 측에서 [공개적으로](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) 공유되면 Microsoft Teams의 모든 사용자가 사용할 수 있습니다.
2. *보드가 임베드되면 MS 팀에서 보드 액세스 권한을 변경할 수 있는 권한이 있는 사용자(예: "누구나 볼 수 있음"에서 "비공개")는 누가 있나요?*- 연결된 보드에 연결된 사용자도 연결된 보드에 대한 액세스를 변경할 수 없습니다. 그러나 누구나 탭에서 **설정을** 클릭한 다음 동일한 탭에서 다른(또는 동일한) 보드를 선택하고 선택한 보드의 다른 액세스 레벨을 선택할 수 있습니다.
3. *두 개의 이메일로 Miro에 등록되어 있으며 두 번째 Miro 프로필에서 Miro 보드를 임베드하고 싶습니다. Miro 프로필을 전환하려면 어떻게 해야 하나요?*- 선택기는 동일한 브라우저에서 Miro에서 인증된 사용자의 보드를 표시합니다. 다른 브라우저 탭에서 Miro를 열고 로그아웃한 다음 두 번째 Miro 프로필에 로그인하세요.
   Microsoft Teams 데스크톱 앱을 사용하는 경우 앱에서 로그아웃합니다 -; 앱 내에서 Miro에서도 로그아웃됩니다. 그런 다음 앱에 로그인하고 [보드를](#h_5af20ae6-78c0-4e6c-ab20-e4968c89c97f) 임베드해 보세요. Miro에 로그인하라는 메시지가 표시되고 다른 Miro 프로필에 로그인할 수 있습니다.
