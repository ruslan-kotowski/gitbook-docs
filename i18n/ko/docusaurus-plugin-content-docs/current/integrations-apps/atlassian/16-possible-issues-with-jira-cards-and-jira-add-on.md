---
title: "Jira \uCE74\uB4DC\uC640 Jira \uC560\uB4DC\uC628 \uAD00\uB828 \uAC00\uB2A5\uD55C\
  \ \uC774\uC288"
article_id: 360017572654
translation_id: 26103834946194
locale: ko-kr
sidebar_position: 19
created_at: '2025-04-17T09:51:37Z'
updated_at: '2025-11-27T12:20:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Jira [카드](https://help.miro.com/hc/articles/360017572434) 또는 [Jira 애드온](https://help.miro.com/hc/articles/360017572414-Jira-Add-on)을 설치하거나 사용하는 동안 문제를 겪고 있다면 이 가이드가 도움이 될 수 있습니다.

## Jira 카드에 대한 제안

| **메****시지 / 이슈** | **이슈의 가능한 원인과** **해결 단계** |
| --- | --- |
| **연결** | |
| OAuth 1.0 (Jira 서버 & Data Center)에만 해당됩니다.  **Jira가 연결되지 않았습니다** 오류는 개인 신원 정보를 사용하여 Miro에 연결하려고 할 때 발생합니다.  **Jira 카드를 추가할 수 없음** 팝업은 보드에서 Jira 카드 앱을 사용하려고 할 때 나타납니다.  mceclip0.png | Jira 카드 앱이 설치되어 있지만 Miro 팀이 Jira와 연결되어 있지 않습니다.  다음 설치 가이드를 따르세요: [Jira 카드 설정 및 제거 방법.](https://help.miro.com/hc/articles/360019501754-How-to-set-up-and-to-uninstall-Jira-Cards) 팀 관리자가 아닌 경우 관리자에게 요청하세요. |
| **Jira 요청 ... 실패: 시간 초과 발생 / 알 수 없는 호스트 / 연결 거부됨** | Jira는 인트라넷에서만 접근 가능하며, 잘못된 IP 주소로 Jira 시스템에 통신하고 있습니다.  우리의 [**IP 주소, 도메인 및 하위 도메인**](https://help.miro.com/hc/articles/360017572694-Add-Miro-to-Allowed-Domains)를 허용 목록에 추가해 통합이 필요한 액세스 수준을 제공하세요.   만약 Jira Server 구버전을 사용 중이라면, [다크 기능](https://confluence.atlassian.com/jirakb/how-to-manage-dark-features-in-jira-959286331.html)이 Miro에 대한 액세스를 차단하지 않는지 확인하세요. |
| OAuth 1.0. (Jira 서버 및 데이터 센터)에만 적용됩니다.  **Jira의 애플리케이션 링크가 올바르게 구성되지 않았습니다** | - 링크 또는 웹훅 구성 시 일부 단계를 놓쳤습니다  - Jira 카드용 링크 구성을 하지 않고 [Jira 애드온](https://help.miro.com/hc/articles/360017572414-Jira-add-on)를 설치했습니다.  처음부터 [Jira 카드 통합](https://help.miro.com/hc/articles/360019501754)을 설치해보세요.   웹훅을 수동으로 생성하려 했던 경우 자동으로 생성해보세요. |
| OAuth 1.0에만 적용됩니다. (Jira 서버 및 데이터 센터)  **Jira 인스턴스의 애플리케이션 링크가 올바르게 구성되지 않았거나 토큰이 만료되었습니다. 애플리케이션 링크를 확인하고 통합을 다시 연결하세요.** | - Jira의 애플리케이션 링크가 재구성됨  - 토큰이 만료됨  - 토큰이 취소됨  애플리케이션 링크가 올바르게 구성되어 있는지 확인하고 Miro를 Jira 카드에 다시 **연결**해 보세요.  보안 수준이 높은 Jira를 사용하거나 프록시를 사용하는 경우, 통합에 필요한 액세스 수준을 제공하기 위해 [**우리의 IP 주소, 도메인 및 하위 도메인을 허용**](https://help.miro.com/hc/articles/360017572694-Add-Miro-to-Allowed-Domains) 해야 합니다.   Jira 서버를 사용 중이라면, 오래된 버전에서 Miro의 접근을 차단하는 [Dark Features](https://confluence.atlassian.com/jirakb/how-to-manage-dark-features-in-jira-959286331.html)이 없는지 다시 확인하세요. |
| OAuth 1.0 (Jira 서버 & 데이터 센터)만 해당됩니다.  앱 링크는 URL, Consumer Key, Consumer Name, Public Key 이상의 정보를 요청합니다. | 구성 메뉴의 **응답 인증** 탭을 보고 있습니다.  - **요청 인증**으로 전환합니다. **응답 인증**은 구성할 필요가 없습니다.  - 단계를 건너뛸 수 없다면, *아무* 임시 값을 추가하십시오. 나중에 제거할 수 있습니다: **애플리케이션 링크** 목록 페이지에서 Miro **카드** 링크를 편집하고 임시 값을 제거하십시오. |
| OAuth 1.0에 적용됩니다. (Jira 서버 및 데이터 센터) 에만 해당됩니다.  **Jira URL이 유효하지 않음 /**  **Jira 기본 URL 입력 /**   **잘못된 요청. 디시리얼라이제이션.** | 귀하의 Jira가 사설 네트워크에 있거나 귀사의 방화벽이 외부 네트워크 연결을 차단합니다.  [NAT Gateway IP 주소(및 포트)를 허용 목록에 추가하세요](https://help.miro.com/hc/articles/360017572694-Add-Miro-to-Allowed-Domains).   *nslookup을 사용하여 IP 주소를 조회할 경우, 로드 밸런서의 주소가 반환될 수 있으며 이는 시간이 지나면 변경될 수 있습니다. |
| 프록시를 사용하거나 외부 및 내부 Jira URL이 일치하지 않습니다.  **Jira URL** 필드에 Miro가 접근할 수 있는 주소를 입력하여 리버스 프록시를 설정해 줍니다. 또한 이 [Atlassian 가이드](https://confluence.atlassian.com/jirakb/configure-jira-server-to-run-behind-a-nginx-reverse-proxy-426115340.html)의 단계를 따르십시오. 이를 통해 외부 및 내부 URL이 다른 경우에도 통합을 통해 Jira와 Miro 간에 요청을 성공적으로 전달할 수 있습니다. 또한 [프록시 서버에서 시간 초과 값을 연장하는 것도 고려해 보십시오.](https://help.miro.com/hc/articles/360017572694-Add-Miro-to-Allowed-Domains) 엔드포인트 목록은 여기에서 확인할 수 있습니다:[Jira 카드 자주 묻는 질문](https://help.miro.com/hc/articles/360013463739-Jira-Cards-FAQ) |
| SSL 인증서에 문제가 있습니다 (자체 서명된 인증서는 지원되지 않습니다).  Jira 서버의 활성 SSL 인증서를 확인하세요. [이 도구](https://www.ssllabs.com/ssltest/)가 도움이 될 수 있습니다: Jira URL을 입력하고 연결 확인 결과를 확인하세요. 예를 들어, 인증서는 올바를 수 있습니다(**인증서**가 녹색) 그러나 서버 인증서 체인이 불완전할 경우(**키 교환**이 노란색), 시스템에서 인증서를 업데이트해야 한다는 응답을 받을 수 있습니다. 문제 해결을 위해 [이 사이트](https://whatsmychaincert.com/)를 참조하세요. |
| 당신의 Jira는 SSO(통합로그인) 하에 있습니다(이는 **“수신 인증이 올바르게 구성되지 않았습니다“** 오류를 초래할 수 있습니다).  통합의 연결 요청을 위해 SSO 프로세스가 적용되지 않도록 설정하십시오. 이를 위해, 다음 엔드포인트들은 SSO 프로세스에서 제외되어야 합니다:   ``` GET \{JIRA_URL\}/rest/api/2/serverInfo  (OAuth 1.0) POST \{JIRA_URL\}/plugins/servlet/oauth/request-token  (OAuth 1.0) POST \{JIRA_URL\}/plugins/servlet/oauth/access-token  (OAuth 2.0) POST \{JIRA_URL\}/plugins/servlet/oauth2/* ``` |
| 설치 중 예상치 못한 문제 발생 | Jira 버전 6.4 이하를 사용 중입니다.  이 Jira 오류로 인해 당사 카드가 이들 버전에서 작동하지 않습니다. [이 Jira 오류](https://jira.atlassian.com/browse/JRASERVER-42811)입니다. Jira를 최신 버전으로 업데이트하세요. |
| **앱 인증 실패. 앱을 다시 인증해주세요.** | 1. 순간적인 연결 끊김. **연결**을 다시 클릭합니다.  2. 인증 과정 중 만료된 토큰 전송. 캐시된 데이터를 정리하고, 깨끗한 환경에서 다시 시작하세요. 즉, Jira에서 새 토큰을 생성하도록 합니다. |
| OAuth 1.0에만 적용됩니다. (Jira Server & Data Center)  **Jira 오류: "Webhook 'Miro'을(를) 생성할 수 있는 권한이 없습니다."** | Jira에서 관리자 권한이 없습니다. 통합 설정을 위해 Jira 관리자에게 역할을 관리자 역할로 업그레이드해달라고 요청하십시오. |
| **Jira 요청 실패: 인증된 경로를 찾을 수 없음으로 인해 PKIX 경로 생성 실패** | 서버 인증서에 문제가 있습니다.     **해결책**으로 IT 부서에 연락하여 귀사의 인증서를 확인하도록 **요청**하시길 권장합니다(웹 서버를 다시 로드하고, 인증서가 신뢰할 수 있는 공개 인증서임을 확인하는 등). |
| **Miro를 통해 Jira에 대한 권한 부여 불가. 오류: 예외 (예: io.netty.handler.timeout.ReadTimeoutException)** | 이를 발생시키는 원인은 Jira 인프라 설정에서 HTTP/2 프로토콜 지원이 명시되어 있으나, 이를 사용하려 할 때 데이터 전송이 이루어지지 않는 경우일 수 있습니다. 서버 설정 파일에서 HTTP/2 설정이 올바르게 되어 있는지 확인하세요.  필요 시, 문제 해결 전 까지는 서버 설정에서 HTTP/2 지원을 임시로 끄기하여 하위 호환성을 유지하고 서비스가 중단되지 않도록 하세요. |
| **카드 작업하기** | |
| Jira 카드가 업데이트되지 않습니다 | OAuth 1.0(Jira 서버&데이터 센터)에만 해당됩니다.  수동 웹훅을 사용하고 있습니다.  통합을 끄고 **자동 웹훅**을 사용해 다시 연결하세요. 자동 웹훅이 잘 작동한다면 수동 웹훅이 잘못 구성된 것입니다.  또한, [Jira Cards를 위한 WebHook 설정 방법](https://help.miro.com/hc/articles/360017731113-How-to-Set-Up-WebHook-for-Jira-Cards?source=answerbot)을 참조하세요. |
| OAuth 1.0 및 OAuth 2.0(Jira 서버 & 데이터 센터)에 해당됩니다.  자동 웹훅을 사용하는 경우, 첫 번째 문제 해결 단계로 통합을 다시 연결해 보세요. 이것이 도움이 되지 않으면, Jira 카드가 더 이상 업데이트되지 않는 데에는 몇 가지 이유가 있을 수 있습니다. 예를 들어:  - Miro 보드가 다른 팀으로 이동되었거나 백업을 통해 다운로드된 경우  - Jira 이슈가 Jira 측의 한 프로젝트에서 다른 프로젝트로 이동된 경우  - Jira 이슈가 위치한 프로젝트에 대한 접근 권한이 없는 경우  - (Enterprise 전용) 보드 소유자가 비활성화되었거나 제한된 무료 라이선스를 가진 경우  - (OAuth1.0에만 해당) Jira 카드가 현재 사용하고 있는 것과 같은 Jira 인스턴스에 위치하지 않습니다 . |
| OAuth 1.0 (Jira 서버 및 데이터 센터)에만 적용됩니다.  어떤 변경도 가하지 않았는데 Jira 카드가 업데이트되지 않고 있으며, **Jira의 애플리케이션 링크가 올바르게 구성되지 않았습니다.** | 오류 메시지는 Miro가 연결된 Jira에 요청할 수 없을 때, 인증 오류*로 인해 나타날 수 있습니다. 이는 통합을 설정한 사용자가* *토큰을 철회하거나* *Jira가 발급된 토큰의 수명이 짧게* 설정된 경우, 시간이 지나면서 토큰이 무효화되어 다시 연결하여 새로운 유효 인증 토큰을 받아야 하는 경우에 발생할 수 있습니다. |
| **카드 편집** 옵션이 빈창을 반환합니다. | OAuth 1.0 (Jira 서버 및 데이터 센터)에서만 해당됩니다.  Jira ver. 7.6 이상을 사용합니다.  보안상의 이유로 Atlassian은 콘텐츠가 iFrame에 임베드되는 것을 허용하지 않을 수 있으며, 이는 Jira 카드 편집용 팝업 창에도 영향을 미칠 수 있습니다. [이 지침](https://confluence.atlassian.com/jirakb/security-headers-in-jira-939919914.html)을 차선책으로 사용할 수 있습니다. |
| Jira 카드를 추가할 수 없습니다 | OAuth 1.0. (Jira 서버 및 데이터 센터)에만 적용됩니다.  수동 웹훅을 생성하고 설정 정보를 저장하지 않았습니다.  **Jira URL** 필드가 [Miro 설정](https://help.miro.com/hc/articles/360019501754-How-to-set-up-and-to-uninstall-Jira-Cards#Step_2_-_Connection)에서 작성되어 있는지 확인하세요. 반드시 **연결**을 클릭하세요 |
| **편집** 아이콘이 표시되지 않습니다. | OAuth 1.0.(Jira Server & Data Center)만 해당됩니다.  Jira 서버 버전 7.6 이상을 사용하고 있습니다.  이 버전의 보안 업데이트로 인해 편집 아이콘이 표시되지 않을 수 있습니다. |
| 사용자의 프로필은 해당 Jira 이슈를 편집할 수 없는 권한입니다.  Jira에서 이슈를 열고 편집 모드를 사용할 수 있는지 확인하세요. |
| 메시지가 표시됩니다: *로그인되지 않았으며 선택된 이슈에 대해 게스트로서 수행할 수 있는 권한이 없습니다. 로그인하세요* | 저희 통합 서비스가 쿠키를 사용하는 방식 때문에 Jira에서 이 페이지에서 로그인이 불가능할 수 있습니다.  다른 브라우저 탭에서 Jira에 로그인하세요.  브라우저에서 타사 쿠키가 허용되는지 확인하세요. |
| Jira는 SSO(통합로그인) 상태이며, IdP는 iframe을 통한 인증을 허용하지 않습니다.  Miro 데스크톱 앱에서 작업 중인 경우 [miro.com](https://miro.com/app/)에서 Miro 브라우저 버전으로 전환하는 것을 권장합니다. |
| Miro에서 특정 프로젝트를 선택할 때 Jira 카드를 변환/생성할 옵션 없음:  - 이슈 유형 필드에 데이터가 없음  - 변환/생성 버튼이 활성화되지 않음  mceclip0.png | Jira에서 프로젝트에 대한 액세스 권한이 없습니다. 액세스 권한을 부여받을 수 있는지 확인하세요. |
| **Jira 이슈를 생성할 수 없음** Jira 카드를 변환/생성하려고 할 때:   mceclip3.png | Jira 이슈를 생성할 권한이 없습니다.  Jira 관리자에게 연락하여 Jira 측에서 필요한 권한을 부여받으세요. 이렇게 보여야 합니다:  mceclip2.png |
| 일부 사용자 지정 필드가 **Jira 이슈로 변환/편집** 메뉴에 표시되지 않습니다  **Jira 이슈를 만들 수 없습니다. 필요한 필드(...) 지원되지 않음**Miro 내에서 Jira 이슈를 만들 때 오류 발생 | 필드는 보드 Jira 카드 선택기에서 활성화되지 않았습니다.  이 가이드를 따라 [우리의 앱 내](https://help.miro.com/hc/articles/360017572434#attributes) Jira 선택기를 사용하여 맞춤형 필드를 설정하세요. |
| **카드에 표시할 필드 선택**에 Jira의 사용자 지정 필드가 표시되지 않는 경우, Jira 인스턴스의 프로젝트에 대해 구성된 일부 [화면](https://confluence.atlassian.com/adminjiracloud/defining-a-screen-776636475.html)이 필드를 Miro로부터 차단할 수 있습니다.  *프로젝트 설정 > 화면 > 기본 화면 스킴*으로 이동하여 필요한 필드가 허용되어 있는지 확인하세요. |
| Miro는 복잡한 데이터 유형 필드를 지원하지 않습니다.  Miro는 기본 사용자 지정 필드는 지원하지만 복잡한 필드는 지원하지 않습니다. [Jira 카드 필드 구성](https://help.miro.com/hc/articles/360017572434#attributes)을 수행하고, 지원되지 않는 필드는 제거하세요. |
| **보고자**를 선택할 수 없습니다. Jira 카드를 편집하거나 생성할 때 | Jira의 **생성** 메타데이터에 **보고자** 필드가 없습니다: 선택된 프로젝트의 Jira **생성**[화면](https://confluence.atlassian.com/adminjiracloud/defining-a-screen-776636475.html)에 이 필드가 없습니다.  *프로젝트 설정 > 스크린*으로 이동하여 **생성** 화면에 **보고자** 필드가 존재하는지 확인하세요. |
| 선택한 프로젝트의 이슈에 리포터를 설정할 수 있는 필요한 권한이 없습니다.  Jira 관리자에게 자신의 액세스 수준을 확인받고, 선택한 프로젝트에서 리포터 필드를 설정/변경할 수 있도록 권한이 부여되어 있는지 확인하도록 요청하세요. 이렇게 하려면, 관리자에게 Jira에 로그인 > *설정* > *이슈* > *권한 스키마* 로 이동하여 **리포터 수정** 필드를 확인하도록 하세요 (목록에 **응용 프로그램 액세스**: **로그인한 사용자 전원**을 추가해 주세요): mceclip0.png |
| 감사 추적을 위해 보고자 필드는 편집할 수 없으며, 이슈를 생성한 사람으로 설정됩니다.  필드를 사용할 수 없는 것은 예상된 동작입니다. |
| 일부 필드는 **편집 모드**로 카드에서 표시되지만, 보드의 Jira 카드에는 나타나지 않습니다. | Miro는 Jira에서 업데이트를 받지 않습니다.   - 다른 네트워크로 전환하세요 - 통합을 다시 연결하세요 |
| OAuth 1.0에만 해당합니다. (Jira 서버 및 데이터 센터)  **Jira를 사용할 수 없음** 오류가 Jira 카드 앱 설정에 표시됨  mceclip0.png | 1. 팀 관리자에게 통합을 끄고 다시 연결하도록 요청하세요.  2. 귀하의 Jira는 방화벽, 보안 방해 요소 등으로 보호되어 있어 Miro에서 접근할 수 없습니다.  Miro와 Jira 간에 Jira 카드가 동기화되면, 귀하의 Jira가 웹훅을 전송할 수 있다는 의미입니다. 그래서 보드에서 업데이트를 볼 수 있는 것입니다.  해결책으로, IT 부서와 문제를 논의하고 Miro가 [정상적으로 허용](https://help.miro.com/hc/articles/360017572694)되었는지 재확인하도록 요청하세요.   Jira 서버를 사용 중이며 구버전일 경우, [다크 기능](https://confluence.atlassian.com/jirakb/how-to-manage-dark-features-in-jira-959286331.html)이 Miro에 대한 접근을 차단하지 않는지 확인하세요. |
| OAuth 1.0에 적용됩니다. (Jira 서버 및 데이터 센터) 전용.  **Jira 웹훅 문제** Jira 카드 앱 설정 내 오류 | - Jira 측에서 웹훅을 변경/삭제했습니다  - Miro가 Jira로부터 '잘못된 요청' 응답을 받았습니다    해결책으로, 통합을 끄고 [다시 연결](https://help.miro.com/hc/articles/360019501754-How-to-set-up-and-to-uninstall-Jira-Cards)할 것을 제안합니다. |
| **Ctrl + V** (*Windows*) 또는 **Cmd + V** (*Mac*)를 사용하여 Jira 이슈 링크를 보드에 붙여넣을 때, 이것이 Jira 카드로 변환되지 않고 URL로 붙여넣어집니다 | 보드가 아직 로딩 중입니다. 큰 이미지나 PDF 문서가 있는 보드에서 발생할 수 있습니다.   보드를 연 후 최소 10초 동안 기다려 보드가 완전히 로드되게 하세요. 그런 다음 링크를 다시 붙여넣어 보세요. |
| 보드의 Jira 카드에 설명이 보이지 않습니다 | 카드 세부 정보를 보려면 카드를 클릭하고 **확장**을 선택하여 보드의 사이드바에서 카드 세부 정보를 확인하세요. |
| 사용 가능한 스프린트를 검색할 때 "0개의 일치하는 스프린트 표시" | 1. 모든 스프린트가 종료되었거나 완료된 경우 발생합니다.   2. Jira에서 사용 중인 필터가 프로젝트를 포함하고 있지 않습니다. 보드 필터에 필요한 프로젝트를 JQL에 추가하세요. 그러면 스프린트가 Jira와 Miro 둘 다에서 나타납니다. |
| OAuth 1.0. (Jira Server & Data Center)에서만 적용 가능합니다.  SSL 연결이 실패했습니다... | 이 오류는 Miro가 귀하의 Jira에 접근할 수 없음을 의미합니다.  Miro 팀 관리자에게 문의하여 Jira 카드 설정의 **Jira 기본 URL** 필드에 연결 가능한 주소가 포함되어 있는지 확인하도록 요청하세요. |
| Miro의 Jira 카드에서 "담당자" 필드에 사용자가 표시되지 않음 | Jira에서 전역 수준의 "사용자 열람" 권한이 설정되어 있는지 확인하세요. [전역 권한 관리 방법](https://confluence.atlassian.com/adminjiraserver072/managing-global-permissions-828787760.html)에 대해 자세히 알아보세요. |

## Jira 애드온 제안

| **메시지 / 이슈** | **가능한 원인 및 문제 해결 단계** |
| --- | --- |
| **게스트로서 선택한 이슈에 대한 작업을 수행하기 위한 권한이 없으며 로그인되어 있지 않습니다. 로그인하세요** | 저희 플러그인이 쿠키를 사용하기 때문에 아쉽게도 이 페이지에서 Jira 로그인을 할 수 없습니다.  다른 브라우저 탭에서 Jira에 로그인하세요. |
| 애드온 페이지에서 **설치** 버튼을 클릭한 후 다음 오류가 발생할 수 있습니다:  hiccup.png | 순간적인 연결 끊김.  이 경우 잠시 후 다시 설치를 시도하세요. |
| Jira 플러그인 구성 중 또는 완료 후, 어떤 단계에서 다음 페이지로 진행할 수 없습니다. | 쿠키나 캐시 문제로 인해 프로세스가 중단됩니다.  브라우저에서 *atlassian.com* 도메인의 메모리를 지우고 다시 시도하세요. |
| 설치에 성공한 후, Miro에 *등록되지 않은* Jira 사용자들은 첨부된 보드 대신 Miro 로그인 메뉴를 보게 됩니다. | Jira 정책이 일부 플러그인 기능을 차단합니다.  안타깝게도, 이 문제는 최근 Jira API 업데이트로 인해 발생하였으며 현재로서는 수정이 불가능합니다. |
| 애드온이 인증 정보를 기억하지 못하고 매번 로그인을 요구합니다.  Jira 이슈에 보드를 추가하려고 할 때, 보드 선택기에 "죄송합니다, 통합이 사용할 수 없습니다"라는 오류가 표시됩니다. | 브라우저에서 타사 쿠키가 차단되었습니다.  해결책으로, 브라우저에서 쿠키를 활성화하는 방법에 대한 [설명서](https://uca.edu/it/knowledgebase/allowing-third-party-cookies/#Chrome)를 따르십시오. 이는 주로 최신 보안 정책으로 인해 Mozilla와 Safari에서 발생합니다. Safari의 경우, [이 솔루션](https://support.apple.com/en-ke/guide/safari/sfri40732/12.0/mac/10.14)도 도움이 될 수 있습니다. |
