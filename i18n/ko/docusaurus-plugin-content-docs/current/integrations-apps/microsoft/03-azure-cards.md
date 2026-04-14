---
title: Azure 카드
article_id: 360033799934
translation_id: 360033799934
locale: ko-kr
sidebar_position: 4
created_at: '2019-08-13T10:01:30Z'
updated_at: '2025-11-25T16:05:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: azure-cards
availability:
  notes: '사용자: 전체 사용자 플랜: Business, Enterprise 플랫폼: 브라우저, 데스크톱, 모바일'
---

Azure 카드를 사용하면 Azure 보드(이전 VSTS 클라우드 솔루션인 Azure DevOps 서비스의 일부)에서 작업 항목을 Miro 보드로 가져올 수 있습니다. 원격 회고, 스토리 크기 조정, 백로그 우선 순위 지정, 스토리 매핑, 기타 팀 활동에 필수적인 요소가 될 수 있습니다. Miro 칸반 및 사용자 스토리 매핑 프레임워크에서도 사용할 수 있습니다.

Azure 카드는 Azure 보드와 직접 통합하여 다양한 팀 활동의 원활한 워크플로 관리를 가능하게 함으로써 Miro 경험을 향상시킵니다.

## 주요 기능

Azure 카드 통합은 여러 가지 주요 기능을 제공합니다.

- 앱 내 Azure 보드 작업 항목 선택기를 사용하여 Azure 카드를 가져오세요. 여기에는 다양한 정렬 옵션이 포함됩니다
- 앱 내 선택기에서 Azure 보드 작업 항목 검색
- 확대 및 축소 중에 자동으로 읽기 쉬운 카드 보기 변경

:::note
Azure 카드는 항상 카드 폴링으로 업데이트되므로 [웹훅](../atlassian/14-how-to-set-up-webhooks-for-jira-data-center.md)에 장애가 발생하더라도 사용자가 항상 카드 업데이트를 받을 수 있습니다.
:::

## Azure 카드 통합 설정하기

설정은 다음 두 가지 수준에서 필요합니다.

1. 앱은 모든 팀에 대해 조직 레벨로 추가하거나, 특정 팀에 대해 팀 레벨로 추가해야 합니다.
2. 앱이 추가된 후 통합은 개인 수준에서 Azure 카드를 가져오기 위해 연결되고 인증되어야 합니다.

이 프로세스는 Miro와 Azure DevOps에서 특정 관리 권한이 필요합니다.

:::note
Miro에서 Azure 카드를 성공적으로 설정하려면, **Azure 관리자와 Miro 관리자가 동일한 계정이어야 합니다**.

Azure 카드를 추가하려면 Miro 팀 또는 회사 관리자 권한**과** Azure 보드의 프로젝트 컬렉션 관리자 그룹 권한이 필요하지만, 연결이 완료된 후 이러한 권한은 다운그레이드될 수 있습니다. 그러나 관리자는 제거할 수 없으며 Azure 프로젝트에 대한 액세스를 유지해야 합니다.
:::

### 조직 또는 팀에 Azure 카드 추가하기

Miro 회사 관리자는 모든 팀에 Azure 카드를 추가할 수 있으며, 팀 관리자는 관리하는 특정 팀에 추가할 수 있습니다. 이 단계를 통해 Azure Cards 앱을 연결할 수 있습니다.

> 팀 수준에서 Azure 카드를 연결하려면 팀 관리자여야 합니다.

1. **프로필 설정**으로 이동하세요(메인 메뉴 햄버거 아이콘을 클릭하고 **프로필 설정**을 선택하거나, 대시보드에서 오른쪽 상단 모서리의 아바타를 클릭하고 **설정**을 선택하세요).
2. **앱**을 클릭한 다음 오른쪽의 **앱 추가** 탭으로 이동하세요.
3. "Azure 카드"를 입력하고 드롭다운 목록에서 선택하세요. **추가**를 클릭하세요.
4. 다음 대화 상자에서 **모든 팀** 또는 **특정 팀 내**를 선택(필요한 경우 팀 선택)한 다음 **다음 단계를** 클릭하세요.
5. "Azure 카드 검토 및 추가" 화면에서 **추가**를 클릭하세요. 회사 또는 팀에 앱이 추가됩니다.
6. **앱 관리** 탭으로 이동해 Azure 카드를 검색한 다음, **승인을** 클릭하세요. 이제 앱이 회사 또는 팀 수준에서 승인됩니다.
7. 그런 다음 Azure 조직을 Miro에 연결하세요. 앱 패널에서 **앱 관리**로 이동하세요.
8. 앱 목록에서 "Azure 카드"를 검색하고 **설정**을 클릭하세요.
9. Azure 카드의 설정 패널에서 **Azure 인스턴스** URL을 추가하고 **연결**을 클릭하세요. Microsoft Azure 로그인 신원 정보를 제공하세요.
10. 인증 대화 상자에서 **승인**을 클릭하여 Azure와 Miro 연결을 완료합니다.

