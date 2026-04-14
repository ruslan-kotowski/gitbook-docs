---
title: "\uBCF4\uB4DC\uB97C \uC774\uB3D9\uD558\uB294 \uBC29\uBC95"
article_id: 360017730093
translation_id: 21574836912146
locale: ko-kr
sidebar_position: 4
created_at: '2024-09-24T17:37:58Z'
updated_at: '2026-03-27T16:09:50Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
availability:
  roles: board_owner
  notes: 'Relevant for: All plans'
backstage_link:
  entity_kind: capability
  entity_id: move-board-to-space
---

> **실행 가능한 사용자:** 보드 소유자
> **해당 대상:** 모든 플랜

모든 Miro 사용자는 여러 팀의 구성원이 될 수 있습니다. 귀하의 Miro 프로필은 이메일 주소입니다. Miro 보드를 한 팀에서 다른 팀으로 이동하거나, 다른 프로필로 Miro 보드를 전송할 수 있습니다.

:::note
Enterprise 플랜에서는 보드 공동 소유자와 콘텐츠 관리자가 [Miro REST API](https://developers.miro.com/reference/update-board)를 사용해 보드를 이동할 수 있으며, 이는 보드 소유자만 보드를 이동할 수 있는 Miro UI 경험과 의도적으로 다릅니다.
:::

:::note
Enterprise 플랜의 회사 관리자는 [비관리자 사용자와 보드 소유자에게 보드를 팀으로 이동하는 옵션을 제한할 수 있습니다.](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) 모든 비관리자 사용자와 보드 소유자에게.
:::

## 일반적인 시나리오

여기는 보드를 이동하는 여러 일반적인 시나리오와 이러한 작업을 수행하는 방법을 설명하는 이 글의 섹션이 나와 있습니다:

- 두 개의 **Miro 프로필**(Miro에 연결된 이메일 주소)을 사용하고 있으며, 한 프로필에서 다른 프로필로 보드를 옮기고 싶습니다.
  *이 섹션의* [*링크*](04-how-to-move-a-board.md)*를 참고하시고, **Free 플랜** 탭을 이용하세요.*
- **Free 플랜에서 유료 플랜으로 업그레이드**했으며, 보드를 유료 플랜으로 옮기고 싶습니다.
  *이 섹션의* [*링크*](04-how-to-move-a-board.md)*를 참고하시고, **Free 플랜** 탭을 이용하세요.*
- 두 **유료 팀 간에 보드를 이동**하려고 합니다.
  *단계를 따르려면* [*이 섹션*](04-how-to-move-a-board.md)*을 참조하세요. **유료 및 Education 플랜** 탭을 사용하십시오.*

## 팀 간 보드 이동

:::warning
보드를 다른 팀으로 옮기면 [버전 기록](12-board-history-versions.md)이 사라집니다. 버전 기록을 유지하고 싶다면, 대신 [보드 내용을 복사](../working-on-the-board/09-copy-as-text-or-as-an-image.md)하는 것이 좋습니다.
:::

보드를 팀 간에 옮기기 위해 필요합니다:

- 보드의 소유권을 갖고 있어야 합니다
- 양쪽 팀의 멤버여야 합니다

보드를 다른 팀으로 옮기는 방법은 두 가지가 있습니다: 대시보드에서 옮기거나, 보드 내에서 직접 옮기는 방법입니다.

### 보드 내에서 직접 보드를 옮기는 방법

1. 보드를 열고 보드 이름 오른쪽에 있는 세 점 아이콘(**...**)을 클릭하세요 (상단 왼쪽 코너)
2. 보드 > 이동 > 다른 팀 *![moving-board-three-dots.png](../../../../../../docs/using-miro/managing-boards/images/21537437708306_moving-board-three-dots.png)*으로 이동하세요.

### 대시보드를 사용하여 보드 이동하는 방법

1. 대시보드로 이동하여 팀의 모든 보드를 확인합니다.
2. 이동하고 싶은 보드의 카드 위에 마우스를 올립니다.
3. 세 점 아이콘을 클릭한 후, **팀으로 이동**을 클릭합니다.
   대화상자가 열립니다.
4. 보드를 이동할 조직을 선택합니다.
5. 그 조직 내의 팀을 선택합니다.
6. 클릭 **이동**.

### 보드를 다른 스페이스로 이동하는 방법

1. 보드를 열고 보드 이름 오른편(왼쪽 상단)에 있는 세 점 아이콘(**...**)을 클릭합니다
2. **보드 > 이동 > 다른 스페이스**로 이동합니다. 팀원들에게 보드가 다른 스페이스로 이동되었음을 알릴 수 있습니다.![moving-boards-spaces.png](../../../../../../docs/using-miro/managing-boards/images/21537453797394_moving-boards-spaces.png)*보드를 다른 스페이스로 이동하는 예시*

### 사용자 액세스 거부됨

보드가 이동되는 팀의 일원이 아닌 공동 작업자는 액세스 거부 메시지를 보게 됩니다.

보드를 이동한 후 액세스를 잃게 될 사용자 이메일을 확인하는 두 가지 방법이 있습니다. 사용자가 10명 미만인 경우, **액세스 거부 메시지**에서 **사용자 이메일 보기**를 클릭하여 이메일 목록을 확인할 수 있습니다. 사용자가 10명 이상인 경우, 이메일 목록을 다운로드할 수 있는 링크가 제공됩니다.

모든 공동 작업자가 보드에 대한 접근 권한을 유지하도록 하려면 보드를 이동하기 전에 [새 팀에 회원을 초대](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md)할 수 있습니다.

또한 **그냥 이동**을 선택하고 보드가 이동된 후 다시 공동 작업자를 추가할 수 있습니다.

![warning when moving a board.png](../../../../../../docs/using-miro/managing-boards/images/16759524012690_warning%20when%20moving%20a%20board.png)
*팀 간 보드를 이동할 때 나오는 접근 권한 거부 메시지*

**보드를 Free 팀으로 이동하면**, 모든 팀 구성원과 공유됩니다.

![private boards are not available in free teams.png](../../../../../../docs/using-miro/managing-boards/images/16759539790738_private%20boards%20are%20not%20available%20in%20free%20teams.png)
*개인 보드는 Free 팀에서 사용할 수 없습니다*

## 프로필 간 보드 이동

Miro의 프로필은 회원가입 시 등록한 이메일 주소입니다. 만약 두 개의 다른 이메일 주소로 회원가입했다면, 두 개의 프로필을 보유한 것입니다. 한 프로필에서 다른 프로필로 보드를 옮길 수 있습니다.

### 프로필 간 보드를 이동하는 방법

유료, Education 플랜 Free 플랜

보드가 유료 또는 Education 팀에 있으며 이를 다른 유료 또는 Education 팀으로 이동하려면, 보드 백업을 저장한 후 해당 팀에 업로드하세요.

1. 대시보드를 엽니다.
2. 이동하려는 보드의 카드를 마우스를 올려봅니다.
3. 세 점 아이콘을 클릭합니다.
4. **보드 백업 다운로드**를 클릭합니다.
5. .rtb 파일이 기기에 저장됩니다.

   ![board-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136352530_board-backup.png)
6. 두 번째 Miro 프로필에 로그인합니다.
7. 보드를 이동할 팀으로 전환합니다.
8. + **새로 만들기** > **가져오기** > **백업 가져오기**를 클릭합니다.
9. 파일 선택기가 열립니다.
10. 이전에 저장한 .rtb 백업 파일을 선택하고 **열기**를 클릭합니다. 그러면 보드가 대시보드에서 사용 가능해집니다.

    ![board-import-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136353682_board-import-backup.png)

보드가 Free 팀에 위치해 있거나 보드를 Free 팀으로 이동해야 하는 경우, 다음 단계를 따르세요.

1. 프로필 #1로 Miro에 로그인합니다.
2. 프로필 #2와 보드를 공유합니다. **공유**를 클릭하세요.
   ![free-sharing-board.png](../../../../../../docs/using-miro/managing-boards/images/23122136354066_free-sharing-board.png)
3. 프로필 #2의 이메일 주소를 입력 > **초대장 보내기**를 클릭하세요.

   ![free-sharing-board-dialog.png](../../../../../../docs/using-miro/managing-boards/images/23122136354706_free-sharing-board-dialog.png)
4. 보드의 소유권을 프로필 #1에서 프로필 #2로 이전합니다. **공유** 버튼 > **공유 설정** > 프로필 #2 선택 > 드롭다운에서 **소유자**를 선택합니다.
5. 프로필 #2로 Miro에 로그인하여 보드를 확인합니다.
6. 보드를 다른 팀으로 이동합니다.

:::warning
두 번째 프로필이 Free 플랜에 있는 경우 무료 프로필을 유료 프로필로 초대하면 유료 플랜의 라이선스를 점유하게 됩니다. 이로 인해 플랜의 라이선스 수를 초과하면 추가 라이선스에 대한 요금이 부과될 수 있습니다.
:::

## 자주 묻는 질문

**보드 메뉴에서 팀으로 이동하는 옵션이 보이지 않는 이유는 무엇인가요?**

보드 소유자이면서 여러 팀의 멤버인 경우에만 보드를 팀 간 이동할 수 있습니다. 만약 당신이 보드 소유자가 아니라면, 보드를 [복제](03-how-to-duplicate-a-board.md)([보드 콘텐츠 설정](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)에서 허용된 경우)하여 복사한 보드를 이동시킬 수 있습니다.

보드 이동 옵션은 Enterprise 플랜의 경우 회사 관리자가 제한할 수도 있습니다.

**내 보드 소유권을 다른 사용자에게 어떻게 이전할 수 있나요?**

[다른 공동 작업자에게 보드 소유권을 이전하는 방법](05-how-to-transfer-board-ownership.md)을 배우세요.

**보드를 다른 팀으로 이동할 때 보드 링크가 변경되나요?**

아니요, 보드 URL은 변경되지 않습니다.

**템플릿 보드를 다른 사용자의 팀으로 이동할 수 있나요?**

네, 해당 사용자가 본인의 팀으로 초대하도록 요청한 후 보드를 이동하실 수 있습니다. 또는 [보드를 공유](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md)하고 그들이 [보드를 복제](03-how-to-duplicate-a-board.md)하여 [보드 내용 설정](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)에서 사용할 수 있게 할 수 있습니다.

**스페이스를 팀 간에 이동할 수 있나요?**

아니요, 개별 보드만 이동할 수 있습니다.

**여러 개의 보드를 일괄로 이동할 수 있나요?**

아니요, 현재는 지원되지 않습니다.

**보드를 이동하려고 했는데 아무것도 일어나지 않거나 오류 메시지가 나타납니다. 어떻게 해야 하나요?**

다른 브라우저에서 이동을 시도하거나 시크릿 모드에서 시도해 보세요. 다른 네트워크나 장치로 전환해서 시도해 볼 수도 있습니다.

다른 방법으로 [보드를 복제](03-how-to-duplicate-a-board.md)하고 복제한 보드를 이동해 보세요. 그래도 해결되지 않는다면, [Miro 지원에 문제를 보고](../tools/troubleshooting/06-contacting-miro-support.md)하세요.
