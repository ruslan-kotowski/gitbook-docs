---
title: "Enterprise Guard \uBC0F Microsoft Purview DSPM\uC758 AI \uD1B5\uD569 \uAC1C\
  \uC694 (\uBCA0\uD0C0)"
article_id: 28617278171154
translation_id: 28617278171154
locale: ko-kr
sidebar_position: 0
created_at: '2025-08-07T15:17:38Z'
updated_at: '2026-01-12T11:27:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Microsoft Entra ID(이전 명칭: Azure AD)를 ID 공급자로 사용하는 조직의 경우, Enterprise Guard는 AI 프롬프트와 응답을 Microsoft Purview 데이터 보안 상태 관리(DSPM)로 안전하게 전달합니다. 그 결과 보안 및 규정 준수 팀은 단일 신뢰 플랫폼에서 생성 AI 사용을 모니터링, 감사 및 제어할 수 있으며, 운영 비용을 줄이고 데이터 유출 및 오용과 같은 위험을 완화하며 Miro의 엔터프라이즈급 AI 거버넌스를 강화할 수 있습니다.

:::note
베타 릴리스는 다이어그램, 마인드맵, 문서, 프로토타입, 스티커 메모, 테이블을 포함한 Miro AI 포맷을 지원하지만, 이미지는 지원하지 않습니다. 이미지 및 더 많은 AI 기능에 대한 지원을 추가하기 위해 작업 중입니다.
:::

## **대상**

이 기능은 Miro 및 Microsoft Entra ID(이전 명칭: Azure AD)/Microsoft Purview를 관리하는 Enterprise Guard 고객을 위한 베타 릴리스에서 제공됩니다.

## **받을 수 있는 것**

- **중앙 집중식 가시성:** Microsoft Purview의 AI 허브에서 Miro AI 사용 보기
- **감사 가능성:** 검토를 위해 프롬프트(사용자 입력)와 응답(AI 출력)이 기록됩니다.
- **거버넌스 정렬:** 기존 Purview 워크플로를 사용하여 모니터링, 경고 및 보유를 관리하세요.

## **요구 사항**

### **Miro**

- Enterprise 플랜에 **Enterprise Guard**가 활성화된 경우.
- 당신은 **회사 관리자**입니다.
- Miro에서 SSO 제공업체로 구성된 Microsoft **Entra ID**.
- **Enterprise 통합** 페이지에 대한 액세스 (보이지 않는 경우, 액세스 권한을 **회사 관리자**에게 요청하세요).
- 이 기능을 베타에서 활성화하려면, 고객 성공 매니저에게 문의하세요.

### **Microsoft**

- 활성화된 **Microsoft Purview** 라이선스.
- 귀하의 **Microsoft Entra ID 테넌트 ID** (Miro SSO에 사용된 동일한 테넌트로, 귀하의 Microsoft 조직/테넌트를 식별하는 GUID입니다).
- 애플리케이션에 테넌트 전체의 관리자 동의를 **부여할 수 있는 Entra 역할**.

## **작동 방식**

1. Miro 관리자가 Miro에서 **Enterprise 통합** 페이지를 통해 Microsoft Entra 테넌트를 연결합니다.
2. 이를 통해 Microsoft 테넌트에 **Miro AI 거버넌스** 애플리케이션이 설치됩니다 (테넌트 전체의 관리자 동의를 통해).
3. 사용자가 해당 테넌트를 통해 Miro에 로그인하고 Miro AI를 사용할 때, Miro는 프롬프트/응답을 Microsoft Purview로 전달합니다.
4. 액티비티는 Microsoft Purview의 **DSPM for AI → 액티비티 탐색기**에 나타납니다 (AI 액티비티를 나열하는 Purview 보기, 수집 시간이 필요함).

## **데이터 가시성 및 지연 시간**

- 로그된 데이터: **Miro에서 SSO(통합로그인)를 통해 로그인을 한 사용자가 생성한 AI 프롬프트와 응답**
- 위치: 어디서 보나요? **Microsoft Purview → DSPM for AI → Activity explorer** (AI 활동을 나열하는 Purview 보기입니다). 감사 로그에서 정보를 볼 수도 있습니다.
  **참고:** Miro AI 기능 전반에 걸친 모든 텍스트 기반 프롬프트와 응답이 Purview로 전달됩니다. 현재 이미지는 Microsoft Purview로 전달되지 않습니다.
- 지연 시간: Miro에서 AI 작업 후 **10-30분 이내에** 기록이 나타납니다.

## **알려진 제한 사항**

- 베타 버전은 이미지 제외 Miro AI 포맷을 지원합니다. 다이어그램, 마인드맵, 문서, 프로토타입, 스티커 메모, 테이블을 포함합니다. 곧 다가올 릴리즈에서 이미지 및 더 많은 AI 기능에 대한 지원을 추가하기 위해 노력하고 있습니다.
- Miro에서 한 번에 **하나의 Microsoft Entra 테넌트 ID**만 구성할 수 있습니다.
- 다중 IdP 또는 다중 테넌트 환경에서는 **구성된 테넌트**를 통해 Miro에 로그인한 사용자의 **활동만** Microsoft Purview에 로그됩니다.

## **보안 및 개인정보 보호**

Miro는 프롬프트와 응답을 **사용자의 Microsoft 테넌트**로 전달하여 Purview에서 모니터링할 수 있도록 합니다. **거버넌스, 보유, 접근 제어**는 Microsoft 환경에서 관리됩니다.

##

## **FAQ**

- **Q: 어떤 Miro AI 기능이 기록되나요?**
  **A:** 모든 Miro AI 기능의 텍스트 기반 프롬프트와 응답이 Purview로 전달됩니다. 현재 이미지 콘텐츠는 Microsoft Purview로 전달되지 않습니다.
- **Q: 모든 사용자를 포함하나요?**
  **A:** 구성된 Microsoft Entra 테넌트를 사용해 Miro에 인증된 사용자만 포함됩니다.
- **Q: Miro에서 로그를 내보낼 수 있나요?**
  **답변:** Microsoft Purview를 사용하여 내보내기 및 보유를 관리하세요. Miro는 귀하의 Microsoft 테넌트로 활동을 전송하며, 이는 귀하의 정책에 따라 관리됩니다.
- **질문: 보안과 개인정보 보호는 어떻게 되나요?**
  **답변:** Miro는 AI 프롬프트와 응답을 **귀하의 Microsoft 테넌트**에 전송하여 Purview에서 모니터링할 수 있도록 합니다. **거버넌스, 보유 및 액세스 제어**는 Microsoft 환경에서 관리됩니다.

## **지원 및 리소스**

- Entra 동의 요구 사항에 대해서는 애플리케이션에 **테넌트 전체 관리자 동의를 부여**하기 위한 Microsoft 문서를 참조하세요.
- Enterprise Guard 설정 지침에 대해서는 [이 문서](../../enterprise-subscription-management/integrations/03-set-up-microsoft-purview-dspm-for-miro-ai.md)를 참조하세요.
