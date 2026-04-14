---
title: 구글용 스마트 칩 및 스마트 스크린샷
article_id: 11845494577554
translation_id: 11845494577554
locale: ko-kr
sidebar_position: 11
created_at: '2023-06-06T12:19:20Z'
updated_at: '2025-08-15T13:44:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-workspace-smart-chips
availability:
  notes: '사용자: 모든 사용자 플랜: 모든 플랜 사용 가능 환경: 데스크톱, 브라우저 (Google Docs, Slides, Sheets
    사용 시)'
---

Google은 스마트 칩(Smart Chips)이라는 인터랙티브 구성 블록을 활용한 스마트 캔버스를 통해 강력한 협업 기능을 제공합니다. Google용 Miro 스마트 칩을 사용하면 Google 문서, 슬라이드 또는 스프레드시트에 직접 Miro 보드의 바로가기를 추가하여 협업 기능을 강화할 수 있습니다.

또한, Miro는 스마트 스크린샷 기능을 제공하여, Miro 보드와 위젯을 Google 문서, 슬라이드 및 스프레드시트에 이미지로 직접 붙여넣어 콘텐츠 동기화를 강화된 기능으로 유지할 수 있습니다.

![Miro smart chip board preview in Google Docs](../../../../../../docs/integrations-apps/google/images/21017516136210_miro_smart_chip_board_preview.png)
*Google 문서의 Miro 스마트 칩 애드온*

## Miro 스마트 칩 설정

다음 단계에 따라 Miro 보드 링크를 Google 문서, 슬라이드 또는 스프레드시트에 스마트 칩으로 통합하세요.

