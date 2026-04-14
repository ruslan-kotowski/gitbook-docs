---
title: "Microsoft \uBC0F Power BI \uD1B5\uD569 \uC124\uC815"
article_id: 25132703621394
translation_id: 25132703621394
locale: ko-kr
sidebar_position: 3
created_at: '2025-03-06T10:27:14Z'
updated_at: '2025-11-25T15:49:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
---

:::note
Microsoft 또는 Power BI와의 Miro 통합에 대한 포괄적인 관리자 문서, 자세한 다이어그램과 추가 FAQ를 포함한 정보를 보려면 [Microsoft 관리자 문서](https://docs.google.com/document/d/1Gw94z5Pc-elS-pRXKGZVBWKKNEIFR9y9yzAAkbXKwMM/edit?usp=sharing) 또는 [Power BI 관리자 문서](https://docs.google.com/document/d/1hMepF163jQF8LI-U8ES8DzHVMW4TltXDr14fJ2KU29k/edit?tab=t.0#heading=h.gu9ng058yy7y)를 참조하세요.
:::

이 문서에서는 Miro와 Microsoft 또는 Power BI 통합 설정 방법을 설명합니다.

## Microsoft 또는 Power BI 통합 설정

Microsoft 또는 Power BI 통합을 설정하려면 사용자가 Miro에서 자신의 Microsoft 또는 Power BI 콘텐츠에 대한 권한을 부여할 수 있도록 허용해야 합니다.

### 전제 조건

- Microsoft Entra에 관리자 액세스 권한이 있는지 확인하세요.
- 회사 관리자가 Miro 조직에 Microsoft 또는 Power BI를 승인했습니다. (이는 조직에서 앱 설치를 제한하는 경우 Miro 측 앱 승인 정책을 의미합니다).

### 절차

Microsoft Entra를 구성하여 Miro 통합을 허용하는 데 중점을 둡니다.

1. **Entra**에 관리자 권한으로 로그인하세요.
2. **Enterprise 애플리케이션** > **동의 및 권한**으로 이동하세요.
3. **사용자가 승인할 수 없는 앱에 대해 관리자 승인을 요청할 수 있도록** **예**를 선택합니다.
4. **관리자 동의 요청을 검토할 수 있는 사람**에서 애플리케이션에 대한 관리자 동의 요청을 검토하도록 허용할 사용자, 역할 또는 그룹을 선택합니다.

:::note
위의 4단계에서 지정된 Entra 관리자는 Microsoft Entra의 **Enterprise 애플리케이션 > 관리자 승인 요청** 섹션으로 이동해 "Contenthub PowerBI Integratio" (또는 유사한 이름의) 애플리케이션을 조직을 위해 검토하고 승인할 수 있습니다.
:::

## Microsoft 또는 PowerBI 통합을 검증하세요

Miro 보드 링크를 복사해 붙여넣으세요.

앱이 회사 관리자에 의해 사전 승인된 경우, 화면의 모달 지침을 따르세요. Miro는 iFrame으로 앱 콘텐츠를 보드에 추가합니다.

앱이 사전 승인되지 않은 경우, **추가 및 승인** 모달이 열려 회사 관리자에게 요청을 보낼 수 있습니다. 요청을 보내세요.

회사의 관리자가 응답하면 알림을 받게 됩니다.

**추가 정보:** [앱 관리](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md) 참조.
