---
title: 사용되지 않음 – OAuth 1.0을 사용해 Jira 카드를 설정 및 끄기
article_id: 360019501754
translation_id: 26579021107602
locale: ko-kr
sidebar_position: 14
created_at: '2025-05-08T15:35:20Z'
updated_at: '2025-11-25T16:03:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '해당 대상: Jira Cloud, Jira Server(온프레미스), Datacenter(LDAP로 보호됨 포함) 설정한 사람:
    Miro 팀 관리자 및 Jira 시스템 관리자로 프로젝트 관리 권한이 있는 경우'
---

> 다음 OAuth1.0 인증 방법은 2025년 7월 31일부터 Miro에서 더 이상 지원되지 않습니다. 생략된 [인증 프로토콜 OAuth1.0](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively.)은 Jira에서 사용되지 않으며 사용하지 않아야 합니다. 이 변경 사항은 보안 모범 사례에 따라 권장되는 OAuth2.0으로의 광범위한 전환의 일부입니다. Miro의 서비스와의 계속적인 지원 및 호환성을 보장하기 위해 사용자에게 OAuth2.0으로 마이그레이션할 것을 권장합니다.

## Jira에서 Miro 구성

:::warning
기술적 이슈가 발생한 경우 [발생 가능한 문제 및 해결 방법](https://help.miro.com/hc/articles/360017572654)에 대한 기사를 참고하세요.
:::

:::tip
아티클 [Jira 카드 자주 묻는 질문](https://help.miro.com/hc/articles/360013463739)과 [Jira 카드 웹훅 설정 방법](https://help.miro.com/hc/articles/360017731113)에서 Jira 카드에 대해 더 알아보세요.
:::

Jira Cloud 설정 Jira Server 및 Jira 데이터 센터

:::note
Jira 버전에 따라 메뉴가 다를 수 있지만, 일반적인 흐름은 동일하다는 점을 유의하세요. 아래 지침은 [Atlassian 지원](https://confluence.atlassian.com/adminjiraserver071/using-applinks-to-link-to-other-applications-802592232.html)에서도 확인할 수 있습니다.
:::

### 1단계 - 애플리케이션 링크

먼저, 애플리케이션 링크를 만들고 구성하세요.

1. **Jira 설정** > **제품** > **통합** > **애플리케이션 링크** > **링크 생성:
   ![mceclip1.png](https://help.miro.com/hc/article_attachments/26578999551506)***이 Jira 인터페이스는 Jira 버전에 따라 다를 수 있습니다.*
2. **직접 애플리케이션 링크**를 선택하고 **애플리케이션 URL** 필드에 `https://miro.com/`을 입력하세요.
   중요: 이 형식으로 URL을 입력해야 합니다. **계속**을 클릭하세요.
   ![mceclip2.png](https://help.miro.com/hc/article_attachments/26579021093650)
    *링크 생성 중*
3. 다음 메뉴에서 **계속하기**를 다시 클릭하세요.
4. **리뷰 링크** 메뉴에서 URL이 여전히 정확히 `https://miro.com/`인지 다시 확인하고 원하는 **애플리케이션 이름**을 입력하세요. 아래로 스크롤하여, 하단에서 **수신 링크 생성** 옵션을 선택합니다. *나머지 필드 건너뛰기*하고 **계속하기**를 클릭하세요.
   ![mceclip3.png](https://help.miro.com/hc/article_attachments/26579021095314)  *애플리케이션 이름 필드만 작성해야 합니다*
5. 여기에서는 Miro의 가치에 대한 필드를 볼 수 있습니다. 값을 얻으려면 Miro에 로그인하세요.
   - 팀 수준 통합을 위해 **[팀 설정](https://help.miro.com/hc/articles/360021841280)** > **앱 및 통합** > **Jira 카드**로 이동하세요.
   - 조직 수준의 통합을 위해 [**회사 설정**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **앱** > **앱 관리** > **Jira 카드** > **설정**으로 이동하세요.
     > 앱 목록에 Jira 카드가 없는 경우, 섹션의 상단으로 스크롤한 다음, **앱 설치**를 클릭하고 Miro 마켓플레이스에서 앱을 설치하세요. 목록에서 Jira 카드를 확인한 후, 클릭해 엽니다.


     플러그인 탭이 열리고 **1단계**를 보게 됩니다. 필요한 값을 얻으려면:

     ![Jira_Cards_values.jpg](https://help.miro.com/hc/article_attachments/26578999557650)*Jira 카드 값*
     값을 복사해 Atlassian **리뷰 링크** 메뉴에 추가하세요.
6. 처리 중 메시지가 잠시 표시됩니다.
   ![mceclip4.png](https://help.miro.com/hc/article_attachments/26578999557778)
    *링크 생성의 마지막 단계*

이로써 Atlassian 측의 단계를 완료했습니다. 링크는 애플리케이션 링크 목록에 표시됩니다.

### 2단계 - 연결

Miro에서 Jira 카드 설정으로 돌아가 두 가지 옵션 중 하나를 선택하세요: 웹훅을 수동으로 생성하거나 자동으로 생성합니다. 수동으로 선택하는 경우, 옵션을 체크 해제하세요. [이 기사](https://help.miro.com/hc/articles/360017731113)에서 더 많은 정보를 확인하세요. 자동 웹훅을 사용하실 것을 강력히 권장합니다. 플러그인에 대한 큰 업데이트가 있을 경우 다시 설정할 필요가 없습니다.

마지막으로 Jira URL을 입력하고 **연결을** 클릭하세요:

![step_2.jpg](https://help.miro.com/hc/article_attachments/26579021099026)*Jira 카드 연결*

Jira URL을 얻으려면 귀하의 Jira 인스턴스의 기본 URL을 복사해주세요. 다음 포맷을 수락합니다:

`https://your-server.example.com/`
[https://your-server.example.com/
https://your-ip-address/](https://your-server.example.com/)[https://your-ip-address/](https://your-server.example.com/)

Jira URL이 승인되지 않는 경우, [이 기사](https://help.miro.com/hc/articles/360017572654)를 참조하세요. Miro가 Jira에 충분한 접근 권한이 있는지도 확인하여 [연결을 설정하세요.](https://help.miro.com/hc/articles/360017572694)

이제 Jira 인스턴스를 Miro 팀에 연결했습니다.

:::warning
Atlassian은 2024년 2월부로 Jira 서버 지원을 중단했지만, Miro는 향후에도 Jira 서버에 대한 Jira 카드 통합을 계속 지원할 예정입니다.
:::

1. `https://your-jira-server/plugins/servlet/applinks/listApplicationLinks`[.](https://your-jira-server/plugins/servlet/applinks/listApplicationLinks)으로 이동합니다 "애플리케이션 링크"가 선택되지 않은 경우 클릭하세요. ![jira_server_create_application_links.png](https://help.miro.com/hc/article_attachments/26578999559314)*Jira 서버 애플리케이션 링크*
2. **링크 만들기**를 클릭하세요. "Atlassian 제품"을 선택하고 **애플리케이션 URL**, "https://miro.com"을 제공합니다. **계속하기**를 클릭하세요. ![jira_server_create_link.png](https://help.miro.com/hc/article_attachments/26578999559954)*애플리케이션 URL 구성*
3. "애플리케이션 연결" 대화 상자로 이동됩니다. **애플리케이션 이름** (즉, Miro Jira 카드)을 추가하고, **애플리케이션 유형**으로 "일반 애플리케이션"을 선택하세요.
   "다음에서 링크를 생성 중"이라는 항목에 Jira 애플리케이션 URL이 표시되고, "이 애플리케이션으로" 항목 아래에 `https://miro.com`이 표시되어야 합니다. **계속**을 클릭하세요.![jira_server_link_applications.jpg](https://help.miro.com/hc/article_attachments/26578999561106)*애플리케이션 세부 사항 링크 구성*
4. 링크 구성이 처리됩니다. 완료되면 Jira Server의 "애플리케이션 링크" 영역에 새 링크가 표시됩니다. ![jira_server_application_links_created.png](https://help.miro.com/hc/article_attachments/26578999562770)*Jira 서버에서 구성한 애플리케이션*
5. 다음으로, 애플리케이션 세부정보를 구성해야 합니다. 애플리케이션 세부 정보를 편집하려면 애플리케이션의 연필 아이콘을 클릭하세요.
6. 구성 대화 상자에서 **인커밍 인증** 옵션을 클릭합니다. **소비자 키, 소비자 이름, 공개 키**, 선택적으로 설명을 입력하세요.
   - 팀 수준의 통합과 관련된 정보는 [**팀 설정**](https://help.miro.com/hc/articles/360021841280) > **앱 및 통합** > **Jira 카드**에서 확인할 수 있습니다.
   - 조직 수준의 통합에 대한 정보는 [**Company settings**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **앱** > **앱 관리** > **Jira 카드** > **설정**에서 확인할 수 있습니다.
     ![jira_server_config_oauth.png](https://help.miro.com/hc/article_attachments/26579021102482)*Jira Server에서 수신 인증 정보 구성*
     ![jira_webhooks_jira_server_config.png](https://help.miro.com/hc/article_attachments/26578999564306)*Miro의 Jira 애플리케이션 링크 세부정보*
7. 수신 인증 옵션의 끝으로 스크롤하여 **저장**을 클릭합니다. 인증 상태가 이제 확인되었으며, 이 Jira Server를 Miro 내에서 Jira 카드와 함께 사용할 수 있습니다. Miro 측에서 "Jira Server"와 "OAuth 1.0"을 반드시 선택하세요.![jira_server_welcome_to_jira.png](https://help.miro.com/hc/article_attachments/26578999565330)

### 사용자 승인

통합이 연결된 후, 각 최종 사용자는 적절한 권한을 설정하기 위해 자신의 개인 Jira 프로필을 연결해야 합니다. 이는 각 사용자의 Miro 쪽 접근이 *Jira 인스턴스의 접근과 정확히 동일하도록* 보장합니다. 최종 사용자가 처음으로 Jira 카드를 가져오거나 편집하려고 할 때, 개별 사용자 신원 정보를 사용하여 Jira에 로그인하라는 메시지가 표시됩니다.

완료 후 사용자는 화이트보드에 카드를 작업으로 추가할 수 있습니다. Jira에서 이루어진 모든 변경 사항은 보드의 Jira 카드에 반영됩니다.

> 만약 사용자가 Jira 신원 정보가 없고 카드가 추가된 보드에 접근할 수 있다면, 카드 제목, 이슈 유형, 우선순위, 담당자, 그리고 Jira 카드에서 표시되도록 설정된 모든 속성을 볼 수 있습니다. 그러나, 작성 허가가 없으면 카드를 확장해서 다른 속성을 보거나 편집할 수 없습니다. 사용자가 Jira 신원 정보를 연결하지 않으면 담당자 아바타가 보이지 않고 카드의 전반적인 모습이 달라질 것입니다.

### 여러 Miro 팀에 대해 하나의 Jira 인스턴스 사용하기

카드를 팀 수준이나 조직 수준에서 설치할 수 있습니다. 팀이 여러 개인 경우 조직 수준의 설정을 활용해 각 팀에 대해 설정 절차를 반복하지 않도록 할 수 있습니다. 기존 애플리케이션 링크는 모든 팀에 사용됩니다.

팀이나 조직을 Jira 인스턴스에 연결하면, 해당 Miro 팀이나 조직을 위한 새로운 웹훅이 Jira 웹훅에 생성됩니다. 웹훅을 만드는 것은 업데이트 요청을 위한 채널을 설정하는 것입니다.

조직 수준의 설정을 지정하면 이미 연결된 팀은 현재 설정을 유지하게 됩니다. 그러나 언제든지 조직 수준의 설정으로 전환할 수 있습니다.

또한, 필요에 따라 팀이 조직 수준의 설정을 재정의하여 다른 Jira 인스턴스에 연결할 수 있습니다.

Enterprise 고객으로 여러 팀 수준의 연결을 기본 조직 수준 연결로 이전하려는 경우 계정 팀에 문의하세요.

:::warning
여러 팀을 개별적으로 연결하려면 각 팀에 대한 웹훅에 고유한 이름을 지정하는 것을 권장합니다. Jira 웹훅 페이지로 이동해 새로 생성된 웹훅을 편집하세요.
:::

여러 Jira 인스턴스를 하나의 Miro 팀에 연결하는 것은 지원되지 않습니다.

## 플러그인 끄기

팀 수준 통합을 위해 **팀 설정** > **앱 및 통합** > **Jira 카드**로 이동하세요. 그런 다음 **팀에서 제거**를 선택하세요.

조직 수준의 통합을 위해 Jira 앱 사용을 제한하려면 **회사 설정** > **앱** > **앱 관리** > **Jira 카드**로 이동하세요. 그런 다음 토글을 끄기 위치로 이동합니다.

:::warning
조직에서 Jira를 끄면 모든 Enterprise 팀의 사용자가 Jira 카드를 사용할 수 없습니다. 앱 관리 및 제한에 대해 더 알아보려면, [앱 관리](https://help.miro.com/hc/articles/4404659741458)를 참조하세요.
:::

**추가 정보:** [Jira 카드 사용 방법](https://help.miro.com/hc/articles/360017572434)을 참조하세요.
