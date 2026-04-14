---
title: "\uBCF4\uB4DC \uB0B4\uBCF4\uB0B4\uAE30 \uBB38\uC81C"
article_id: 360020567820
translation_id: 360020567820
locale: ko-kr
sidebar_position: 3
created_at: '2021-03-18T12:15:46Z'
updated_at: '2025-11-05T13:45:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Miro 보드를 이미지, PDF, 또는 CSV 파일로 [내보내기](../../import-and-export/export/03-how-to-export-your-board.md)할 수 있습니다. Miro 보드를 내보내는 데 문제가 발생하면 아래의 가능한 해결책을 살펴보세요.

## 보드를 내보낼 수 없습니다

**내보내기 버튼이 보드에서 사라졌어요**

내보내기 버튼은 **세 점 아이콘** (**...**) 메뉴 아래, 그리고 **보드** 하위 메뉴에 있습니다.

보드 메뉴에 내보내기 옵션이 없습니다[보드 메뉴](../../../getting-started/start-here/your-first-board/05-toolbars.md):

1. 보드 소유자/공동 소유자가 보드 설정에서 사용자에게 내보내기를 허용했는지 확인하세요.

   보드 소유자의 이름을 확인하려면, 왼쪽 상단 구석에 있는 보드 이름을 클릭하여 보드 정보 카드를 열면 됩니다. 해당 정보를 볼 수 없는 경우, 초대 이메일에서 보드로 초대한 사용자의 이름을 확인할 수 있습니다.

   보드 소유자에게 문의하여 **공유** 창에서 **공유 설정** 옵션을 활성화해 달라고 요청하세요. > **사용 권한**. 소유자/공동 소유자는 사용자가 [보드 콘텐츠를 복사](../../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)할 수 있는지 확인해야 합니다.
   ![.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044218642_.gif.png)
   *보드 복사 권한 설정*
2. 브라우저, 플랜 및 기기가 내보내기를 지원하는지 확인하세요. 지원 여부는 아래에서 확인할 수 있습니다. 브라우저, 플랜 또는 기기가 내보내기 옵션을 지원하지 않는 경우, 다른 브라우저나 기기로 전환하거나 [팀을 업그레이드](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md)하는 것을 추천합니다.

   |  |  |  |  |  |  |
   | --- | --- | --- | --- | --- | --- |
   |  | Free 플랜 | | Starter, Business, Enterprise, Education 플랜 | | CSV로 내보내기 (모든 플랜) |
   |  | 저해상도 | 고해상도 워터마크 없는 | 저해상도 | 고해상도 워터마크 없는 |
   | Google Chrome | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Safari | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Firefox | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Opera | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Edge < 79 | ✘ | ✘ | ✘ | ✔ | ✘ |
   | [데스크톱 앱](../../../getting-started/apps-for-devices/05-desktop-app.md) | ✔ | ✘ | ✔ | ✔ | ✔ |
   | 태블릿 | ✔ | ✘ | ✔ | ✔ | ✘ |
   | 모바일 | ✘ | ✘ | ✘ | ✘ | ✘ |

**저화질 내보내기 문제**

문제를 해결하려면 브라우저 탭과 백그라운드 탭을 닫으세요. 다른 브라우저로 전환해보는 것도 좋습니다.

고화질로 내보내려면 다음 작업을 수행하세요:

- 내보내기 대상이 아닌 프레임은 숨기세요. 숨겨진 프레임의 내용은 내보내지 않습니다.
- 보드를 내보내기 위해 더 작은 보드로 분할하세요.

**일반 팁**

- 내보낼 모든 항목을 프레임에 넣으세요. 프레임 안에 포함된 위젯만 내보내집니다.
- PDF 안의 PDF를 피하세요. 보드에 PDF가 있고 이를 PDF로 내보내고자 할 경우, 보드의 PDF를 저화질 이미지로 대체하세요.
- 고해상도 이미지를 JPEG로 변환하거나 외부 도구를 사용해 크기를 줄이세요.
- 관련 사건을 확인하려면 Miro 상태 페이지를 체크하세요.
- 보드를 프레임으로 나누고 각각의 프레임을 별도로 내보내세요. 나중에 외부 도구를 사용해 개별 PDFs를 다시 결합할 수 있습니다.
- 큰 보드를 작은 보드로 나누고 [스페이스](../../spaces/01-spaces.md)를 사용해 관련된 보드를 조직화하고 그룹화하세요.

**"PDF 문서를 생성하는 중에 문제가 발생했습니다"**

보드를 프레임으로 나누어 프레임을 별도로 내보내보세요. 문제가 보드 크기 때문에 발생할 수 있습니다.

이 방법으로 해결되지 않는다면, [브라우저 콘솔 로그](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md)를 확인하세요. 로그에 다음 메시지가 포함되어 있다면:

```
ERR_CONNECTION_ABORTED
```

*위치:*

내보내기가 귀하의 기기에서 실행 중인 보안 소프트웨어 또는 네트워크 내의 방화벽에 의해 차단되었습니다.

귀하 또는 시스템 관리자가 Miro가 내보내기 작업을 수행할 수 있도록 바이러스 백신 프로그램 및/또는 방화벽의 설정을 구성해야 합니다.

궁금한 점이 있으면, [Miro 지원](../../tools/troubleshooting/06-contacting-miro-support.md)에 문의하세요.

**보드를 PDF로 내보낼 때 아무 일도 발생하지 않고 Miro에서 오류가 표시되지 않습니다**

