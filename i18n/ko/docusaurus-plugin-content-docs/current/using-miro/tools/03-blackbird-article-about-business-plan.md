---
title: "SCIM\uC5D0 \uB300\uD55C Balckbird \uBB38\uC11C \uD14C\uC2A4\uD2B8"
article_id: 25902000474898
translation_id: 25902000474898
locale: ko-kr
sidebar_position: 3
created_at: '2025-04-08T15:00:21Z'
updated_at: '2025-05-07T11:29:05Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

테스트 문서

도메인 간 ID 관리 시스템(SCIM)은 Miro와 사용자의 ID 공급자(IdP) 간의 사용자 관리 및 프로비저닝 관리를 자동화할 수 있게 해줍니다.

> **사용 가능 대상:**[Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) 플랜
> **설정 기준:** 회사 관리자

## 알아야 할 중요

- **자동화된 프로비저닝을 구성하기 전에 Enterprise 플랜에서 SAML 기반 SSO가 제대로 설정되어 있고 작동하고 있어야 합니다.**
  SAML SSO(통합로그인) 구성 [가이드를](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) 확인하세요.
- **Miro 팀과 그룹 동기화는 선택 사항입니다.**
  IdP 그룹을 Miro의 팀과 동기화할 수 있습니다. 그러나 IdP 그룹이 의도치 않게 혹은 일시적으로 삭제되어 해당 그룹의 모든 사용자가 Miro에서 비활성화되고 보드와 스페이스의 재할당이 발생하는 문제를 피하기 위해, IdP 그룹을 Miro 팀과 동기화하지 마세요. [Teams API](https://developers.miro.com/reference/enterprise-create-team)를 사용해 팀을 만들고 관리할 수 있습니다. SCIM API를 통해 그룹을 관리하는 방법에 대한 자세한 내용은 [Miro 개발자 문서](https://developers.miro.com/docs/groups)를 참조하세요.
- **SCIM에서 이메일 주소 변경 시 다음과 같은 검증 규칙이 적용됩니다:**
  - **관리 사용자 확인:** 사용자의 현재 도메인이 SCIM 요청을 시작한 조직에 의해 클레임되지 않은 경우, 이메일 업데이트가 차단되고 400 오류가 발생합니다.
  - **대상 이메일 도메인 인증:** 대상 이메일 도메인이 SCIM 요청을 시작한 조직이 아닌 다른 조직에 의해 클레임된 경우, 이메일 업데이트가 차단되고 400 오류가 발생합니다. SCIM 요청을 시작한 조직이 대상 이메일 도메인을 소유한 경우, 이메일 확인 없이 이메일 업데이트가 허용됩니다. 감사 로그는 사용자가 멤버로 있는 각 조직에서 업데이트를 기록합니다.
  - **도메인 제어 및 SSO(통합로그인):** 이메일 업데이트는 도메인 제어(IDC) 또는 SSO(통합로그인)를 통한 도메인 인증을 기반으로 허용됩니다. 시작하는 조직에서 CD로 또는 SSO(통합 로그인)로 대상 이메일 도메인이 인증된 경우, 업데이트가 진행될 수 있습니다.
    ![scim-diagram-2.png](images/26547024902034_scim-diagram-2.png)
    *SCIM 이메일 변경 검증 워크플로 다이어그램*

### Miro SCIM이 작동하는 규칙

- SCIM과 동기화된 변경 사항은 주로 새로 할당된 사용자에게 적용됩니다. 이미 구독을 받고 있는 사용자의 상태는 보완되지만 변경 사항이 그룹/팀 수준에서 적용되어 덮어쓰이지 않을 수 있습니다. 예를 들어:
  a) 사용자가 Miro 측에서 Team1의 멤버이고 IDP가 Team2에 추가하기 위해 업데이트를 전송해도 Team1의 상태에는 영향을 미치지 않습니다.
  b) IDP가 User1에 변경 사항이 포함된 업데이트를 전송해도 다른 팀 멤버는 영향을 받지 않습니다. **지원되는 기능** > **그룹 동기화 및 푸시 그룹**을 참조하여 팀 상태를 덮어쓰고 모든 사용자를 한 번에 다시 동기화하세요. 새로운 푸시를 시도하고 시작해보세요.
