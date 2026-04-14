---
title: "\uB85C\uADF8\uC778\uD560 \uC218 \uC5C6\uC2B5\uB2C8\uB2E4"
article_id: 360020993079
translation_id: 360020993079
locale: ko-kr
sidebar_position: 9
created_at: '2021-04-09T06:31:47Z'
updated_at: '2025-11-25T16:04:24Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Miro 프로필에 로그인하는 데 문제가 있는 경우 이 가이드를 따르세요.

## 이메일 및/또는 비밀번호 문제

이메일/비밀번호가 작동하지 않습니다

다음은 살펴볼 수 있는 두 가지 솔루션입니다

1. 로그인하는 데 사용하는 이메일/비밀번호에 오타가 없는지 다시 확인하세요.
2. 입력한 자격 증명이 올바르면 [비밀번호를 초기화하세요](../../managing-your-profile/05-how-to-change-your-password.md).
3. 이메일이나 비밀번호에 **& " < >** 기호가 포함되어 있으면 [지원팀에 문의하세요.](https://help.miro.com/hc/requests/new?)

:::warning
이메일과 비밀번호를 10번 시도한 후 **프로필이 잠겨** 있습니다. 먼저 [프로필을 잠금 해제](../../tools/troubleshooting/14-profile-lockout.md)한 다음 비밀번호를 초기화해야 할 수 있습니다.
:::

비밀번호를 초기화할 수 없습니다

비밀번호 초기화 이메일을 받지 못하면 세 가지 이유가 있을 수 있습니다:

1. **이메일이 잘못되었습니다**
입력한 이메일에 오타가 없는지 확인하세요. 오타가 있는 경우 재설정 요청을 다시 시도하세요.

2. **이메일이 아직 Miro에 등록되지 않았습니다**
이 경우 비밀번호 초기화 링크가 이메일 주소로 전송되지 않습니다. [가입 페이지](https://miro.com/signup/)에서 새 프로필을 등록하세요. 이메일이 등록되어 있으면 해당 메시지가 표시됩니다.
![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)

3. **이메일 배달 이슈가 있습니다**

- 스팸, 프로모션, 정크, 소셜 및 **업데이트** 폴더를 열고 재설정 요청 이메일이 있는지 확인하세요.</span>
- 방화벽으로 인해 이메일이 받은 편지함에 도달하지 못할 수도 있습니다.

  시스템 관리자에게 *문의해<em> Miro 도메인 및 하위 도메인을 허용 목록에 추가하도록 요청하세요: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) 및 [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/) 및 이메일 전송 시스템의 IPS를 허용 목록에 추가하세요.

  다음은 전용 IP 목록입니다: 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. [이 기사](../../tools/troubleshooting/02-allowlist-miro-mailers.md)에서 허용 목록에 추가해야 하는 발신자에 대한 자세한 정보를 확인하세요.*

비밀번호를 초기화했지만 여전히 로그인할 수 없습니다

여전히 프로필에 액세스할 수 없는 경우:

1. 새 비밀번호를 입력하세요.
2. 브라우저의 비공개(시크릿) 모드로 로그인하거나 다른 브라우저를 사용하세요.

하나의 이메일로 로그인했지만 리디렉션되고 다른 이메일로 로그인된 것을 발견했습니다.

다른 인증 방법을 사용해 로그인하는 경우(Google, Slack, Office 365, Apple ID, Facebook)에 이슈가 발생할 수 있습니다.

![새_로그인_서드파티.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)
*로그인 페이지의 대체 로그인 옵션*

실수로 Google/Office 365/등 이메일 주소를 다른 이메일로 등록된 Miro 프로필에 연결했을 수 있습니다. 이 경우 다음을 시도하세요.

1. 잘못된 이메일 연결을 제거하려면 **프로필 설정** > **통합**으로 이동한 다음 Google/Office 365/등 옆의 **로그아웃**을 클릭하세요.
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Google 로그인으로 연결 제거하기*
2. 로그아웃하고 이메일로 다시 로그인하세요.

