---
title: Miro 보드 임베드
article_id: 360016335640
translation_id: 360016335640
locale: ko-kr
sidebar_position: 2
created_at: '2020-09-09T07:54:13Z'
updated_at: '2025-09-19T09:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: '사용자: 보드 편집자 플랜: 모든 플랜 플랫폼: 웹, 데스크톱, 모바일'
---

여러 앱과 웹사이트에 Miro 보드나 특정 항목(프레임 또는 형식)을 임베드하여 팀원들이 도구를 변경하지 않고도 컨텍스트 내에서 작업할 수 있습니다.

임베드는 보드의 [공유 설정](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md)을 상속받습니다:

- **공개 링크 켜짐** — 링크를 가지고 있는 사람 누구나 보기 가능 (유료 및 Education 플랜에서는 댓글 작성 및 편집 가능).
- **공개 링크 꺼짐** — 초대된 공동 작업자만 로그인 후 임베드를 열 수 있습니다.

[Enterprise 관리자](../../../plans-billing/miro-plans/04-enterprise-plan.md)는 [보안 설정](../../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)에서 공개 링크 사용 가능 여부를 관리할 수 있습니다.

## 임베드 방법 선택하기

Miro는 보드를 임베드할 수 있는 두 가지 방법을 제공합니다:

- **지원되는 앱 사용**:

  - Zoom, Teams, Confluence, Jira, Notion 같은 플랫폼에서 작업하기.
  - 원활한 워크플로를 위한 기본 통합 기능을 원할 때.
  - 사용자가 주로 해당 플랫폼을 통해 상호작용할 때.
  - 가장 간단한 설정 프로세스가 필요할 때.
- **임베드 코드 사용**:

  - 웹사이트, 블로그, 맞춤형 플랫폼에 임베드하기.
  - WordPress, Webflow, 다른 웹 빌더와 함께 작업하기.
  - 크기와 외형에 대한 더 많은 제어가 필요할 때.
  - 플랫폼이 iFrame을 지원하지만 Miro와의 기본 통합이 없는 경우.

## 지원되는 앱에 보드 임베드하기

Miro는 여러 지원되는 앱을 통해 쉽게 Miro 보드를 공유할 수 있습니다. 지원되는 앱에는 다음이 포함됩니다:

