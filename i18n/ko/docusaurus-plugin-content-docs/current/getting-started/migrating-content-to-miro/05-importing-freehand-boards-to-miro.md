---
title: Freehand 보드를 Miro로 가져오기
article_id: 18580556555538
translation_id: 18580556555538
locale: ko-kr
sidebar_position: 9
created_at: '2024-04-26T16:34:28Z'
updated_at: '2025-11-25T15:42:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: '사용자: 적합한 플랜을 가진 모든 사용자 플랜: Starter, Business, Education, Enterprise 플랫폼:
    브라우저, 데스크톱, 모바일 (Miro에 접근하고 가져오기를 시작하기 위해)'
---

이 글은 Freehand 보드를 Miro로 가져오는 방법에 대해 설명하며, 단일 및 일괄 가져오기를 위한 Freehand 보드 준비 방법을 포함합니다.

:::note
Miro에서 가져온 콘텐츠를 편집해도 Freehand의 원본 콘텐츠와 동기화되지 않습니다.
:::

:::note
무료 또는 제한된 라이선스 하의 Freehand 보드만 가져올 수 있습니다.
:::

## Freehand에서 Miro로 보드 하나 가져오기

Freehand 개별 보드를 Miro의 `.RTB` 파일 형식으로 내보내서 Miro에 쉽게 가져올 수 있습니다. 방법을 알려드리겠습니다:

1. Miro로 내보내려는 Freehand 보드에 액세스하세요.
2. Miro의 독점 형식인 .RTB로 파일을 Freehand에서 직접 다운로드하세요. **툴** 메뉴로 이동하여 **Miro 보드로 내보내기**를 선택하세요. 기본 다운로드 폴더에 파일이 저장됩니다. 다운로드가 완료되면 Freehand에서 알림을 드립니다.
3. Miro 대시보드를 여세요.
4. Miro 대시보드의 오른쪽 상단 영역에서 **+ 새로 만들기** 버튼을 클릭하고, **가져오기**를 클릭한 다음 **백업 가져오기**를 클릭하세요.
5. 시스템에서 이전에 다운로드한 `.RTB` 파일을 선택하세요.
6. 모든 콘텐츠가 이제 새 Miro 보드에 편집 가능한 형식으로 가져와졌습니다.
7. 대부분의 콘텐츠는 원활하게 전환되겠지만, Freehand와 Miro 간의 스타일과 서식 옵션 차이로 인해 약간의 조정이 필요할 수 있습니다. Miro에서 Freehand 오브젝트 매핑 이해하기에서 잠재적인 차이점에 대한 지침을 참고하세요.

## Freehand에서 Miro로 여러 파일 일괄 가져오기

Miro는 여러 Freehand 보드를 한 번에 이관하기 위한 일괄 가져오기 프로세스를 제공합니다. 먼저, Freehand 보드가 올바르게 준비되었는지 확인하세요.

**필수 조건: 일괄 가져오기를 위해 Freehand 보드를 준비하세요**

Freehand에서 다음 단계에 따라 보드를 준비하세요:

1. Freehand에서 왼쪽 패널 메뉴 바에서 **문서**를 선택합니다. 드롭다운 메뉴가 열립니다.
2. **모든 문서** 또는 **내가 작성한 문서**를 선택하고, Miro로 가져올 보드의 기간을 지정하세요.
3. 가져오려는 각 보드에 대해 세 점 아이콘(**...**)을 선택하고 **Select**를 선택하세요.
4. 화면 하단의 대화 상자에서 **이동**을 선택하세요.
5. 보드를 이동할 스페이스를 선택하세요. 일괄 가져오기 도구로 쉽게 처리할 수 있도록 이를 통합합니다.

   여러 파일을 준비하여 Miro로 일괄 가져오기에 성공했습니다.

준비된 Freehand 보드를 Miro로 일괄 가져오려면, 다음에 임베드된 Miro 보드 가이드에 제공된 지침을 따르세요.

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1IT00=/?pres=1&amp;frameId=3458764590689727256&amp;embedId=507813406404&amp;&amp;autoplay=yep" width="100%"></iframe>

