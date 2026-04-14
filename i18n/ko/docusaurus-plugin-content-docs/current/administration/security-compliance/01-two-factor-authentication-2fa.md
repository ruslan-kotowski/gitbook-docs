---
title: 이중 인증(2FA)
article_id: 27356474050834
translation_id: 27356474050834
locale: ko-kr
sidebar_position: 1
created_at: '2025-06-12T12:01:03Z'
updated_at: '2025-06-24T08:19:34Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  notes: '실행 가능한 사용자: 팀 관리자, 회사 관리자 어떤 플랜: Starter, Business, Education, Enterprise
    어떤 플랫폼: 브라우저, 데스크톱, 모바일'
---

이중 인증(2FA)은 사용자 계정에 접근하기 전에 두 가지 고유한 인증 방법을 요구하여 온라인 계정의 보안을 한층 강화합니다.

Miro 관리자는 팀에 대해 2FA를 활성화할 수 있으며, 팀 멤버의 2FA를 재설정할 수 있습니다. 사용자는 30일 동안 기기를 신뢰할 수 있는 옵션이 있습니다.

:::note
이 문서는 Starter, Business, Education 플랜의 2FA에 대해 설명합니다. [이중 인증(2FA) (관리자 가이드)](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)에 대해 알아보세요.
:::

## 이중 인증(2FA) 활성화

Starter 및 Education 플랜의 경우, 팀 관리자 역할을 갖고 있는지 확인하세요.

Business 플랜의 경우 회사 관리자 역할이 있는지 확인하세요.

이 단계를 따르세요:

1. Miro 대시보드에서 오른쪽 상단의 아바타를 클릭하고 **관리자 콘솔**을 선택하세요.
2. (Starter) **보안** > **권한**으로 이동하세요.
   **권한**으로 이동하세요.
   **Security** > **Authentication**으로 이동합니다.
3. **이중 인증(2FA)**에서 **로그인 시 이중 인증을 요구합니다**를 켜기로 전환하세요.

## 사용자를 위한 이중 인증(2FA) 설정

2FA가 활성화된 팀에서는 사용자가 이메일과 비밀번호에 추가하여 인증 앱을 사용해 인증해야 합니다.

[이중 인증(2FA) 사용자 가이드](02-two-factor-authentication-2fa-–-user-guide.md)에서 2FA 설정 방법을 알아보세요.

## 신뢰할 수 있는 디바이스

2FA로 Miro에 로그인하는 사용자는 기기를 신뢰하도록 선택할 수 있습니다.

신뢰할 수 있는 기기를 사용해 로그인할 때 사용자는 첫 번째 인증 요소로만 인증하라는 메시지를 받게 되며, 신뢰할 수 있는 기기이기 때문에 두 번째 인증 요소는 생략됩니다.

![](../../../../../../docs/administration/security-compliance/images/27358547112978_image.png)

*기본적으로 신뢰할 수 있는 기기는 2FA가 활성화됩니다.*

로그인 시 **이 기기를 30일 동안 신뢰**가 기본으로 선택되며, 사용자가 선택 해제할 수 있습니다.

:::note
신뢰 기기 기간은 Enterprise 플랜에서만 수정할 수 있습니다. 자세한 내용은 [이중 인증(2FA) 관리자 가이드](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)를 참조하세요.
:::

신뢰하지 않을 기기를 실수로 신뢰한 경우, 사용자는 모든 곳에서 로그아웃할 수 있습니다. **프로필**로 이동한 후 **프로필 설정**에서 **모든 곳에서 로그아웃**을 클릭하세요.

## 이중 인증(2FA) 재설정

사용자가 이중 인증 수단에 접근할 수 없게 된 경우, 관리자가 2FA를 초기화하도록 요청할 수 있습니다.

Starter 및 Education 플랜의 사용자의 2FA를 재설정하려면 팀 관리자 역할을 가지고 있어야 합니다.

사용자의 2FA를 재설정하려면 Business 플랜에서 회사 관리자 역할을 갖고 있는지 확인하세요.

다음 단계를 따르세요:

1. Miro 대시보드에서 오른쪽 상단의 아바타를 클릭하고 **관리자 콘솔**을 선택하세요.
2. **사용자**> **모든 사용자**로 이동합니다.
3. 사용자를 찾은 다음, 행 끝에 있는 **세 점 아이콘**을 선택하세요.
4. **이중 인증 재설정**를 클릭합니다.
   사용자가 이메일로 재설정 지침을 받습니다.