:::note
Google Workspace 조직이나 팀을 위해 Miro 애드온을 설치해야 할 수도 있습니다. 사용할 수 없는 경우 관리자에게 문의하세요. [자세히 알아보기](https://support.google.com/a/topic/1056395?hl=en&ref_topic=27380).
:::

1. Google 문서에 Miro 보드 링크를 붙여넣고 **탭** 키를 누르세요. Google이 링크가 칩 링크인지 확인합니다.
2. 여기에서 Google이 Miro의 Google 워크스페이스 애드온이 이미 설치되어 있는지 확인합니다. 그런 다음 두 가지 조치 중 하나가 수행됩니다:
   1. 이미 Google 워크스페이스 애드온이 설치되어 있는 경우, 스마트 칩을 설치할 필요가 없습니다—이미 보유하고 있습니다. 링크를 클릭하면 보드의 미리보기가 표시됩니다.
   2. 애드온이 설치되어 있지 않으면 Google 워크스페이스 마켓플레이스에서 설치하라는 프롬프트가 표시됩니다.

      > ✏️ 애드온을 설치하려면 Google 관리자에게 요청해야 할 수도 있습니다.
3. 다음으로, Google은 Miro 계정에 연결하도록 요청할 것입니다. 이는 특정 보드 정보를 표시하고 연결하려는 보드에 대한 액세스 권한이 있는지 확인하는 데 필요합니다. **Miro에 연결**을 클릭하세요.

   ![Connect Miro to Google Workspaces dialog](../../../../../../docs/integrations-apps/google/images/21017529158034_Google%20Smart%20Chips%20connect.png)
*Miro를 Google 워크스페이스에 연결 중*
4. 여기에서 두 가지 조치 중 하나가 진행됩니다:
   1. 이미 보드에 접근 허가를 받은 경우, 보드 소유자와 마지막 수정 날짜와 같은 메타데이터와 함께 보드의 미리보기가 포함된 칩이 표시됩니다.
   2. 승인이 필요하면 **액세스 요청** 버튼이 표시됩니다. 클릭하면 요청이 보드 소유자에게 전송됩니다.

      ![Miro smart chip request access to board button](../../../../../../docs/integrations-apps/google/images/21017529156882_miro_smart_chip_request_access_to_board.png)*비공개 보드에 액세스 요청*
5. 액세스가 승인되면 보드의 미리보기가 포함된 칩이 표시됩니다. 미리보기가 보이지 않으면 문서를 새로 고치세요.
6. 이제 보드가 문서에 추가되었으며, 클릭하면 Miro 보드로 이동합니다. 보드에 액세스할 수 있는 사용자는 누구나 Google 문서에서 스마트 칩을 생성할 수 있습니다.

   ![Connected Miro smart chip board link in Google Docs](../../../../../../docs/integrations-apps/google/images/21017516138642_Connecting%20Google%20Smart%20Chip.gif)
*Miro 스마트 칩 보드 링크를 Google 워크스페이스에 연결하기*

## Miro 스마트 스크린샷 사용하기

Miro 측면 패널 통합을 통해 문서를 벗어나지 않고 Google 문서, 슬라이드 또는 스프레드시트에 Miro 보드 콘텐츠를 직접 임베드할 수 있습니다. 이 기능은 Miro 보드에 원활하게 액세스할 수 있도록 하며, 강화된 기능으로 시각적 콘텐츠를 삽입할 수 있게 합니다.

### Miro 측면 패널

Google 문서, 슬라이드, 시트의 Miro 측면 패널에는 다음 기능이 포함됩니다:

- **보드 직접 액세스:** 애플리케이션을 전환하지 않고 Google 문서, 슬라이드, 시트에서 Miro 보드에 직접 액세스하세요.
- **보드 선택:** "Miro 보드 임베드 선택" 버튼을 사용해 이용 가능한 Miro 보드 중에서 선택하세요.
- **인터랙티브 프리뷰:** Miro 보드에서 삽입하기 전에 특정 콘텐츠를 보고 선택하세요.
- **정확한 배치:** 문서에서 커서가 위치한 곳에 정확히 콘텐츠를 삽입하세요.
- **스마트 기능:** 임베드된 콘텐츠는 원본 Miro 보드와의 연결을 유지합니다.

### Miro 측면 패널 사용 방법

1. Google 문서, 슬라이드, 시트에서 Miro 콘텐츠를 삽입할 위치에 커서를 놓으세요.
2. Miro 통합 아이콘을 클릭해 오른쪽 측면 패널을 여세요.
   ![Screenshot 2025-07-11 at 11.05.03.png](../../../../../../docs/integrations-apps/google/images/28006926984466_Screenshot%202025-07-11%20at%2011.05.03.png)
3. **Miro 보드 임베드 선택**을 클릭하여 사용 가능한 Miro 보드를 선택하세요.
   ![Screenshot 2025-07-11 at 11.09.05.png](../../../../../../docs/integrations-apps/google/images/28006941150482_Screenshot%202025-07-11%20at%2011.09.05.png)
4. 보드 미리보기에서 임베드할 특정 영역, 프레임, 또는 콘텐츠를 찾아 선택하세요.
   ![Screenshot 2025-07-11 at 11.10.17.png](../../../../../../docs/integrations-apps/google/images/28006926986130_Screenshot%202025-07-11%20at%2011.10.17.png)
5. 드롭다운 옵션을 사용하여 다른 보기 설정이나 선택 항목을 선택하세요.
6. **확인**을 클릭하여 커서 위치에 콘텐츠를 삽입하세요.

임베드된 콘텐츠는 원본 Miro 보드와 스마트 칩 연결을 통해 문서에 스크린샷으로 나타납니다.

:::note
**참고:** Miro 측면 패널을 사용하려면 Miro Google 워크스페이스 애드온이 설치되어야 합니다. 이 기능은 Google 문서, Google 슬라이드, Google 스프레드시트 모두에서 작동합니다.
:::

## 애드온을 관리자로 관리하기

Miro 애드온을 관리하는 Google 워크스페이스 관리자라면 다음 사항을 검토하세요:

1. Google 워크스페이스 애드온은 Google 측에서만 설치하거나 제거할 수 있습니다.
2. Google 스마트 칩에 대한 액세스를 제한하려면 Google 측에서만 수행할 수 있습니다. Miro는 사용자가 스마트 칩을 설치하고 사용하는 것에 대해 제어할 수 없습니다.

## 자주 묻는 질문

Google의 Miro 스마트 칩에 대한 자주 묻는 질문에 대한 답변입니다.

Miro 스마트 칩과 Miro 측면 패널의 차이점은 무엇인가요?

스마트 칩은 Google 문서 내에서 Miro 보드로의 클릭 가능한 링크를 생성하고, Miro 측면 패널은 Miro 보드의 시각적 콘텐츠를 직접 Google 문서와 슬라이드에 임베드할 수 있도록 합니다. 측면 패널은 문서를 벗어나지 않고도 특정 보드 콘텐츠를 선택하고 삽입할 수 있는 통합된 방법을 제공합니다.

어떤 Google Workspace 애플리케이션이 Miro 통합을 지원하나요?

스마트 칩은 Google 문서와 함께 작동하고, Miro 측면 패널은 Google 문서와 슬라이드 모두에서 작동합니다. Google Sheets에 대한 지원은 Google에서 결정하며, 업데이트는 도움말 센터에서 확인하세요.

스마트 칩은 어떤 유형의 링크와 작동하나요?

Google용 Miro 스마트 칩은 Miro 보드 및 보드 오브젝트에 대한 링크를 지원합니다.

임베드된 Miro 보드 요소는 어떻게 업데이트되나요?

Miro 측면 패널을 통해 임베드된 콘텐츠는 원본 Miro 보드와 연결을 유지합니다. 자동으로 동기화되지는 않지만 임베드된 콘텐츠를 새로 고쳐서 Miro 보드의 최신 버전이 반영되도록 할 수 있습니다.

Google 문서 측면 패널은 어떻게 작동하나요?

Google 문서의 측면 패널은 문서를 벗어나지 않고도 Miro 보드에 직접 액세스할 수 있게 합니다. Miro 통합 아이콘을 클릭해 오른쪽 측면 패널을 열고, "Miro 보드 임베드 선택"을 사용해 이용 가능한 보드 중에서 선택하세요. 패널을 사용하면 특정 영역이나 프레임을 미리 보고 선택한 후 문서의 커서 위치에 삽입할 수 있습니다.
