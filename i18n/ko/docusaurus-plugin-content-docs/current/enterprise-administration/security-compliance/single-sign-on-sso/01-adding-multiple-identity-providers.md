---
title: 여러 ID 공급자 추가
article_id: 16287287497234
translation_id: 16287287497234
locale: ko-kr
sidebar_position: 1
created_at: '2024-01-10T10:51:24Z'
updated_at: '2026-02-18T08:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '사용 가능 대상: Enterprise 설정 가능한 사용자: 회사 관리자'
---

:::note
여러 ID 공급자를 추가하는 기능은 Enterprise 고객에게만 제공되는 비공개 기능입니다. 이 기능에 액세스하여 활성화하려면 Miro 계정 팀 관리자 또는 고객 성공 매니저에게 문의하세요. Miro 지원에서는 이 기능을 활성화할 수 없습니다.
:::

SSO(통합로그인)를 위해 여러 ID 공급자(IdP)를 사용하세요. 이는 각 지사 또는 자회사가 자체 IdP를 보유하지만 동일한 Miro 구독에 대한 액세스가 필요한 대기업에 특히 유용합니다.

## 여러 ID 공급자를 추가하기 위한 준비

여러 ID 공급자 애플리케이션을 추가한 후에도 [SSO(통합로그인)](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) 기능이 계속 작동하도록 하려면, 기존 IdP 애플리케이션의 구성을 업데이트해야 합니다.

엔트라 ID와 일부 다른 IdP는 조직이 다중 ID 공급자(다중 IdP) 프라이빗 기능을 활성화하지 않으면 새로운 구성 형식을 지원하지 않습니다. 로그인 중단을 방지하려면, 고객 성공 매니저와 함께 다중 IdP 프라이빗 기능을 활성화하고 동시에 구성을 업데이트하는 방법에 대한 단계별 지침을 받도록 협의하는 것을 권장합니다.

### Enterprise 설정 구성 방법

1. SCIM 끄기.
2. SSO 설정 업데이트.
3. SSO 기능 확인.

#### SCIM 끄기

현재 여러 IdP와 [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)을 지원하지 않습니다. Enterprise 플랜에서 SCIM을 끄려면 **회사** 설정 > **계정** > **Enterprise 통합**으로 이동하여 **SCIM 프로비저닝**을 끄세요.

#### SSO 설정 업데이트

**이전 설정**

Miro SSO가 처음 IdP에 구성될 때, 다음과 같은 구성값이 사용된 것으로 보입니다:

- **Callback URL/ACS:** https://miro.com/sso/saml
- **Entity ID:** https://miro.com

**새로운 구성**

IdP가 Miro와 관련된 구성을 인식할 수 있도록 하기 위해, 아래 값을 업데이트해야 합니다. **설정** > **보안** > **인증**으로 이동합니다.

이 값들은 조직에서 멀티 IdP 개인 기능을 활성화하면 SSO 설정에 표시되며 다음과 같은 형식을 가지게 됩니다:

- **Callback URL/ACS:** https://miro.com/sso/saml/&lt;org_id&gt;/&lt;saml_settings_id&gt;
- **Entity ID:** "https://miro.com/&lt;org_id&gt;/&lt;saml_settings_id&gt;

![Callback URL and Entity ID in the Enterprise admin console](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/23763575205778_image.png)

*Enterprise 관리자 콘솔에서의 Callback URL 및 Entity ID*

#### SSO 기능 확인

IdP 구성을 완료한 후, SSO가 제대로 작동하는지 로그아웃하고 다시 로그인하여 테스트하세요.

## 새 ID 공급자 추가

새로운 IdP를 추가하는 절차는 기존의 [SSO(통합로그인) 구성](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)과 유사하지만, 몇 가지 주요 변경 사항이 포함되어 있습니다:

- **새로운 항목:** 'IdP 이름'과 'IdP 설명'(선택 사항)입니다. 이러한 항목은 사용자가 SSO를 통해 여러 IdP를 사용할 경우, 올바른 IdP를 로그인 시 확인할 수 있도록 돕습니다.

  이 항목들은 관리자 설정에 표시되며, 사용자가 SSO로 로그인할 때 보여질 수 있기 때문에, 꼭 필요한 의도로 이름을 설정할 것을 권장합니다(예를 들어, 비즈니스 유닛이나 IdP 이름 등).

  ![idP-name-and-IdP description.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016020733970_idP-name-and-IdP%20description.png)
*IdP 이름 및 IdP 설명 추가 옵션*
- **읽기 전용 필드:** 'Callback URL' (허용 Callback URL, Assertion Consumer Service URL, Reply URL) 및 'Entity ID' (식별자, Relying Party Trust 식별자)는 이제 조직에서 multi-IdP 비공개 기능이 활성화되면 Miro IdP 설정에서 자동으로 생성됩니다.

  기존에는 이 값들이 모든 IdP 구성에 동일하여 고정되어 있었습니다. 생성된 후에는 IdP 공급자의 설정 내 해당 필드에 이 값을 복사하여 붙여넣어야 합니다.

  ![Callback-ID-and-Entity-ID-fields.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034166290_Callback-ID-and-Entity-ID-fields.png)
*Callback URL 및 Entity ID 필드*

## 다수의 ID 공급자(IdP) 관리하기

> **💡** 한 번에 최대 20개의 ID 공급자를 추가하고 활성화할 수 있습니다.

ID 공급자를 추가한 후, 각각의 설정을 필요에 따라 켜거나 끌 수 있습니다. IdP를 끄려면, **회사** 설정 > **계정** > **인증**에서 IdP를 비활성화하면 됩니다.

![Toggle-on-or-off-IdPs.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034165010_Toggle-on-or-off-IdPs.png)
*IdP를 켜거나 끄는 옵션*

## 여러 IdP가 있는 이메일 도메인의 로그인 보기

사용자의 이메일 도메인이 여러 IdP 구성과 연결된 경우, 로그인 시 하나를 선택할 수 있습니다. 이러한 구성이 별도의 도메인을 가지고 있다면, 사용자는 자동으로 관련 IdP로 라우팅됩니다.

![sso-screenshot.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/22437449166610_sso-screenshot.png)
*로그인 시 여러 IdP의 보기*
