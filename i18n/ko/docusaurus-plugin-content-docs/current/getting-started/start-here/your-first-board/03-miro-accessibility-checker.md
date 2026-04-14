---
title: "Miro \uC811\uADFC\uC131 \uAC80\uC0AC\uAE30"
article_id: 19479150111378
translation_id: 19479150111378
locale: ko-kr
sidebar_position: 3
created_at: '2024-06-11T13:49:03Z'
updated_at: '2025-07-30T17:01:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: accessibility
---

Miro의 사명 핵심에는 모두를 위한 접근성 보장이 포함되어 있습니다. Miro는 누구나 참여할 수 있는 경험을 만드는 데 도움이 되는 도구를 개발했습니다. Miro 접근성 검사기는 Miro 보드가 최대한 포용적이고 접근 가능하도록 도와주기 위해 설계되었습니다.

## Miro 접근성 검사기란 무엇인가요?

Miro 접근성 검사기는 모든 사용자가 접근성 장벽에 구애받지 않고 효과적으로 협업할 수 있도록 지원하는 혁신적인 도구입니다. 여러분의 Miro 보드에서 접근성 표준에 맞지 않을 수 있는 부분을 식별하기 위해 다양한 검사를 수행하며, 모든 사용자를 위해 콘텐츠를 개선할 수 있는 실행 가능한 인사이트를 제공합니다.

## Miro 접근성 검사기를 사용하는 이유는 무엇인가요?

접근 가능한 경험을 만드는 것은 단지 규정 준수에 관한 것이 아닙니다. Miro 접근성 검사기는 모든 참여자가 자신의 접근성 요구에 관계없이 끊김 없고 매력적인 경험을 가질 수 있도록 가이드하여 더 포용적인 콘텐츠를 만드는 데 도움을 줍니다.

## Miro 접근성 검사기를 사용하려면:

1. **세로 세 점 아이콘** (![icon-main.svg](../../../../../../../docs/getting-started/start-here/your-first-board/images/28438530164626_icon-main.svg)) 메뉴 > **접근성** > **접근성 검사기**.![new-accessibility-checker.png](../../../../../../../docs/getting-started/start-here/your-first-board/images/28438515675410_new-accessibility-checker.png)
   *접근성 검사기는 보드 툴바 > 메인 메뉴 > 접근성 > 접근성 검사기에서 찾을 수 있습니다*
2. Miro 접근성 검사기가 보드를 자동으로 스캔하여 잠재적인 접근성 문제를 찾아냅니다. 이에는 색 대비, 이미지 설명, 프레임 제목에 대한 검사가 포함되어, 모든 사용자가 콘텐츠를 인식할 수 있도록 보장합니다.
3. 스캔이 완료되면, 검사기가 발견한 내용을 자세한 보고서로 제시할 것입니다. 이 보고서는 식별된 이슈를 해결하는 방법에 대한 구체적인 권장 사항을 포함하고 있습니다. 보고서는 이슈를 두 가지 범주로 나눕니다: 설명과 색상 대비.
   ![Accessibility checker shows 4 accessibility issues found on the board](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175122578_f4530230-4f9f-4155-b801-1554c1393a56.png)*접근성 검사기에서 4개의 접근성 이슈가 보드에서 발견되었습니다.*
4. 체커의 권장 사항을 따라 보드를 수정하세요. 색상을 조정하거나 객체에 설명을 추가하는 작업이 필요할 수 있습니다.
5. 선택한 이슈를 활성화하면 보드에서 해당 이슈로 이동하여 손쉽게 변경할 수 있습니다.
   ![보드에 대조가 불충분한 텍스트 개체가 선택되었습니다](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175123346_8f32a246-8d3d-4558-8a3d-d5adf1167df7.png)
   *보드에서 대비가 부족한 텍스트 오브젝트가 선택되었습니다*