:::note
일괄 가져오기에 대한 중요 메모:
- 일괄 마이그레이션에 사용되는 Freehand 토큰은 받은 날짜로부터 2주 동안만 유효합니다.
- 2024년 12월 31일 오후 11시 59분 EST부터 Freehand 및 관련 마이그레이션 토큰이 중단되고 무효화됩니다. 사용자는 더 이상 새 토큰을 생성하거나 마이그레이션을 위해 Freehand에 액세스할 수 없습니다.
:::

## 모범 사례 검토

원활한 마이그레이션 경험을 위해 Freehand에서 Miro로 콘텐츠를 이동할 때 가장 중요한 모범 사례와 주요 고려사항을 이해하는 것이 중요합니다. 아래 임베드된 Miro 보드에 있는 자세한 안내 사항을 검토해 주세요:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1FWSM=/?pres=1&amp;frameId=3458764590691451227&amp;embedId=480338444592&amp;autoplay=yep" width="100%"></iframe>

## Miro에서의 오브젝트 매핑

이 표는 Freehand의 객체가 Miro에서 일반적으로 어떻게 가져와 표현되는지를 포괄적으로 비교해주며, 필요한 경우 수동 조정에 대한 메모도 포함하고 있습니다.

|  |  |  |
| --- | --- | --- |
| **Freehand** | **Miro** | **손질 필요** |
| 보드 | 칸반 | 없음 |
| 카드 | 카드 | Freehand의 Jira 카드는 Miro에서도 Jira 카드로 가져옵니다. 그러나 사용자들은 Jira 계정을 Miro에서 다시 인증해야 하므로 기존 인스턴스에 연결되지 않습니다.    ADO, Trello, Asana 카드는 지원되지 않습니다. |
| 공동 작업자 및 공유 | 수동으로 다시 만들 수 있습니다 | 없음 |
| 댓글 | 수동으로 생성할 수 있습니다 | 없음 |
| 커넥터/선 | 커넥터/라인 | 없음 |
| 그림/다이어그램/도형 | 도형, 텍스트 및 커넥터 | 없음 |
| 동적 데이터 테이블 | CSV | 컨텐츠는 Miro 보드에서 .CSV 파일로 다운로드하고 편집할 수 있습니다. |
| 임베드:    Google 및 Microsoft 문서, YouTube, Spotify, Loom | 소스의 이름(예: Google, YouTube) 및 임베드할 URL | 사용자가 문서를 다시 임베드하려면 [URL을 통해 업로드](../../using-miro/import-and-export/import/05-uploading-files-to-boards.md)할 수 있습니다. |
| 이모티콘 리액션 | 수동으로 재생성할 수 있습니다 | 없음 |
| 프레임 | 프레임 | 없음 |
| 표(테이블) | 테이블 | 없음 |
| 그룹화된 오브젝트 | 오브젝트 그룹 해제됨 | 오브젝트를 다시 그룹화하려면 관련된 모든 오브젝트를 선택하고 **Cmd/Ctrl + G**를 누르거나 컨텍스트 메뉴에서 **오브젝트 그룹화**를 클릭하세요. |
| 이미지 | 이미지 | 없음 |
| 페이지 | 임베디드 문서 | 콘텐츠는 Miro 보드에서 .docx 파일로 다운로드하고 편집할 수 있습니다. |
| 프로토타입 | 소스의 이름(InVision)과 임베드를 위한 URL | 사용자가 문서를 다시 임베드하려면 URL을 통해 업로드하여 다시 임베드할 수 있습니다. |
| 스마트 위젯:    플립 카드, 투표, 이거나 그것, 차트, 카운터, 리더보드, 스피너, 부저, 사용자, 스토리 포인트, 티셔츠 크기, 타이머, 액션 버튼 | 가져오기 시 스마트 위젯의 PNG가 생성됩니다 | 콘텐츠는 편집할 수 없습니다. |
| 스티커 메모 | 스티커 메모 | 스티커 메모 내 텍스트의 글꼴 크기를 조정해야 할 수 있습니다. |
| 타임라인 (간트) | CSV | Miro 보드에서 콘텐츠를 .CSV 파일로 다운로드하고 편집할 수 있습니다. |
| 와이어프레임 | 와이어프레임 | 일부 오브젝트를 다시 그려야 할 수 있습니다. |

