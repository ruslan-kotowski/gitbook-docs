---
title: "Enterprise \uD50C\uB79C\uC5D0\uC11C\uC758 \uC0AC\uC6A9\uC790 \uD504\uB85C\uBE44\
  \uC800\uB2DD"
article_id: 4403139914130
translation_id: 4403139914130
locale: ko-kr
sidebar_position: 13
created_at: '2021-07-01T07:59:23Z'
updated_at: '2025-11-25T16:05:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: scim
---

자동 프로비저닝 기능을 통해 회사 도메인 내 모든 신규 사용자들이 Enterprise 구독에 라우팅되며 회사 자산에 접근할 수 있습니다.

Miro Enterprise는 여러 가지 프로비저닝 옵션을 제공합니다: 초대, Just-in-Time 프로비저닝 (JIT), 범도메인 아이덴티티 관리 시스템 (SCIM), 도메인 제어.

> **사용 가능 대상:** Enterprise 플랜

## 초대

대시보드에서 **멤버 초대** 버튼을 사용해 구독에 사용자를 초대할 수 있습니다. 초대는 즉시 발송되며 추가 설정이 필요하지 않습니다.

Miro에서 작업을 공유하고 공동 작업할 수 있는 방법에 대해 자세히 알아보려면 [Enterprise 플랜의 초대 관리](05-manage-user-invitations-on-enterprise-plan.md) 및 [보드 공유 및 공동 작업자 초대](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)를 방문하세요.

![invite_members_button.jpg](../../../../../../docs/enterprise-administration/user-management/images/21017653284754_invite%20members%20button.jpg)*Miro 대시보드에서 구성원 초대 옵션*

## JIT(Just-In-Time) 프로비저닝

JIT 프로비저닝은 [SSO(통합로그인)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)과 통합되어 있으며, 기업 SSO 도메인에 등록된 모든 신규 사용자를 Enterprise 플랜의 특정 팀에 자동으로 추가합니다.
JIT 프로비저닝은 Miro SSO 설정에서 쉽게 활성화할 수 있습니다. [SSO 설정 방법](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)을 알아보세요.

![user_provisioning_jit_provisioning.png](../../../../../../docs/enterprise-administration/user-management/images/21017682931730_user_provisioning_jit_provisioning.png)*SSO 설정에서 JIT 프로비저닝 활성화*

## 크로스 도메인 ID 관리 시스템(SCIM)

SSO(통합로그인)과 [통합된](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) SCIM은 선택한 ID 공급자를 통해 Enterprise 플랜에서 사용자를 자동으로 프로비저닝하고 관리할 수 있도록 해줍니다.

SCIM이 활성화되면 특정 팀에 사용자를 추가하고, 세부 정보와 이메일을 업데이트하며, 선택한 ID 공급자 내에서 직접 활성화 상태를 관리할 수 있습니다. 이 기능은 Miro 계정과 ID 공급자 간의 사용자 정보 교환을 자동화합니다.

SCIM은 Miro와 ID 공급자 간의 사용자 정보 교환을 자동화하여, ID 공급자로부터 중앙에서 Enterprise 플랜에 대한 직원 접근을 관리할 수 있도록 해줍니다.

[SCIM 기능](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)에 대해 더 알아보고, [Entra ID](../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md), [OKTA](../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md), [OneLogin](../security-integrations/system-for-cross-domain-identity-management-scim/06-setting-up-automated-provisioning-with-onelogin.md) 설정 단계를 검토하세요.

## 도메인 제어

[도메인 제어](../canvas-25-admin-features/domain-control/01-domain-control.md) 를 통해 새 사용자를 Enterprise 구독에 자동으로 추가하고, 기업 사용자가 별도의 Miro 구독을 만들 수 없도록 제한하며, 도메인 내 사용자 활동을 모니터링할 수 있습니다.

도메인 제어를 사용하면, 기업 사용자를 위한 프로비저닝 규칙을 설정할 수 있습니다:

- 도메인 내 새로 등록된 사용자가 구독 권한을 요청할 수 있음
- 도메인 내 새로 등록된 사용자가 자동으로 구독에 가입됨
- 도메인 내 새로 등록된 사용자가 자동으로 구독에 가입되고, 도메인 사용자가 새로운 Miro 팀을 생성할 수 없음

![Add-a-domain-Image1.png](../../../../../../docs/enterprise-administration/user-management/images/21017653288082_Add-a-domain-Image1.png)*Miro 보안 설정의 도메인 제어*

## 라이선스 작동 방식

새 사용자를 초대할 때 회사 관리자는 구독 설정에 따라 초대받은 사람의 라이선스를 선택할 수 있습니다.

관리자가 아닌 사람에 의해 초대되거나 JIT, SCIM 또는 도메인 제어를 통해 귀하의 구독에 자동으로 프로비저닝된 사용자는 *기본 라이선스*가 할당됩니다:

- **비플렉시블 라이선싱(non-FLP) 플랜의 경우:** 기본 라이선스는 풀 라이선스입니다 (조직에 남아 있는 풀 라이선스가 부족하면, 캡처된 사용자에게 [제한된 무료 라이선스](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)가 부여됩니다).
- **플렉시블 라이선싱 프로그램(FLP) 플랜의 경우:** 기본 라이선스는 Free 또는 [제한된 무료 라이선스](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)일 수 있습니다.

:::note
우리의 [Enterprise 라이선싱 모델](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md), [플렉시블 라이선싱 프로그램에서의 라이선스 관리](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md), [요청 관리](09-request-management-on-enterprise-plan.md)를 통한 라이선스 할당 및 업그레이드 관리에 대해 자세히 알아보세요. 및 [소프트웨어 자산 관리](../security-integrations/software-asset-management/01-software-asset-management-miro-enterprise.md)를 통해 라이선스 사용 현황을 추적하는 방법.
:::

## 자주 묻는 질문

도메인 제어를 통해 새로운 사용자를 수집하도록 설정하면, 특정 도메인의 사용자에게 자동으로 Enterprise 구독 내 기본 팀을 배정하여 JIT와 유사하게 작동하나요?

예, 그러나 도메인 제어는 Enterprise 플랜의 SSO(통합 로그인)를 설정하지 않아도 작동할 수 있습니다.

자동으로 프로비저닝된 사용자가 보드 작업을 시작하기 전까지 풀 라이선스를 받지 않도록 할 수 있나요?

네, [플렉시블 라이선싱 프로그램](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md)으로 가능합니다.

Enterprise 구독에 여러 프로비저닝 옵션을 설정할 수 있나요?

네, 여러 프로비저닝 옵션을 동시에 사용할 수 있습니다.
