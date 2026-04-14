---
title: 플렉시블 라이선싱 프로그램(FLP)에서의 라이선스 관리
article_id: 360018622159
translation_id: 360018622159
locale: ko-kr
sidebar_position: 5
created_at: '2020-12-29T10:44:01Z'
updated_at: '2026-02-23T18:22:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: '해당 대상: Enterprise 플랜'
---

플렉시블 라이선싱 프로그램(FLP)에서의 라이선스 관리, 신규 사용자에게 제공되는 라이선스 관리 옵션 및 기존 라이선스 전환 방법에 대해 알아보세요.

:::tip
FLP 라이선싱이 처음이라면, 먼저 [플렉시블 라이선싱 프로그램](03-flexible-licensing-program-flp.md)과 [Enterprise 플랜에서의 사용자 접근 수준](../../user-management/11-user-access-levels-on-enterprise-plan.md)을 읽어보셔서 우리의 라이선싱 모델, 라이선스 유형 및 Miro 역할이 어떻게 연계되는지 이해하시기를 권장합니다.
:::

## 신규 사용자에게 라이선스 할당

멤버 게스트 방문자

회사의 기본 라이선스 설정에 따라, 새로운 멤버는 Free 또는 제한된 무료 라이선스를 할당받습니다. 구독에 대한 새로운 멤버의 기본 라이선스를 설정하려면 Miro의 담당자에게 연락하세요.

새로운 멤버는 기본 라이선스를 할당받습니다:

- 관리자가 아닌 구성원이 초대할 때
- 자동으로 [Just-in-Time 프로비저닝](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), [도메인 제어](../../canvas-25-admin-features/domain-control/01-domain-control.md) 또는 [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)을 통해

회사 관리자는 초대된 구성원의 라이선스를 선택할 옵션도 있습니다.

- **Free** 를 선택하면 사용자가 보드를 편집하거나 생성, 보드 초대, 공동 소유자 권한 부여, 또는 [프로젝트](../../../using-miro/sharing-boards/16-projects.md)에 편집자로 추가될 때 즉시 Standard 또는 Full(legacy) 라이선스로 업그레이드됩니다.
- 편집 권한 없이 멤버를 초대하려면 **Free Restricted**를 선택하세요.

보드에 초대된 게스트는 항상 **Free** 라이선스를 받습니다. Enterprise 플랜에서 게스트를 [초대하는 방법](../../../using-miro/sharing-boards/07-collaboration-with-guests.md)을 확인하세요.

[방문자](../../../using-miro/sharing-boards/08-collaboration-with-visitors.md)는 공개적으로 공유된 보드를 무료로 이용할 수 있으며, 라이선스가 필요하지 않습니다.

## 라이선스를 업그레이드 또는 다운그레이드하는 방법

> **실행 가능한 사용자:** 회사 관리자

**Free** 라이선스는 사용자가 보드를 생성 또는 편집하는 즉시 자동으로 Standard 또는 Full (과거) 라이선스로 업그레이드됩니다.

제한된 무료에서 Standard나 Full(레거시)로 전환  Standard나 Full(레거시)에서 제한된 무료로 전환 라이선스 일괄 변환

제한된 무료 라이선스는 회사 관리자가 수동으로 또는 [Enterprise 워크플로 자동화](../enterprise-workflow-automation/01-enterprise-workflow-automation.md)의 일부로 Standard 또는 풀(기존) 라이선스로 업그레이드할 수 있습니다.

제한된 무료 라이선스를 풀 라이선스로 업그레이드하려면:

1. **Teams**를 열거나 **조직 설정** > **사용자** > **모든 사용자** > **활성 사용자**를 엽니다.
2. 제한된 무료 사용자의 옆에 있는 **세 점**(**...**) 아이콘을 클릭합니다.
3. **Standard 멤버로 변경**을 선택합니다.

회사가 관리자는 사용자의 액세스를 제한하고 추가 풀 라이선스를 해제하려는 경우, 풀 라이선스를 제한된 무료 라이선스로 다운그레이드할 수 있습니다.

풀 멤버는 무료 라이선스로 다운그레이드할 수 없습니다. 무료 라이선스는 새로운 사용자에게만 할당할 수 있습니다.

풀 라이선스를 제한된 무료 라이선스로 다운그레이드하려면:

1. **팀** 또는 **조직 설정**을 열고 **사용자** > **모든 사용자** > **활성 사용자**를 엽니다.
2. **세 점 아이콘** **(...)**을 제한된 무료 사용자 옆에서 클릭합니다.
3. **제한된 무료 사용자로 변경**을 선택합니다.

여러 라이선스를 한 번에 일괄 변환하려면:

1. **조직 설정** > **사용자** > **모든 사용자** > **활성 사용자**를 엽니다.
2. 변환하려는 사용자들을 개별적으로 선택하거나 필터를 적용하여 사용자를 선택합니다. 사용자를 최대 50명까지 선택할 수 있습니다.
3. **일괄 작업**을 클릭하고 새 라이선스 옵션을 선택합니다.
