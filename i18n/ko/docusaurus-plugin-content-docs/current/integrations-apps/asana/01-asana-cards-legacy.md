---
title: "Asana \uCE74\uB4DC (\uB808\uAC70\uC2DC)"
article_id: 360039492573
translation_id: 360039492573
locale: ko-kr
sidebar_position: 1
created_at: '2019-11-25T10:03:42Z'
updated_at: '2025-11-25T16:05:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: asana-cards
---

:::warning
이 페이지는 레거시 Asana 통합을 설명합니다. 새로운 통합에 대해서는 [Asana (베타) 문서](asana)를 참조하세요.
:::

**주요 기능**

- Asana 작업을 Miro 보드로 가져와 팀의 진행 상황을 시각화하세요
- Asana 필터를 사용하거나 작업 이름으로 검색하여 Miro에서 직접 가져올 작업을 찾을 수 있습니다
- 자동 동기화: Asana 작업에서 발생한 모든 변경 사항이 Miro의 Asana 카드에 자동으로 반영됩니다

> **사용 가능 대상**: Starter, Business, Enterprise 플랜*관리자가 Miro 팀에 Asana 사용 권한을 부여해야 할 수 있습니다. 팀 레벨에 설치된 경우에만 팀 구성원이 Asana 카드 앱을 사용할 수 있습니다.*

### Asana 카드 설치 방법

1. 먼저, 활성화된 Miro 계정과 활성화된 Asana 계정이 필요합니다. Miro 프로필이 없는 경우, [여기](https://miro.com/signup/)에서 회원가입하세요.
2. Miro 마켓플레이스에서[Asana Cards](https://miro.com/marketplace/asana-cards/?backUrl=%2Fmarketplace%2F)*를 엽니다.* **앱 가져오기** 버튼을 클릭합니다.
   Asana를 설치할 팀을 선택하도록 요청받습니다. 팀을 선택하고 **설치 및 인증**을 클릭합니다.
   > ⚠️ 관리자가 아닌 사용자는 설정에서 앱 설치가 허용되지 않은 경우 앱을 설치할 수 없습니다.

![install_Asana_cards.jpg](../../../../../../docs/integrations-apps/asana/images/21020254087442_install%20Asana%20cards.jpg)
*Asana 카드 권한 부여*

3. 다음 단계는 Asana 카드 앱 설정에서 **연결**을 클릭하는 것입니다.

![connect_Asana_and_Miro.jpg](../../../../../../docs/integrations-apps/asana/images/21020265147410_connect%20Asana%20and%20Miro.jpg)
*팀 설정의 Asana 카드 앱 설정*
다른 팀 구성원들은 보드 작성 툴바에서 Asana 카드 아이콘을 찾을 수 있으며, 그곳에서 각자의 Asana 계정에 연결할 수 있습니다.

![Asana_cards_on_the_toolbar.jpg](../../../../../../docs/integrations-apps/asana/images/21020254085010_Asana%20cards%20on%20the%20toolbar.jpg)
*툴바의 Asana 카드*

4. Asana Connect의 Asana 계정 접근을 허용하세요. 현재 앱에 로그인되어 있지 않다면, Asana에서 인증 요청을 받을 것입니다.

**![grant_permission_to_Asana.jpg](../../../../../../docs/integrations-apps/asana/images/21020254090386_grant%20permission%20to%20Asana.jpg)*****Miro가 Asana 계정에 접근을 허용하기***

### Asana 카드를 가져와 사용하는 방법

1. Miro를 Asana 계정과 연결한 후, Miro 보드에 Asana 카드를 자유롭게 추가할 수 있습니다. 카드 선택기를 열려면 생성 바에서 **도구, 미디어 및 통합** (**+**)**을** 선택하세요. 패널이 열립니다. 'Asana 카드'를 검색하여 선택합니다.
2. 피커를 사용하면 작업을 필터링할 수 있습니다. 먼저 워크스페이스를 선택하고, 프로젝트, 태그 또는 담당자로 카드를 필터링하세요. 프로젝트 목록은 생성일 순으로 정렬됩니다.

   > ⚠️ 피커는 사용자가 Asana에서 접근할 수 있는 작업만 표시합니다. Miro 사용자가 접근할 수 없는 작업의 소스 페이지를 열면, 접근할 수 없다는 메시지가 나타납니다.

   ![Asana_picker.gif](../../../../../../docs/integrations-apps/asana/images/21020254098578_Asana%20picker.gif)
   **보드로 Asana 카드 가져오기**

카드를 Asana에서 열려면 **소스** 버튼을 클릭하세요.
![go_to_source.jpg](../../../../../../docs/integrations-apps/asana/images/21020265150226_go%20to%20source.jpg)
**카드의 소스 버튼**

Asana 카드를 [칸반](../../using-miro/advanced-tools/02-columns-formerly-kanban.md) 및 [사용자 스토리 맵](../../using-miro/advanced-tools/07-user-story-mapping.md) 프레임워크에 자유롭게 추가하려면 간단히 드래그하세요.

:::warning
아직 Miro 쪽에서는 Asana 카드의 생성이나 편집이 불가능하지만, Asana 쪽에서 이루어지는 모든 변경사항은 Miro에서 동기화됩니다(카드 업데이트에 약간의 지연이 발생할 수 있습니다).
:::

![Asana_cards_and_kanban.gif](../../../../../../docs/integrations-apps/asana/images/21020254093074_Asana%20cards%20and%20kanban.gif)
*Asana 카드를 칸반에 추가하기*

### 카드의 색상 변경

카드의 색상을 변경하려면, 카드를 클릭하고 컨텍스트 메뉴에서 **채우기 색상**을 선택하세요. 카드를 복제할 경우, 새로운 색상이 적용됩니다. ![asana_card_color.png](../../../../../../docs/integrations-apps/asana/images/21020254100242_asana_card_color.png)
*카드의 채우기 색상 변경하기*

### Asana 카드 제거 방법

팀 단위로 Asana 카드를 제거하려면, 팀 설정 **> 앱 & 통합 > Asana 카드**로 이동하여 스크롤을 내린 후, **팀용 제거**를 클릭하세요.

**개인 단위로 앱을 제거하려면,** **개인용 제거**를 클릭하세요.

![uninstall_Asna_Cards.jpg](../../../../../../docs/integrations-apps/asana/images/21020265153426_uninstall%20Asna%20Cards.jpg)
*Asana 카드 제거*

### 자주 묻는 질문

1. *어떤 IP를 Asana 카드의 허용 목록에 추가해야 하나요?*
   *-*18.203.61.162, 54.220.74.201, 54.216.81.236, 54.73.153.141, 52.215.228.26, 52.16.47.17, 54.217.180.21.
