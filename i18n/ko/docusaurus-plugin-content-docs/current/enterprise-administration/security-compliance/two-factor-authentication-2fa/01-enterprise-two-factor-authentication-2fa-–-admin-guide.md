---
title: Enterprise 2단계 인증 (2FA) – 관리자 가이드
article_id: 7935391125394
translation_id: 7935391125394
locale: ko-kr
sidebar_position: 1
created_at: '2022-10-04T08:57:18Z'
updated_at: '2026-01-13T13:35:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '해당 대상: Enterprise 플랜 설정자: 회사 관리자'
---

## 조직을 위한 이중 인증 (2FA)

2단계 인증(2FA)은 사용자 이름과 비밀번호 외에 온라인 프로필에 추가적인 보안 층을 추가합니다. Enterprise 회사 관리자는 사용자가 조직의 Miro 구독에 액세스할 때 추가적인 신원 증명을 필수로 요구할 수 있습니다. 이 요구사항은 이메일 주소와 비밀번호를 사용한 모든 로그인에 적용됩니다.

SSO를 사용하는 회사의 경우, 2FA는 비-SSO 외부 공동 작업자에게만 적용됩니다. SSO를 사용하지 않는 회사의 경우, 2FA는 모든 사용자에게 적용됩니다.

:::note
이 글은 Enterprise 플랜을 위한 2단계 인증(2FA)에 대해 설명합니다. 다른 플랜에 대한 내용은 [관리에서 이중 인증(2FA)](../../../administration/security-compliance/01-two-factor-authentication-2fa.md)을 참조하세요.
:::

## 조직에 2단계 인증 강제 설정하기

:::note
2단계 인증(2FA)를 활성화하기 전에 조직 내 모든 사용자와 외부 공동 작업자를 포함한 영향을 받는 모든 사용자에게 알리는 것이 중요합니다. 원활한 전환을 위해, 이 과정을 돕기 위해 제공된 [2FA 사용자 가이드](../../security-integrations/two-factor-authentication-2fa/02-enterprise-two-factor-authentication-2fa-–-user-guide.md)를 공유할 것을 권장합니다.
:::

## 사용자를 위한 2FA 활성화 방법

1. 관리자 콘솔 > **보안** > **인증**으로 이동합니다.
2. **SSO가 아닌 사용자에게 2FA 시행**을 활성화합니다.

![2FA-enable.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24790277317394_2FA-enable.png)*SSO가 아닌 사용자에게 2FA 인증 시행*

### 2FA 기기 신뢰하기

활성화되면, 2FA 사용자에게 기기에서 다음 X일 동안 매 로그인 시 2FA를 건너뛸 수 있는 체크박스가 표시됩니다. 여기서 "X"는 관리자가 설정한 기간입니다. 사용자 기기를 7일에서 90일까지 신뢰할 수 있습니다. 기본값으로는 2FA 기기 신뢰가 활성화되어 있습니다. 그러나 관리자는 관리자 콘솔에서 이 기능을 끌 수 있습니다.

![2FA-trusted-devices.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24790277323410_2FA-trusted-devices.png)

:::warning
2FA 기기 신뢰가 비활성화되면, 사용자들은 매 로그인 시 2FA 코드를 입력해야 합니다. 이 경우 로그인 속도가 느려집니다.
:::

신뢰 기간이 지나면 2FA를 다시 요구합니다.

사용자가 새로운 기기나 브라우저로 로그인하거나 브라우저 쿠키를 삭제하면 2FA는 건너뛰지 않습니다.

## 사용자를 위한 2FA 재설정

사용자가 2FA 방법에 대한 접근을 잃는 경우, 관리자가 사용자의 2FA를 재설정할 수 있습니다. 사용자가 2FA 방법의 재설정을 요청하면, 해당 관리자에게 이메일로 알림이 전달됩니다.

:::note
관리자는 조직 내 사용자의 이메일 도메인이 인증된 경우에만 2단계 인증을 재설정할 수 있습니다. 사용자가 재설정을 요청할 경우, 조직 내의 모든 관리자가 승인할 수 있습니다.
:::

사용자의 2FA 방법을 재설정하는 방법:

- **관리자 콘솔** > **사용자** > **활성 사용자** 탭으로 이동합니다.
- 2FA 방법을 재설정해야 하는 사용자를 찾습니다.
- 사용자 행에서 **세 점 아이콘** (**...**)을 클릭합니다.
  ![reset-2fa.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24650686629138_reset-2fa.png)
  *관리자 콘솔에서 2단계 인증 재설정*
- **이중 인증 재설정**을 클릭합니다.
  확인을 묻는 대화 상자가 열립니다.
- 대화 상자에서 **2FA 재설정** 버튼을 클릭합니다.
- 사용자에게 초기화 지침이 전송되었음을 확인하는 메시지가 화면 상단에 나타납니다.

## 사용자 경험에 미치는 영향

- SSO(통합로그인)를 사용하지 않는 사용자들은 다음 로그인 시 두 번째 인증 수단을 설정하라는 프롬프트가 나타납니다. 이 과정은 진행 중인 세션에서 로그아웃되지 않습니다.
- 사용자들은 모바일 기기와 Microsoft Authenticator, Google Authenticator, Authy와 같은 시간 기반 일회용 비밀번호(TOTP) 애플리케이션을 사용하여 2FA 설정이 필요합니다.
- 2FA를 사용하는 사용자에게는 유효한 TOTP 코드를 입력할 수 있는 기회가 3번으로 제한됩니다. 이 한도를 초과하면 인증 프로세스를 다시 시작해야 합니다.
- 2FA 로그인이 모바일과 태블릿 앱에서 가능합니다만, 초기 등록 프로세스는 브라우저 및 데스크톱 애플리케이션에서만 지원됩니다.

## 중요 사항

2FA 강제 적용은 *이메일 및 비밀번호 인증하거나 이메일을 통해 발송된 매직 링크를 사용하는 사용자*에게만 적용됩니다.

- SSO(통합로그인)을 사용하는 외부 공동 작업자에게 2FA가 활성화되지 않습니다.
- Enterprise 조직의 외부 공동 작업자가 이미 자신의 조직에서 SSO를 통해 인증하고 있다면, 해당 사용자는 Miro의 모든 팀과 보드에 SSO를 통해 계속해서 액세스할 수 있습니다.
- 사용자가 Google, Microsoft, Slack과 같은 타사 로그인 통합을 통해 인증할 경우, 해당 로그인 방법을 통해 계속해서 모든 Miro 팀과 보드에 액세스할 수 있습니다. 관리자는 이러한 사용자에게 각각의 로그인 통합에서 2차 인증을 설정하도록 권장할 수 있습니다. 그러나 Miro의 인증 절차에서는 이러한 사용자에게 2차 인증 설정을 요구하지 않습니다.

## 감사 로그

관리자는 아래의 감사 로그 이벤트를 통해 2FA를 설정한 사용자와 2FA 로그인 성공 및 실패를 추적할 수 있습니다.

- `mfa_setup_succeeded` - 사용자가 두 번째 인증 요소를 성공적으로 설정한 경우
- 2FA로 로그인에 성공한 경우 `sign_in_succeeded` 이벤트에 MfaFactorType 속성을 포함하도록 업데이트
- 2FA로 로그인 실패 시(사용자가 시도 횟수를 초과한 경우, 비기술적 실패) `sign_in_failed` 이벤트에 MfaFactorType 속성을 포함하도록 업데이트
