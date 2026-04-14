---
title: "Miro AI \uAD00\uB9AC\uC790 \uBCF4\uC548"
article_id: 11277533556626
translation_id: 30755851853586
locale: ko-kr
sidebar_position: 4
created_at: '2025-11-03T14:31:31Z'
updated_at: '2026-03-27T16:19:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: free, starter, business, enterprise, education
---

이 글은 관리자에게 Miro가 Enterprise급 보안을 어떻게 보장하는지, Miro AI를 어떻게 켜고 끄는지, 자주 묻는 질문을 설명합니다.

> **사용 가능 대상:** 모든 플랜

**자세한 정보:** [Miro AI 백서](../../canvas-25-admin-features/data-security/05-miro-ai-whitepaper.md)

## Miro AI란 무엇인가요?

창의성, 협업, 생산성을 지원하는 Miro AI로 아이디어의 잠재력을 최대한 끌어내세요.

Miro는 기계 학습 모델과 사용자의 입력을 활용하여 보드의 콘텐츠를 생성하거나 수정합니다. Miro AI는 마인드맵 생성, 콘텐츠 요약, 스티커 메모 생성 등을 할 수 있습니다.

**자세한 정보:** [AI와 함께하는 생성 및 편집 개요](../../../using-miro/miro-ai/03-create-with-ai.md)

## 엔터프라이즈급 보안

Miro는 모든 규모의 분산된 팀이 꿈을 펼치고, 설계하며, 미래를 함께 만들어 나갈 수 있는 혁신을 위한 엔터프라이즈 준비된 온라인 워크스페이스입니다.

하지만, 훌륭한 협업에는 뛰어난 보안이 필요하므로, 우리는 귀하의 정보를 가능한 한 안전하게 보호하기 위해 업계 최고의 관행과 표준을 제공합니다. 보드와 콘텐츠를 어떻게 보호하는지 알아보세요.

