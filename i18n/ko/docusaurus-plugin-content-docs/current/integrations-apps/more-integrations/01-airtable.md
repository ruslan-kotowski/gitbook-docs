---
title: Airtable
article_id: 360012807619
translation_id: 360012807619
locale: ko-kr
sidebar_position: 1
created_at: '2020-03-24T12:09:00Z'
updated_at: '2025-08-05T07:33:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '사용자: 모든 Miro 사용자, 유료 Airtable 플랜 사용자 Miro 플랜: 모든 플랜 플랫폼: 브라우저'
---

Airtable을 사용할 때 화이트보드 시각화의 힘을 업무에 활용하세요! Miro에서 데이터를 Airtable로 내보내고 Airtable의 베이스에 Miro 보드를 임베드하여 Airtable 내에서 직접 보거나, 댓글을 달거나, 편집할 수 있습니다.

## Miro 보드에서 Airtable로 데이터 내보내기

Airtable Sync 통합 기능을 사용하면 Miro 보드에서 데이터를 내보내고(예: 스티커 메모, 카드) Airtable에서 이를 정리할 수 있습니다. 이 기능에 대한 설정 및 사용 방법을 알아보려면 [Airtable의 공식 문서](https://support.airtable.com/docs/airtable-sync-integration-miro)를 방문하세요.

## Airtable 베이스에 Miro 보드 임베드하기

### Airtable에 Miro 앱 설치하기

:::warning
Miro 앱은 **Safari** 브라우저에서 사용할 수 **없습니다**.
:::

Airtable의 베이스 편집자는 Miro 앱을 설치할 수 있습니다. 이를 수행하려면:

1. Airtable 베이스를 열고 오른쪽 상단 모서리의 **확장 프로그램**을 클릭합니다.

   ![](../../../../../../docs/integrations-apps/more-integrations/images/21017651877394_Airtable%20extensions.jpg)오른쪽 상단 모서리에 있는 Airtable 확장 프로그램 버튼." >
   *Airtable 베이스의 오른쪽 상단 모서리에 있는 확장 프로그램 버튼.*
2. **확장 프로그램 추가**를 클릭하세요.

   ![Airtable에서 확장 프로그램 추가 옵션.](../../../../../../docs/integrations-apps/more-integrations/images/21017647938834_add%20an%20extension.jpg)
   *새 확장 프로그램을 추가하는 옵션.*
3. Airtable 마켓플레이스에서 "Miro"를 검색하고 **추가**를 클릭하세요.

   ![Miro 앱 in Airtable 마켓플레이스.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933714_Miro%20in%20Airtable.jpg)
   *Airtable 마켓플레이스의 Miro 앱.*

### 기존 Miro 보드를 Airtable 베이스에 추가하기

Miro 앱이 Airtable 베이스에 추가되면, 확장 프로그램 패널에 나타나는 Miro 앱 섹션에서 **보드 추가**를 클릭하세요.

![Airtable에서 Miro 보드 추가 버튼.](../../../../../../docs/integrations-apps/more-integrations/images/21017651876498_add%20a%20Miro%20board.jpg)
*Airtable에서 Miro 앱을 통해 Miro 보드 추가하기.*

Miro 보드 선택기가 나타납니다. 브라우저에서 이미 Miro에 로그인하지 않은 경우, 로그인 또는 Miro 계정 생성을 하라는 메시지가 표시됩니다.

보드를 선택한 후, 드롭다운 메뉴를 사용하여 Airtable에서 표시될 공유 권한을 설정하세요. 세 가지 옵션이 있습니다:

- **누구나 볼 수 있음:** Airtable에서는 누구나 임베드된 보드의 콘텐츠를 [볼 수](../../using-miro/sharing-boards/01-board-access-rights.md) 있습니다.
- **누구나 댓글 작성 가능:** Airtable에서는 누구나 임베드된 보드에 [댓글을 남길 수](../../using-miro/sharing-boards/01-board-access-rights.md) 있습니다. (참고: 이 옵션은 Miro [Free 플랜](../../plans-billing/miro-plans/09-free-plan.md)에 저장된 보드에는 사용할 수 없습니다.)
- **비공개:** 보드는 Miro 측에서 설정된 기존의 공유 설정을 따릅니다.

  > ✏️ Miro [Enterprise 플랜](../../plans-billing/miro-plans/04-enterprise-plan.md) 사용자의 경우, 액세스 설정은 조직 전체의 액세스 제어를 따르며, 일부 공유 옵션이 제한될 수 있습니다. 자세히 알아보기: [임베드 통합을 위한 Enterprise 공유 정책 관리하기](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).

![Airtable에 Miro 보드를 추가할 때 공유 설정 옵션.](../../../../../../docs/integrations-apps/more-integrations/images/21017651879826_board%20access%20in%20Airtable.jpg)
*Airtable에 Miro 보드를 추가할 때 공유 설정*.

임베드된 Miro 보드는 이후 Airtable 베이스에 표시되며, 설정된 권한에 따라 볼 수 있고, 댓글을 달거나 편집할 수 있습니다.

![Embedded Miro board within an Airtable base.](../../../../../../docs/integrations-apps/more-integrations/images/21017651872402_Miro%20board%20in%20Airtable.jpg)
*Airtable에 임베드된 Miro 보드.*

임베드된 보드를 다른 보드로 교체하려면, Airtable의 Miro 앱에서 기어 아이콘(**설정**)을 클릭하고, **보드 선택**을 선택한 뒤 Miro 선택기에서 다른 보드를 선택하세요.

![Airtable에서 임베드된 Miro 보드 교체.](../../../../../../docs/integrations-apps/more-integrations/images/21017647932690_replacing%20a%20board.jpg)
*Airtable에서 임베드된 Miro 보드 교체.*

### Airtable에서 새 Miro 보드 만들기

Airtable에서 직접 새 Miro 보드를 만들려면 다음을 수행하세요:

1. Airtable의 Miro 앱 섹션에서 **보드 추가**(또는 보드가 이미 임베드되어 교체하는 경우 **보드 선택**)를 클릭하세요.
2. Miro 선택기에서 **새 보드** 만들기 옵션을 선택하세요.

![Airtable 내 선택기에서 새 Miro 보드 만들기.](../../../../../../docs/integrations-apps/more-integrations/images/21017651880466_add%20a%20new%20board%20to%20Airtable.jpg)
*Airtable 선택기에서 새 Miro 보드 만들기.*

새 보드는 Miro 계정에 생성되어 Airtable 베이스에 임베드됩니다.

### Airtable에서 Miro 보드 제거하기

Airtable 베이스에서 임베드된 Miro 보드를 제거하려면, 해당 베이스 내에서 Miro 앱 확장 프로그램을 제거하거나 재구성해야 합니다. 확장 패널에서 Miro 앱의 드롭다운 메뉴를 클릭하고 확장 프로그램을 제거하거나 관리하는 옵션을 선택하세요.

![Airtable 확장 프로그램 패널에서 Miro 앱 삭제.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933074_deleting%20the%20app.jpg)
*Airtable 확장 프로그램 패널에서 Miro 앱 삭제.*
