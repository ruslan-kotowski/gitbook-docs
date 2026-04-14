---
title: OAuth 2.0을 사용하여 Jira 데이터 센터에 연결
article_id: 25753304280466
translation_id: 26513382875026
locale: ko-kr
sidebar_position: 8
created_at: '2025-05-06T09:04:44Z'
updated_at: '2025-05-21T09:27:19Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '실행 가능한 사용자: 회사 관리자 중 Jira 시스템 관리자 권한을 가진 사용자 어떤 플랜: Enterprise 어떤 플랫폼: 브라우저,
    데스크톱'
---

:::note
OAuth 2.0을 사용한 Jira 데이터 센터 연결은 조직 수준에서만 활성화됩니다.
:::

## 전제 조건

- 다음 권한을 보유하고 있는지 확인하세요:
  - Jira 시스템 관리자 권한
  - Miro 회사 관리자 역할
- Jira 데이터 센터에서 OAuth 2.0 애플리케이션 링크를 생성하세요. 방법을 알아보려면 (외부) [Atlassian Jira 애플리케이션 지원](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Create%20an%20incoming%20link%20using%20application%20links)을 참조하세요.
  - 프롬프트가 표시되면 다음 리디렉션 URL을 사용하세요.
    https://integrations.miro.com/api/external-auth/oauth2/callback
  - 자동 웹훅을 사용하려면 범위에 **관리자**를 선택하세요.

## Miro를 OAuth 2.0을 사용해 Jira 데이터 센터에 연결하기

1. Miro 대시보드에서 오른쪽 상단의 아바타를 선택하고 (Enterprise) **관리자 콘솔** 또는(Starter 및 Business) **설정**으로 이동합니다.
2. 왼쪽 사이드바에서 **앱 및 통합 ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **앱**> **앱 관리** 탭으로 이동합니다.
3. **아래 목록에 있는 앱만 허용**이 활성화되어 있는지 확인하세요.
4. **앱** 열에서 **Jira 카드**에 대해 **설정**을 선택하세요.
5. **새 연결 추가**를 선택합니다.
6. **Jira 설정**에서 **Jira 데이터 센터**를 선택하세요.
7. **인증 방법**에서 **OAuth 2.0**을 선택하세요.
8. **Jira URL**에는 Jira 인스턴스 URL을 입력하세요.
9. 조직의 모든 팀에 대해 이 연결을 기본 연결로 설정하려면 **기본값으로 설정**을 클릭하세요.
10. Jira **클라이언트 ID** 입력
    **추가 정보**: (외부) [수신 링크 구성](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application)을 참조하세요.
11. Jira **클라이언트 시크릿 키**를 입력하세요.
    **추가 정보**: (외부) [수신 링크 구성](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application)을(를) 참조하세요.
12. 범위를 선택하세요
    자동 웹훅을 사용하려면, **관리자** 또는 **시스템 관리자**를 선택하세요.
13. (선택 사항) Jira에서 Miro로 실시간 업데이트를 받으려면, **웹훅 자동 생성**을 선택하세요.
    > 수동으로 웹훅을 나중에 추가할 수 있습니다.
14. **연결**을 선택하세요.
    > 사용자가 Jira 관련 작업을 처음 시도할 때, 인증하라는 메시지가 표시됩니다. 재인증할 필요가 없습니다.

## 다음은 무엇인가요?

연결된 Jira 인스턴스를 보고 관리하려면 **관리자 콘솔** | **설정** > **앱 및 통합 ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **앱 관리**로 이동하세요. 그런 다음 **앱** 열 아래에서 **Jira 카드**에 대해 **설정**을 선택하세요.

팀을 기본 Jira 인스턴스에 연결하는 방법을 알아보려면 [조직의 팀을 기본 Jira 설정에 연결하기](https://help.miro.com/hc/articles/26438407676434)를 참조하세요.

## 자주 묻는 질문

**스코프로 관리자를 선택하면 모든 사용자가 Jira에서 관리자 권한을 가져야 합니까?**

아니요. 관리자 범위는 사용자가 Miro에서 가질 수 있는 가장 높은 범위를 의미합니다. 범위는 사용자에 따라 Jira에서의 권한에 따라 제한됩니다.

**팀 수준에서 Jira 데이터 센터를 OAuth 2.0으로 연결할 수 있나요?**

아니요. 조직 레벨에서만 가능합니다.
