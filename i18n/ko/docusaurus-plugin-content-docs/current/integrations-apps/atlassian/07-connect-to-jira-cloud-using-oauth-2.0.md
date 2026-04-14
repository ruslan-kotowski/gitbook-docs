---
title: Jira Cloud에 OAuth 2.0 사용하여 연결하기
article_id: 8588617184402
translation_id: 26810591371922
locale: ko-kr
sidebar_position: 7
created_at: '2025-05-19T13:04:44Z'
updated_at: '2025-10-21T12:18:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '사용 가능 대상: LDAP로 보호된 Jira Cloud 포함 플랜: Starter, Business, Enterprise, Education
    설정 책임자: (Enterprise) 회사 관리자, 또는 (다른 모든 플랜) Jira 관리자 권한이 있는 팀 관리자'
---

:::warning
기술적 문제가 발생할 경우, [가능한 문제와 해결 방법](https://help.miro.com/hc/articles/360017572654)에 대한 기사를 참고하십시오.
:::

:::tip
Jira 카드에 대해 더 알고 싶다면 [Jira 카드 자주 묻는 질문](https://help.miro.com/hc/articles/360013463739) 기사를 참고하세요.
:::

## Jira와 Miro 연결

### 앱 설치

1. 통합을 활성화하려면, [대시보드](https://help.miro.com/hc/articles/360017571294-What-is-on-your-dashboard)의 오른쪽 상단에서 아바타를 클릭한 후 **앱 및 통합**을 선택하세요: ![mceclip0.png](../../../../../../docs/integrations-apps/atlassian/images/21017417672210_mceclip0.png)
   *앱 관리*
2. **검색** 줄에 "Jira 카드"를 입력하고 팝업 메뉴의 오른쪽 하단 모서리에 있는 파란색 **연결** 버튼을 클릭하세요.
3. **Jira 카드 추가** 창이 표시됩니다. 여기서 설치를 확인하거나 통합 설치를 원하는 팀을 선택해야 합니다(여러 팀의 멤버일 경우). 통합 **추가**를 클릭하세요. 대시보드 상단에서 **앱이 설치되었습니다:**라는 확인 메시지를 확인할 수 있습니다.
   ![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)
   *확인 메시지*

### Jira 프로필 연결

1. 대시보드에서 아바타를 다시 클릭하고 **설정 > 팀 >** *팀 이름* **> 앱 & 통합 > Jira 카드**로 이동하여 **연결**을 클릭합니다:
   ![mceclip2.png](../../../../../../docs/integrations-apps/atlassian/images/21017004818066_mceclip2.png)
   *통합 설정*
2. Jira 페이지로 연결 승인 요청이 나옵니다. Jira에 로그인한 후 **수락**을 클릭하세요.

### Jira 인스턴스를 Miro 팀에 연결하기

OAuth 2.0을 통해 여러 Jira 인스턴스를 동일한 팀 및 보드에 연결할 수 있습니다. 설정에서 앱을 승인 후, **다른 인스턴스 연결** 옵션을 볼 수 있습니다.

1. 작성 툴바에서 Jira 카드 피커를 실행합니다 (앱을 추가하려면 **더 많은 앱 +** 버튼을 사용해야 할 수도 있습니다).
2. 피커에서 **설정**을 클릭합니다.
3. 설정의 **앱 & 통합** 섹션으로 이동합니다. **다른 인스턴스 연결** 옵션을 찾아서 연결할 추가 Jira 인스턴스를 선택합니다.![mceclip0.png](../../../../../../docs/integrations-apps/atlassian/images/21017417672210_mceclip0.png)*Miro 계정의 Jira 카드 설정*

팀 관리자는 팀 구성원이 연결한 모든 인스턴스를 볼 수 있습니다:

![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)

:::warning
각 최종 사용자는 인스턴스의 카드를 다루기 위해서 Miro 보드에서 연결되어 있는 각 Jira 인스턴스에 대해 인증을 받아야 합니다.
:::

> ✍️ 한 번에 활성화할 수 있는 인스턴스는 하나만 가능하며, 사용자들은 해당 인스턴스에서 카드를 불러올 수 있습니다. 비활성화된 인스턴스에서 가져온 기존 카드들은 Miro 보드에서 계속 작업할 수 있습니다.

### Jira에서 실시간 업데이트 설정

양방향 동기화의 실시간 이점을 최대한 활용하려면 추가한 Jira 인스턴스에 대해 웹훅을 구성해야 합니다. 이를 통해 Jira에서 수행한 업데이트가 Miro에 실시간으로 반영됩니다.

1. 작성 툴바에서 Jira 카드 선택기를 실행합니다 (앱을 추가하려면 **더 많은 앱 +** 버튼을 사용해야 할 수도 있습니다).
2. 선택기에서 **설정**을 클릭합니다.
3. 설정의 **앱 및 통합** 섹션으로 이동합니다.
4. **연결된 인스턴스** 섹션에서 이전에 추가한 인스턴스 목록을 볼 수 있습니다.
5. 각 인스턴스 옆에는 **웹훅 추가** 버튼이 있습니다. 이를 클릭하여 해당 인스턴스에 대한 Jira에서 Miro로의 실시간 업데이트를 설정할 수 있습니다.
6. 추후에 이 인스턴스에서 웹훅을 제거하려면 위의 단계를 따라 연결된 인스턴스 옆에 있는 **웹훅 제거** 버튼을 클릭하면 됩니다.

:::note
인스턴스에 웹훅을 추가하려면 Miro *및* Jira의 관리자가 되어야 합니다.
:::

이제 완료되었습니다! 이제 Jira 작업을 카드로 화이트보드에 추가할 수 있습니다. Jira에서 수행된 모든 변경 사항은 보드의 Jira 카드에도 반영되며, 그 반대의 경우도 마찬가지입니다.

## 플러그인 제거

**팀 설정 > 앱 및 통합 > Jira 카드**로 이동하여 **팀용 제거**를 클릭하세요.

:::tip
[Jira 카드를 사용하는 방법에 대한 주요 기사](https://help.miro.com/hc/articles/360017572434)도 꼭 확인해 보세요!
:::
