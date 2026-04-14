---
title: Miro AI 레퍼런스
article_id: 20970362792210
translation_id: 20970362792210
locale: ko-kr
sidebar_position: 18
created_at: '2024-08-26T09:34:26Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: '실행 가능한 사용자: 모든 사용자 사용 가능 플랜: Free, Starter, Business, Enterprise, Education
    사용 가능 플랫폼: 브라우저, 데스크톱, 모바일'
---

이 참조 문서는 Miro AI 기능을 설명합니다.

## Miro AI 모델

모델은 일반적으로 프로바이더 인프라, Microsoft의 Azure AI 서비스 또는 AWS Bedrock에 호스팅됩니다. AWS 마켓플레이스를 통해 Miro를 구매한 고객의 경우, 모든 모델은 AWS Bedrock에 호스팅됩니다.

### AI를 활용한 창작 및 반복

| **Miro AI 기능** | **설명** | **모델** |
| --- | --- | --- |
| 대화 요약 | Miro 보드의 긴 댓글 스레드를 요약합니다. | GPT 4o-mini |
| 다이어그램 생성 - 데이터 흐름도 | 사용자 프롬프트와 선택한 보드 내용을 바탕으로 데이터 흐름도를 생성합니다. | GPT-4o |
| 다이어그램 편집 - 워크플로 차트 | 사용자 프롬프트와 선택한 보드 콘텐츠를 기반으로 워크플로 차트를 편집합니다. | GPT-4o |
| 다이어그램 생성 - 마인드맵 | 사용자 프롬프트와 선택한 보드 콘텐츠를 기반으로 마인드맵을 생성합니다. | GPT 4o-mini |
| 다이어그램 편집 - 마인드맵 | 사용자 프롬프트와 선택한 보드 콘텐츠를 기반으로 마인드맵을 편집합니다. | GPT-4o |
| 다이어그램 생성 - ERD | 사용자 프롬프트에서 엔티티 관계 다이어그램 (ERD)을 생성합니다. **AI로 생성** 옵션. | GPT 4o-mini |
| 다이어그램 편집 - ERD | 사용자 프롬프트와 선택한 보드 콘텐츠를 기반으로 ERD를 편집합니다. | GPT-4o |
| 다이어그램 디지털화 | 손으로 그린 다이어그램 이미지를 Miro에서 완전히 편집 가능한 다이어그램으로 변환합니다. | Claude 3.7 Sonnet (AWS Bedrock) |
| 문서 생성 | 사용자 프롬프트와 선택한 보드 콘텐츠를 기반으로 Miro 문서를 생성합니다. **AI로 생성** 옵션입니다. | GPT-4o |
| 문서 편집 | 사용자 프롬프트와 선택한 보드 콘텐츠를 기반으로 Miro 문서를 편집합니다. | GPT-4o |
| 이미지 생성 | 사용자 프롬프트와 보드 오브젝트 컨텍스트를 기반으로 이미지를 생성합니다. **AI로 생성** 옵션입니다. | Segmind Stable Diffusion 1B (SSD-1B) + StabilityAI Diffusion XL Refiner 1.0 |
| 이미지 편집 | 사용자 프롬프트와 보드 오브젝트 컨텍스트를 기반으로 이미지를 편집합니다. **AI로 생성하기** 옵션. | GPT-4o |
| 이미지를 프로토타입으로 변환 | 스케치 또는 프로토타입 이미지를 편집 가능한 Miro 프로토타입으로 변환합니다. | Miro 고유 모델 + Claude 3.7 Sonnet |
| 이미지 대체 텍스트 | 이미지에 대한 대체 텍스트를 생성합니다. AI 크레딧을 소모하지 않습니다. | Miro 독점 모델 |
| 스티커 메모 생성 | 사용자 프롬프트와 선택한 보드 콘텐츠를 사용해 Miro 스티커 메모를 생성합니다. | GPT-4o |
| 스티커 메모 편집 | 사용자 보드와 선택한 보드 콘텐츠를 기반으로 Miro 스티커 메모를 편집합니다. | GPT-4o |
| 스티커 캡처 | 실제 스티커 메모 이미지를 Miro 스티커 메모로 변환합니다. | Miro 전용 모델 |
| 프로토타입 생성 | 사용자 프롬프트와 선택한 보드 콘텐츠를 기반으로 Miro 프로토타입을 생성합니다. | GPT-4o + Claude 4.5 Sonnet + GPT 4o-mini + Gemini 2.5 Flash Image (nano-banana) |
| 프로토타입 화면 편집 | 사용자 프롬프트와 선택한 보드 콘텐츠를 기반으로 Miro 프로토타입 화면을 편집합니다. | Claude 4.5 Sonnet + Gemini 2.5 Flash Image (nano-banana) |
| 배경 제거 | 이미지의 배경을 제거합니다. | Miro 독점 모델 |
| 스마트 드로잉 | 연필 드로잉을 선, 도형, 또는 스티커 메모로 변환합니다. | Miro 독점 모델 |
| 테이블 생성 | 사용자 프롬프트와 선택한 보드 콘텐츠를 기반으로 Miro 테이블을 생성합니다. | Claude 3.7 Sonnet |
| 테이블 편집 | 사용자 프롬프트와 선택한 보드 콘텐츠를 기반으로 Miro 테이블을 편집합니다. | Claude 3.7 Sonnet |

