---
title: "\uB514\uC2A4\uD50C\uB808\uC774\uB85C \uC804\uC1A1"
article_id: 4406230245010
translation_id: 34703702380306
locale: ko-kr
sidebar_position: 10
created_at: '2026-04-10T12:06:03Z'
updated_at: '2026-04-10T12:06:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: interactive-displays
---

즉시 협업을 시작하세요. "Send to display" 기능을 사용하여 어떤 Miro 보드라도 인터랙티브 디스플레이에 실행하세요.

> ***Miro 유저 인터페이스 업데이트 점진적 출시***
> Miro는 보드를 보다 포괄적이고 직관적으로 만들기 위해 유저 인터페이스를 개선하고, 프로젝트의 진화인 스페이스를 도입하고 있습니다. 이번 업데이트는 몇 주에 걸쳐 모든 Miro 계정에 점진적으로 적용될 예정입니다.
>
> 이미 향상된 UI와 스페이스 레이아웃을 가지고 있는 경우, 이 문서에서 설명하는 진입점이 변경되었을 수 있습니다.
>
> 가장 최신의 문서를 보려면 [Miro의 새로운 간소화된 유저 인터페이스](../../using-miro/working-on-the-board/02-miro's-new-simplified-user-interface.md)를 참조하세요.
>
> 이번 업데이트가 완료되면 이 문서는 업데이트될 예정입니다.

인터랙티브 디스플레이에 Miro를 설정하는 방법을 [배우세요](07-interactive-displays.md).

## Send to Display 사용 방법

1. 인터랙티브 디스플레이에서 Miro 앱을 열거나 브라우저를 열고 [miro.com/displays](https://miro.com/displays/)로 이동합니다.
2. 개인 장치에서 Miro 보드를 엽니다.

**노트북 또는 태블릿에서**

1. 노트북 또는 태블릿의 Miro 보드에서 보드 바에 있는 세 점 아이콘을 선택합니다.
   **주** 메뉴가 열립니다.
2. **인터랙티브 디스플레이로 보내기**를 선택합니다.
3. 인터랙티브 디스플레이에 표시되는 고유한 페어링 코드를 입력합니다. 이렇게 하면 노트북 또는 태블릿에서 디스플레이로 보드가 전송됩니다.

**모바일 기기에서**

:::note
모바일 기기를 사용하는 경우, 먼저 [iOS](https://apps.apple.com/us/app/miro-collaborative-whiteboard/id1180074773) 또는 [Android](https://play.google.com/store/apps/details?id=com.realtimeboard&hl=en&gl=US) 용 Miro 모바일 앱을 다운로드하세요.
:::

1. 모바일 기기에서 Miro 보드를 열고 오른쪽 상단의 **설정** 아이콘을 탭하세요.
   **![board_settings.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967840616850_board%20settings.jpg)**
   *모바일 앱에서 보드 설정 열기*
2. **인터랙티브 디스플레이로 보내기**를 탭합니다.
   **![send_to_interactive_display.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967865515794_send%20to%20interactive%20display.jpg)**
   ***모바일 앱에서 인터랙티브 디스플레이로 보내기 옵션***
3. 인터랙티브 디스플레이에 표시되는 고유 페어링 코드를 입력합니다. 그러면 모바일 기기의 보드가 디스플레이로 전송됩니다.
   ![enter_code.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967892004114_enter%20code.jpg)
   *코드를 입력하는 옵션*

:::tip
세션이 끝난 후에는 데이터를 보호하기 위해 디스플레이에서 로그아웃하는 것을 잊지 마세요. 깜빡한 경우, 15분 이상 활동이 없으면 자동으로 로그아웃됩니다.
:::

## 문제 해결

Windows 데스크톱 앱에서 화면에 보드 보내기 옵션이 보이지 않는 경우 다음의 문제 해결 단계를 시도해보세요.

1. [데스크톱용 Miro 앱](https://miro.com/apps/)을 설치합니다.
2. Miro 데스크톱 앱 아이콘을 마우스 오른쪽 버튼으로 클릭하고, **속성**을 선택합니다.
   ![properties.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4949111804946_properties.jpg)*Miro 앱 속성*
3. **바로가기** 탭으로 전환하여, 아래 플래그를 CLI 인자로 **대상** 필드에 추가하고, 확인을 눌러 변경사항을 적용하세요.

   ```
   --public-device
   ```

   ![target_field.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4949083211538_target%20field.jpg)*Miro 속성의 바로가기 탭*
4. 이제 앱을 실행할 때마다 보통 송출 옵션이 기본으로 표시됩니다.

:::tip
Miro가 지원하는 [인터랙티브 디스플레이](07-interactive-displays.md)에 대해 자세히 알아보시고, [하이브리드 협업을 위한 적합한 디스플레이 선택 방법](09-selecting-the-right-interactive-display-for-hybrid-collaboration.md)에 대해 읽어보세요.
:::
