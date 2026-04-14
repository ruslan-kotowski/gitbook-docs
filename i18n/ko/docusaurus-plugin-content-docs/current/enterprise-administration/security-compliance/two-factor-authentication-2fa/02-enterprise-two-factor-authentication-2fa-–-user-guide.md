---
title: Enterprise 이중 인증(2FA) – 사용자 가이드
article_id: 7935469290002
translation_id: 7935469290002
locale: ko-kr
sidebar_position: 2
created_at: '2022-10-04T09:00:42Z'
updated_at: '2025-11-06T13:50:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '쉽게 연관 지을 수 있는 대상: Starter, Business, Education, Enterprise'
---

## 이중 인증(2FA)이란?

이중 인증(2FA)은 온라인 계정에 더 많은 보안을 추가합니다. 회사의 관리자가 이중 인증(2FA)을 활성화하면, 이메일과 비밀번호를 사용한 Miro 로그인 시 추가적인 보안 단계가 뒤따르게 됩니다. 이 추가 단계는 정규 로그인 정보 외에 추가적인 검증이 필요하여 계정을 더욱 안전하게 보호합니다.

:::tip
조직을 위해 [Enterprise 플랜](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md) 및 [다른 모든 플랜](../../../administration/security-compliance/01-two-factor-authentication-2fa.md)에서 이중 인증(2FA)을 활성화하는 방법을 알아보세요.
:::

## 이중 인증(2FA) 설정 방법