### AI 탑재 팀원

|  |  |  |
| --- | --- | --- |
| **Miro AI 기능** | **설명** | **모델** |
| AI 팀원 - 애자일 코치 | 회고에서 주요 테마를 식별하고, 다음 단계에 대한 제안을 제공합니다. | GPT-4o |
| AI 팀원 - 프로덕트 리드 | 프레임, 스티커 메모 또는 텍스트에 댓글로 피드백과 제안을 제공합니다. 또한 해결 아이디어를 스티커 메모로 제공합니다. | GPT-4o |
| AI 팀원 - 프로덕트 마케팅 동맹 | 프레임, 스티커 메모 또는 텍스트에 댓글로 피드백과 제안을 제공합니다. | GPT-4o |

### AI 클러스터링

| **Miro AI 기능** | **설명** | **모델** |
| --- | --- | --- |
| 스티커 메모 키워드 클러스터링 | 스티커 메모를 키워드별로 그룹화하며, 각 그룹에 제목을 추가합니다. | Claude 3.5 Haiku + Amazon Nova Micro |
| 스티커 메모 감정 클러스터링 | 스티커 메모를 감정, 즉 의견과 관점별로 긍정적, 중립적, 부정적 그룹으로 묶습니다. | Claude 3.5 Haiku |

### AI 기반 텍스트 편집

다음 표에서는 Miro AI가 지원하는 텍스트 편집 기능을 보여줍니다:

|  |  |  |
| --- | --- | --- |
| **Miro AI 기능** | **설명** | **모델** |
| 톤 변경 | 선택한 텍스트의 톤을 친근하고 전문적이며 비즈니스 또는 재미있는 스타일로 조정합니다. | GPT-5 nano |
| 맞춤법 및 문법 수정 | 선택한 텍스트의 맞춤법 및 문법을 수정합니다. | GPT-5 |
| 명확성 재작업 | 선택한 텍스트를 명확하게 다시 작성합니다. | GPT-5 Chat |
| 텍스트 단축 | 선택한 텍스트를 명확성과 가독성을 유지하되 더 짧고 간결하게 재구성합니다. | GPT-5 mini |
| 번역 | 선택된 텍스트를 영어, 스페인어, 독일어, 프랑스어, 일본어, 포르투갈어, 한국어, 폴란드어, 이탈리아어, 터키어, 아랍어, 러시아어, 덴마크어, 핀란드어, 노르웨이어, 네덜란드어, 스웨덴어 또는 태국어로 번역합니다. 개별 또는 여러 개의 객체를 동시에 번역할 수 있습니다. | GPT-5 mini |

### AI 탑재 마인드맵

| **Miro AI 기능** | **설명** | **모델** |
| --- | --- | --- |
| 마인드맵 생성 | 선택한 루트 노드에서 마인드맵을 생성합니다. | GPT 4o-mini |
| 마인드맵 - 아이디어 추가 확장 | 선택한 루트 노드 또는 자식 노드에서 아이디어를 생성합니다. | GPT 4o-mini |
| 마인드맵 - 주제로 확장 | 선택된 루트 노드 또는 자식 노드에서 주제를 생성합니다. | GPT 4o-mini |
| 마인드맵 - 질문으로 확장 | 선택된 루트 노드 또는 자식 노드에서 질문을 생성합니다. | GPT 4o-mini |

### AI 탑재 슬라이드

Miro 슬라이드는 다음 모델을 사용합니다:

- Amazon Titan
- Claude 4 Sonnet
- Claude 3.7 Sonnet
- Claude 3.5 Sonnet
- GPT-5
- GPT-4o
- Stable Diffusion 3.5 Large
- Stability Image Core

### Miro Insights

