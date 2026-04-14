---
title: '웹훅 설정 방법: Jira 데이터 센터'
article_id: 360017731113
translation_id: 26964575047570
locale: ko-kr
sidebar_position: 15
created_at: '2025-05-26T12:22:01Z'
updated_at: '2026-01-14T09:25:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '대상: Jira 시스템 관리자 플랜: 모든 Miro 플랜 (Jira 서버/데이터 센터 통합의 경우 OAuth 1.0) 플랫폼: 브라우저,
    데스크톱 앱 (설정 절차용)'
---

Miro 보드의 [Jira 카드](https://help.miro.com/hc/articles/360017572434)가 최신 상태로 유지되도록 하려면, 데이터 변경이 발생할 때마다 Miro가 Jira로부터 메시지를 받아야 합니다. 이러한 Jira 이벤트는 웹훅을 통해 Miro로 전송됩니다.

이 가이드는 OAuth 1.0 및 OAuth2.0을 사용하여 Jira 서버와 Jira 데이터 센터용 웹훅을 생성하는 두 가지 방법을 제공합니다.

## 웹훅을 자동으로 생성하기

[Jira 카드 통합을 설정할 때](https://help.miro.com/hc/articles/360019501754), Jira Server나 Jira Data Center에 연결하는 경우 **웹훅 자동 생성** 옵션을 활성화한 상태로 두세요. 이것이 권장하는 방법입니다.

:::note
웹훅 자동 생성을 위해서는 Jira 시스템 관리자 계정으로 Jira에 로그인해야 합니다.
:::

![jira-webhooks-server-config.png](../../../../../../docs/integrations-apps/atlassian/images/21304245707026_jira-webhooks-server-config.png)
*Jira 카드 설정, 2단계: "웹훅 자동 생성**"**이 활성화됨*

웹훅이 자동으로 생성된 후에는 Jira 웹훅 페이지로 가서 고유 이름을 지정하는 것이 좋습니다. 특히 여러 Miro 팀을 Jira 인스턴스에 연결할 계획이라면 더욱 중요합니다.

:::note
OAuth2.0 연결의 경우, Miro 측의 연결은 회사 차원에서 설정됩니다. 모든 Miro 팀에 대해 하나의 웹훅이 생성됩니다.
:::

:::note
Miro 팀 수준에서 OAuth 1.0 연결의 경우, 팀마다 하나의 웹훅이 생성됩니다. Miro 회사 수준에서는 모든 팀에 대해 하나의 웹훅이 생성됩니다.
:::

## 웹훅을 수동으로 생성하기

웹훅을 수동으로 생성하려고 한다면 다음 단계를 따르세요.

**Miro에서 웹훅 URL 얻기**

1. Miro의 Jira 카드 설정에서 (Jira 서버/데이터 센터와 연결할 때의 2단계), **웹훅 자동 생성** 옵션의 선택을 해제합니다.
2. 조직의 **Jira URL**을 복사하여 붙여넣고 **연결 및 설정 저장**을 클릭합니다.
   ![jira-webhooks-configure-jira-url-cropped.png](../../../../../../docs/integrations-apps/atlassian/images/21304245708818_jira-webhooks-configure-jira-url-cropped.png)
   *Jira 카드 설정, 2단계: "웹훅 자동 생성" 해제*
3. Jira에서 통합 연결을 허용합니다.
4. 이 과정을 완료하면, Miro가 **웹훅 URL**을 제공합니다:
   ![webhook_URL.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016928565010_webhook%20URL.jpg)*Miro에서 제공한 웹훅 URL*

:::note
Jira 시스템 관리자가 아닌 경우, Miro에서 제공한 **웹훅 URL**을 복사하여 Jira 시스템 관리자에게 보내세요. 아래 지침을 사용해 Jira 쪽에서 웹훅을 생성할 수 있도록 하세요.
:::

**Jira에서 웹훅 생성**

아래는 Miro에서 얻은 URL를 사용하여 Jira에서 웹훅을 생성하는 단계입니다. 공식 Atlassian 문서에서 [Jira Server](https://developer.atlassian.com/server/jira/platform/webhooks/) 및 [Jira Cloud](https://developer.atlassian.com/cloud/jira/platform/webhooks/) 가이드를 참조할 수도 있습니다(본 문서는 Server/Data Center에 중점을 두고 있습니다).

1. Jira에서 **웹훅** 페이지로 이동하려면, **Jira 관리** > **시스템** > **고급** > **웹훅**으로 이동합니다 (Jira 버전에 따라 경로가 약간 다를 수 있습니다). 또는 `/plugins/servlet/webhooks`를 Jira 인스턴스 URL에 추가하여 직접 링크를 사용할 수도 있습니다 (예: `https://YourJiraInstanceName/plugins/servlet/webhooks`).
2. 웹훅 페이지의 오른쪽 상단에서 **웹훅 생성**을 클릭합니다.
3. **이름**란에 웹훅을 설명하는 이름을 입력합니다 (예: "Miro 통합 웹훅").
4. 웹훅 상태를 **활성**으로 설정합니다.
5. Miro 설정에서 복사한 **웹훅 URL**을 URL 필드에 붙여넣습니다.
   ![system_webhooks.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941532050_system%20webhooks.jpg)
   *Jira의 시스템 웹훅 설정*
6. **이벤트** 섹션의 **이슈** 아래에서 **업데이트됨** 및 **삭제됨** 이벤트를 선택합니다.
7. **생성**을 클릭하여 웹훅을 저장합니다.
   ![Jira_Webhook_settings.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941533074_Jira%20Webhook%20settings.jpg)
   *Jira 웹훅 이벤트 설정*
8. Jira에서 웹훅을 생성한 후 Miro의 Jira 카드 설정의 **단계 2**로 돌아가 **Jira URL**이 정확히 입력되어 있는지 확인하고 **연결**을 클릭합니다.

이제 웹훅이 생성 및 구성되었습니다. Miro 보드의 Jira 카드는 Jira에서 변경될 때 자동으로 업데이트됩니다.