- SCIM으로 프로비저닝된 모든 사용자는 구독의 *기본 라이선스*가 할당됩니다.
  a) 플렉시블 라이선싱 프로그램이 없는 Enterprise 구독의 경우: 풀 라이선스. 구독에 라이선스가 부족하면 사용자가 [제한된 무료](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) 라이선스로 프로비저닝되기 시작합니다.
  b) [플렉시블 라이선싱 프로그램](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)이 활성화된 Enterprise 구독의 경우: [기본 구독 라이선스](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md)에 따라 무료 또는 제한된 무료 라이선스입니다.
  *- 일부 사용자가 기본 라이선스와 다른 라이선스로 프로비저닝되어야 하는 경우:*
  *위에서 설명한 대로 모든 사용자는 기본 라이선스로 프로비저닝됩니다. 그러나 **UserType** 속성을 전체 값으로 사용하여 일부 또는 전체를 즉시 업데이트할 수 있습니다. 이 속성으로 업데이트된 사용자는 사용자 측에 가동 중지 시간 없이 풀 라이선스로 업그레이드됩니다.*
- SCIM으로 프로비저닝된 모든 사용자는 [도메인 제어](../../enterprise-administration/canvas-25-admin-features/domain-control/01-domain-control.md) 기능의 영향을 받습니다. 즉, 사용자가 ID 공급자에서 하나의 보안 그룹에만 속해 있지만 도메인 제어 설정이 3개 팀을 지정된 팀으로 정의하면 사용자는 해당 3개 팀에도 추가됩니다.
- 서비스를 보호하기 위해 Miro는 30초마다 사용 가능한 API 호출 수를 제한합니다.

  | 요청 유형 | 제한 레벨 |
  | --- | --- |
  | SCIM/사용자 가져오기    GET scim/users/\{userId\} | 첫 번째 속도 한도 레벨 1 |
  | POST scim/users/\{userId\}    PUT scim/users/\{userId\}    패치 scim/users/\{userId\}    DELETE scim/users/\{userId\} | 세 번째 속도 한도 레벨 3 |
  | GET scim/그룹    패치 scim/Groups/\{groupId\} | 네 번째 속도 한도 레벨 4 |
  | GET scim/Groups/\{groupId\} | 세 번째 속도 한도 레벨 4 |

  한도 레벨에 대한 자세한 내용은 [**여기를**](https://developers.miro.com/reference#ratelimiting) 참고하세요. **요청 수가 한도를 초과하면 Miro는 표준 **429 요청이 너무 많음** 응답을 반환합니다.**

## 지원되는 기능

자세한 Miro SCIM 스키마는 [**여기에서**](https://developers.miro.com/docs/scim) 찾을 수 있습니다.

Miro는 다음과 같은 프로비저닝 기능을 지원합니다:

- **새 사용자 만들기**
  IdP에서 Miro 애플리케이션에 할당된 새 사용자는 Miro Enterprise 구독에서 Enterprise 멤버로 생성됩니다. 동일한 이름의 Miro 팀에 동기화된 사용자 그룹에 추가된 사용자가 팀 멤버로 팀에 추가됩니다
- **사용자 프로필 업데이트 푸시**
  지원되는 속성 및 변경 사항은 아래를 참조하세요
- **그룹 동기화 및 푸시**
  IdP 그룹과 멤버를 Miro Enterprise 구독 내의 팀에 동기화하여 사용자 멤버십을 자동으로 관리하세요. 진행 중인 동기화가 그룹 사용자에 대한 특정 업데이트를 동기화된 Miro 팀에 전송하고, 푸시가 이루어지면 팀 상태가 덮어쓰여집니다. 이 경우 그룹이 진실의 소스로 간주되며, Miro 측에서 회사 관리자가 수동으로 변경한 경우 해당 상태 역시 덮어씁니다.
- **그룹/팀 이름 분리**
  Miro는 그룹과 팀을 이름으로 동기화하므로 정확한 동일한 이름을 가져야 합니다. 그러나 초기 동기화가 생성된 후에는 둘 중 하나 또는 둘 모두에게 편리한 이름을 지정할 수 있습니다. [여기에서](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md) 분리 예제를 볼 수 있습니다
- **그룹/팀에서 사용자 제거 (Enterprise 구독이 아닌 경우, 아래 참조)**
  그룹에서 사용자를 제거하면 다음 그룹 푸시 중에 동기화된 Miro 팀에서도 제거됩니다.
- **사용자 비활성화**
  IDP에서 사용자를 비활성화/삭제하거나 사용자의 애플리케이션 액세스를 비활성화하면 *비활성화*되어 Miro Enterprise 플랜에서 사용자가 비활성화됩니다.</span> 상황에 따라 사용자를 비활성화하면 가장 오래된 팀 관리자에게 콘텐츠가 다시 할당될 수 있습니다.
  - IDP 끝에서 사용자를 비활성화했지만 Miro 앱에 할당된 상태로 유지하면, Miro 끝의 팀 멤버십은 변경되지 않고, 콘텐츠는 재할당되지 않습니다. 사용자는 단순히 **활성** 상태에서 **비활성화** 상태(사용자 섹션)로 이동하며, 라이선스를 더 이상 사용하지 않게 됩니다.
  - 사용자가 일부 *동기화된* 팀의 구성원인 동안 IDP에서 사용자를 삭제하거나 Miro 앱에서 사용자를 분리해 비활성화하는 경우 해당 사용자가 *해당* 팀에서 추가로 제거되고, 해당 팀의 콘텐츠는 가장 오래된 팀 관리자에게 재할당됩니다.
  - IDP에서 사용자를 *삭제하거나* Miro 앱에서 *사용자를 분리해* 비활성화하면, 사용자가 *동기화된* 팀의 구성원이 아닌 경우 사용자의 팀 멤버십은 변경되지 않으며, 콘텐츠도 재할당되지 않습니다.
  **Enterprise 구독**에서 사용자를 제거하는 것이 기본적으로 지원되지 않습니다 그러나 [API를 사용해 수동으로 기능을 추가해](https://developers.miro.com/docs/scim#section-delete-user-by-id) 사용자가 **비활성화** 상태로 설정되지 않고 구독에서 완전히 제거되도록 할 수 있습니다. 이 시나리오에서는 콘텐츠가 각 팀 멤버에게 다시 할당됩니다. 관리자가 자동으로 할당된 콘텐츠에 대한 소유권을 설정할 수는 없습니다. 그러나 이것은 사용자를 수동으로 비활성화할 때 Miro 설정에서 [설정할 수 있습니다](../../enterprise-administration/user-management/01-deactivated-users.md).
- **사용자 재활성화**
  사용자를 애플리케이션에 다시 할당하거나 IDP에서 사용자 프로필을 재활성화하면 이전에 프로비저닝되고 비활성화된 경우 Miro Enterprise 구독에서 다시 활성화됩니다.
- **결제 그룹 할당 자동화**
  SCIM을 사용하여 새 사용자를 [billing groups](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/01-billing-groups.md)에 자동 할당하세요. ID 공급자(IdP)가 설정되면 비용 센터를 결제 그룹에 연결하세요. 이를 통해 해당 비용 센터의 모든 현재 및 향후 사용자가 적절한 결제 범주로 자동 정렬됩니다.

직접 **API** 호출을 보내 Enterprise 플랜에서 사용자를 제거할 수도 있습니다. 문서는 [여기](https://developers.miro.com/docs/scim#section-delete-user-by-id)에서 참고하세요. *직접* 통화만 사용자가 제거됩니다. **삭제** 이벤트가 *ID 솔루션에 의해 시작된 경우* 이를 **비활성화** 요청으로 처리됩니다.

### 지원되는 속성

:::warning
참고:
- **이메일** / 기본 매개 변수 / 고유 식별자 / **사용자 이름**)은 Miro에서 필요한 유일한 값이며 이메일 형식이어야 합니다.
- 이미 동기화된 사용자만 이메일 업데이트가 가능합니다. 즉, IdP와 Miro의 이메일이 동일할 때 첫 번째 동기화가 이루어져야 하며, 그렇지 않으면 Miro는 사용자를 인식하지 못하고 새 이메일 아래에 중복된 Miro 프로필이 생성됩니다.
- 이메일 업데이트는 할당 목록이 아닌 사용자의 IdP 프로필에서 이루어져야 합니다.
- 다른 속성과 달리 사용자의 **이메일**을 업데이트하면 이전 이메일과 새 이메일 모두 Miro에 로그인할 새 이메일 주소를 사용하라는 알림 편지를 받게 됩니다.
:::

| 속성 이름 | SCIM 속성(클레임) |
| --- | --- |
| 이메일 | 사용자 이름.  **현재 이메일 형식이어야 합니다** |
| *아래 나열된 속성은 필수가 아니며, 존재할 경우 Miro가 수락합니다 (Miro로 전송된 다른 속성은 무시됩니다).* | |
| 전체 이름 | displayName;      형식      givenName + " " + familyName;      사용자 이름 |
| 사용자 유형 | 사용자 유형 지원되는 값: 전체 |
| 활성 | 활성       지원되는 값: "true" 또는 "false" |
| 프로필 사진 | **photos.^[type=='photo'].value** 또는     **photos.^[type==photo].value** (Okta)     **photos[type eq "photo"].value** (엔트라)       이미지의 텍스트 URL이어야 합니다.       지원되는 파일 유형: jpg, jpeg, bmp, png, gif  파일 유형을 정의하려면 url에 파일 확장자가 정의되어 있어야 합니다 (예: `https://host.com/avatar_user1.jpg`) 또는 url 요청에 파일 콘텐츠와 함께 Content-Type 헤더가 반환되어야 합니다 (예: Content-Type = 'image/jpeg')        다운로드할 최대 파일 크기: 31457280바이트 |
| 사용자 역할 | roles.^[primary==true].value (Okta)      roles[primary eq "True"].value (Entra)  지원되는 값: **ORGANIZATION_INTERNAL_ADMIN** **ORGANIZATION_INTERNAL_USER** |
| 직원 번호 | 직원 번호 |
| 비용 센터 | costCenter |
| 조직 | 조직 |
| 부문 | 부문 |
| 부서 | 부서 |
| 관리자 이름 | manager.displayName |
| 관리자 ID | manager.value  "값" 필드에 SCIM 표준의 문자열 유형이 있지만 managerId       내부 Miro 필드의 유형은 Long입니다. "값" 속성이 아닌 경우       숫자 값 이 값을 무시함 |

:::warning
비밀번호 변경은 지원되지 않으며 이 변경을 지원할 계획이 즉시 없습니다.
⚠️ **사용자 이름**, **사용자 유형** 및 **역할.값**은 [비활성화된 사용자](../../enterprise-administration/user-management/01-deactivated-users.md)에 대해 업데이트할 수 없습니다.
:::

모든 속성은 내보낸 CSV 사용자 목록에 표시되며, 이는 [활성 사용자](../../enterprise-administration/user-management/12-user-management-overview-on-enterprise-plan.md) 섹션에서 다운로드할 수 있습니다.

![회사 설정에서 CSV 파일로 다운로드.jpg](images/26547032837650_download%20as%20CSV%20in%20company%20settings.jpg)
*사용자 목록 다운로드 옵션*

![mceclip3.png](images/26547032839186_mceclip3.png)

## SCIM 구성

### 1단계: Miro에서 SCIM 옵션 활성화

Miro Enterprise 플랜에 SCIM을 활성화하려면 **회사** 설정 > **엔터프라이즈 통합**으로 이동하여 SCIM 프로비저닝 기능을 활성화하세요**.</strong>** 거기서 IdP를 구성하기 위한 기본 URL과 API 토큰을 얻을 수 있습니다.

![scim.png](images/26547024905874_scim.png)
*Miro 설정의 SCIM*

### 2단계: ID 공급자 구성

설정은 사용하는 ID 공급자에 따라 달라집니다. Miro는 사전 구성된 Okta 및 Entra ID를 지원하지만, SCIM 설정이 가능한 경우 원하는 ID 공급자를 사용할 수 있습니다.

OKTA - [여기에서 설정 지침을 확인하세요](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md).

Entra ID - 설정 지침은 [여기에서](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md) 확인하세요.

## 새 토큰 생성

1. 회사 **설정** > **Enterprise 통합**으로 이동하세요.

2. <span>**SCIM 프로비저닝** 섹션에서 **새 토큰 생성**을 클릭하세요.

![scim.png](images/26547024905874_scim.png)
*Miro 설정의 SCIM*

2. **새 SCIM 토큰 생성** 창에서 **생성**을 클릭하세요.

![generate_token.png](images/26547032841874_generate_token.png)

3. 새 토큰을 생성한 후 IDP 공급자에서 새 토큰을 구성해야 합니다.

## 발생 가능한 이슈 및 해결 방법

*1. 허용 목록 오류로 인해 사용자가 프로비저닝되지 않습니다.*
![mceclip0.png](images/26547024910226_mceclip0.png)
*Okta ID 공급자의 오류 예*

보안 설정에서 사용자의 도메인 주소가 허용 목록에 추가되었는지 확인하세요. [**Security** 설정](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)

*항목 2. 단일 ID 솔루션(IDP1)으로 최종 사용자를 인증했지만 다른 IDP2를 통해 SCIM을 활성화하려면 다음 두 가지 조건에서 가능합니다:*

1. IDP2는 베어러 토큰으로 API 호출을 수행할 수 있습니다.
2. 두 ID 공급자가 동기화 중(SCIM으로 프로비저닝된 사용자가 IDP1에도 존재하므로 Miro에서 인증할 수 있음).

자세한 내용은 [Miro 지원팀에 문의](https://help.miro.com/hc/en-us/requests/new?referer=help-center-article)하세요.