|  |  |  |
| --- | --- | --- |
| **Checkmark.png**  **공식 인증 및 승인** | **Security_lock.png**  **신뢰할 수 있는 보호** | **Fingerprint.png**  **안전한 액세스 관리** |
| 업계 모범 사례 및 규제 요구 사항 | 지적 자산 보호 및 관리 | Miro AI 액세스 권한을 가진 사람 |
| - 일반적으로 Miro 데이터는 데이터 레지던시에 따라 EU, 미국, 호주의 서버에 저장되지만, Miro AI와의 상호작용은 모델 사용 가능 여부에 따라 선택한 지역 외부에서 처리될 수 있습니다. 자세한 내용은 [Miro의 데이터 레지던시](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md)를 참조하세요. - 데이터는 보관되지 않으며 AI 모델 학습에 사용되지 않습니다. - 사용 및 참여 조건에 대해 알아보려면 [AI 기능 추가 조항](https://miro.com/legal/ai-features-addendum/)을 참조하세요. - Miro AI가 데이터를 처리하는 방식에 대해 자세히 알아보려면 [Miro AI 개인정보 취급방침](https://miro.com/legal/privacy-policy/#miro-ai)을 참조하세요. | - Miro AI는 ISO 27001 및 SOC2 인증과 프라이버시 약속을 준수합니다. - 저희의 보안 접근 방식, 관리 모델, GDPR 및 CCPA 준수 방법에 대해 알아보시려면 [신뢰 센터](https://miro.com/trust/)를 방문하세요. - Miro는 Miro AI가 생성한 콘텐츠에 대한 권리를 주장하지 않습니다. 자세한 내용은 이 기사 끝의 자주 묻는 질문을 참조하세요. | - Miro AI는 멤버만 사용할 수 있습니다. 게스트와 방문자는 Miro AI를 사용할 수 없습니다. |

## Miro AI 활성화 및 비활성화 방법

> **사용 가능 대상:** Enterprise, Education 플랜

다음 단계를 따르세요:

1. **관리자 콘솔**로 이동하세요.
   **홈** 대시보드에서, 오른쪽 상단에 있는 아바타를 선택하십시오. 그런 다음 **관리자 콘솔**을 클릭하세요. 또는 어떤 보드에서든 아바타를 클릭하고 **프로필 설정**을 선택하세요.
2. **Miro AI** > **기능**으로 이동하세요.
3. **Miro AI**에서 다음 옵션 중 하나를 선택하세요:
   - **아무도 사용할 수 없음**
     회사의 Miro AI 기능을 모두 끕니다
   - **모두 사용할 수 있음**
     회사의 Miro AI 기능을 모두 켭니다
   - **특정 팀만 사용 가능**
     지정한 팀만 Miro AI를 사용할 수 있습니다.
4. (선택 사항) Miro AI 베타 기능을 활성화하세요.
   Miro AI가 성공적으로 활성화되거나 비활성화되었습니다.

## 자주 묻는 질문

### Miro AI 모델 & 모델 훈련

**사용자 데이터는 어떻게 사용되나요?**

Miro AI를 통해 제출된 데이터는 AI 모델의 응답을 생성하여 사용자에게 제공하는 데에만 사용됩니다. 사용하는 AI 기능에 따라 AI 모델은 Miro 또는 Microsoft Azure AI에 호스팅될 수 있습니다. 두 경우 모두, 제출된 입력 데이터는 모델 훈련에 사용되지 않으며, 콘텐츠 및 사용 데이터는 Miro의 [개인정보 취급방침](https://miro.com/legal/privacy-policy/)에 따라 사용됩니다.

**제 데이터는 어디에서 처리되나요?**

일반적으로 귀하의 Miro 데이터는 귀하의 데이터 레지던시에 따라 EU, US, AU의 서버에 저장됩니다. 그러나 Miro AI와의 상호작용은 모델의 지역 내 가용성에 따라 선택한 지역 외부에서 처리될 수 있습니다. 자세한 정보는 [Miro의 데이터 레지던시](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md)를 참조하세요.

**Miro AI는 어떤 AI 모델을 사용하나요?**

Miro AI가 사용하는 AI 모델에 대해 알아보려면 [Miro AI 개요](../../../using-miro/miro-ai/18-miro-ai-reference.md)를 참조하세요.

**Miro가 고객 데이터를 사용해 모델을 훈련하나요?**

Miro는 고객 데이터를 사용해 모델을 훈련하거나 개선하지 않습니다. 미래에 Miro가 고객 데이터를 사용해 모델을 개선하고 Miro AI 기능의 성능을 향상시키는 기능을 도입할 경우, 셀프 서비스 고객은 옵트아웃을 선택할 수 있는 기능이 제공됩니다. Enterprise 고객은 기본적으로 옵트아웃 상태이며, 명시적으로 옵트인을 해야 합니다.

**Miro AI 모델은 얼마나 자주 업데이트되나요?**

Miro는 다양한 사용 사례에 Azure OpenAI 모델을 사용합니다. 업데이트는 주로 Azure에서 제공하는 모델 업데이트에 따라 달라집니다. 자체 개발 모델은 품질 결과를 보장하기 위해 필요에 따라 업데이트됩니다.

### 신뢰할 수 있고 안전한 AI

**Miro AI가 생성한 콘텐츠의 지적 재산권은 누구에게 있나요?**

Miro와 사용자 간에는 Miro가 Miro AI에 의해 생성된 콘텐츠에 대한 권리를 주장하지 않습니다. Miro AI가 생성한 출력물에 대한 권리는 기본 AI 제공업체에 의해 결정됩니다. 예를 들어, Microsoft Azure AI (OpenAI 이용약관)에서는 OpenAI가 서비스에 의해 생성되고 반환되는 출력물의 모든 권리, 소유권, 이익을 사용자에게 양도합니다. 자세한 내용은 [AI 기능 부록](https://miro.com/legal/ai-features-addendum/)과 [Miro AI 개인정보 취급방침](https://miro.com/legal/privacy-policy/#miro-ai)을 참조하세요.

**AI 결과가 검증되고 정확한가요?**

LLM의 특성 때문에 생성된 모든 콘텐츠가 정확하지 않을 수 있습니다. 출력 결과는 항상 사용하기 전에 확인해야 합니다.

**Miro는 악의적이거나 불법적인 프롬프트 사용을 어떻게 방지하나요?**

Miro는 Azure와 협력하여 콘텐츠 모더레이션 서비스를 활용하여 악의적이거나 부적절한 출력을 필터링합니다. Miro는 프롬프트 추적 기능을 제공하지 않습니다.
