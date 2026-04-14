---
title: 조직의 팀을 기본 Jira 설정에 연결하기
article_id: 26438407676434
translation_id: 26441940543890
locale: ko-kr
sidebar_position: 6
created_at: '2025-05-02T14:35:25Z'
updated_at: '2025-10-21T12:07:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '실행 가능한 사용자: 회사 관리자 해당 플랜: Enterprise 해당 플랫폼: 브라우저, 데스크탑'
---

회사 관리자는 조직 내 팀을 일괄적으로 글로벌 Jira 설정을 사용하도록 연결할 수 있으며, 이는 팀 수준에서 지정된 설정을 덮어씁니다.

## 필수 조건

- Miro에서 회사 관리자 역할을 가지고 있는지 확인하세요.
- [OAuth 2.0을 사용하여 Jira 데이터 센터에 연결하기](https://help.miro.com/hc/articles/25753304280466)에 기본 연결이 되어 있는지 확인하세요.

## 기본 Jira 설정에 팀 연결하기

1. Miro 대시보드에서 오른쪽 상단의 아바타를 선택하고 **관리 콘솔** | **설정**으로 이동합니다.
2. 왼쪽 사이드바에서 **앱 및 통합 ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **앱** > **앱 관리** 탭으로 이동합니다.
3. **아래 목록의 앱만 허용**이 활성화되어 있는지 확인합니다.
4. **앱** 열에서 **Jira 카드**에 대해 **설정**을 선택합니다.
5. **기본 인스턴스에 팀 추가**에서 연결할 팀을 각각 선택하거나 **모두 선택**을 클릭합니다.

   > ✏️ 목록에는 전역 조직 설정을 사용하지 않는 팀만 표시됩니다.
6. **&lt;number of teams&gt;개 팀을 기본값에 추가**를 클릭합니다.

   > ✏️ 귀하의 조직 내 전역 Jira 인스턴스를 이미 사용하고 있지 않은 사용자는 마이그레이션되며, 재인증해야 합니다.

   > ✏️ 다른 Jira 인스턴스에서 마이그레이션된 사용자는 Miro에서 Jira 관련 작업을 처음 시도할 때 재인증을 요청받습니다.

## 자주 묻는 질문

**팀이 글로벌 Jira 연결을 무기한 사용할 수 있나요?**

아니요. 필요하면 나중에 특정 팀의 Jira 설정을 변경할 수 있습니다.

**어떤 팀이 글로벌 Jira 연결을 사용해야 하나요?**

조직 설정을 사용하는 것이 일반적으로 선호되며, 이는 관리의 번거로움을 줄여줍니다. 팀 연결이 조직과 같은 설정을 공유하는 경우, 기본 조직 설정으로 팀을 온보딩하는 것을 권장합니다.
