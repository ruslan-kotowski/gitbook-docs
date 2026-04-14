---
title: Miro에서 Jira OAuth 1.0 사용되지 않음
article_id: 28738797627538
translation_id: 28739454182162
locale: ko-kr
sidebar_position: 13
created_at: '2025-08-13T12:34:26Z'
updated_at: '2025-10-20T14:49:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '대상: 회사 관리자 플랜: Starter, Business, Enterprise, Education 플랫폼: 브라우저, 데스크탑'
---

Jira OAuth 1.0 인증은 2025년 8월부터 사용되지 않습니다.

귀하의 조직이 이미 Jira OAuth 2.0으로 업데이트를 완료했다면, 이 문서를 무시해도 좋습니다. 회사 관리자에게서 별도의 조치가 필요하지 않습니다. 회사 관리자를 통해 귀하의 조직이 OAuth 2.0을 사용하는지 확인할 수 있습니다.

:::warning
귀하의 조직이 아직 OAuth 2.0으로 업데이트하지 않았다면, Miro와의 Jira 통합, Jira Cloud, 서버 및 데이터 센터를 포함하여 통합이 중단될 수 있습니다.
:::

오직 회사 관리자만이 조직 내 팀을 업그레이드할 수 있습니다.

차질이 발생할 경우, 귀하의 조직이 OAuth 2.0 인증으로 업데이트될 때까지 Miro와 Jira 간의 동기화가 중단됩니다. 기존의 Jira 카드는 Miro 보드에 남아 있습니다.

차질이 생기면, 가져오기가 불가능하고, 카드 갱신이 되지 않으며, 세부 정보를 로드할 수 없고, 플래너 생성과 업데이트도 불가능합니다.

차질을 방지하기 위해, Miro는 귀하의 회사 관리자에게 즉시 Jira OAuth 2.0으로 업데이트할 것을 권장합니다.

:::tip
관리자들은 OAuth 버전을 확인할 수 있습니다.
:::

## OAuth 1.0이 사용되지 않게 된 이유

Atlassian이 OAuth 1.0 인증 프로토콜을 사용하지 않게 되었고 지원하지 않고 있습니다.

**추가 정보:** (외부 링크) [Rest API용 OAuth 1.0a (사용되지 않음)](https://developer.atlassian.com/cloud/jira/platform/jira-rest-api-oauth-authentication/)을 참조하세요.

## OAuth 버전 확인

Enterprise 팀 관리자 또는 Starter나 Business 플랜의 관리자로서, 팀이 OAuth 1.0 또는 OAuth 2.0을 사용 중인지 확인할 수 있습니다.

다음 단계에 따라 진행하세요:

1. Miro 대시보드에서 오른쪽 상단의 아바타를 클릭하고 **관리자 콘솔**을 선택합니다.
2. **팀** > **[팀 이름]**으로 이동합니다.
3. **앱**을 클릭합니다.
4. **Jira 카드**를 찾아서 클릭합니다.
5. **관리자 설정** > **Jira 구성**으로 이동합니다.
   구성에서 팀이 사용하는 OAuth 버전을 확인할 수 있습니다.
6. (선택 사항) 확인하려는 다른 팀에 대해서도 1-5번 단계를 반복합니다.
7. OAuth 2.0을 사용하지 않는 팀에 대해 회사 관리자에게 알립니다.

## 회사 관리자 찾기

회사 관리자를 확인하려면 다음 단계를 따르세요.

:::note
(Enterprise) 팀 개인정보 보호가 활성화된 경우, 회사 관리자가 아닌 사용자는 멤버 목록을 볼 수 없습니다.
:::

1. Miro에서 **팀 프로필 설정**으로 이동합니다.
2. **멤버** 페이지를 엽니다.
3. **추가 역할**을 클릭합니다.
4. **회사 관리자** 역할이 있는 사용자를 찾습니다.

:::tip
팀이 OAuth 2.0으로 업그레이드하고 잠재적인 중단을 피할 수 있도록 이 문서를 회사 관리자에게 공유하세요.
:::

## 회사 관리자를 위한 OAuth 2.0으로 업그레이드

회사 관리자로서 귀하는 귀하의 조직을 OAuth 2.0으로 업그레이드하는 데 도움을 줄 수 있는 다음의 리소스를 가지고 있습니다:

- [OAuth 2.0을 사용하여 Jira Cloud에 연결하기](https://help.miro.com/hc/articles/8588617184402)
- [OAuth 2.0을 사용하여 Jira Data Center에 연결하기](https://help.miro.com/hc/articles/25753304280466)
- [조직 내 팀을 기본 Jira 설정에 연결하기](https://help.miro.com/hc/articles/26438407676434)

## 임시 솔루션

OAuth 2.0가 현재 회사에서 사용이 어려운 경우, Miro는 OAuth 1.0을 사용하는 [임시 솔루션](https://help.miro.com/hc/articles/27689156602514)을 제공합니다.

하지만, Miro는 Atlassian의 현재 표준을 따르는 가장 안전하고 미래 지향적인 인증 방식인 OAuth 2.0으로의 업그레이드를 권장합니다.

## 추가 도움말

회사 관리자 또는 귀하께서 질문이 있으시면, [Miro 지원](https://help.miro.com/hc/articles/360020185799)에 문의하세요.
