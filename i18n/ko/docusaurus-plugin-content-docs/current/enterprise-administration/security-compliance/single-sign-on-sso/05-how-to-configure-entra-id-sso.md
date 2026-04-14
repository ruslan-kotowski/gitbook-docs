---
title: Entra ID SSO(통합로그인) 구성 방법
article_id: 360022722233
translation_id: 360022722233
locale: ko-kr
sidebar_position: 5
created_at: '2019-05-07T12:03:08Z'
updated_at: '2025-11-25T16:04:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '사용 가능 대상: Business 플랜, Enterprise 플랜 설정 가능한 사용자: 회사 관리자'
---

> *💡 브라우저의 시크릿 모드 창에서 SSO(통합로그인)를 구성하는 것이 강력히 권장됩니다.* 이렇게 하면 표준 창에서 세션을 유지할 수 있으며, 잘못 구성된 경우 SSO(통합로그인) 승인을 해제할 수 있습니다.

SSO(통합로그인)를 프로덕션에 활성화하기 전에 테스트 인스턴스를 설정하려면, [지원팀에 문의](https://help.miro.com/hc/requests/new?referer=help-center-article)해 도움을 받으세요. SSO(통합로그인)를 구성한 사람만 이 테스트 인스턴스에 추가됩니다.

> **⚠️ SSO(통합로그인) 관련 주요 기사** [**여기**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)**에서 규칙, 지원 기능, Miro 측의 선택적 구성을 확인하세요.**

## 앱 추가 및 구성

 1. Entra ID Enterprise 애플리케이션 갤러리에서 Miro 사전 구성 애플리케이션을 찾습니다 ([Enterprise Applications](https://portal.Entra.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/) > +새 애플리케이션).

2. 애플리케이션을 생성하고 **2.**를 클릭하세요. **SSO(통합로그인) 설정** (또는 왼쪽에서 **SSO(통합로그인)**을 선택하고 **SAML** 로그인 방식을 선택하세요).

3. **기본 SAML 설정**이 이미 구성되어 있습니다:

:::warning
모든 설정이 완료된 후 SSO(통합로그인) 로그인이 실패하는 경우, 엔티티 ID를 `https://miro.com`에서 `https://miro.com/`으로 변경해 보세요
:::

:::warning
로그인 URL, Relay State 및 로그아웃 URL(단일 로그아웃의 경우)은 이러한 기능이 지원되지 않으므로 비워 두어야 합니다.
:::

**속성과 클레임**도 이미 설정되어 있습니다:

:::warning
참고:
a) UPN은 Miro에서 사용자를 인식하는 주요 매개변수가 되며, 이 매개변수는 Entra 측에서 업데이트할 수 없습니다. SCIM을 사용하지 않고 Miro에서 사용자 이메일을 업데이트해야 하는 경우, [지원팀에 문의하세요](https://help.miro.com/hc/requests/new?referer=help-center-article).
b) Miro는 [**이름,** **성,** **표시 이름** 및 **프로필 사진**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)을 수락합니다. 다른 속성은 SSO(통합로그인)로 지원되지 않지만, [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)을 통해 전송할 수 있습니다.
:::

### 인증서 작성

1. Microsoft Entra에서 **SAML 서명 인증서** > **서명 옵션**을 **SAML 어설션 서명** 또는 **SAML 응답 및 어설션 서명**으로 설정했는지 확인하세요.

2. **다운로드**  **Base64** 파일.

## Miro 플랜에서 SSO(통합로그인) 구성하기

1. **Base64**로 다운로드한 파일을 텍스트 편집기에서 열고, 파일에서 **x509** 인증서를 복사하세요.

2. Miro에서 **보안 > 인증** 아래에 복사한 **x509** 인증서를 **키 x509 인증서** 상자에 붙여넣으세요.

3. Microsoft Entra 설정 UI에서 **로그인 URL**을 복사한 다음, Miro **보안 > 인증** 페이지로 이동하여 **SAML 로그인 URL** 상자에 붙여넣으세요.

4. Miro **보안 >** **인증** 페이지의 **이 도메인의 사용자는 SSO를 사용해 로그인합니다** 섹션에서 최소한 하나의 회사 도메인을 추가했는지 확인하세요.

:::warning
Miro에서 **IdP에서 프로필 사진 동기화**가 선택 해제되어 있는지 확인하세요. Entra ID는 사용자 프로필 사진 동기화를 지원하지 않습니다. **IdP에서 프로필 사진 동기화**가 선택 해제된 경우, 사용자는 자신의 프로필 사진을 설정할 수 있습니다.
:::

4. **저장**을 클릭하세요.

SSO 구성이 완료되었습니다.

## UPN과 이메일 주소가 다를 때 클레임 구성

Miro에서 **NameID**로 사용할 수 있는 이메일 형식의 어떠한 Entra 속성도 설정할 수 있습니다.

#### **IdP 및 SP 시작 로그인**

*IdP 시작 로그인*의 경우, Entra는 Miro로 사용자가 결정한 값을 **NameID**로 보냅니다 (**user.mail** 아래 예시 참고).

이 플로우로 최종 사용자는 포털 콘솔의 아이콘을 통해 Miro에 액세스합니다 (예: `https://myapplications.microsoft.com/`). 그곳에서 Miro로 요청이 전송되고, *정의한 **NameID**를 사용해 사용자가 로그인됩니다.*Miro는 이 속성이 Miro에서 사용자의 **이메일**과 일치하기를 기대합니다. 일치하지 않을 경우 인증에 실패합니다.

*SP 시작 로그인*의 경우, Miro는 사용자 **UPN**에 대한 요청을 보내며, 이 값이 Miro에서 사용자의 **이메일**과 일치하기를 기대합니다. 일치하지 않으면 인증에 실패합니다.

이제 Miro 설정의 **SAML 로그인 URL** 필드에는 Entra 인스턴스의 Miro 앱 **로그인 URL**이 포함되어야 합니다. 이 URL은 [Miro 로그인 페이지](https://miro.com/sso/login/)에서 사용자를 안내하는 데 사용됩니다.

사용자가 앱에서 로그인 URL로 이동되면, SAML 요청이 생성됩니다. 이 흐름을 통해 사용자는 Miro 로그인 페이지에 입력한 이메일 주소로 로그인이 이뤄지며, Miro는 Entra로부터 요청하여 이것이 UPN 속성인지를 요구합니다.

#### **설정 방법**

사용자가 UPN보다 Entra의 **이메일**을 사용하여 Miro에 액세스할 수 있도록 하려면 Miro의 **SAML 로그인 URL** 필드를 Entra 콘솔에서 가져온 앱의 **URL**로 채우면 됩니다. 그런 다음 SP 시작 흐름은 다음과 같습니다:

1. 사용자는 Miro에 있는 이메일인 Miro 이메일 주소를 입력하여 Miro에 액세스합니다. Miro는 해당 사용자가 정의된 사용자 프로필로 로그인되어야 한다고 이해합니다.
2. 사용자는 IDP 시작 로그인을 위해 사용되는 앱 링크로 이동합니다.
3. 해당 링크는 **NameID** 속성 *당신이 정의한*을 활용하여 Miro로 전송합니다.
4. 따라서 사용자는 정의한 **NameID**로 이전에 정의된 사용자 프로필로 Miro에 로그인됩니다.

Miro에 대해 자동 프로비저닝 기능을 활성화하려면 [이 문서](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)를 확인하세요.

설정 중에 문제가 발생했다면 [이 문서](../../../using-miro/tools/troubleshooting/10-i-can't-log-in-via-sso.md)를 확인하세요.

## Entra 테스트 도구

테스트 도구로 이동하려면 애플리케이션의 설정에서 **싱글 사인인** 탭을 선택하고 섹션 하단까지 스크롤하세요.

Entra는 연결을 확인하고 오류 메시지를 해결하기 위해 테스트 로그인 프로세스를 사용할 것을 제안합니다. 테스트가 완료되면 상황을 해결하는 방법에 대한 지침이 제공됩니다.

Entra/ADFS에서 관리하는 신원 정보로 워크스테이션이 인증되는 것을 유념하세요. Miro에 로그인하려고 다른 신원 정보를 사용하려는 경우, ID 공급자가 기본 신원 정보를 전송하여 불일치가 발생할 수 있으므로 로그인 시도가 실패할 수 있습니다. 예를 들어, 사용자가 SSO 관리자일 경우 다른 사용자 신원 정보로 로그인 절차를 테스트할 때 이런 일이 발생할 수 있습니다.

## 또는 Miro에서 테스트할 수 있습니다

1. 위의 단계를 완료해 SSO 설정을 구성합니다.
2. **SSO 구성 테스트** 버튼을 클릭합니다.
3. 결과를 검토합니다.
   1. 문제가 발견되지 않으면 **SSO 구성 테스트에 성공했습니다**라는 확인 메시지가 표시됩니다.
   2. 문제가 발견되면 **SSO 구성 테스트에 실패했습니다**라는 확인 메시지와 함께 수정해야 할 사항을 안내하는 자세한 오류 메시지가 표시됩니다.

##
