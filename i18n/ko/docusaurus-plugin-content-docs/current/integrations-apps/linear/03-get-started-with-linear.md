---
title: Linear 시작하기
article_id: 30629568232722
translation_id: 30629568232722
locale: ko-kr
sidebar_position: 3
created_at: '2025-10-29T13:35:01Z'
updated_at: '2026-02-23T11:34:34Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '사용자: 모든 사용자 플랜: Business, Enterprise 플랫폼: 브라우저, 데스크톱'
---

Miro의 Linear 통합은 Miro 보드와 Linear 이슈 간의 원활한 양방향 동기화를 가능하게 함으로써 협업을 강화합니다. 이슈를 Miro 안에서 직접 가져오고, 보고, 편집하여 워크플로가 최신 상태로 유지되며 팀이 조율되고 생산성을 유지할 수 있도록 합니다.

> **참고:** 관리자만 Miro 팀에 대한 Linear 통합을 승인할 수 있습니다. 팀 멤버는 팀 차원에서 설치된 후에만 통합을 사용할 수 있습니다.

## 사전 요구 사항

Linear 통합을 사용하기 전에 다음을 확인하세요:

- 활성화된 Miro 계정 ([여기에서 가입](https://miro.com/) 필요 시)
- 활성화된 Linear 계정
- 조직에서 앱 설치를 제한하는 경우 관리자 승인

## Linear를 Miro에 연결

Linear 통합을 시작하려면 Linear 계정을 Miro에 연결해야 합니다. Miro 보드를 열고 생성 바의 **도구 > 미디어 & 통합 (+)**을 클릭합니다. **Linear**를 검색하고 **연결**을 클릭하세요.

인증 시 다음을 선택할 수 있습니다:

- 신원 정보를 사용하기 (권장)
- API 키나 액세스 토큰 사용

인증 절차를 완료한 후, Linear 계정이 Miro와 동기화되기 시작합니다. 큰 계정의 경우 초기 동기화가 몇 분에서 몇 시간까지 걸릴 수 있습니다. 동기화가 완료되면 이메일로 알려드립니다.

## Linear 이슈를 보드에 추가

연결되면 Linear 이슈를 Miro 보드에 추가할 수 있습니다. **툴 > 미디어 & 통합 (+)**에서 Linear 이슈 선택기를 통해 **Linear**를 검색하세요. 선택기에서 상태, 담당자, 프로젝트별로 이슈를 필터링한 후, 이를 Linear 이슈 위젯으로 가져올 수 있습니다.

선택기에는 Linear에서 접근할 수 있는 이슈만 표시됩니다.

## Linear 이슈 작업

### Miro에서 이슈 편집

Miro 내에서 직접 Linear 이슈를 편집할 수 있습니다. Linear 이슈 위젯을 클릭하고 측면 패널 아이콘을 사용해 이슈 세부 정보를 엽니다. 여기서 속성을 수정한 후 **업데이트**를 클릭해 Linear와 변경 사항을 동기화할 수 있습니다.

### 워크플로 정리하기

Miro는 Linear 이슈를 효과적으로 정리하는 데 도움이 되는 여러 툴을 제공합니다:

[테이블](../../using-miro/formats/14-tables.md), [타임라인](../../using-miro/formats/15-timeline.md), [컬럼](../../using-miro/advanced-tools/02-columns-formerly-kanban.md), [유저 스토리맵](../../using-miro/advanced-tools/07-user-story-mapping.md) 툴은 워크플로의 구조를 다르게 구성할 수 있도록 도와줍니다. Linear 이슈를 이들 툴로 간단히 드래그 앤 드롭하여 필요한 대로 정리하세요.

Columns 위젯에서 이슈를 이동할 수 있지만, 이 작업이 Linear의 상태를 자동으로 업데이트하지는 않습니다.

### 이슈 탐색 및 사용자 지정

Linear 통합은 이슈를 다룰 수 있는 여러 방법을 제공합니다:

Linear에서 이슈의 전체 세부 정보를 보려면, 세부 보기 또는 측면 패널에서 **소스** 아이콘을 클릭하세요. **보기 전환** 아이콘을 사용하여 측면 패널과 모달 창 보기 사이를 전환할 수 있으며, **채우기 색상** 아이콘을 사용하여 시각적 조직을 위해 이슈에 색상을 지정할 수 있습니다.

## 추가 기능

### 액션 숏컷

Linear 통합은 [액션 숏컷](../../using-miro/facilitation-tools/03-action-shortcuts-beta.md)을 지원하여 다음을 빠르게 할 수 있습니다:

Linear 이슈 선택기를 열거나 맞춤형 바로 가기를 사용해 새로운 Linear 이슈를 생성할 수 있습니다.

## 통합 삭제

팀 단위 또는 개인 단위로 Linear 통합을 제거할 수 있습니다.

팀 단위로 제거하려면:

1. Team settings > Apps & Integrations으로 이동합니다
2. **Linear** 를 찾아서 team에서 제거를 클릭합니다

개인 단위로 제거하려면:

1. Apps & Integrations 에서 설정으로 이동합니다
2. **Linear** 를 찾아서 나를 위해 제거를 클릭합니다

## 자주 묻는 질문

### 누가 통합을 사용할 수 있나요?

Linear 통합은 적절한 Linear 권한을 가진 Miro 팀 또는 조직의 승인된 사용자에게 제공됩니다.

### Miro에서 누가 Linear 이슈를 볼 수 있나요?

보드 접근 권한(보기, 댓글, 편집 권한)을 가진 모든 사용자는 가져온 Linear 이슈를 볼 수 있습니다. 보드에서 이슈를 보기 위해 Linear 승인 권한은 필요하지 않습니다.

### Miro에서 Linear 권한은 어떻게 작동하나요?

통합은 Linear 권한을 존중합니다. Linear 접근 권한에 따라 이슈를 검색, 가져오기 또는 편집할 수 있으며, Miro 보드에 가져온 이슈는 모든 보드 사용자에게 보이게 됩니다. 이 이슈를 편집하려면 여전히 적절한 Linear 권한이 필요합니다.
