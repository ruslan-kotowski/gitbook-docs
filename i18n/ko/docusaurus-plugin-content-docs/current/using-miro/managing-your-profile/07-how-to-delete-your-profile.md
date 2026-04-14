---
title: 프로필 삭제
article_id: 360017571354
translation_id: 360017571354
locale: ko-kr
sidebar_position: 7
created_at: '2019-02-11T10:08:54Z'
updated_at: '2026-01-07T13:30:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
availability:
  notes: '설정 기준: 프로필 소유자'
---

Miro에서 프로필을 삭제하면 시스템에서 정보가 제거됩니다. 프로필과 팀은 서로 다른 두 가지 요소임을 유의하세요.

- 프로필은 등록 및 이메일 주소에 연결된 데이터를 나타냅니다.
- 팀은 다른 팀 멤버와 함께 속한 공간이며, 멤버가 콘텐츠를 만들고 보드를 저장할 수 있습니다

모든 프로필은 여러 팀과 연동될 수 있습니다. 팀을 제거하려면 [여기에서](../../administration/team-management/06-delete-and-restore-teams.md) 방법을 알아보세요.
:::warning
프로필 삭제는 취소할 **수** 없습니다.
:::

:::warning
프로필 삭제해도 활성 구독이 취소되지 않습니다. 더 이상 갱신을 중지하려면 [설정에서 구독을](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md) 취소하세요.
:::

### 프로필 삭제

1. [프로필 설정을](https://miro.com/app/settings/user-profile/) 엽니다.

2. 페이지 하단으로 스크롤하고 **내 프로필 삭제를** 선택하세요.

![Delete_profile.png](../../../../../../docs/using-miro/managing-your-profile/images/21017429126546_Delete%20profile.png)
*프로필 삭제하기*

3. 이 시점에서 [보드를](../import-and-export/export/05-how-to-save-board-backup.md) 삭제하기 전에 백업을 저장하거나 [내보내는](../import-and-export/export/03-how-to-export-your-board.md) 것이 좋습니다.

![profile_removal_modal.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017429125778_profile%20removal%20modal.jpg)*프로필 제거 확인 메시지*

4. 잠시 후 확인 링크가 있는 이메일을 받게 됩니다. 링크를 클릭해 완료하세요. 프로필 삭제를 완료하려면 **프로필** 삭제를 클릭할 때 브라우저에서 Miro 프로필에 로그인해야 합니다.

![Profile_deletion_email.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017416055186_Profile%20deletion%20email.jpg)
*프로필을 삭제하는 확인 이메일*

### 프로필 제거 후 콘텐츠는 어떻게 되나요?

프로필을 제거하면 보드가 삭제됩니다.

팀의 유일한 관리자인 경우 콘텐츠가 *완전히* 제거됩니다. 관리자 권한은 시간순으로 처음 초대된 멤버에게 부여됩니다.

팀에 다른 관리자가 있으면 콘텐츠가 삭제되고 관리자 중 한 사람에게 재할당됩니다. 이는 관리자가 [90일 이내에 보드를 복원할](../managing-boards/08-how-to-restore-a-deleted-board.md) 수 있다는 의미입니다. 유료 사용자는 휴지통에서 보드를 찾을 수 있으며 무료 사용자는 링크를 통해 복원할 수 있습니다.

### 자주 묻는 질문

1. *[SSO(통합로그인)로](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) Miro에 로그인하면 프로필을 삭제할 수 있나요?*
   - 네, 그럴 수 있습니다. 그러나 조직이 [SCIM을](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) 사용하는 경우 이메일이 SCIM을 통해 Miro에 프로비저닝되는 한 프로필이 즉시 다시 생성됩니다.
2. *Miro 프로필에 연결된 이메일 주소를 변경하려면 어떻게 해야 하나요?*
   - 이 가이드 사용: [이메일 변경 방법](04-how-to-change-your-email.md)
3. *확인 링크가 있는 이메일을 받지 못했습니다. 어떻게 해야 하나요?*
   - 다음 단계를 시도하세요.

- **스팸, 프로모션,** **정크, 소셜**, **업데이트** 폴더를 열고 Miro 확인 이메일이 있는지 확인하세요.
- 받은 편지함이 가득 찼는지 확인해 이메일 받은 편지함의 메모리 한도에 도달하지 않았는지 확인하세요. 가득 찬 경우 새 이메일을 받으려면 일부 기존 이메일을 삭제해야 할 수 있습니다. 이메일을 삭제한 후 프로필 삭제를 다시 요청하세요
- 방화벽으로 인해 이메일이 받은 편지함에 도달하지 못하고 있을 수 있습니다. *시스템 관리자에게* 문의해 주세요. [miro.com*,](http://miro.com/) *.miro.com, [mirostatic.com*,](http://mirostatic.com/) mirostatic.com*, *.mirostatic.com, realtimeboard.com*, *.realtimeboard.com과 같은 도메인과 하위 도메인을 허용하도록 요청하세요. [다음은](../tools/troubleshooting/02-allowlist-miro-mailers.md) 허용 목록에 필요한 메일러에 대한 자세한 정보가 있는 문서입니다
- 두 솔루션도 도움이 되지 않으면 [Miro 지원에 문제를](../tools/troubleshooting/06-contacting-miro-support.md) 보고하세요.