:::note
Miro 프로필의 이메일과 일치하는 Google/Office 365/Slack 이메일에 연결을 설정해 이슈를 방지하세요.
:::

## SSO(통합로그인) 로그인이 작동하지 않습니다

기사를 확인하세요: [SSO 로그인 시 발생할 수 있는 문제](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## 로그인 시 무한 로딩

Miro 신원 정보를 입력하고 나서 끝없이 로딩 문제가 발생하는 사용자에게는 다음을 권장합니다:

1. 다른 **브라우저에서** 로그인하세요.
2. 브라우저의 비공개(시크릿 모드) 모드를 사용해 로그인하세요.시크릿 모드/다른 브라우저에서 이슈가 재현되지 않으면 브라우저 캐시를 지우세요.

   Chrome 캐시 지우기

   1. `https://miro.com/`로 이동하여 Chrome의**개발자 도구** 를 엽니다 (**커맨드 + 옵션 + J** *Mac에서는*, **Ctrl + Shift + J** *Windows에서는*).
   2. 탭 **애플리케이션 > 스토리지**을 선택하세요. **사이트 데이터 지우기** 버튼이 파란색으로 표시됩니다.  버튼을 클릭하면 Chrome 브라우저에 저장된 Miro의 모든 데이터가 제거되어 새 작업 세션을 시작할 수 있습니다.
   ![사이트_데이터_삭제.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
   *Chrome에서 사이트 데이터 지우기 옵션*
3. VPN을 사용 중인 경우**VPN**, 켜기/끄기를 켜세요.
4. 회사에서 방화벽이나 Miro를 차단할 수 있는 프록시를 사용하고 있는지 IT 부서에 문의하세요.</span> <span>[이 지침](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)을 따라 **Miro를 허용 목록에 추가**하거나 우회 경로를 제공하세요.
5. 인터넷 연결을 확인하세요. 네트워크 대역폭이 최소 8Mb/s에 도달하지 않으면, **더 빠른 다른 네트워크로** **전환하세요**.
6. 이용 가능하다면 **모바일 핫스팟**에 연결해보세요. 그런 다음 원래 네트워크에 다시 연결하세요.
7. 그래도 도움이 되지 않으면 [요청을 제출하고](https://miro.com/contact/recover/) [브라우저 콘솔 로그를 지원팀에 보내세요](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

## Miro 데스크톱 앱의 로그인 이슈

1. 데스크톱 앱에서 Miro에 액세스할 수 없는 경우 브라우저를 사용해 로그인하세요. 그래도 로그인할 수 없으면 위의 단계를따르세요. 브라우저에서 Miro에 액세스할 수 있는 경우 아래 단계를 따르세요.
2. 애플리케이션 데이터를 초기화하세요.

Windows에서 앱 데이터 초기화하기

아래 스크린샷과 같이 **Alt > 도움말**을 눌러 애플리케이션 데이터를 초기화하도록 선택하세요.

​![Windows에서 앱 데이터 초기화.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725434514_reset%20app%20data%20on%20Windows.jpg)
*Windows용 데스크톱 앱에서 앱 데이터 초기화하기*

메뉴를 찾을 수 없다면 MS Store에서 다운로드한 앱을 사용하고 있을 가능성이 높습니다. 이 경우 앱 데이터를 초기화하려면 Windows **설정**> **앱**> **앱 및 기능**> 목록에서 **Miro**를 찾은 후 **고급 옵션**> **초기화**를 선택하세요.

이렇게 해도 즉시 도움이 되지 않으면  **C:\Users\username\AppData\Roaming\RealtimeBoard**  및  **C:\Users\username\AppData\Local\RealtimeBoard**에서 모든 앱 파일을 삭제하세요.

> **✏️** 만약  **Appdata**  폴더가 숨겨져 있는 경우,  [여기](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) 를 클릭하여 표시 방법을 확인하세요.

Mac에서 앱 데이터 초기화하기

상단 메뉴에서 Miro를 클릭하고 아래 스크린샷과 같이 **애플리케이션 데이터 초기화**를 선택하세요.

![Mac에서 앱 데이터 초기화.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
*Mac에서 앱 데이터 초기화하기*

그런 다음 앱에 다시 로그인하여 이슈가 해결되었는지 확인하세요.

재설정해도 즉시 효과가 없으면 Finder 창을 열고 **커맨드 + Shift + G** 를 누른 다음 **~/Library/Application Support/RealtimeBoard**를 붙여넣고 모든 앱 파일을 삭제하세요.

3. 문제가 지속되면 웹사이트에서 다운로드한 최신 버전의 앱을 사용하고 있는지 [확인하세요.](https://miro.com/apps/)

## Google/Office 365/Slack/등 로그인

Google/Office/Slack/등을 통해 로그인할 수 없습니다.

1. 표준 신원 정보(이메일 및 비밀번호)를 사용해 Miro에 로그인하세요. 비밀번호를 기억하지 못하거나 비밀번호가 없을 경우, [비밀번호를 초기화하세요](../../managing-your-profile/05-how-to-change-your-password.md).
2. 프로필 설정으로 **이동한 다음** > **통합**에서 Google/Office 365/등 옆의 **로그아웃을** 클릭하고 연결을 다시 구성하세요.</span>
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Google 로그인으로 연결 제거하기*

데스크톱 앱에서 Google/Office/Slack/등을 통해 로그인할 수 없습니다

살펴보세요 이러한 문제 해결 단계를.

Google/Office 365/등을 통해 Miro에 로그인했지만 이메일 서비스가 변경되었습니다. 지금 로그인하려면 어떻게 해야 하나요?

새 서비스 신원 정보(이메일 및 비밀번호)를 사용해 Miro에 로그인하세요. 비밀번호를 기억하지 못하거나 비밀번호가 없으시면 [비밀번호를 재설정하세요](../../managing-your-profile/05-how-to-change-your-password.md).

## 태블릿/모바일의 로그인 문제

1. 브라우저 버전에 로그인할 수 있는지 확인하세요. 그렇지 않으면 이러한 문제 해결 단계를사용하는 것이 좋습니다.
2. 브라우저에서 로그인이 잘 작동한다면, 장치의 인증 데이터가 손상된 경우일 수 있습니다. <span>**앱 설정 > 스토리지 > 스토리지 지우기**로 이동하거나 장치에 Miro 앱을 다시 설치하세요.

## 문제 해결 팁

위에서 솔루션을 찾을 수 없는 경우 **다른 브라우저**나 **시크릿 모드**를 사용해 Miro에 로그인하세요. 브라우저의 시크릿 모드에서 모든 것이 정상이라면 브라우저의 캐시와 쿠키를 지우고 표준 모드로 Miro에 로그인하세요.

Chrome 캐시 지우기

1.</span> `https://miro.com/`로 이동하여 Chrome의 **개발자 도구**(**커맨드 + 옵션 + J** *Mac에서*, **Ctrl + Shift + J***Windows에서*)를 여세요.
2. 탭을 선택하세요 **애플리케이션 > 스토리지**. 파란색 버튼이 표시됩니다 **사이트 데이터 지우기.**​  버튼을 클릭해 Chrome 브라우저에 저장된 Miro 데이터가 제거되므로 새 작업 세션을 시작할 수 있습니다.

![사이트_데이터_삭제.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
*Chrome에서 사이트 데이터 지우기 옵션*

그래도 도움이 되지 않으면, [Miro 지원에 문의하세요](https://miro.com/contact/recover/). 이슈를 자세히 설명하세요.

:::note
Miro에 등록하는 데 문제가 있으면 [확인 코드로 문제](../../tools/troubleshooting/12-issues-with-confirmation-code-or-password-reset-emails.md)를 확인하세요.
:::
