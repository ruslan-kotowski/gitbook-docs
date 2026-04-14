---
title: Enterprise 플랜에서의 요청 관리
article_id: 360017237379
translation_id: 360017237379
locale: ko-kr
sidebar_position: 9
created_at: '2020-10-27T12:09:40Z'
updated_at: '2026-02-19T11:00:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: access-request-management
availability:
  notes: '해당 사항: Enterprise 플랜 실행 가능한 사용자: 회사 관리자'
---

Miro에서는 라이선스, 팀 및 조직 접근, SSO 요청이 기본적으로 이메일을 통해 회사 관리자에게 전송됩니다. 고급 요청 관리 기능을 사용하면 회사 관리자가 이러한 요청을 받는 방식과 처리 방식을 맞춤화할 수 있습니다.

### 요청 유형

요청 유형은 네 가지 범주로 나뉩니다:

- 조직 가입 요청
- 팀 참여 요청
- 라이선스 요청
- SSO 문제 관련 요청

Enterprise 플랜에 대한 다양한 요청 시나리오를 확인하세요.

### 요청 관리 옵션

회사 관리자는 여러 요청 관리 옵션을 통해 요청 유형에 맞춰 프로세스를 맞춤 설정할 수 있습니다.

:::note
회사 관리자 전체 또는 특정 회사 관리자에게 이메일을 보내는 옵션에는 팀 관리자도 포함됩니다.
:::

- 모든 회사 관리자에게 이메일 보내기
- 특정 회사 관리자에게 이메일 보내기
- 서비스 데스크 티켓 생성
- 사용자 지정 URL로 리디렉션

## 요청 관리 구성

:::note
[Miro에서 라이선스 요청을 직접 관리](04-license-requests-on-enterprise-plan.md)하려면 **모든 회사 관리자에게 이메일 보내기** 또는 **특정 관리자에게 이메일 보내기**를 선택하세요. 향후 모든 라이선스 요청은 라이선스 요청 설정에서 받게 됩니다.
:::

### 모든 회사 관리자에게 이메일 보내기

사용자가 액세스 요청을 하면 모든 회사 관리자에게 이메일 알림이 전송됩니다.

1. 회사 **설정**에서 **사용자** > **요청** > **요청 관리**로 이동하세요.
2. 관리할 **요청 유형**을 클릭하세요.
3. 팝업이 열리면 드롭다운을 클릭해 **모든 회사 관리자에게 이메일 보내기**를 선택하세요.

:::note
모든 회사 관리자나 특정 회사 관리자에게 이메일을 보내는 옵션에는 팀 관리자도 포함됩니다.
:::

### 특정 회사 관리자에게 이메일 보내기

회사 관리자는 최대 5개의 이메일 주소를 지정할 수 있습니다. 지정된 이메일로만 요청이 전송됩니다. 이 이메일 주소는 Miro 사용자가 아니어도 됩니다.

1. **회사** 설정 > **사용자** > **요청** > **요청 관리**로 이동합니다.
2. 관리하려는 **요청 유형**을 클릭합니다.
3. 팝업이 열리면 드롭다운을 클릭하여 **특정 회사 관리자에게 이메일 전송**을 선택합니다.
4. 최대 5개의 이메일 주소를 추가합니다. 이메일 필드에 이메일 주소를 입력할 때마다 **추가**를 클릭합니다.

:::note
모든 회사 관리자에게 이메일을 보내는 옵션이나 특정 회사 관리자에게만 이메일을 보내는 옵션에는 팀 관리자가 포함됩니다.
:::

### 서비스 데스크 티켓 생성

사용자가 액세스 요청을 할 때마다 자동으로 서비스 데스크 티켓을 생성합니다. 이 기능은 현재 **ServiceNow** 및 **Jira Service Management**를 지원합니다.

ServiceNow Jira Service Management

1. ServiceNow의 이메일 설정을 구성합니다. ServiceNow에서 Miro에 대한 카탈로그 항목을 생성합니다. ServiceNow를 열고, **시스템 속성** > **이메일 속성**으로 이동하여 인바운드 이메일 수신을 활성화합니다.