- [Zoom](../../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md)
- [Webex](../../../integrations-apps/more-integrations/10-miro-for-webex.md)
- [Microsoft Teams](../../../integrations-apps/microsoft/microsoft-teams/02-miro-for-microsoft-teams-user-guide.md)
- [Jira](../../../integrations-apps/atlassian/02-miro-for-jira-cloud.md)
- [Confluence](../../../integrations-apps/atlassian/01-miro-for-confluence.md)
- [Notion](https://miro.com/marketplace/notion-embed/)
- [Coda](https://miro.com/marketplace/coda-embed/)
- [Productboard](https://miro.com/marketplace/productboard-embed/)
- Medium

다른 앱에 Miro 보드를 임베드하면, 해당 앱 사용자에 대한 접근 권한을 별도로 설정하여 보드를 보기, 댓글 작성, 또는 편집할 수 있도록 할 수 있습니다. Miro 측의 보드 접근에는 영향을 미치지 않습니다. [임베드된 보드의 공유 및 권한 설정](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)에 대해 알아보세요.

지원되는 앱에 보드를 임베드하려면:

1. 대상 앱에서 **/miro**를 입력하거나 삽입 메뉴에서 **Miro**를 선택합니다.
2. 보드를 선택합니다.
3. **시작 보기**를 선택합니다:
   - **전체 보드** — 전체 캔버스.
   - **특정 항목** — 프레임이나 형식 (문서, 다이어그램, 테이블, 타임라인, 슬라이드 등).
4. **집중 모드**를 켜서 방해 없는 임베드를 만듭니다. 전체 상호작용을 허용하려면 끕니다.
5. 모든 방문자의 **접근 설정**을 선택합니다:
   - **보기 가능** — 임베드를 보는 사람은 보드를 볼 수 있습니다.
   - **접근 필요** — 임베드를 보는 사람은 보드 보기, 댓글 작성, 편집에 대한 접근이 필요합니다.
6. **보드 임베드**를 선택합니다.

임베드는 보드의 공유 설정을 따릅니다. 모바일 기기에서 모든 임베드는 보기 전용입니다.

## 임베드 코드로 보드 임베드

iFrame을 지원하는 모든 플랫폼에서, 예를 들어 **WordPress**나 **Webflow**에서 이 옵션을 사용하세요.

1. 다음 방법 중 하나로 **공유** 패널을 엽니다:
   - 오른쪽 상단에서 **공유** > **임베드**를 선택하거나,
   - 보드 메인 메뉴에서 **보드** > **내보내기** > **임베드**를 선택하거나,
   - 캔버스에서 임베드하고자 하는 항목(프레임이나 형식)을 선택합니다. 예를 들어, Doc을 선택하세요. 세로 점 세 개의 컨텍스트 메뉴를 열고, **이 문서 임베드**를 선택하세요.
2. **시작 보기**를 선택합니다:
   - **보드** — 전체 캔버스.
   - **특정 항목**, 예를 들어 프레임이나 형식(Doc, 다이어그램, 테이블, 타임라인, 또는 슬라이드).
3. (선택 사항) **시작 영역 설정** – 보드의 정확한 영역을 드래그하여 설정합니다.
4. 상호작용 방식 결정:
   - **보기 전용**을 선택하여 보기를 고정합니다.
   - **보기 전용** 선택을 해제하면 뷰어들이 이동, 확대/축소, 댓글 작성 또는 편집(권한이 있는 경우)할 수 있습니다.
5. **코드 복사**를 선택하여 필요한 곳에 붙여넣습니다.
   대상이 URL만 허용하는 경우, 대신 **링크 복사**를 선택합니다.

각기 다른 시작 보기, 시작 영역, 또는 포커스 오브젝트를 가진 동일한 보드에 대해 여러 임베드를 생성할 수 있습니다.

### 슬라이드 자동 재생

슬라이드 임베드를 자동 재생하려면 **임베드** 탭에서 **자동 슬라이드 간격**을 1초에서 30초로 설정합니다. 다른 보드 안에 보드를 임베드할 때는 자동 재생이 무시됩니다.

## 임베드가 어떻게 나타나는지

- 보드 이름은 클릭할 수 없습니다.
- 미니 맵, [메모](../../essential-tools/17-visual-notes.md) 및 팝업이 기본적으로 닫혀 있습니다.
- **시작 보기 설정**과 같은 일부 메뉴 옵션은 숨겨져 있습니다.
- 모바일에서는 모든 임베드가 보기 전용입니다.
- 타사 쿠키 차단기는 임베드가 제대로 로딩되지 않도록 할 수 있습니다.

## 자주 묻는 질문

**시작 보기와 집중 모드의 차이점은 무엇인가요?**
시작 보기는 초기 위치를 설정하지만 뷰어는 보드를 탐색할 수 있습니다. 집중 모드는 선택된 객체 외에는 모든 것이 숨겨지며 항상 보기 전용입니다.

**집중 모드 임베드를 편집 가능하게 할 수 있나요?**
아니요. 협업을 활성화하려면 **보기 전용**을 해제하고 보드의 공유 설정에서 편집 권한을 부여하세요.

**어떤 위젯이 지원되나요?**
문서, 다이어그램, 테이블, 타임라인, 슬라이드 및 모든 프레임입니다.

**Miro 로고를 제거할 수 있나요?**
아니요. 브랜드 로고를 제거하는 기능은 제공되지 않습니다.

**다른 보드 안에 보드를 임베드할 수 있나요?**
네. 임베드 코드를 복사하여 **iFrame 코드 붙여넣기**로 대상 보드에 붙여넣으세요.