이 알려진 문제는 주로 팝업 창이 비활성화된 Safari 브라우저에서 발생합니다. Safari의 문제를 해결하려면, [이 단계](https://support.apple.com/en-gb/guide/safari/sfri40696/mac)를 따릅니다. miro.com 또는 모든 웹사이트에 대해 팝업 창을 활성화하세요. Miro로 돌아가 보드를 내보내기를 다시 시도하세요.

Chrome을 위한 단계는, [이 단계](https://support.google.com/chrome/answer/95472?hl=en&co=GENIE.Platform%3DDesktop)를 따르세요.

## 내보낸 파일(PDF, 이미지, CSV)에서 이슈가 발생합니다

**내보낸 문서의 이미지/PDF가 흐릿하게 보이는 경우**

저장된 파일에서 업로드된 이미지나 PDF가 흐릿하다면:

1. 보드의 배율을 100%로 설정하고 이미지/PDF가 렌더링된 후에 보드를 내보냅니다
2. 업로드한 이미지/PDF가 내보내기에 너무 복잡하거나 큰 경우입니다. 파일을 줄이기 위해 이미지를 PNG 형식으로 변환하고 보드에 교체한 후 보드를 다시 내보내십시오

Free 플랜에서는 저품질로만 내보내기가 가능합니다. 보드를 고품질로 내보내야 한다면, [유료 팀으로 이동](../../managing-boards/04-how-to-move-a-board.md)하거나 [팀을 업그레이드](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md)하는 것을 권장합니다.

**페이지 순서가 보드의 프레임 순서와 다릅니다**

PDF로 내보낸 프레임의 순서는 프레임 패널에 있는 순서와 동일합니다. 프레임 순서를 변경하려면:

1. 왼쪽 하단에서 보드 개요를 엽니다
2. 프레임을 드래그하여 목록에서 그 위치를 변경합니다. 또한, [Magic 정리](../../essential-tools/07-frames.md) 기능을 사용하여 프레임을 보드에 배치된 순서대로 빠르게 정렬할 수 있습니다
   ![move_frames.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057584914_move%20frames.gif)
   *프레임 순서 변경*

**내보낸 파일이 잘렸어요**

보드를 이미지로 **내보낼 때**, 내보내기할 영역에 원하는 모든 콘텐츠가 포함되었는지 확인하세요.

![save_as_image.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057583890_save%20as%20image.gif)
*보드를 이미지로 내보내기*

보드를 PDF로 **내보낼 때**, 내보내고자 하는 모든 콘텐츠를 포함할 프레임을 생성하세요. 그런 다음 [프레임을 내보내기](../../import-and-export/export/03-how-to-export-your-board.md)하세요.

**내보낸 PDF 파일에 프레임 이름이 포함되지 않음**

보드를 PDF 파일로 내보낼 때, 프레임 제목은 내보내기에 포함되지 않습니다. 프레임에 [텍스트 도구](../../essential-tools/16-text.md)를 사용하여 제목을 대신 넣으면 해당 제목이 PDF에 표시됩니다.

**내보낸 CSV 파일의 데이터가 구조화되어 있지 않음**

현재 CSV 내보내기는 보드의 구조나 관계를 유지하지 않습니다. 그러나 [테이블](../../advanced-tools/05-grid.md)을(를) CSV 파일로 내보내면, 구조는 유지됩니다.

인텔리전트 데이터가 포함된 파일로 [마인드맵](../../advanced-tools/03-mind-map.md)를 내보내려면, [마인드맵 다운로드](https://miro.com/marketplace/mindmapdownloader/?backUrl=%2Fmarketplace%2F)를 사용하세요.

**보드의 글꼴이 내보낸 파일의 글꼴과 다릅니다**

Miro 내보내기는 귀하의 기기에 설치된 운영 체제의 글꼴을 사용합니다. 해당 글꼴이 운영 체제에 없을 경우, 시스템의 유사한 글꼴이 대신 사용됩니다. Miro 보드의 글꼴과 동일한 글꼴이 필요하다면, 보드에서 다른 글꼴을 선택하거나 필요한 글꼴을 기기에 설치하세요.

## 내보낸 파일을 찾지 못하겠습니다

**내 디바이스에서 내보낸 파일을 찾을 수 없습니다**

**브라우저에서 Miro를 사용하는 경우**

파일은 기본적으로 브라우저 다운로드가 저장되는 폴더에 저장됩니다. 브라우저 설정에서 다운로드 옵션을 확인할 수 있습니다.

**Miro 데스크톱 앱이나 태블릿 앱을 사용하는 경우**

디바이스의 다운로드 폴더를 확인하세요. 보드 이름으로 파일을 검색할 수도 있습니다.

**Miro가 보드를 내보낼 때마다 새 폴더를 만듭니다**

> **해당 대상**: [Windows 데스크톱 앱](../../../getting-started/apps-for-devices/05-desktop-app.md)

Miro 앱 설정에 경로가 저장되어 있을 수 있습니다. 경로를 삭제하려면:

1. Miro 데스크톱 앱 삭제
2. Windows 하단 왼쪽 (검색창)에서 **%AppData%** 를 입력하고 폴더 **Local,** 을 열고, 폴더 **RealTimeBoard**를 삭제합니다
3. 다시 **%AppData%** 를 열고, 폴더 **Roaming,** 으로 이동하여 폴더 **RealTimeBoard**를 삭제합니다

[최신 Miro 애플리케이션](https://miro.com/apps/) 재설치합니다.

어떤 해결책도 도움이 되지 않는 경우, [Miro 지원](../../tools/troubleshooting/06-contacting-miro-support.md)에 문의하세요.
