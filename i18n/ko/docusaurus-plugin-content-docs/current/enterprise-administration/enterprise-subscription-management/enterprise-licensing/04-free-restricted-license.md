---
title: "\uC81C\uD55C\uB41C \uBB34\uB8CC \uB77C\uC774\uC120\uC2A4"
article_id: 360011746739
translation_id: 360011746739
locale: ko-kr
sidebar_position: 4
created_at: '2020-02-05T07:29:16Z'
updated_at: '2026-02-19T10:40:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

새로운 사용자가 Miro 구독에 가입할 때, [Enterprise 라이선스 모델](02-enterprise-licensing.md)에 따라 제한된 무료 라이선스가 부여될 수 있습니다.

> **해당:** Enterprise 플랜

## 사용자에게 제한된 무료 라이선스가 부여되는 경우

**플렉시블 라이선싱 프로그램(FLP)에서는**, 다음과 같은 경우에 제한된 무료 라이선스가 사용자에게 부여될 수 있습니다:

- 새로운 사용자의 기본 라이선스가 제한된 무료 라이선스로 설정된 경우
- 회사 관리자가 사용자를 초대하며 초대 창에서 이들에게 제한된 무료 라이선스를 선택하는 경우
- 회사 관리자가 **설정 > 활성 사용자**에서 사용자를 제한된 무료 라이선스로 전환하는 경우

:::note
[플렉시블 라이선싱 프로그램(FLP)](03-flexible-licensing-program-flp.md)과 [FLP에서 라이선스 관리](05-license-management-on-the-flexible-licensing-program-flp.md)에 대해 자세히 알아보세요.
:::

**비플렉시블 라이선싱(non-FLP)**에서는 다음 경우에 사용자가 제한된 무료 라이선스를 받을 수 있습니다:

- 해당 사용자가 Miro에 등록하는 동안 조직이 보유하고 있는 Advanced, Standard, Full (legacy) 라이선스가 부족한 때 자동 캡처 ( [도메인 제어](../../canvas-25-admin-features/domain-control/01-domain-control.md) 또는 [즉시 프로비저닝](../../user-management/13-user-provisioning-on-enterprise-plan.md)) 시 Free Restricted 라이선스가 할당될 수 있습니다.
- 해당 사용자가 조직 내 팀에 초대되었으나, 조직이 보유하고 있는 Advanced, Standard, Full (legacy) 라이선스가 부족한 경우입니다.

여러 사용자를 동시에 초대할 때 초대 목록에 있는 이메일 주소의 순서에 따라 라이선스가 부여됩니다. 조직에 라이선스가 부족한 경우 목록의 마지막 사용자들은 제한된 무료 라이선스를 받게 됩니다. 이 경우 초대한 사람에게 일부 사용자가 제한된 접근을 하게 되는 것을 알리는 팝업 알림이 표시됩니다.

## 사용자를 위한 제한된 무료 라이선스의 작동 방식

제한된 무료 사용자는 참여하는 팀의 보드를 보고 댓글을 달 수 있으며, 회사 관리자에게 편집 접근 권한과 스탠다드 라이선스 또는 풀(기존) 라이선스를 요청할 수 있습니다. 또한 다른 멤버와 함께 조직 내 팀을 발견하고 참여할 수 있습니다.

:::note
회사 관리자는 [요청 관리 설정을 구성](../../user-management/09-request-management-on-enterprise-plan.md)할 수 있습니다.
:::

### 제한된 무료 보드 접근

제한된 무료 라이선스를 가진 사용자에게는 다음과 같은 보기, 댓글, 편집 접근 권한이 적용됩니다:

|  |  |
| --- | --- |
| **보드 공유 방식** | **액세스 수준** |
| 공개 링크 | 지정된 액세스 수준에 따라 Free Restricted 사용자는 보기 또는 편집이 가능합니다. |
| 팀 또는 회사 링크 | 지정된 액세스 수준에 따라 Free Restricted 사용자는 보기 또는 댓글 작성이 가능합니다. |
| [임베드 링크](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md) | 제한된 무료 라이선스 사용자는 부여된 액세스 수준에 따라 보기 또는 댓글이 가능합니다.   설령 임베드 권한을 통해 편집 액세스가 부여되더라도, 제한된 무료 라이선스 사용자는 편집하거나 편집 요청을 할 수 없습니다. |

## 제한된 무료 라이선스 관리 방법

> **실행 가능한 사용자:** 회사 관리자

모든 구독에서 회사 관리자는 팀 또는 회사 설정의 **활성 사용자** 섹션에서 사용자 라이선스를 제한된 무료 라이선스에서 표준 또는 풀(이전) 라이선스로 업그레이드할 수 있습니다.

**플렉시블 라이선스 프로그램(FLP)**

플렉시블 라이선싱 프로그램(FLP) 구독에서는, 회사 관리자는 예약 없이 언제든 고급, 표준, 또는 전체(레거시) 라이선스를 제한된 무료 라이선스로 다운그레이드할 수 있습니다.

제한된 무료 라이선스를 가진 사용자가 편집 액세스를 요청하면, 회사 관리자는 그들의 [요청 관리 설정](../../user-management/09-request-management-on-enterprise-plan.md)에 따라 요청을 받습니다.

:::note
플렉시블 라이선싱 프로그램에서의 [라이선스 관리에 대해 더 알아보기](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

## 자주 묻는 질문

**비 FLP 플랜에 표준 또는 전체(기존) 라이선스를 추가하면 제한된 무료 라이선스는 어떻게 되나요?**

기존의 제한된 무료 사용자들은 자동으로 새로운 표준 또는 전체(기존) 라이선스로 업그레이드되지 않습니다. 회사 관리자가 수동으로 라이선스를 업그레이드할 수 있습니다.
