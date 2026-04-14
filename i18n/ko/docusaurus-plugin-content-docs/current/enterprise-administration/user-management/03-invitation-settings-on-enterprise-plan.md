---
title: "Enterprise \uD50C\uB79C\uC758 \uCD08\uB300 \uC124\uC815"
article_id: 4412315533842
translation_id: 4412315533842
locale: ko-kr
sidebar_position: 3
created_at: '2021-12-13T04:56:26Z'
updated_at: '2026-02-19T10:56:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
---

Enterprise 플랜 초대 설정을 구성하여 누구를 초대할 수 있는지를 관리하세요. 설정을 통해 팀과 회사의 요구 사항을 만족하도록 맞춤형으로 구성할 수 있습니다.

> **사용 가능 대상**: Enterprise 플랜
> **실행 가능한 사용자:** 회사 관리자

:::tip
Miro를 처음 사용하신다면, [팀 및 회사 설정](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md)에 대해 더 알아보세요.
:::

## 팀 초대 설정

원활한 협업을 위해 **모든 팀 멤버**가 팀에 새로운 멤버를 초대할 수 있도록 허용하세요. 팀 초대를 보다 엄격하게 관리하려면 이 옵션을 회사 관리자 및/또는 팀 관리자로 제한하여 모든 초대 요청이 [요청 관리](09-request-management-on-enterprise-plan.md)를 통해 전달되도록 할 수 있습니다. 또한 사용자가 팀에 [게스트](../../using-miro/sharing-boards/07-collaboration-with-guests.md)를 초대할 수 있는지 여부도 관리할 수 있습니다.

### 팀 초대 설정 구성 방법

관리자 콘솔에서 팀 초대 설정을 관리하려면 **팀**으로 이동하여 팀을 선택하세요. 팀 패널이 열립니다. **초대** 아래에서 다음 옵션 중 하나를 선택하세요:

- **회사 관리자만**
  회사 관리자만 새 구성원을 팀에 추가할 수 있습니다.
- **회사 관리자와 팀 관리자**
  회사 관리자와 팀 관리자는 새 구성원을 팀에 초대할 수 있습니다.
- **모든 팀원**
  모든 팀원이 새 구성원을 팀에 초대할 수 있습니다.

:::note
플렉시블 라이선싱 프로그램 (FLP) [구독](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)에서는 팀 초대 설정이 회사 초대 설정으로 보완됩니다.
:::

### 게스트 초대 설정 방법

회사 관리자는 멤버들이 [게스트](../../using-miro/sharing-boards/07-collaboration-with-guests.md)를 초대하는 옵션을 허용하거나 제한할 수 있습니다. 게스트는 초대된 보드에만 접근할 수 있으며 라이선스가 필요하지 않습니다.

**팀** > 팀 선택 > **설정** > **[이름] 팀에 게스트 허용**으로 게스트 초대 설정을 업데이트하세요.

:::note
회사 관리자는 게스트의 자동 비활성화를 30일 동안 활동이 없을 경우 설정할 수 있습니다.
:::

## 초대 시나리오

:::tip
요청 관리 [설정](09-request-management-on-enterprise-plan.md)에 따라, 보드를 공유하거나 팀에 사용자를 초대하려는 요청은 회사 관리자에게 직접 보내거나 특정 사용자에게 이메일로 보내거나, 서비스 데스크 티켓이 생성될 수 있습니다.
:::

**팀에 새 멤버 초대**

게스트가 허용되지 않고, 멤버가 새 멤버를 초대할 수 없는 경우, 보드를 공유하려고 할 때 아래 알림이 표시되며 요청을 제출해야 합니다.

**소유자 또는 공동 소유자 역할 부여**

멤버가 새 멤버를 초대할 수 없는 경우, 특정 보드에서 게스트 또는 [Free 제한 멤버](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)에게 소유자 또는 공동 소유자 역할을 부여하려고 하면 아래 알림이 표시되며 요청을 제출해야 합니다.

**외부 사용자 또는 게스트를 보드 편집에 초대하기**

:::note
외부 게스트란 회사 도메인 이외의 게스트입니다. 이들의 이메일 주소는 외부 회사의 것입니다.
:::

팀에 새 멤버를 초대하는 것이 허용되지 않고, 편집 권한이 있는 게스트가 팀에서 활성화되지 않았다면, 외부 사용자를 보드 편집에 초대하려는 경우 아래 알림이 표시되며
요청을 제출해야 합니다.
요청을 제출한 후, 초대된 이는 보드에 댓글 권한으로 추가되어 보드의 내용을 편집하지 않고도 댓글을 추가할 수 있습니다.

## 회사 초대 설정

회사 초대 설정은 누가 새로운 멤버를 Enterprise 구독에 초대할 수 있는지를 제어합니다. 모든 새로운 멤버는 [라이선싱 모델](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md)과 [기본 라이선스](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md)에 따라 고급, 표준, 전체(레거시), Free, Free 제한 라이선스가 부여됩니다.

### 회사 초대 설정을 설정하는 방법

> **사용 가능 대상**: [플렉시블 라이선싱 프로그램](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)

회사 초대 설정을 관리하려면, **회사** 설정 > **보안** > **공유** > **초대**로 이동하여 다음 옵션 중 하나를 선택하세요:

**회사 관리자만**
회사 관리자만 새 구성원에게 라이선스를 부여할 수 있습니다. 팀 관리자와 구성원은 회사 내 기존 구성원만 팀에 초대할 수 있으며, 새 라이선스를 활성화할 수 없습니다.

**회사 관리자 및 팀 관리자**
회사 관리자와 팀 관리자는 새 구성원을 초대하고 새 라이선스를 추가할 수 있습니다. 팀 관리자는 자신이 팀 관리자인 팀에만 새 구성원을 초대할 수 있습니다.

**모든 멤버**
Enterprise 구독의 모든 멤버는 팀 초대 설정에서 **모든 팀 멤버**를 위한 초대가 허용되는 경우, 사람들을 팀에 초대하여 새로운 라이선스를 추가할 수 있습니다.

## 회사와 팀 설정의 결합

회사 설정은 팀 초대 설정을 보완합니다. 회사 관리자는 팀 설정에서 특정 팀에 사용자를 초대할 수 있는 권한을 설정할 수 있습니다. 이는 회사 관리자가 멤버와 팀 관리자가 자체 팀 초대와 협업을 관리하도록 허용할 수 있음을 의미하지만, 라이선스는 여전히 회사 설정에서 회사 관리자에 의해 통제됩니다.

## 게스트의 자동 비활성화

게스트를 30일간 비활성 상태로 유지하면 자동으로 비활성화됩니다. 이 기능을 사용하여 게스트를 삭제하고 구독의 보안을 유지할 수 있습니다.

기능을 켜면, 30일 이내에 Enterprise 팀에서 활동하지 않은 모든 도메인에 관계없이, 모든 게스트가 자동으로 비활성화됩니다. 30일 기간을 맞춤 설정할 수는 없습니다.

이 설정은 조직 내 모든 팀에 적용됩니다.

**회사** 설정 > **보안** > **공유**로 이동하여 **게스트 자동 비활성화**를 켜세요.

:::tip
설정을 켜자마자 이 작업은 [감사 로그](../security-integrations/security-management/01-audit-logs.md)에 **외부 사용자 만료 설정 활성/비활성화**로 기록됩니다. 비활성화 이벤트도 [감사 로그](../security-integrations/security-management/01-audit-logs.md). 작동자는 **Miro Automation**으로 표시됩니다.
:::