### 특정 팀에 맞춤형 Azure 카드 설정 적용하기

특정 팀에 대해 전사 차원의 설정과 다른 설정이 필요하다면, 팀 관리자가 팀 **앱 및 통합** 영역에서 이를 구성할 수 있습니다.

1. 프로필 설정 페이지에서 **팀**을 클릭하세요.
2. 사용자 지정 설정을 적용하려는 팀을 클릭하세요.
3. 팀 패널에서 **앱 및 통합**을 클릭하세요.
4. **Azure 카드를** 찾아 클릭하세요.
5. 앱 설정 패널에서 오른쪽 드롭다운에서 **사용자 지정 설정 적용**을 선택한 다음 사용자 지정 설정을 원하는 Azure 계정을 연결하세요.
6. Microsoft 계정으로 Azure DevOps에서 Miro를 인증하세요: "Microsoft 계정" 옆의 **연결**을 클릭하고 Microsoft 계정에 로그인해 Miro가 사용할 수 있도록 하세요.
7. **Azure 조직 URL**을(Azure DevOps에서 복사할 수 있음) 입력하고 **연결**을 클릭하세요. Miro는 인스턴스의 개인 설정된 URL 또는 인스턴스 이름으로 끝나는 일반 `https://dev.azure.com/` 주소를 수락합니다.
   ![특정 팀에 커스텀 Azure 카드 설정을 적용하는 방법을 보여주는 애니메이션입니다.](https://help.miro.com/hc/article_attachments/21857687380882)
   *특정 팀에 사용자 지정 Azure 카드 설정 추가하기*

### 개인 Azure 계정을 연결해 Azure 카드를 사용하세요.

Miro 관리자가 앱을 설치하고 승인한 후, Azure 카드를 사용하려는 각 팀 구성원은 개인적으로 자신의 Azure 계정에 대한 연결을 승인해야 합니다. 카드 선택기를 개인화하고 사용자가 액세스할 수 있는 모든 Azure 작업 항목을 가져올 수 있게 합니다.

작성 툴바에서 Azure 카드 아이콘을 찾을 수 있습니다. 아이콘이 없으면 검색해야 할 수 있습니다:

1. 생성 막대에서 **툴, 미디어, 통합** (**+**)을 선택하세요.
   **툴, 미디어, 통합** 패널이 열립니다.
2. **도구** 탭에서 Azure 카드를 검색하고 선택하세요.

귀하의 계정을 연결하려면:

1. 툴바에서 Azure 카드 아이콘을 클릭하세요. 팝업에서 **인증**을 요청합니다.
2. **인증** 버튼을 클릭하고 **계속**을 클릭하세요. 팀 설정 > 앱 및 통합 페이지로 이동합니다.
3. 앱 설정 패널을 사용해 Microsoft 계정을 Miro에 연결하고 사용하고 싶은 Azure 인스턴스를 지정하세요. 이 URL은 Azure DevOps에서 복사할 수 있으며, Miro는 인스턴스의 개인화된 URL이나 인스턴스 이름으로 끝나는 일반 `https://dev.azure.com/` 주소를 수락합니다.
   ![Miro 앱 설정에서 Azure 조직 URL 지정하기.](https://help.miro.com/hc/article_attachments/21857687387666)

:::note
팀 관리자만 초기 팀 또는 회사 수준의 구성을 설정할 수 있습니다. 관리자 설정 중 Azure 조직 URL에 대한 **연결** 버튼이 표시되지 않으면, [팀에 대한 팀 관리자 권한](../../administration/user-management/06-how-to-manage-admin-roles.md)이 있는지 확인하세요.
:::

## Azure 작업 항목을 Miro 보드로 가져오기

Azure 카드 앱을 구성하고 개인 계정을 연결한 후에는 연결된 팀과 관련된 모든 Miro 보드에 Azure 작업 항목을 가져올 수 있습니다. 이 작업을 수행하는 두 가지 주요 방법이 있습니다:

- Azure 작업 항목 URL을 복사해 Miro 보드에 바로 붙여넣습니다. 항목은 자동으로 Azure 카드로 변환됩니다.
- Azure 카드 선택기 사용: 툴바에서 **Azure 카드** 아이콘을 클릭해 선택기를 여세요.

  ![Azure Cards picker interface in Miro.](https://help.miro.com/hc/article_attachments/21857687390610)*Azure 카드 선택기*

  선택기는 모든 필드를 검색할 수 있어 제목, 유형, 상태 등으로 카드를 찾을 수 있습니다. 또한 Microsoft에서 제공하는 강력한 [키워드 검색](https://docs.microsoft.com/azure/devops/project/search/get-started-search?view=azure-devops#start-your-search-with-a-keyword)을 사용할 수 있습니다.

  ![Animation showing search functionality within the Azure Cards picker.](https://help.miro.com/hc/article_attachments/21857720559890)*선택기에서 Azure 카드 검색*

  프로젝트, 담당자, 유형, 영역 및 상태별로 카드를 필터링하여 Miro 내에서 Azure 작업 항목의 고급 필터링 기능을 사용할 수 있습니다.

  ![Filtering options within the Azure Cards picker.](https://help.miro.com/hc/article_attachments/21857720565266)*선택기에서 Azure 카드 필터링하기*

  원래 Azure 작업 항목으로 이동하려면 보드에서 카드를 선택하고 컨텍스트 메뉴에서 **소스** 버튼을 클릭하세요.

  ![Source button on an Azure Card linking to the item in Azure DevOps.](https://help.miro.com/hc/article_attachments/21857687396882)*카드의 소스 버튼*

  Azure 카드는 대화형 [칸반](../../using-miro/advanced-tools/02-columns-formerly-kanban.md) 및 [사용자 스토리 맵](../../using-miro/advanced-tools/07-user-story-mapping.md) 프레임워크의 구성 요소와 독립 실행형 보드 위젯으로 사용할 수 있습니다. Azure 카드를 프레임워크에 드래그하여 추가할 수 있습니다.

  ![Animation showing Azure Cards being used within a Miro Kanban board.](https://help.miro.com/hc/article_attachments/21857687398930)*칸반에서 Azure 카드 작업하기*

## Miro에서 Azure 카드를 직접 생성 및 편집

Miro와 Azure DevOps의 양방향 통합을 통해 팀은 Miro 보드에서 바로 새로운 Azure 작업 항목을 만들고 기존 항목을 편집할 수 있습니다. 이미 존재하는 Miro 카드와 스티커 메모를 Azure 카드로 전환할 수도 있습니다.

### 새 Azure 카드 만들기

Miro에서 새 Azure 작업 항목 만들기:

1. 제작 툴바에서 **Azure 카드**를 선택하고 선택기의 오른쪽 상단에서 **작업 항목 만들기**를 선택하세요.
2. 카드 필드를 입력하고 프로젝트, 항목 유형, 담당자를 선택한 다음 **만들기**를 클릭하세요. 새 항목은 Azure DevOps 디렉토리와 Miro 보드에 생성됩니다.

![Animation showing the process of creating a new Azure Card from Miro.](https://help.miro.com/hc/article_attachments/21857720570002)*Miro에서 Azure 카드 만들기*

### Miro 카드나 스티커 메모를 Azure 카드로 변환하기

기존 Miro 카드나 스티커 메모를 Azure 카드로 변환하려면:

1. 보드에서 스티커 메모 또는 카드를 선택합니다.
2. 오브젝트의 컨텍스트 메뉴에서 변환 옵션(일반적으로 Azure DevOps 아이콘 또는 "Azure 작업 항목으로 변환")을 클릭하세요.
3. 카드 매개 변수를 설정하고 대화 상자에서 프로젝트, 항목 유형 등을 선택한 후 **변환**을 클릭하세요. 스티커 메모/카드의 텍스트가 카드 제목으로 변환됩니다.

> **💡** 스티커 메모 또는 Miro 카드를 Azure 카드로 일괄 변환해 시간을 절약하세요. 변환하려는 모든 오브젝트를 클릭하고 드래그해 선택하고 컨텍스트 메뉴에서 **Azure 작업 항목으로 변환**을 선택하세요.

![Converting a Miro sticky note into an Azure Card.](https://help.miro.com/hc/article_attachments/21857720571666)*스티커 메모를 Azure 카드로 변환하기*

### Azure 카드 편집

Miro에서 Azure 카드를 편집하는 옵션은 툴 간 전환의 번거로움을 제거합니다. 카드 편집하기:

1. Miro 보드에서 Azure 카드를 클릭하세요.
2. 카드의 컨텍스트 메뉴에서 **펜 아이콘(편집)**을 클릭합니다. 팝업 창이 열리면 항목의 필드를 편집할 수 있습니다.
3. **업데이트**를 클릭해 변경 사항을 저장하세요. 변경 사항은 Azure DevOps에도 반영됩니다.

![Editing an Azure Card's details directly within Miro.](https://help.miro.com/hc/article_attachments/21857720575122)*Miro에서 Azure 카드를 편집하는 옵션*

### Azure 카드 색상 변경

보드에서 Azure 카드의 외형을 사용자 지정하려면:

카드의 채우기 색상을 변경하려면 카드를 클릭하고 컨텍스트 메뉴에서 **채우기 색상**을 선택하세요. 카드나 카드를 복제하면 이후의 모든 복사본은 동일한 채우기 색상을 갖게 됩니다.

## Azure 카드 통합 제거

Azure 카드 통합이 더 이상 필요하지 않다면 제거할 수 있습니다. 팀 수준에서 제거하려면 팀 관리자 권한이 필요합니다.

1. **팀 설정 > 앱 및 통합 > Azure 카드**로 이동하세요.
2. 아래로 스크롤하고 **팀 제거**를 클릭합니다.
3. 개인 계정에서만 Azure 카드를 제거하려면 **제거하기를 선택하세요.**

![Options to uninstall Azure Cards for the team or for an individual user.](https://help.miro.com/hc/article_attachments/21857720556306)*팀 전체 또는 개인용으로 앱 제거하기*

## 지원되는 Azure 카드 필드

Miro의 Azure 카드에 대해 지원되는 필드는 다음과 같습니다:

- 제목
- 프로젝트
- 유형
- 상태
- 설명(편집은 지원되지 않음)
- 상위 WI
- 담당자
- 우선순위
- 스토리 포인트
- 영역
- 반복
- 허용 기준

사용자 지정 필드는 지원되지 않습니다.

## Azure 카드 문제 해결

Azure 카드 통합에 문제가 발생하면 아래의 일반 문제 및 해결책을 참조하세요.

URL이 유효하지 않습니다

사용한 URL이 올바르지 않습니다. 맞춤법과 서식을 확인하세요. 예를 들어, Azure 조직 주소는 슬래시로 끝나야 합니다.

Azure 조직 URL에 연결할 수 없습니다

입력한 URL이 존재하지 않습니다. 기존 URL을 입력하거나 맞춤법을 확인하세요. 또한, 다음을 확인하세요:

- 조직이 타사 인증을 받을 수 있는지 확인하세요: **조직 설정 > 정책(보안)** **>** "OAuth를 통한 타사 애플리케이션 액세스"가 활성화되어 있는지 확인하세요.
- Azure 조직이 비공개 네트워크에 있거나 회사 방화벽이 외부 네트워크 연결을 차단합니다. 방화벽과 VPN 설정을 변경해 다음 도메인을 허용 목록에 추가하세요: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com, realtimeboard.com*, *.realtimeboard.com, *static.miro-apps.com 도메인. 프록시를 사용하는 경우 역방향으로 구성해 우리에게 액세스를 허용하세요. 액세스할 수 있는 주소(이 주소가 제한된 Azure DevOps의 실제 주소와 다를 수 있음)로 설정의 **Azure DevOps URL** 필드에 입력해야 합니다. 프록시 서버에서 시간 초과 값을 연장할 수도 있습니다.
- 통합 요청은 모두 Amazon 로드 밸런서를 통해 이루어지므로 Miro에서 특정 네트워크 정보를 제공할 수 없습니다.

서비스 훅 구독을 만들지 못했습니다

현재 로그인한 Azure 사용자에게 필요한 권한이 없습니다. Azure 인스턴스가 Miro에 연결될 예정인 Azure 사용자는 다음 REST API 메소드에 액세스할 수 있어야 합니다.

- [*서비스 훅 구독 생성*](https://docs.microsoft.com/rest/api/azure/devops/hooks/subscriptions/create?view=azure-devops-rest-6.0)("*vso.serviceendpoint_manage"* [범위](https://docs.microsoft.com/azure/devops/integrate/get-started/authentication/oauth?view=azure-devops#scopes) 필요)
- [*프로젝트에 대한 메타데이터를 수신합니다(이 정보는 구독 이벤트에서 작업 항목을 올바르게 지정하는 데 사용됩니다)*](https://docs.microsoft.com/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-6.0)
- *통합을 사용하는 모든 사용자가 액세스할 수 있도록 하려면 다음 방법도 필요합니다.*
  - [*항목 가져오기*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/get%20work%20item?view=azure-devops-rest-6.0)
  - [*항목 나열*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/list?view=azure-devops-rest-6.0)
  - [*항목 유형 가져오기*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/get?view=azure-devops-rest-6.0)
  - [*항목 유형 나열*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/list?view=azure-devops-rest-6.0)

사용자 **username@microsoft.com** 은 지정된 Azure 조직 URL의 어떤 프로젝트에도 액세스할 수 없습니다.

사용 중인 Azure 조직의 모든 프로젝트에 액세스할 수 없습니다. 카드를 가져오려면 Azure 보드 측에서 카드에 액세스할 수 있어야 합니다. Azure 조직 소유자에게 연락해 Azure 조직에 초대하도록 요청하세요. [이 문서](https://docs.microsoft.com/azure/devops/organizations/security/look-up-organization-owner?view=azure-devops)는 조직 소유자의 이름을 찾는 데 도움이 될 수 있습니다.

서비스 훅 구독을 만들지 못했습니다: 사용자 **username@microsoft.com**이 조직 소유자가 아닙니다. 조직 소유자에게 이 단계를 구성하도록 요청하세요.

Miro에서 Azure 카드를 설정하려면 Azure 조직 소유자와 Miro 회사 관리자 모두여야 합니다.

승인이 만료되었습니다. 팀 설정에서 통합을 다시 연결하세요.

Azure 인증이 만료되었습니다. 위의 "개인 Azure 계정을 연결해 Azure 카드를 사용하는 방법" 섹션에 설명된 대로 개인 수준에서 통합을 다시 연결하세요.

작업 중인 카드에 예기치 않은 동작이 나타납니다.

- 카드가 Azure 조직에서 동기화되지 않은 경우 이러한 문제가 발생할 수 있습니다. 예를 들어, 다른 보드에서 카드를 복사했거나 팀 간에 이동된 보드에서 작업하는 경우입니다. 상황을 해결하려면 Azure 항목을 보드에 다시 추가하세요.

반환된 작업 항목 수가 크기 한도 200개를 초과했습니다. 쿼리를 변경해 항목 수를 줄여 반환하세요.

이 오류 메시지가 표시되면 보드에 카드로 추가하기 위한 작업이 너무 많다는 의미입니다. 검색 표시줄을 사용해 작업 수를 제한하세요. 현재 선택기를 열면 필터가 적용되지 않고 지난 3개월 동안의 모든 작업이 표시됩니다. 선택기가 200개 이상의 작업을 표시하려고 할 때마다 이 오류 메시지가 표시됩니다.

Miro 설정에서 Azure 조직을 Miro와 연결하려고 할 때 **연결** 버튼을 받지 못했습니다.

팀 관리자 권한이 있는지 확인하세요. 팀 설정의 **활성 사용자** 탭으로 이동하고 [필요 시 팀 관리자에게 자신을 승격하세요](../../administration/user-management/06-how-to-manage-admin-roles.md). 이는 관리자가 Azure 조직 연결의 초기 설정에 적용됩니다.

:::note
다른 문제가 발생하면 [Miro 지원에](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) 문의하세요.
:::

## Azure 카드 자주 묻는 질문

Azure 카드 통합에 관한 일반적인 질문들에 대한 답변입니다.

Azure 카드에 허용된 IP는 무엇인가요?

Azure 카드 통합이 제대로 작동하려면, 특히 제한된 네트워크 환경에서 다음 IP 주소를 허용 목록에 추가해야 할 수 있습니다.

- 18.203.61.162
- 54.220.74.201
- 54.216.81.236
- 54.73.153.141
- 52.215.228.26
- 52.16.47.17
- 54.217.180.21

Azure 카드 앱을 연결 끊고 제거하면 기존 Azure 카드는 어떻게 되나요?

카드는 데이터 손실 없이 Miro 보드에 그대로 유지되지만, Azure와의 동기화가 중지되고 소스 버튼이 사라집니다.