6. 제안된 조정을 마친 후, 접근성 검사기를 다시 실행해 모든 이슈가 해결되었는지 확인할 수 있습니다.![Accessibility checker shows no issues](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175124114_4522a346-c8de-44a5-b79f-60f8ce5cc9cc.png)
   *접근성 검사기에 문제가 없습니다*

## 접근성 점검

현재 Miro 보드에서 네 가지 접근성 검사가 지원됩니다.

### 색상 대비

색상 대비는 두 색상 간의 밝기 또는 명도 차이로 정의됩니다. 비율이 너무 낮으면 두 색상을 구별하기 어렵거나 불가능할 수 있습니다. 이로 인해 일부 사용자가 Miro 보드에서 텍스트나 도형을 인식하는 데 어려움을 겪을 수 있습니다. 현재 W3C WCAG 2.2 AA 지침은 다음과 같습니다.

- 텍스트는 배경 대비가 최소 4.5:1이어야 합니다![Text with insufficient contrast saying Future is accessible and marked Fail, same text with sufficient contrast marked Pass](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175125522_ff02eeb3-c357-41b9-8c15-f8e17f7affa5.png)
  *대비가 부족한 텍스트 "미래는 접근 가능합니다"가 "실패"로 표시되고, 충분한 대비의 동일 텍스트가 "통과"로 표시됩니다*
- 그래픽 요소는 배경에 대해 최소 3:1의 비율을 가져야 합니다![An arrow with insufficient contrast marked Fail, same arrow with sufficient contrast marked Pass](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175127314_88063df8-8a9d-4191-ac09-6e18f6cb9e74.png)
  *대비가 부족한 경우 "실패"로 표시된 화살표, 대비가 충분한 경우 "성공"으로 표시된 동일한 화살표*

### 이미지 설명

- 이미지 설명은 스크린 리더와 음성 제어 같은 보조 기술에 정보를 제공하여 사용자에게 전달할 수 있도록 합니다.

![이미지 설명 대화 상자. 보드에서 이미지를 선택하고, Ctrl+Enter를 눌러 컨텍스트 메뉴로 포커스를 이동한 후, 오른쪽 화살표를 눌러 설명 버튼에 도달합니다](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175127954_618517d6-3d09-40f9-a9a1-40542fb9181c.png)
*이미지 설명 대화 상자. 보드에서 이미지를 선택하고 Ctrl+Enter 키를 눌러 포커스를 컨텍스트 메뉴로 이동한 다음 오른쪽 화살표 키를 눌러 Description 버튼에 도달하세요*

### 프레임 제목

- 프레임 제목을 제공하면 사용자가 Miro 보드를 보다 쉽게 탐색할 수 있습니다.

![실패로 표시된 이름 없는 프레임, Intro로 레이블된 같은 프레임은 통과로 표시됨](../../../../../../../docs/getting-started/start-here/your-first-board/images/19479175129106_89f69207-a0ac-4bfd-b3ee-1255b23e6c1d.png)

*이름 없는 프레임이 '실패'로 표시되고, 같은 프레임이 '소개'로 레이블되어 '통과'로 표시됨*

## 이슈 분류

Miro 접근성 검사기의 이슈는 두 가지 명확한 중요도 수준으로 분류됩니다:

- 매우 심각 사용자가 보드를 효과적으로 사용할 수 없게 만드는 차단 영향을 주는 이슈입니다.
- 심각한 보조 기술 사용자에게 부정적인 영향을 미칠 수 있는 사용자 경험 관련 이슈

Miro 접근성 검사기를 사용하더라도 모든 접근성 이슈를 잡아내지는 못하며, 모든 사용자가 Miro 보드를 접근 가능하도록 하기 위해 추가적인 조치가 필요할 수도 있습니다. 더 많은 정보는 접근 가능하고 포용적인 Miro 경험을 만드는 방법에 대한 가이드를 참고하세요.

## 지원되는 오브젝트

- 스티커 메모
- 텍스트
- 도형
- 선 그리기
- 연결선
