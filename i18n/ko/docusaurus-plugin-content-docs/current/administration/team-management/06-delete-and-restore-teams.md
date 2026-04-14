---
title: 팀 삭제 및 복원 관리
article_id: 360017571334
translation_id: 360017571334
locale: ko-kr
sidebar_position: 6
created_at: '2019-02-11T10:08:51Z'
updated_at: '2025-11-25T15:58:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: deleted-teams
availability:
  notes: '사용 가능 대상: 팀 관리자, 사용자 관리자, 회사 관리자'
---

### 팀 삭제하기

:::note
Miro에서 [팀](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md)과 사용자 [프로필](https://miro.com/app/settings/user-profile/)(모든 팀이 연결된 사용자 데이터와 이메일)은 서로 다른 개념입니다. 프로필을 삭제하려면 [이 문서](../../using-miro/managing-your-profile/07-how-to-delete-your-profile.md)를 참고하세요.
:::

:::warning
Enterprise 플랜에서는 관리자에게 **삭제 확인을 요청하지 않습니다**. 따라서 백업 저장 요청이 삭제 과정의 마지막 단계일 수 있으니 주의해주세요.
:::

팀 삭제는 팀 관리자 및 회사 관리자가 수행할 수 있습니다. 팀을 삭제하면 **모든 보드와 템플릿이 제거됩니다**. 실수로 삭제한 보드를 복구하려면 [휴지통 관리 도움말](../../using-miro/managing-boards/09-trash-management.md)의 안내를 참고하세요. 팀을 삭제하기 전에 [보드를 다른 팀으로 이전](../../using-miro/managing-boards/04-how-to-move-a-board.md)하거나,[백업을 저장](../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)하거나 [내보내기](../../using-miro/import-and-export/export/03-how-to-export-your-board.md)하는 것이 좋습니다. 팀 멤버에게 해당 작업을 요청할 수도 있습니다.

팀 삭제하기

1. Miro 프로필 설정으로 이동합니다(보드에서는 보드 이름 옆에 있는 **설정** 아이콘을 클릭하세요. Miro 대시보드에서는 아바타를 클릭하고 **설정**을 선택합니다).
2. 왼쪽 패널에서 **팀**을 클릭합니다.
3. 삭제하려는 팀을 클릭합니다.
4. 왼쪽 패널에서 **팀 프로필**을 클릭합니다.
5. **팀 삭제** 버튼을 클릭합니다.![팀_삭제_관리하기_팀_삭제_옵션.png](images/21301614383634_manage_team_deletion_delete_team_option.png)*팀 프로필을 사용해 팀 삭제하기*
6. **팀 삭제**를 클릭해 선택을 확인합니다. 팀과 관련된 모든 보드도 함께 삭제됩니다. ![팀_삭제_관리하기_삭제_확인.png](../../../../../../docs/administration/team-management/images/21019693273234_managing_team_deletion_delete_confirmation.png)*팀 제거 확인 메시지*
7. 단일 팀 조직의 경우 삭제 프로세스를 완료하는 데 필요한 확인 링크가 포함된 이메일을 받게 됩니다. **팀 삭제** 링크를 클릭해 삭제를 완료하세요.
   ![팀_삭제_관리하기_이메일_메시지.png](images/21301614388882_managing_team_deletion_email_message.png)*팀 삭제 확인 이메일*

## 팀 복원 또는 영구 삭제하기

> **해당 플랜:** Business 플랜, Enterprise 플랜
> **사용 가능 대상:** 사용자 관리자, 회사 관리자

팀을 삭제한 후 팀을 복구하거나 영구적으로 삭제할 수 있습니다. 삭제 후 아무 조치도 취하지 않으면 90일 후에 팀이 자동으로 삭제됩니다.

삭제된 팀을 복원하면 팀을 삭제했을 때 제거된 보드나 템플릿도 모두 복원됩니다.

팀을 영구적으로 삭제하면 팀에서 만든 보드나 템플릿도 영구적으로 삭제됩니다. 이 작업은 되돌릴 수 없습니다.

### 삭제된 팀 복원하기

1. 회사 설정 패널에서 **팀**을 클릭합니다.
2. 팀 패널에서 **삭제됨** 탭을 클릭합니다.
3. 복원하려는 팀을 찾습니다. 스크롤하거나 검색창을 사용해 팀을 찾을 수 있습니다.
4. 팀 옆의 **...** 세 점 아이콘을 클릭하고 **팀 복원**을 선택합니다.
5. 팀이 활성 탭으로 다시 이동하며 모든 보드와 템플릿이 복구됩니다.![삭제된_팀_복원하기.gif](images/21301605714450_deleted_teams_restore_team.gif)*삭제된 팀 복원하기*

### 팀 영구 삭제하기

1. 회사 설정 패널에서 **팀**을 클릭합니다.
2. 팀 패널에서 **삭제됨** 탭을 클릭합니다.
3. 복원하려는 팀을 찾습니다. 스크롤하거나 검색창을 사용해 팀을 찾을 수 있습니다.
4. 팀 옆의 **...** 세 점 아이콘을 클릭하고 **영구 삭제**를 선택합니다.
5. **“[팀 이름]” 삭제** 항목에 체크해 삭제를 수행할지 확인하는 단계를 거친 다음, **영구 삭제**를 클릭합니다.*![삭제된_팀_영구_삭제하기.gif](images/21301605715090_deleted_teams_delete_permanently.gif)**팀 영구 삭제하기*

## Business 플랜의 마지막 팀 삭제하기

Business 플랜의 마지막 팀은 삭제할 수 없습니다. 대신 다음 경고 메시지가 표시됩니다. **조직의 마지막 팀은 삭제할 수 없습니다**.

다음과 같은 해결 방법을 사용할 수 있습니다.

1. [구독을 취소](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md)합니다.
2. 결제 기간이 끝나고 팀이 만료되면 [Free 플랜으로 다운그레이드](../../plans-billing/manage-your-subscription-and-plan/04-downgrade-your-plan.md)합니다.
3. 무료 팀을 삭제합니다.

Enterprise 플랜의 경우 [고객 지원에 문의](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)해주세요.

## 자주 묻는 질문

팀을 삭제하면 팀에 연결된 구독도 종료되나요?

추가 요금 발생을 방지하려면 결제 설정에서 구독을 취소하세요. 자세한 내용은 [이 가이드](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md)를 참고하세요.

팀을 삭제하려면 어떤 권한이 필요한가요?

팀을 삭제하려면 회사 관리자 권한이 필요합니다. 회사 관리자가 아닌 경우 [팀 탈퇴](../../using-miro/managing-your-profile/06-how-to-leave-a-team.md) 옵션이 표시됩니다.

팀 삭제를 요청했지만 확인 이메일을 받지 못했습니다. 이메일을 찾으려면 어떻게 해야 하나요?

**스팸, 프로모션,** **정크, 소셜**, **업데이트** 폴더를 열고 확인 이메일이 있는지 살펴보세요.
방화벽으로 인해 이메일이 받은 편지함에 도착하지 못하는 경우도 있습니다. 시스템 관리자에게 문의해 Miro의 도메인 및 하위 도메인을 허용 목록에 추가하도록 요청하세요. 허용 목록에 추가해야 하는 발신자에 대한 자세한 정보는 [이 문서](../../using-miro/tools/troubleshooting/02-allowlist-miro-mailers.md)에서 확인할 수 있습니다.

:::note
초대받은 팀에서 탈퇴하려면 [팀을 탈퇴하는 방법](../../using-miro/managing-your-profile/06-how-to-leave-a-team.md) 문서를 참고하세요.
:::