**신규 사용자:** 회사 이메일 주소로 초기 [가입](https://miro.com/signup/) 과정에서 2FA를 활성화 하도록 안내받습니다.
 **기존 사용자:** 다음 번 [로그인](https://miro.com/login/) 시, 조직에서 2FA가 요구되며 SSO(통합로그인)를 사용하지 않는 경우 2FA 설정을 하도록 안내받습니다.

1. 모바일 기기에 인증 앱을 다운로드하세요. Google Authenticator, Microsoft Authenticator, Authy와 같은 인증 앱은 Miro에 안전하게 로그인할 수 있도록 시간 기반 일회용(TOTP) 코드를 생성합니다. 어느 인증 앱을 선택해야 할지 모르겠다면, 회사 관리자나 IT 관리자에게 문의하세요.

2. Miro 2FA 설정 화면에서 **인증 앱을 가지고 있습니다** 를 클릭하세요.

   ![2FA-setup-step-1-Confirmation-of-authenticator-app-download.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653633554_2FA-setup-step-1-Confirmation-of-authenticator-app-download.png)
   *인증 앱 확인*
3. 인증자 앱을 사용하여 두 가지 옵션이 있습니다:


   QR 코드 스캔하기

   1. 인증자 앱을 엽니다.
   2. 앱을 사용하여 QR 코드를 스캔합니다.
   3. 스캔 후, Miro에서 **코드를 스캔했습니다**를 클릭하세요.

      ![2FA-setup-step-2-Scan-QR-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683263122_2FA-setup-step-2-Scan-QR-code.png)*QR 코드 스캔*

   Miro 코드 수동 입력하기

   1. QR 코드를 스캔할 수 없는 경우, Miro에서 **QR 코드 스캔이 안 되나요?**를 클릭하세요.
   2. 그 후, Miro가 인증 코드를 제공합니다. 이 코드를 **복사**하세요.
   3. 인증 앱을 열고 복사한 코드를 붙여넣으세요.
   4. 앱에 코드를 추가한 후, Miro에서 **코드를 추가했습니다**를 클릭하세요.

      ![2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653636754_2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png)*인증 앱에 붙여넣기 위해 Miro 코드를 복사하는 과정*
4. 인증 앱에서 생성된 6자리 확인 코드를 Miro에 입력하고 **코드 확인**을 클릭하세요.

   ![2FA-setup-step-3-enter-6-digit-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653634706_2FA-setup-step-3-enter-6-digit-code.png)
   *6자리 코드 확인*
5. 6자리 코드를 통해 계정을 성공적으로 인증한 후, Miro에서 제공하는 복구 코드를 받게 됩니다. 이 코드를 안전하게 저장하려면 **복사**를 클릭하세요. 이 코드는 인증 앱에 접근하지 못하게 된 경우 2FA를 재설정할 수 있도록 해주기 때문에 매우 중요합니다.

   코드를 기록했음을 확인하려면 **코드를 기록했습니다**, 그런 다음 **계속하기**를 클릭하여 프로세스를 완료하세요.

   ![Save-2FA-recovery-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683265554_Save-2FA-recovery-code.png)*복구 코드 저장하기*

## 2단계 인증(2FA)을 사용하여 로그인

계정에 대해 2FA를 성공적으로 설정한 후에는 로그인 시마다 Miro에서 6자리 시간 기반 일회용 코드(TOTP 코드)를 입력하라는 요청을 받게 됩니다.

이 코드는 인증 앱에서 생성되며 계정의 보안 레벨을 한층 더 높여 줍니다. 인증 앱을 열고 현재 코드를 가져와 로그인 페이지에 입력하여 계정에 접근하세요.

![2fa-user-guide.png](https://help.miro.com/hc/article_attachments/30847469065874)
*Miro에 2FA로 로그인하기*

로그인 시도를 3번 할 수 있으며 그 이후에는 로그인 과정을 다시 시작해야 합니다.

![Too-many-attempts.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683267346_Too-many-attempts.png)*2FA로 너무 많은 로그인 시도*

### 이중 인증(2FA) 장치를 신뢰하기

관리자가 설정한 경우, 보안 장치를 사용하여 2FA로 계정에 로그인할 때 **이 장치를 신뢰**할 체크박스를 선택할 수 있습니다 (공유 또는 공용으로 접근 가능한 컴퓨터에서는 **이 장치를 신뢰**하지 마세요). 그러면 지정된 기간 동안 두 번째 요소 없이도 로그인할 수 있습니다. 이 기간은 관리자가 7일에서 90일 사이로 설정합니다.

![2FA-signin.png](https://help.miro.com/hc/article_attachments/30847469068434)

*이중 인증으로 로그인할 때, 장치를 신뢰하는 기간이 체크박스 옆에 표시됩니다.*

"이 장치를 신뢰합니다" 옵션이 보이지 않는 경우, 관리자가 이를 조직에 대해 활성화하지 않았다는 의미입니다.

새 장치로 로그인하거나 신뢰된 장치에서 쿠키를 삭제한 경우, 다시 2FA가 필요합니다.

## 이중 인증(2FA) 재설정 방법

인증 앱 문제를 겪거나 장치를 잃어버리거나 기타 사유로 2FA를 재설정해야 하는 경우, 다음 단계를 따르세요:

### 복구 코드가 있는 경우

1. **이중 인증 재설정**을 클릭하세요.
2. 초기 2FA 설정 시 저장해두었던 복구 코드를 사용하세요. 인증 앱을 다시 구성하기 위해 설정 과정이 시작됩니다.

![Reset-two-factor-authentication.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683268114_Reset-two-factor-authentication.png)*이중 인증 재설정 옵션*

### 복구 코드가 없습니다

복구 코드를 분실하였거나 셀프 복구 절차를 이용할 수 없는 경우, 2FA 재설정을 관리자에게 요청해야 합니다.

이메일 도메인이 조직의 인증된 도메인에 포함되어 있지 않으면, 관리자가 2단계 인증을 초기화할 수 없습니다. 직접 초기화를 요청해야 하며, 이후에 관리자가 이를 승인할 수 있습니다.

관리자는 조직 내에서 자신이 직접 초기화를 시작한 경우에 한해 인증된 이메일 도메인을 가진 사용자에 대해서만 이중 인증을 초기화할 수 있습니다. 사용자가 초기화를 요청한 경우에는, 조직의 모든 관리자가 이를 승인할 수 있습니다.

다음 단계를 따르세요:

1. **관리자에게 초기화를 요청하세요**를 클릭합니다.
   ![2fa-user-reset.png](https://help.miro.com/hc/article_attachments/30847469070354)
   *복구 코드가 없는 경우 관리자에게 2FA 초기화를 요청하세요*
2. 2FA를 사용하는 여러 조직에 속해 있는 경우, 요청할 관리자를 소속된 조직에서 선택해야 합니다.
3. 이메일로 인증 코드가 전송됩니다.
4. 인증 코드를 입력합니다.
5. 요청이 선택한 관리자에게 전송되었다는 확인이 표시됩니다.
6. 관리자가 2FA를 재설정하면, 다음번에 로그인할 때 2FA 설정 과정을 다시 거쳐야 합니다.

## 자주 묻는 질문

2FA 설정이 필요한 이유는 무엇인가요?

이중 인증은 귀하의 조직 보안을 강화합니다.
모든 비SSO 사용자는 2FA 설정이 회사 관리자에 의해 강제되는 경우 로그인 시 2단계 인증을 사용해야 합니다.

로그인할 때마다 2FA를 사용해야 하나요?

네. 최초 설정을 완료한 후에는 계정의 보안을 위해 로그인할 때마다 인증 앱을 사용해야 합니다.

2FA 설정 중 "잘못된 코드" 오류가 발생했는데, 코드가 올바른 경우 어떻게 해야 하나요?

기기의 시간대, 날짜, 시간 설정이 정확한지 확인하세요. 문제가 계속될 경우, 다른 기기에서 2FA를 설정해보세요.

공유 장치를 실수로 신뢰한 경우 어떻게 해야 하나요?

공유 장치를 실수로 신뢰한 경우, 해당 장치에서 Miro의 쿠키를 삭제해야 합니다. 이 작업은 간단합니다:

1. 브라우저 주소창 왼쪽에 있는 슬라이더 아이콘을 클릭합니다.
2. 메뉴에서 "쿠키 및 사이트 데이터"를 클릭합니다.
3. 그런 다음 "기기 내 사이트 데이터 관리"를 클릭합니다.
4. 목록에 나열된 각 URL 옆에 있는 휴지통 아이콘을 클릭하여 쿠키 및 사이트 데이터를 삭제합니다.

장치에서 사이트 데이터를 삭제한 후에는 이중 인증을 사용해 다시 로그인해야 합니다.

신뢰된 기기에 접근할 수 없는 경우 어떻게 해야 하나요?

신뢰된 기간이 만료되기 전에 신뢰된 기기에 접근할 수 없는 경우, **모든 기기에서 로그아웃** 옵션을 사용해 모든 기기에서의 접근을 제거할 수 있습니다 (현재 사용 중인 기기는 제외). 이 옵션을 통해 다른 모든 기기에서 로그아웃 되며, 신뢰된 기기에서도 2FA가 해제됩니다. **모든 기기에서 로그아웃** 링크는 사용자 프로필 설정에서 찾을 수 있습니다. 그 후에는 접근 가능한 기기에서 다시 2FA 로그인 과정을 진행해야 합니다.
