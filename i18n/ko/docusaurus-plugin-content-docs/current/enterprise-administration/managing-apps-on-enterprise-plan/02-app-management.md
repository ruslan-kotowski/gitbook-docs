---
title: "\uC571 \uAD00\uB9AC"
article_id: 4404659741458
translation_id: 4404659741458
locale: ko-kr
sidebar_position: 2
created_at: '2021-08-03T15:46:50Z'
updated_at: '2026-01-29T10:00:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: apps-management
---

조직 및 팀 수준에서 앱과 권한을 관리하는 방법을 알아보세요.

> **대상:** Business 플랜, Enterprise 플랜
> **실행 가능한 사용자:** 팀 관리자, 회사 관리자

### 앱을 관리할 수 있는 사람은 누구인가요?

조직 수준의 앱 관리는 회사 관리자에게만 Enterprise 플랜에서 가능합니다. 팀 수준의 앱 관리는 Business 및 Enterprise 플랜에서 팀 관리자와 회사 관리자가 수행할 수 있습니다.

### 조직 또는 특정 팀을 위한 앱 추가

앱 관리 기능을 통해 조직 내의 모든 사용자 또는 특정 팀에 앱을 추가하고 승인합니다.
 **회사** 설정 > **앱 및 통합** > **앱**으로 이동합니다. 이 섹션에서 회사 관리자는 모든 팀 또는 특정 팀에 앱을 추가할 수 있습니다.

![apps-access.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803476626_apps-access.png)*회사 설정에서의 앱 관리 제어*

검색창에 앱 이름이나 클라이언트 ID를 입력하세요. 드롭다운 목록에서 앱을 선택하고 **추가**를 클릭합니다.

![add-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780909714_add-app.png)*회사 설정에서 앱 추가하기*

조직 내 모든 팀에 앱을 추가하거나 특정 팀을 선택할 수 있습니다. 이미 일부 팀에 앱이 추가된 경우 해당 태그가 표시됩니다. 팀에 다시 앱을 추가하면 팀 멤버는 앱을 다시 인증해야 합니다. **추가**를 클릭하여 완료합니다.

![add-apps-where.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780917010_add-apps-where.png)
*Google Drive 앱을 설치할 대상을 선택하는 과정*

모든 팀에 앱을 추가하는 경우, 새로 생성된 모든 팀에 앱이 추가됩니다.

### 사전 추가된 앱

일부 앱은 사용자에게 이미 사전 추가되어 있습니다. 추가 인증이나 개별 로그인이 필요할 수 있습니다. 이러한 사전 추가된 앱은 다음과 같습니다: [Box](../../integrations-apps/more-integrations/05-box-legacy.md), [Dropbox](../../integrations-apps/more-integrations/06-dropbox.md), [Google Drive](../../integrations-apps/google/05-google-drive.md), [OneDrive](../../integrations-apps/microsoft/06-onedrive.md), [Smartsheet](../../integrations-apps/more-integrations/15-smartsheet-app-for-miro.md), [Azure Cards](../../integrations-apps/microsoft/03-azure-cards.md), [Jira Cards](../../integrations-apps/atlassian/03-jira-cards.md),[Brandfetch](https://miro.com/marketplace/brandfetch/), [Google Images](../../integrations-apps/google/06-google-images.md), [Slack](../../integrations-apps/more-integrations/14-slack.md). 이 앱들은 회사 승인 목록에 없는 경우 미리 추가되지 않습니다. 이 목록을 관리할 수 있습니다, 회사 관리자라면.

### 조직을 위한 앱 사전 승인

앱을 추가하는 경우, 동시에 사전 승인할 수도 있습니다. 앱이 관리자에 의해 미리 추가되고 사전 승인된 경우, 조직의 사용자는 즉시 사용할 수 있습니다. 일부 앱은 여전히 개별적으로 외부 서비스에 로그인이 필요할 수 있습니다.

이 기능은 Miro Web SDK로 개발된 앱에만 제공됩니다. Miro Web SDK는 Miro의 기능을 확장하는 도구입니다. 이는 Miro 보드 내에서 실행되는 강력한 앱을 구축할 수 있는 도구 상자입니다.

### 개별 사용자 관리를 위한 앱 승인

기본적으로 사용자는 자신이 속한 팀에 대해 어떤 앱이든 추가할 수 있습니다. 회사 관리자는 사용자가 특정 앱만 추가할 수 있도록 사용자 앱 관리를 제한할 수 있습니다.

회사 관리자는 **회사** 설정 > **앱 및 통합** > **앱** > **앱 관리**로 이동하여, **아래 목록에서만 앱 추가를 제한하기** 옵션을 전환하여 사용자에 대한 앱 추가를 제한할 수 있습니다.

![manage-apps.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780921490_manage-apps.png)*Enterprise 플랜에서 승인된 앱 추가 제한*

제한이 설정된 경우, 승인된 앱만 Enterprise 사용자에게 추가될 수 있습니다. 사용자를 위한 앱을 승인하려면 해당 앱 옆의 토글을 활성화하거나, 내부 개발 앱의 경우에는 대응되는 필드에 클라이언트 ID를 붙여 넣어 승인하세요.

기존에 추가된 앱을 제한하려면 목록에서 해당 앱을 찾아서, 앱 옆의 토글이 꺼져 있는지 확인하세요. 제한된 경우, 모든 Enterprise 팀의 사용자가 해당 앱을 사용할 수 없게 됩니다.

조직에서 앱이 제한되면, 사용자는 [앱 사용 요청을 회사 관리자에게 보낼 수 있습니다](03-app-request-flow.md).

Enterprise 플랜에 저장된 Miro 보드 내 마켓플레이스에서 승인된 앱을 사용할 수 있습니다.

### 팀에서 앱 사용 허용 또는 제한

팀과 회사 관리자는 팀 차원에서 앱 사용을 관리할 수 있습니다: 팀원이 새로운 앱을 팀에 추가할 수 있도록 허용하거나 제한할 수 있습니다. 설정은 각 팀별로 구성됩니다.

![add-apps-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780928914_add-apps-team.png)*팀 설정에서의 앱 및 통합*

[Miro 앱 및 통합](../../integrations-apps/integrations-basics)에 대해 자세히 알아보세요.
