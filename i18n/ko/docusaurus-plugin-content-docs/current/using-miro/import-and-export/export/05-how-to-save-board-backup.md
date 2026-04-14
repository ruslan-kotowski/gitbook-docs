---
title: 보드 백업 저장 방법
article_id: 360017572774
translation_id: 360017572774
locale: ko-kr
sidebar_position: 5
created_at: '2019-02-11T10:14:51Z'
updated_at: '2025-12-02T10:14:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
availability:
  notes: '실행 가능한 사용자: 보드 소유자, 보드 공동 소유자, [콘텐츠 관리자 권한](../../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)을
    가진 회사 관리자 - [Enterprise 플랜](../../../plans-billing/miro-plans/04-enterprise-plan.md)
    사용 가능 플랜: Starter, Business, Enterprise, Education 사용 가능 플랫폼: 브라우저, 데스크톱'
---

보드 백업을 저장해 보드의 아카이브 사본을 만듭니다. 백업을 통해 콘텐츠의 안전성을 확보하고 다른 Miro 사용자와 보드를 공유할 수 있습니다.

## 보드 백업 저장

백업을 생성하려면:

1. 보드를 열고 **세로 세 점** (![icon-main.svg](../../../../../../../docs/using-miro/import-and-export/export/images/27743904151698_icon-main.svg)) 아이콘을 클릭합니다.
2. **보드** 하위 메뉴를 선택합니다.
3. 그런 다음 **내보내기** 하위 메뉴를 선택합니다.
4. **보드 백업 다운로드** 옵션을 선택하고 화면의 지시에 따릅니다.

![backup-entry-point.png](../../../../../../../docs/using-miro/import-and-export/export/images/21537453245330_backup-entry-point.png)
*보드 백업 다운로드*

대시보드에서도 백업을 저장할 수 있습니다. **세 점 아이콘** (**...**)을 클릭하여 보드 메뉴를 열고 옵션에서 **보드 백업 다운로드**를 선택합니다.

*.rtb* 파일은 기기에 저장됩니다.

:::warning
**보드 소유자**와 공동 소유자만 **유료** 팀의 보드 백업을 다운로드할 수 있습니다. 내보내기 메뉴에서 이 옵션이 회색으로 표시된다면, 이 기능이 [사용 중인 플랜에 포함](../../../plans-billing/miro-plans/02-plans-and-features-available.md)되어 있는지, 그리고 [보드의 소유자](../../sharing-boards/01-board-access-rights.md) 또는 [보드 공동 소유자](../../sharing-boards/06-co-owners-of-boards-and-spaces.md)인지 확인하세요.
:::

## 백업에서 보드 복원

보드 백업을 업로드하는 옵션은 유료 팀의 모든 사용자에게 가능합니다. 보드의 보관된 사본을 다른 Miro 사용자에게 보내 그들이 유료 팀에서 보드 복사본을 재생성할 수 있도록 할 수 있습니다.

백업에서 보드를 복원하려면:

1. 대시보드에서 [대시보드](https://miro.com/app/dashboard/)로 이동한 후, **새로 만들기**를 클릭합니다.
2. **가져오기**를 선택합니다.
3. 그런 다음 **백업 가져오기**를 선택합니다.
   대화상자가 나타납니다.
4. 본인의 **.rtb* 보드 백업 파일을 선택합니다.
5. 선택을 확인한 후, 동일한 콘텐츠가 있는 새로운 보드가 팀에 생성됩니다. 보드 제목에는 **복원됨**이 포함됩니다.

보드를 복원한 후에는 팀 내의 다른 스페이스로 보드를 이동할 수 있는 기능도 있습니다.

![backup-import.png](../../../../../../../docs/using-miro/import-and-export/export/images/21537453249938_backup-import.png)
*백업에서 보드 복원*

## 문제 해결

보드 백업의 다운로드와 업로드에는 제한이 있습니다. 다운로드의 경우, **1GB**의 제한이 있습니다. 보드가 그보다 크다면, 보드를 더 작은 보드로 나누거나, 다운로드된 백업 대신 [보드 버전](../../managing-boards/12-board-history-versions.md)을 사용하시기 바랍니다.

업로드의 경우, Miro 인터페이스는 최대 **1GB**의 보드 백업을 업로드할 수 있습니다. 더 큰 백업 파일을 업로드하려면, Miro 지원 팀에 문의하세요:

1. Miro에 로그인한 후 [지원 양식](../../tools/troubleshooting/06-contacting-miro-support.md)을 사용하여 요청을 제출하세요.
2. 요청에 백업 파일을 첨부하거나 클라우드 스토리지에 업로드한 후, 다운로드 가능한 링크를 보내주세요.
3. 백업 파일이 1GB 미만이지만 업로드에 문제가 있는 경우, 이 페이지의 [문제 해결 단계](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md)를 확인하세요.

백업을 업로드하는 중 **최적화된 리소스 0에 대한 기존 리소스 복제를 찾을 수 없음** 오류가 발생할 경우, 이는 보드 백업에 삭제해야 할 리소스가 포함되어 있다는 것을 의미합니다. [.*rtb* 파일을 Miro 지원](../../tools/troubleshooting/06-contacting-miro-support.md)에 보내주시면, 리소스 데이터를 삭제하여 백업이 성공적으로 업로드되도록 도와드리겠습니다.

:::note
백업 저장에 문제가 발생할 경우, [이 글](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md)의 문제 해결 단계를 시도해보세요.
:::

## 자주 묻는 질문

**보드 백업을 다운로드할 수 있는 옵션이 없어요. 왜 그런가요?**

유료 팀의 보드 소유자/공동 소유자이거나 [콘텐츠 관리자 권한](../../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)을 가진 [Enterprise 플랜](../../../plans-billing/miro-plans/04-enterprise-plan.md)의 회사 관리자만 보드 백업을 저장할 수 있습니다.

**보드가 삭제되면 어떻게 해야 하나요?**

이 가이드를 확인하세요: [삭제된 보드 복원하는 방법](../../managing-boards/08-how-to-restore-a-deleted-board.md).

**여러 보드를 일괄 백업할 수 있나요?**

현재로서는 불가능합니다. 각 보드를 개별적으로 백업해야 합니다.