고객 피드백을 종합하기 위해, [Miro Insights](https://help.miro.com/hc/articles/25438311770770)는 GPT-4o를 사용합니다.

### AWS 마켓플레이스 고객

**AWS 마켓플레이스 모델**

| **Miro AI 기능** | **모델** |
| --- | --- |
| 대화 요약 | Claude Haiku 3.7 (AWS Bedrock) |
| 다이어그램 생성 – 플로우 차트 | Claude Sonnet 3.7 (AWS Bedrock) |
| 다이어그램 편집 – 플로우 차트 | Claude Sonnet 3.7 (AWS Bedrock) |
| 다이어그램 만들기 – 마인드맵 | Claude Sonnet 3.7 (AWS Bedrock) |
| 다이어그램 편집 – 마인드맵 | Claude Sonnet 3.7 (AWS Bedrock) |
| 다이어그램 만들기 – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| 다이어그램 편집 – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| 문서 생성 | Claude Sonnet 3.7 (AWS Bedrock) |
| 문서 편집 | Claude Sonnet 3.7 (AWS Bedrock) |
| 스티커 메모 만들기 | Claude Sonnet 3.7 (AWS Bedrock) |
| 스티커 메모 편집 | Claude Sonnet 3.7 (AWS Bedrock) |
| 스티커 캡처 | Claude Sonnet 3.7 (AWS Bedrock) + Miro 고유 모델 |
| 이미지 생성 | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| 이미지 편집 | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| 이미지 대체 텍스트 | Claude Sonnet 3.7 (AWS Bedrock) |
| 프로토타입 생성 | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| 프로토타입 화면 편집 | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| 이미지를 프로토타입으로 변환 | Claude Sonnet 3.7 + Miro 전용 모델 |
| 테이블 생성 | Claude Sonnet 3.7 (AWS Bedrock) |
| 테이블 편집 | Claude Sonnet 3.7 (AWS Bedrock) |
| 다이어그램 디지털화 | Claude Sonnet 3.7 (AWS Bedrock) |
| 키워드별 스티커 메모 클러스터링 | Claude Sonnet 3.7 (AWS Bedrock) + Miro 자체 모델 |
| 감정별 스티커 메모 클러스터링 | Miro 자체 모델 |
| AI 팀원 | Claude Sonnet 3.7 (AWS Bedrock) |
| AI 기반 텍스트 편집 | Claude Sonnet 3.7 (AWS Bedrock) |
| AI 기반 마인드맵 | Claude Sonnet 3.7 (AWS Bedrock) |

## 모델 선택하기

다음 목록에서는 [모델 선택 기능](10-select-your-own-model-beta.md)을 사용하여 [워크플로](04-flows-overview.md) 및 AI 팀원에서 사용할 수 있는 모델을 보여줍니다.

### 대규모 언어 모델

**Claude**

- Claude 3.7 Sonnet
- Claude Sonnet 4

**OpenAI**

- GPT-4o
- GPT-4o 미니
- OpenAI o4-미니
- GPT-5
- GPT-5 미니
- GPT-4.1
- GPT-4.1 미니

### 이미지 모델

**Stability AI**

- 안정적인 이미지 코어
- 안정적인 이미지 울트라
- 안정적인 확산 3.5 대형

**Amazon**

- Amazon Titan Image Generator
- Amazon Nova 캔버스

**Google**

- Gemini 2.5 Flash 이미지 (Nano Banana)
- Vertex AI 이미지 생성 3
- Vertex AI 이미지 생성 3 Fast
- Vertex AI 이미지 생성 4

## Miro AI 크레딧과 애드온

Miro는 매월 계정에 정해진 수의 AI 크레딧을 할당합니다. 할당된 크레딧의 양은 사용 중인 플랜에 따라 다릅니다. 할당은 매월 1일에 초기화됩니다.

각 AI 작업을 수행할 때 AI 크레딧이 소모됩니다. 대부분의 AI 작업은 작업당 하나(1) 크레딧을 소모하지만, 일부 기능은 더 많은 크레딧을 소모할 수 있습니다.

AI 크레딧 할당량을 늘리고 싶다면 선택적으로 Miro AI 크레딧 애드온 구독을 구매할 수 있습니다. 자세한 내용은 [Miro AI 크레딧 및 애드온](../../plans-billing/billing-and-payments/03-miro-ai-credits.md)을 참고하세요.

## Miro AI 프라이버시 및 보안

2025년 2월 3일부터 Miro는 AI 요약, 다이어그램, AI 팀원 같은 Miro AI 기능을 개선하기 위해 Free 플랜 사용자의 AI 상호작용 데이터를 수집합니다.

Miro가 AI 상호작용을 통해 Miro AI를 개선하는 방법과 데이터 선호도를 조절하는 방법에 대한 자세한 내용은 [Miro AI 품질 향상](19-miro-ai-quality-improvements.md)을 참고하세요.