## 주요 제한 사항

Freehand에서 Miro로 콘텐츠를 이전할 때 매끄러운 전환을 위해 다음의 제한 사항 및 구조적 차이점에 유의하세요:

- Miro 텍스트 상자에는 공백을 포함하여 최대 6,000자까지 입력할 수 있습니다. 이 한도를 넘어가는 텍스트는 모두 잘립니다.
- Miro 스티커 메모는 Freehand처럼 색상 팔레트 조정이나 텍스트 글머리 기호 기능을 지원하지 않으며, 일부 서식이 다를 수 있습니다.
- Freehand 스마트 위젯은 정적 이미지(PNG)로 가져오며 Miro에서 편집할 수 없습니다.
- Freehand에서 Miro로 댓글, 이모티콘 리액션, 프로토타입은 이전되지 않습니다.
- 일괄 가져오기에 필요한 Freehand 토큰은 받은 날짜로부터 2주 동안만 유효합니다.
- 2024년 12월 31일 오후 11시 59분(EST)부터 Freehand 및 관련된 모든 마이그레이션 토큰이 중단되고 무효화됩니다. 사용자는 더 이상 새 토큰을 생성하거나 Freehand에 액세스할 수 없습니다.

### Freehand와 Miro의 조직 구조 비교

이동 계획을 효과적으로 세우려면 Freehand의 조직 구조가 Miro의 조직 구조와 어떻게 연결되는지 이해하는 것이 중요합니다:

**자유형 조직 레이어**

- 팀 InVision에서 액세스할 수 있는 각 하위 도메인은 팀으로 간주됩니다. 하위 도메인 하나만 액세스할 수 있다면 팀도 하나입니다.
- 그룹: 팀 내에서 문서를 그룹화하고 공유할 수 있도록 돕는 문서 폴더입니다.
- 스페이스: 문서를 위한 그룹 내 추가 조직 레이어입니다.

:::note
팀이 Freehand의 스페이스 개요 기능을 사용했을 경우, 이 콘텐츠를 Miro로 수동 마이그레이션해야 합니다. 스페이스 개요 콘텐츠를 Miro 보드에 복사하는 것을 권장합니다.
:::

**Miro 조직 레이어**

- 조직: Miro에서 일반적으로 하나의 조직에만 접근할 수 있습니다.
- 팀 사용자가 보드와 프로젝트에서 협업하는 공유 워크스페이스(일부 컨텍스트에서 이전에 스페이스로 알려졌으며, Miro의 발전하는 용어에 유의하세요; 일반적으로 팀이 주요 협업 워크스페이스입니다).
- 프로젝트: 팀 내에서 보드 모음을 생성하여 보드의 조직 관리, 검색 및 공유를 용이하게 합니다.

InVision 그룹을 Miro 프로젝트(또는 팀 내에서 보드를 조직하기 위한 폴더/스페이스와 개념적으로 유사한 것)와 거의 동등하게 생각하십시오. 각 InVision 그룹을 마이그레이션할 계획이라면, 동일한 이름의 Miro 프로젝트를 만드는 것을 권장합니다. 예를 들어, "Acme Corp Relaunch Project"라는 InVision 그룹이 있다면, 동일한 이름인 "Acme Corp Relaunch Project"를 적절한 Miro 팀 내에 Miro 프로젝트로 설정할 것을 제안합니다.

:::tip
Freehand 이전에 대한 추가 질문은 [Miro 지원](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)에 문의하거나 직접 Miro 고객 성공 매니저에게 연락하세요.
:::
