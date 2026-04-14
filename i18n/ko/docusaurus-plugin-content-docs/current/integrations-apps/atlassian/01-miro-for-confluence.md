---
title: Confluence용 Miro
article_id: 360020712594
translation_id: 21830704028050
locale: ko-kr
sidebar_position: 3
created_at: '2024-10-07T13:21:50Z'
updated_at: '2026-03-12T09:15:22Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: '사용 가능 대상: 모든 Miro 플랜; Confluence Cloud(Miro에 임베드), Confluence Cloud/Server/DC(Confluence에
    임베드) 실행 가능한 사용자: Confluence 관리자'
---

Miro와 Confluence는 양방향 동기화를 통해 두 플랫폼에서 최신 콘텐츠를 언제든지 이용할 수 있도록 지원합니다.

## Miro와 Confluence의 작동 방식

Miro 보드와 Confluence 문서를 임베드하고, 즉시 동기화하여 변경 사항을 추적할 수 있습니다. 임베드 액세스 수준을 설정하여 언제나 올바른 사용자가 원하는 정보를 확인할 수 있습니다.

Miro 보드에 Confluence 문서 임베드

Confluence 문서에 Miro 보드 임베드

## Miro 보드 내 Confluence 문서 임베드

Confluence 문서를 Miro 보드에 임베드하려면 단순히 링크를 복사하여 붙여넣기만 하면 됩니다. 참고로, **Miro에 Confluence 문서를 임베드하려면 Confluence Cloud가 필요합니다.**