2. [인바운드 이메일 액션 생성](https://docs.servicenow.com/bundle/tokyo-servicenow-platform/page/administer/notification/task/t_CreatingAnInboundEmailAction.html). **발신자**에서**이 발신자만이 이 인바운드 작업을 트리거합니다** 아래 필드에 [notification@miro.com](mailto:notification@miro.com)을 입력합니다.

3. [이메일 본문에서 필드 값 설정](https://docs.servicenow.com/bundle/rome-servicenow-platform/page/administer/notification/reference/r_SetFieldValsFromTheEmailBody.html)을 통해 추가 설정을 구성하고 Miro 이메일을 ServiceNow 티켓으로 변환하는 프로세스를 설정하세요. 예를 들어, 새로 생성된 티켓을 특정 인물에게 지정할 수 있습니다.

4. Miro로 가서, **회사** 설정 > **사용자** > **접근 요청** > **요청 관리**에서 **ServiceNow에서 티켓 생성하기**를 선택합니다. 이메일 필드에 ServiceNow 이메일 주소를 입력하세요.

1. Jira Service Management의 이메일 설정을 구성합니다. 서비스 프로젝트에서 **프로젝트 설정** > **이메일 요청**을 선택하세요. [이메일 서비스 제공업체를 선택하고 Miro와 연결하기 위한 프롬프트를 따르세요](https://support.atlassian.com/jira-service-management-cloud/docs/receive-requests-from-an-email-address/).

2. Miro로 이동하여 **회사** 설정을 열고, **사용자 관리** > **접근 요청** > **요청 관리**에서 **Jira Service Management에서 티켓 생성**을 선택합니다. 이메일 필드에 Jira Service Management 이메일 주소를 입력합니다.

### 맞춤 URL로 리디렉션

요청자는 다음 단계로 이동하기 위해 선택한 URL로 리디렉션됩니다.

1. 회사의 **설정**에서  **사용자** > **접근 요청** > **요청 관리**로 이동합니다.
2. 관리하고자 하는 **요청 유형**을 클릭합니다.
3. 팝업 창이 열립니다. 드롭다운을 클릭하고 **맞춤형 URL로 리디렉션**을 선택하세요.
4. 사용자 지정 URL필드에 리디렉션 링크를 입력하세요.

## 요청 시나리오

아래 시나리오는 Miro에서 다양한 요청이 어떻게 트리거되는지를 설명합니다. 각 요청 유형을 어떻게 관리할지 결정하기 위해 이 시나리오를 검토하세요.

|  |  |
| --- | --- |
| **조직 가입 요청** | - 새 사용자가 [도메인 제어](../canvas-25-admin-features/domain-control/01-domain-control.md)(신규 사용자 캡처로 설정되지 않은 경우)와 함께 회사 관리 구독 팀에 참여 요청할 때. |
| **라이선스 요청** | - Free 제한 사용자가 [Standard](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) 또는 Full (이전 버전) 라이선스를 요청한 경우 - 멤버가 제한된 무료 사용자에게 Standard 또는 Full(최신) 라이선스를 요청할 때, 멤버가 구독에 새 사용자를 초대할 수 있는 권한이 [초대 설정](03-invitation-settings-on-enterprise-plan.md)에 없는 경우. - Standard 또는 Full(최신) 사용자가 Advanced 라이선스를 요청할 때. - 멤버가 제한된 무료 라이선스를 가진 사용자를 초대하거나 편집 권한을 주려고 할 때. |
| **팀 참여 요청** | - 비 관리자가 팀의 구성원이 아닌 사용자에게 보드를 공유하려고 시도하고, *게스트 초대가* 설정에서 꺼져 있으며, 새로운 팀 구성원 초대는 관리자만 할 수 있습니다.[설정 초대](03-invitation-settings-on-enterprise-plan.md)만 가능합니다. - 새로운 멤버를 초대할 수 없는 멤버가 특정 보드에 소유자 또는 [공동 소유자](../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) 역할을 팀의 멤버가 아닌 사용자의 역할로 부여하려고 할 때입니다. - Enterprise 사용자가 조직 내 사용자에게 발견 가능한 팀에 참여 요청을 할 때입니다. [discoverable for users in their organization](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md). - 팀 내 특정 보드에 초대된 [게스트](../../using-miro/sharing-boards/07-collaboration-with-guests.md)가 팀 참여를 요청할 때 |
| **SSO 문제 관련 요청** | - 사용자가 IdP에서 Miro에 대한 접근 권한이 없고 SSO를 통해 로그인에 문제가 있을 때. |

## 자주 묻는 질문

**티켓을 생성하도록 설정했는데도 여전히 이메일을 받는 이유는 무엇인가요?**

팀 관리자가 [초대 설정](03-invitation-settings-on-enterprise-plan.md)에서 팀에 새 사용자를 초대할 수 있도록 허용된 경우, 요청 관리 설정을 다르게 했더라도 이 팀과 관련된 초대 요청을 이메일로 받게 됩니다. 팀 관리자인 회사 관리자도 이러한 이메일을 계속 받을 수 있습니다.

**팀 관리자는 팀에 참여 요청이 있는지 어떻게 알 수 있나요?**

팀에 사용자를 초대할 수 있는 권한이 있는 경우, 요청 관리 설정과 상관없이 요청 관련 이메일을 받게 됩니다.
