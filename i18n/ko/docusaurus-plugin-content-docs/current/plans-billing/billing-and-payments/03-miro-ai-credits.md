---
title: Miro AI 크레딧
article_id: 19756209116178
translation_id: 19756209116178
locale: ko-kr
sidebar_position: 3
created_at: '2024-06-25T21:32:21Z'
updated_at: '2026-03-04T08:31:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '실행 가능한 사용자: 모든 사용자, 결제 관리자, 회사 관리자 해당 플랜: Free, Starter, Business, Enterprise
    플랫폼: 브라우저, 데스크톱, 모바일'
---

Miro AI 크레딧은 Miro에서 AI 기능을 사용할 수 있게 해줍니다. 각 AI 작업을 수행할 때마다 AI 크레딧을 소비합니다.

Miro는 매달 계정에 일정 수의 AI 크레딧을 할당합니다. 잔액은 [플랜에 따라](#ai-credits-per-plan) 다릅니다.

Enterprise와 Free 플랜의 경우, 잔액은 매월의 첫 번째 날에 초기화 됩니다. Starter와 Business 플랜은 월별 갱신일에 잔액이 초기화 됩니다. 예를 들어, 연간 플랜을 사용 중이고 갱신일이 3월 3일이면 구독 기간 동안 매월 3일에 잔액이 초기화됩니다.

**더 많은 정보:** [플랜별 AI 크레딧](#ai-credits-per-plan)을 참조하세요.

계정의 AI 크레딧이 부족해지면, Miro에서 추가 AI 크레딧 옵션을 보여주는 모달이 나타나며 여기에는 유료 [Miro AI 크레딧 애드온](../../using-miro/miro-ai/17-miro-ai-credits-add-on.md)이 포함됩니다.

팀의 모든 멤버는 AI 액션을 수행할 때 AI 크레딧을 소모할 수 있습니다. 게스트와 방문자는 AI 액션을 수행할 수 없으며 AI 크레딧을 소모하지 않습니다.

> **팁:** 유료 플랜에서 [AI 크레딧 잔고](#check-ai-credit)를 확인할 수 있습니다.

## Miro AI 크레딧 소비

모든 AI 작업은 월별 배정된 AI 크레딧에서 소모됩니다. 예를 들어, [Miro Prototypes 애드온](../../using-miro/miroverse/prototyping/07-miro-prototypes-add-on.md)은 AI로 생성된 화면 당 5개의 AI 크레딧을 소비하며, AI로 생성된 이미지에는 3개의 AI 크레딧이 소비됩니다.

다음 표는 AI 생성 결과물에 대한 크레딧 소비 내역을 보여줍니다:

| 기능별 AI 결과물 | 소비된 크레딧 |
| --- | --- |
| AI 검색 | 0 크레딧 |
| 캐치업 | 1 크레딧 |
| 다이어그램 | 5 크레딧 |
| 문서 | 2 크레딧 |
| 이미지 | 3 크레딧 |
| 프로토타입 | 화면당 5 크레딧 |
| 배경 제거 | 1 크레딧 |
| 사이드킥 | 2 크레딧 |
| 슬라이드 | 슬라이드당 5 크레딧 |
| 스티커 메모 | 1 크레딧 |
| 테이블 | 5 크레딧 |
| 텍스트 | 1 크레딧 |

> **참고:** AI 팀원은 프롬프트를 실행할 때마다 2개의 AI 크레딧을 소모합니다. 프롬프트를 가능한 한 구체적으로 작성해 목표를 달성하기 위해 필요한 실행 횟수를 줄이세요.

> **참고:** Miro AI가 출력을 생성하지 못하고 오류 메시지를 표시하는 경우, AI 크레딧은 소모되지 않습니다.

> **참고:** 이미지 대체 텍스트 생성과 같은 접근성 기능은 AI 크레딧을 소모하지 않습니다.

### 예시 AI 크레딧 소모 시나리오

#### UX 플로우를 위한 프로토타입 생성

온보딩 플로우를 위해 Miro Prototypes 애드온을 사용하여 6개의 화면을 생성합니다.

프롬프트에 따라 Miro AI는 편집할 수 있는 6개의 개별 프로토타입 화면을 생성합니다.

- **대략적인 크레딧 소모:** 30 AI 크레딧.
- **소모 내역:** 각 화면당 5 AI 크레딧, 6개 화면 생성(5*6) = 30 AI 크레딧 소모.

#### 슬라이드 프레젠테이션 생성 및 반복

보드에 있는 메모를 기반으로 전략 덱을 생성하고 특정 슬라이드를 반복적으로 수정합니다.

Miro AI는 보드의 컨텍스트를 스캔하여 레이아웃, 텍스트, 시각 요소가 포함된 10장의 슬라이드로 구성된 구조적인 슬라이드 프레젠테이션을 생성합니다.

그러고 나서, Miro AI에게 'Executive Summary' 슬라이드를 다시 작성하고, 'Next Steps'라는 새 슬라이드를 추가하도록 프롬프트합니다.

- **대략적인 크레딧 소비량:** 60 AI 크레딧.
- **소비량 세부 사항:**
  - 슬라이드당 5 AI 크레딧, 10슬라이드에 대해 (5*10) = 50 AI 크레딧 소비.
  - 추가로 'Executive Summary' 슬라이드 수정을 위해 5 AI 크레딧.
  - 추가로 'Next Steps' 슬라이드를 생성하기 위해 5 AI 크레딧.

> **팁:** 프롬프트를 가능한 한 상세하게 만들어 한 번의 생성에 필요한 크레딧 수를 최소화하세요.

## 플랜별 AI 크레딧

다음 표는 플랜별로 매월 할당되는 크레딧 수를 보여줍니다.

| 플랜 | AI 크레딧 |
| --- | --- |
| Free | 10 크레딧/월 |
| Starter | 25 크레딧/라이선스/월 |
| Business | 50 크레딧/라이선스/월 |
| Enterprise | 라이선스 등급에 따라 다릅니다. Enterprise AI 크레딧을 참조하세요. |
| Education | 100 크레딧/월 |

:::note
[Miro Prototypes 애드온](../../using-miro/miroverse/prototyping/07-miro-prototypes-add-on.md)은 매월 최소 350개의 추가 AI 크레딧을 조직에 제공합니다. (Enterprise) 회사 관리자는 Miro 계정 관리자와 함께 더 많은 크레딧 수를 지정할 수 있습니다.
:::

조직 전체에 대해 Miro는 라이선스당 크레딧을 사용하여 월별 AI 크레딧 할당량을 계산합니다. 조직 내에서 수행되는 모든 AI 작업은 해당 할당량에서 크레딧을 소모합니다.

청구 주기 동안 사용자를 추가하거나 제거하면 Miro는 크레딧 할당량을 동적으로 조정합니다. AI 크레딧 할당량은 다음 청구일에 맞춰 새로운 팀 규모에 맞게 업데이트됩니다.

(Enterprise, Free) Miro AI 크레딧의 월별 할당량은 매달 1일에 초기화됩니다.

(Business, Starter) Miro AI 크레딧의 월별 할당량은 플랜 갱신일에 초기화됩니다.

:::tip
AI 크레딧 잔액을 늘리기 위해 Starter, Business, Enterprise 플랜에서는 [Miro AI 크레딧 애드온](../../using-miro/miro-ai/17-miro-ai-credits-add-on.md)을 구매할 수 있습니다.
:::

### Enterprise AI 크레딧

Enterprise 구독에서는 월별 라이선스당 할당되는 크레딧 수가 [라이선스 등급](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/03-miro-ai-credits-for-enterprise-plans.md)에 따라 달라집니다. 회사 관리자는 관리자 콘솔에서 AI 크레딧 할당 및 사용량을 모니터링할 수 있습니다.

**관리자 콘솔**에서 **청구** > **구독**으로 이동하세요.

> **참고:** (Enterprise) 라이선스 등급은 변경될 수 있습니다. Enterprise 등급별 할당에 대한 자세한 내용은 [Enterprise 플랜의 Miro AI 크레딧](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/03-miro-ai-credits-for-enterprise-plans.md)을 참조하세요.

## AI 크레딧 잔액 확인

유료 Miro 구독에서 결제 관리자 및 회사 관리자는 언제든지 조직의 AI 크레딧 잔액을 확인할 수 있습니다. 무료 플랜에서는 크레딧 잔액이 표시되지 않습니다.

### Starter 및 Business 플랜

**관리 콘솔** > **결제**로 이동합니다. **결제** 보기는 AI 크레딧 사용량 및 남은 잔액을 보여줍니다.

### Enterprise 플랜

**관리 콘솔** > **결제** > **구독**으로 이동합니다. **구독** 보기는 사용한 AI 크레딧과 남은 잔액을 보여줍니다.

## Miro AI 크레딧 애드온

Miro AI 크레딧 애드온은 월간 AI 크레딧 한도를 증가시키는 유료 구독입니다.

**자세한 내용:** [Miro AI 크레딧 애드온](../../using-miro/miro-ai/17-miro-ai-credits-add-on.md)을 참조하세요.
