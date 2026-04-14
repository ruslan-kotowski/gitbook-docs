---
title: 지식
article_id: 29737566936850
translation_id: 29737566936850
locale: ko-kr
sidebar_position: 9
created_at: '2025-09-25T08:24:51Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: sticky-notes
availability:
  notes: '실행 가능한 사용자: 팀 멤버 사용 가능한 플랜: Business, Enterprise 지원 플랫폼: 브라우저, 데스크톱, 모바일'
---

Miro의 Knowledge는 Glean, Microsoft Copilot(베타), Miro Insights와 같은 제공업체와 통합되어 회사의 지식을 캔버스에서 직접 활용할 수 있게 합니다.

Knowledge는 팀이 내부 정보와 웹 검색 결과를 원활하게 가져와 Miro 캔버스를 프롬프트로 사용하여 더 빠르게 개발할 수 있게 합니다.

이미 사용 중인 지식 시스템을 연결한 후, 회사의 지식을 문서, 테이블, 스티커 메모, 슬라이드와 같은 포맷으로 쉽게 변환할 수 있습니다.

Knowledge는 웹 검색을 포함하여 다음의 통합을 지원합니다.

- [Amazon Q](../../integrations-apps/amazon-web-services-aws/03-amazon-q-beta.md) (베타)
- [Gemini Enterprise](../../integrations-apps/google/01-gemini-enterprise-integration.md) (베타)
- [Glean](../../integrations-apps/glean/01-glean-for-miro.md)
- [Microsoft Copilot](../../integrations-apps/microsoft/01-microsoft-copilot-integration.md) (베타)
- [Miro Insights](../tools/use-miro-insights/02-use-miro-insights-on-the-canvas.md)

기업 관리자는 각 통합을 팀을 위해 활성화하고 승인해야 합니다.

:::note
Microsoft Copilot 및 Gemini Enterprise와 같은 일부 통합은 각각의 제공자와의 유료 라이선스가 필요합니다.
:::

특정 지식 통합에 대해 더 알아보려면 [통합 & 앱](../../integrations-apps)을 참조하세요.

## 주요 기능

- **지식 통합**
  Miro는 선도적인 업체인 [Glean](../../integrations-apps/glean/01-glean-for-miro.md), [Microsoft Copilot](../../integrations-apps/microsoft/01-microsoft-copilot-integration.md)(베타), [Amazon Q](../../integrations-apps/amazon-web-services-aws/03-amazon-q-beta.md)(베타), Miro Insights와 연결하여 기업의 지식을 직접 캔버스에 적용할 수 있게 합니다.
- **엔터프라이즈 지식을 프롬프트로 사용하기**
  얻은 지식을 문맥으로 활용하여 [Miro AI](01-miro-ai-overview.md)에 프롬프트를 제공하고 아이디어 도출에서 창작으로 더 빠르게 발전시킬 수 있습니다.
- **다양한 접근 지점**
  지식 기능은 Miro의 여러 진입점에서 사용할 수 있으며, 이는 [AI 팀원](07-sidekicks.md) 및 [워크플로](04-flows-overview.md)를 포함하여 특정 단계에서 적절한 콘텐츠를 명확히 지정할 수 있습니다.

:::note
관리자는 Miro AI 권한, 웹 검색 기능 및 포맷 생성 기능을 관리하여 조직의 정책을 준수할 수 있습니다.
:::

## 지식을 활용하여 회사 정보 검색

다음의 진입점 중 하나에서 지식에 접근하세요.

:::note
지식 제공자를 처음 연결할 때 인증 요청을 받습니다.
:::

- [**AI 팀원**](06-sidekicks-overview.md)
  생성 바 위에서 **AI 팀원**을 클릭하세요. **AI 팀원** 패널이 열립니다. 프롬프트 상자에서 **지식**을 클릭합니다. 지식 제공자를 연결하거나 켜짐 위치로 전환합니다.
  ![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)*AI 팀원 패널에서 Miro에서 회사 지식을 가져오기 위해 지식 제공자를 선택합니다.*
  AI 팀원의 프롬프트를 작성하세요. 옵션으로 캔버스의 객체를 선택하여 컨텍스트를 추가할 수 있습니다. 프롬프트를 실행하면 선택된 제공자를 활용하여 지식을 얻습니다.

  > 💡 맞춤형 AI 에이전트로 캔버스에서 작업을 도와주는 전문 AI 팀원을 만들기 위해 Knowledge를 사용하세요.
- [**Docs**](04-flows-overview.md) **워크플로에서**
  Doc 컨텍스트 메뉴에서 **AI로 편집**을 클릭합니다. **AI 팀원** 패널이 열립니다. 프롬프트 상자에서 **Knowledge**를 클릭합니다. 지식 제공자를 연결하거나 선택합니다. 프롬프트를 실행하면 Knowledge가 선택한 제공자를 활용합니다.
- [**AI 지침 블록**](05-flows.md)**의 워크플로**
  AI 지침 블록에서 **지식 베이스 선택**을 클릭하세요. 지식 공급자를 연결하거나 선택하세요. AI 지침을 실행하면 선택한 공급자가 지식을 활용합니다.
- **독립형 채팅**
   Miro 독립형 채팅 앱에서 Knowledge 리소스에 접근할 수 있습니다.
  - 생성 바 위에서 **AI 팀원**을 클릭합니다. **AI 팀원** 패널이 열립니다. **Hey \{Your name\}** 위에서 아래쪽 화살표를 클릭한 후, **더 많은 AI 팀원 탐색**을 클릭합니다. **Knowledge** 탭을 클릭합니다.
  - 생성 바에서 **툴, 미디어, 그리고 통합**을 선택합니다. 귀하의 Knowledge 공급자를 검색하고 선택합니다. 예를 들어, **Gemini**.채팅 패널이 열립니다.
