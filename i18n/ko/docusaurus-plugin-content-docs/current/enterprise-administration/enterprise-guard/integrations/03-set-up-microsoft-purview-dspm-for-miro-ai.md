---
title: "Miro AI (\uBCA0\uD0C0)\uB97C \uC704\uD55C Microsoft Purview DSPM \uC124\uC815"
article_id: 28698434922386
translation_id: 28698434922386
locale: ko-kr
sidebar_position: 8
created_at: '2025-08-11T19:20:50Z'
updated_at: '2026-01-12T11:28:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Miro AI가 Microsoft Purview의 DSPM for AI에 나타나도록 Microsoft Purview 데이터 보안 상태 관리(DSPM)를 설정하는 방법을 소개합니다. 설정 후 이벤트를 확인하고 통합 관리 방법을 배우게 됩니다.

## **사전 요구 사항**

### **Miro**

- **Enterprise Guard**가 활성화된 Enterprise 플랜.
- **회사 관리자** 자격이 필요합니다.
- **Microsoft Entra ID**가 Miro에서 **SSO 제공자**로 구성되어 있습니다.
- 베타에서 이 기능을 활성화하려면 고객 성공 매니저에게 문의하세요.

### **Microsoft**

- DSPM for AI를 지원하는 활성화된 Microsoft Purview 라이선스.
- Miro SSO용으로 사용되는 Microsoft Entra ID 테넌트 ID (Microsoft 조직/테넌트를 식별하는 GUID).
- 애플리케이션에 테넌트 전체의 관리자 동의를 부여할 수 있는 Entra 역할.

## **Miro에서 통합 설정**

1. Miro에서 **Enterprise 설정 → Enterprise 통합**을 엽니다.
2. 아래로 스크롤한 다음 **Microsoft Purview DSPM for AI**를 켭니다.
3. 테넌트 ID 상자에 **Microsoft Entra 테넌트 ID**를 입력합니다.
4. **연결**을 클릭합니다.
5. 프롬프트가 나타나면 **테넌트 전역 관리자 권한**을 부여할 수 있는 계정으로 Microsoft Entra에 로그인합니다.
6. **Miro AI 거버넌스** 애플리케이션에 대한 동의를 검토하고 **허용**을 클릭합니다.
7. Miro로 돌아가 통합이 **연결됨**으로 표시되는지 확인합니다.

## **Microsoft Purview에서 액티비티 확인**

1. Miro에서 단순한 AI 작업을 수행합니다 (예: 보드에서 **스티커 메모** 요약하기).
2. 수집을 위해 **최대 10–30분** 기다립니다.
3. Microsoft Purview에서 **Microsoft Purview → AI용 DSPM → 액티비티 탐색기**로 이동합니다 (AI 활동을 나열하는 Purview 보기). 감사 로그에서도 정보를 확인할 수 있습니다.
   참고: Miro AI 기능에서 텍스트 기반의 모든 프롬프트와 응답이 Purview로 전송됩니다. 현재 이미지 콘텐츠는 Microsoft Purview로 전송되지 않습니다.
4. **최근** 이벤트를 필터링하여 Miro에서 활동(예: 프롬프트 및 응답)을 찾습니다.

## **통합 관리**

- **연결 해제**: Miro에서 **Enterprise 통합 → Microsoft Purview for AI → 연결 해제**로 이동하세요.
- **테넌트 변경**: 먼저 **연결 해제**를 하고 다른 **테넌트 ID**를 사용하여 다시 **연결**하세요.

## **문제 해결**

- **통합 옵션 누락**: 조직에 **Enterprise Guard**가 설정되어 있는지 확인하고 계정이 **Enterprise 통합**에 접근할 수 있는지 확인하세요. **회사 관리자**에게 접근 권한을 요청하세요.
- **테넌트 ID 불일치 또는 연결 오류**: 테넌트 ID가 Miro **SSO**용으로 사용되는 Microsoft Entra 테넌트와 **정확히 일치해야** 합니다.
- **승인 실패 또는 로그인 반복**: **테넌트 전역 관리자 승인**을 제공할 수 있는 계정으로 로그인하세요(당신의 Microsoft 관리자와 협력).
- **활동이 보이지 않음**: **구성된 테넌트**를 통해 Miro에 로그인한 사용자가 테스트 AI 작업을 수행했는지 확인하고, **10~30분** 기다린 후, **Purview 라이선스**를 확인하고, **DSPM for AI → 활동 탐색기**를 확인하세요.
- **다수의 테넌트/IdP**: Miro에는 오직 **하나의 테넌트**만 구성할 수 있습니다. 다른 테넌트/IdP의 SSO를 통해 로그인한 사용자의 활동은 **전달되지 않습니다**.

## **알려진 한계**

자세한 내용은 [개요 문서의 알려진 제한 섹션](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md)을 참조하세요.