Miro 보드에 Confluence 링크를 붙여넣으면 [Miro 스마트 링크](https://help.miro.com/hc/articles/360017730993)로 나타납니다. Confluence 링크를 처음 붙여넣을 때는 Confluence 액세스를 승인하기 위해 **연결**을 클릭해야 합니다.

:::warning
보안을 위해 공개 Miro 보드에서는 Confluence 링크의 세부 사항이 표시되지 않으며, 사용자는 비공개 보드에서만 Confluence 링크의 제목을 볼 수 있습니다. 사용자는 Confluence 계정을 승인한 후에 페이지 제목을 확인할 수 있으며, 승인 이후에 Confluence 문서를 확장하고 편집할 수 있습니다(부여된 액세스 수준의 권한에 따라 다름).
:::

![Connect_Confluence.png](https://help.miro.com/hc/article_attachments/21830703933586)*Miro에서 Confluence 페이지를 연결하는 모습*

Confluence가 승인되면 보드에 접근하는 사용자들은 이제 문서 제목, 제공자 아이콘, 링크 소스를 볼 수 있습니다. 사용자들은 Miro 스마트 링크를 전체 화면 모드로 확장할 수도 있습니다.

:::tip
Miro 스마트 링크 제목은 URL에서 추출됩니다. Confluence 문서 제목을 수정한 경우, Miro 스마트 링크에서 업데이트된 제목을 보려면 링크를 다시 붙여넣어야 합니다.
:::

![Connected_Confluence_card.png](https://help.miro.com/hc/article_attachments/21830693002898)*Miro 스마트 링크로 연결된 Confluence 페이지*

사용자가 확장 아이콘을 클릭하면, Miro 내에서 문서를 보기 및 편집하기 전에 자신의 Confluence 계정을 인증해야 합니다.

![Expanded_Confluence_card.png](https://help.miro.com/hc/article_attachments/21830693016338)*확장된 Confluence 문서*

## Confluence 문서에 Miro 보드 임베드하기

Confluence 문서에 Miro 보드를 임베드하려면 Miro Plugin for Confluence 또는 Atlassian Smart Links를 통해 직접적으로 할 수 있습니다. 이 작업은 Confluence Cloud, Server, 혹은 DC에서도 수행할 수 있습니다.

### 1단계: Miro Plugin 설정

먼저, Atlassian 마켓플레이스에서 [Miro for Confluence 앱](https://marketplace.atlassian.com/apps/1217530/miro-for-confluence?tab=reviews&hosting=cloud)을 설치하세요.

**Miro for Confluence 앱 설치 방법**

> **실행 가능한 사용자**: Confluence 관리자

1. 관리자로 Confluence 인스턴스에 로그인합니다
2. **애드온 (앱)**을 선택합니다
3. **새로운 앱 찾기** 또는 **새로운 애드온 찾기**를 선택합니다
4. **Miro for Confluence**를 검색하세요
5. **앱 가져오기**를 클릭하세요

![Miro_for_Confluence.png](https://help.miro.com/hc/article_attachments/21830703948050)*Miro for Confluence 앱*

앱이 성공적으로 설치되면 다음과 같은 메시지가 표시됩니다:

![success_message.jpg](https://help.miro.com/hc/article_attachments/21830703954194)
*앱이 성공적으로 설치되었습니다*

### 2단계: Confluence 페이지에 보드 임베드하기

Confluence 페이지에 Miro 보드를 임베드하는 방법은 세 가지입니다:

1. Confluence 문서에서 **/miro**를 직접 입력하기.
   ![Typing_miro_on_the_doc.png](https://help.miro.com/hc/article_attachments/21830703957394)
   *Confluence 페이지에서 /miro를 입력하여 보드를 임베드하는 방법*
2. 앱 툴바에서 Miro를 검색해 임베드합니다. Confluence 문서에서 **삽입**을 클릭하고 앱 목록에서 **Miro**를 선택합니다.
   ![Miro_plugin.jpg](https://help.miro.com/hc/article_attachments/21830693037330)
   *앱 목록에서 Miro를 선택해 보드를 임베드합니다*
3. Miro 링크를 Confluence에 Atlassian Smart Links로 직접 붙여넣어 임베드합니다.

### 3단계: 보드 선택기에서 보드를 선택하세요

보드 선택기가 열립니다. 임베드하고자 하는 보드를 드롭다운에서 선택하거나 검색하세요. 사용자는 Miro에서 본인이 접근할 수 있는 보드만 볼 수 있으며, 편집자 권한이 있는 경우에만 보드를 임베드할 수 있습니다.

![Board_picker.png](https://help.miro.com/hc/article_attachments/21830703968786)*보드 선택기에서 임베드할 보드를 선택하는 중*

임베드된 보드의 **시작 보기**를 선택하세요.

![Set-the-starting-view-for-your-embed.png](https://help.miro.com/hc/article_attachments/21830693041810)*임베드된 Miro 보드의 시작 보기를 설정하는 중*

Confluence 페이지의 **모든 방문자**에 대한 액세스 수준을 선택하세요.

- **보기 가능:** Confluence 페이지에 있는 모든 방문자가 보드를 볼 수 있게 합니다.
- **액세스 필요:** Miro에서 보드에 대한 액세스가 있는 사람만 보기를 제한합니다.

![Access-level-for-embed.png](https://help.miro.com/hc/article_attachments/21830693044754)*Confluence 페이지의 Miro 보드에 대한 액세스 수준 설정*

### 4단계: 보드 임베드

**보드 임베드**를 클릭하면 Miro 보드가 iFrame으로 Confluence 페이지에 삽입됩니다. 사용자는 보드를 보고 탐색할 수 있습니다.

:::note
Enterprise 플랜 사용자에게는 조직 전체의 액세스 설정이 따르므로 일부 권한이 제한될 수 있습니다. [Enterprise 플랜에 대한 임베드 보드 관리](https://help.miro.com/hc/articles/4405088016274)에 대해 자세히 알아보세요.
:::

![Miro-board-embedded-in-confluence.png](https://help.miro.com/hc/article_attachments/21830703986066)*Miro 보드가 Confluence 페이지에 임베드됨*

Miro에서 직접 보드를 열려면 Miro 로고를 클릭하세요.

![Open-embedded-board-in-miro.png](https://help.miro.com/hc/article_attachments/21830703987986)
*Miro에서 보드를 여는 옵션*

#### **Confluence Cloud와 Confluence Server의 사용자 경험**

임베드된 보드의 창 크기 메뉴는 Confluence Cloud와 Confluence Server에서 다릅니다.

Confluence Cloud에서는 창 크기 메뉴가 **전체 너비로 가기** 옵션과 함께 표시됩니다:

![Go-full-width-Miro-board-confluence.png](https://help.miro.com/hc/article_attachments/21830693059986)
*Confluence 브라우저의 창 크기 메뉴*

Confluence Server에서는 작은, 중간 또는 큰(**S/M/L**) 창 크기를 선택할 수 있는 메뉴가 표시됩니다:

![Miro_in_Confluence_Server.jpg](https://help.miro.com/hc/article_attachments/21830693062930)*Confluence 앱의 창 크기 메뉴*

## Atlassian Smart Links를 통해 Miro 보드 임베드하기

Atlassian Smart Links 기능을 사용하여 Confluence에 Miro 보드를 임베드할 수도 있습니다. 이 기능을 사용하면 앱 설치 없이 보드를 자동으로 임베드할 수 있습니다.

Confluence 페이지로 이동하여 보드 링크를 간단히 붙여넣거나 **/link**를 입력하여 삽입하세요. 기능을 처음 사용할 때는 Miro 팀과 연결하라는 메시지가 표시됩니다. **연결하여 미리보기**를 클릭하고, Miro에서 권한을 승인한 후 임베드할 보드를 위한 팀을 선택하세요.

:::note
Miro 측 임베드된 보드에 접근할 수 있는 사용자들만이 Miro와 Atlassian 계정을 연결한 후 임베드된 Miro 보드 미리보기를 사용할 수 있습니다. 모든 Confluence 사용자가 보드 미리보기를 사용할 수 있도록 하려면 Miro 앱을 사용할 수 있습니다.
:::

![install_Atllassian_links.jpg](https://help.miro.com/hc/article_attachments/21830703999634)
*임베드할 팀 선택하기*

Confluence 페이지에 Miro 보드 링크를 붙여 넣으면 자동으로 위젯으로 변환됩니다. 링크를 클릭하여 표시 옵션을 확인하세요. Miro 보드를 **URL**, **인라인** 텍스트, **카드** 또는 **임베드**로 표시할 수 있습니다.

![Confluence_widget.png](https://help.miro.com/hc/article_attachments/21830704004370)*Confluence의 Miro 보드 위젯*

보드를 임베드로 표시하는 경우, 보드의 크기를 드래그하여 조정할 수 있습니다.

![changing_embed_size.gif](https://help.miro.com/hc/article_attachments/21830693073426)
*Confluence에서 Miro 임베드 크기 조정*

:::warning
브라우저에서 타사 쿠키가 차단된 경우 임베드된 보드 표시가 예상치 못한 문제를 일으킬 수 있습니다.
:::

## Confluence용 Miro 앱 사용 중지

앱을 끄려면 **Atlassian 마켓플레이스** > **앱 관리** > **Miro for Confluence Cloud** > **제거**로 이동하세요.

*![Uninstall_Confluence_plugin.jpg](https://help.miro.com/hc/article_attachments/21830704012178)*
*설치된 Atlassian 앱 목록에 있는 Miro for Confluence 앱*

## Confluence에서의 마이그레이션 및 보드 영향

온-프레미스에서 클라우드 인스턴스로 또는 클라우드 간에 마이그레이션하는 경우에도 Miro 플러그인은 별도의 마이그레이션 단계가 필요하지 않습니다. Confluence는 URL 기반 임베드인 iFrame을 통해 Miro 보드를 표시하며, 이는 Confluence가 보드 링크만 저장하고 보드는 Miro에 그대로 남아 있음을 의미합니다.
