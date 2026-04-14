---
title: "\uAD6C\uAE00 \uB4DC\uB77C\uC774\uBE0C"
article_id: 360017731253
translation_id: 360017731253
locale: ko-kr
sidebar_position: 6
created_at: '2019-02-11T10:14:01Z'
updated_at: '2025-01-13T14:51:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-drive-onedrive
---

**Google 드라이브를** 사용하면 파일을 온라인으로 안전하게 저장하고, 어디에서나 액세스하고, 다른 사용자와 협업할 수 있습니다. Google 드라이브 통합을 사용하면 보드에서 작업에 집중하고 문서를 쉽게 추적할 수 있습니다.

![Google_Drive_on_the_Upload_menu.jpg](https://help.miro.com/hc/article_attachments/21857818106386)

> **설정 기준:** 각 사용자를 별도로 (관리자는 관리자가 아닌 사용자가 앱 설치를 제한할 수 있음)
> **사용 가능 환경:** 브라우저 버전, [데스크톱](../../getting-started/apps-for-devices/05-desktop-app.md) 앱(전체 기능 및 파일 편집), [태블릿 앱](../../getting-started/apps-for-devices/11-tablet-app.md), [모바일](../../getting-started/apps-for-devices/08-mobile-app.md) 앱(제한된 기능, 편집 기능은 지원되지 않음)

### Google 드라이브 활성화

Google Drive에서 파일을 추가하려면 플러그인을 설치하고 Google 드라이브를 Miro에 연결해야 합니다.

:::warning
관리자 이외의 사용자는 **앱 및 통합** 설정에서 허용되지 않는 앱을 설치할 수 없습니다.
:::

[Miro 마켓플레이스에서](https://miro.com/marketplace/google-drive/?backUrl=%2Fmarketplace%2F) 앱을 설치하세요. **앱** 받기를 클릭하면 플러그인을 설치할 팀을 선택하라는 메시지가 *표시됩니다.install_Google_Drive.jpgGoogle 드라이브 플러그인을 설치할 때 팀 선택하기*altalt![](https://help.miro.com/hc/article_attachments/21857834430098)

보드에서 플러그인을 설치할 수도 있습니다. 제작 툴바에서 화살표를 클릭하고 **Google Drive를** 검색한 다음 **추가를** 선택하세요. 팝업 창에서 **앱** 받기를 클릭하세요.

![Google_Drive_on_the_toolbar.jpg](https://help.miro.com/hc/article_attachments/21857834432274)

그런 다음 Google 드라이브를 Miro에 연결하세요. 간단한 방법은 두 가지가 있습니다.

1.  **프로필 설정으로** 이동하세요. 보드 왼쪽 상단 모서리의 톱니 바퀴를 클릭하거나 대시보드에서 프로필 아이콘을 클릭하고 **설정을** 선택하세요. 그런 다음 통합 탭을 클릭하고 **Google 드라이브를** 찾고 **연결을** 클릭하세요.

![connect_Google_Drive.jpg](https://help.miro.com/hc/article_attachments/21857834433810)*통합 페이지의 Google 드라이브*

2. 툴바의 **업로드** 메뉴에서 **Google 드라이브를** 클릭해 보드 내에서 Miro 프로필을 Google 드라이브에 연결하세요.

![Google_Drive_on_the_Upload_menu.jpg](https://help.miro.com/hc/article_attachments/21857818106386)*툴바의 Google 드라이브 아이콘*

필요한 Google 계정에 대한 인증 확인 및 앱이 파일에 액세스하도록 **허용:**

![permissions.jpg](https://help.miro.com/hc/article_attachments/21857834437266)
*Google 드라이브 권한*

이는 Google Drive의 표준 권한임을 유의하세요.

- 보드의 Google 드라이브 파일 선택기를 위해 **모든 Google 드라이브 파일을 보고** 다운로드하세요. Google 드라이브에서 Miro로 문서를 가져올 수 있습니다

- **이 앱과 함께 사용하는 특정 Google 드라이브 파일만 확인, 편집, 생성 및 삭제** - Miro 보드를 Google 드라이브에 저장할 수 있습니다.

Google 드라이브 애플리케이션은 드라이브에서 만든 파일(보드 링크 등)만 관리합니다.  Miro는 Google 드라이브 내의 콘텐츠를 관리할 수 있는 기회가 없습니다. 통합을 구현하려면 **Google Drive API** v3를 사용하세요. 이 API에서는 쓰기 액세스 권한을 전체 디스크 액세스 권한과 별도로 요청할 수 없는 방식으로 범위가 그룹화됩니다. 살펴보고 싶다면 Google 문서 의 권한인 [Google API 범위를](https://developers.google.com/identity/protocols/googlescopes) 확인하세요.

Miro에 연결된 Google 계정을 변경해야 하는 경우 **프로필 설정** > **통합으로** 이동한 다음 **Google 드라이브** 옆의 **로그아웃을** 클릭하고 다른 계정에 연결하세요.

![Google_Drive_log_out_in_settings.jpg](https://help.miro.com/hc/article_attachments/21857818118418)*프로필 설정의 Google 드라이브 연결*

### Google 드라이브 및 공유 드라이브에서 파일 추가하기

> **사용 가능 환경:** 브라우저 버전, [데스크톱 앱](../../getting-started/apps-for-devices/05-desktop-app.md), [태블릿 앱](../../getting-started/apps-for-devices/11-tablet-app.md), [모바일](../../getting-started/apps-for-devices/08-mobile-app.md) 앱(제한된 기능)

:::warning
Miro 보드에 액세스할 수 있는 모든 사용자는 Google 측에서 제한되어 있더라도 가져온 문서를 추출할 수 있습니다. 파일을 보호하려면 문서에 액세스할 수 없는 개인과 보드를 공유하지 않는 것이 중요합니다.
:::

Google 드라이브에서 파일 추가하기:

1. 문서 URL을 보드에 바로 붙여넣습니다. URL을 [도형이나](../../using-miro/essential-tools/11-shapes.md) [스티커](../../using-miro/essential-tools/14-sticky-notes.md) 메모에 붙여넣으면 문서가 보드에 삽입되지 않고 링크가 단순 텍스트로 추가된다는 점에 유의하세요. Google 스프레드시트에서 특정 시트에 대한 링크를 복사해 Miro 보드에 붙여넣으면 붙여넣은 스프레드시트는 여전히 Miro의 첫 번째 페이지에서 시작됩니다.

   또는:
2. 툴바에서 **업로드** 버튼을 클릭하고(위 스크린샷에 표시) **Google 드라이브를** 선택하세요. 그러면 선택기 메뉴가 표시됩니다. 추가하려는 모든 문서를 선택하고 **선택을** 클릭하세요. 검색 표시줄을 사용해 Google Drive에서 문서를 찾을 수도 있습니다.

:::tip
[모바일](../../getting-started/apps-for-devices/08-mobile-app.md) 앱의 보드에 Google 드라이브 문서를 추가하려면 업로드 메뉴를 통해 문서 URL을 붙여넣으세요.
:::

![select_a_file_in_Google_Drive.gif](https://help.miro.com/hc/article_attachments/21857834442386)*Google Drive에서 문서 선택하기*

**공유 드라이브에서** 문서 추가 - 탭으로 전환하고 파일을 선택하세요.

![team_drive.jpg](https://help.miro.com/hc/article_attachments/21857818121234)*Google 드라이브 선택기의 팀 드라이브*

### Google 문서 편집

> **사용 가능 환경:** 브라우저 버전, [데스크톱 앱](../../getting-started/apps-for-devices/05-desktop-app.md)

Google 문서, 스프레드시트, 슬라이드를 보드에 바로 임베드하고, 이동 및 크기를 조정하고, 문서의 페이지를 스와이프할 수 있습니다.

문서를 클릭하면 페이지 전환, 페이지 **고정,** **페이지** 추출, 콘텐츠 **편집,** **다시 로드**, **업데이트** 또는 **소스로** 이동하는 옵션이 포함된 컨텍스트 메뉴가 표시됩니다.

문서 편집을 시작하려면 컨텍스트 메뉴에서 펜 아이콘을 클릭하거나 문서를 두 번 클릭하세요. 문서가 팝업으로 열리고 Google 드라이브처럼 편집할 수 있습니다. **편집을** 완료하려면 닫기 또는 회색 영역을 클릭하세요. 모든 변경 사항은 자동으로 저장되고 보드와 Google 문서에 표시됩니다.

![google_drive_edit_docs.gif](https://help.miro.com/hc/article_attachments/21857834445970)*내장 Google 문서 편집하기*

원하면 **소스** 버튼을 클릭해도 되며 다음 탭에서 문서를 편집할 수 있도록 열립니다.

Google 드라이브에서 직접 편집한 경우(특히 오프라인으로 작업할 때) 컨텍스트 메뉴에서 **업데이트** 버튼을 사용해 보드의 임베드를 새로 고치세요. 내장 Google 드라이브 파일은 Miro 보드에서 자동으로 업데이트되지 않습니다(파일이 Miro에서 편집되지 않은 경우).

![update_button.jpg](https://help.miro.com/hc/article_attachments/21857834447250)*업데이트 버튼*

### 액세스 권한 관리

Google Drive 및 Miro의 액세스 권한은 *별도로* 설정되어 있습니다. 즉, 누군가 보드에서 Google 문서를 편집하려면 *편집자의* 권한으로 문서를 Google 드라이브에서 공유하고 [*편집자로* 보드에](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) 초대해야 합니다.

다른 사용자가 Google에서 문서를 편집할 수 있도록 허용했지만 [보기 또는 댓글 작성](../../using-miro/sharing-boards/01-board-access-rights.md) 권한으로만 보드에 초대하면 문서의 편집 모드를 활성화할 수 없습니다. 그 반대로, 사용자를 편집자로 보드에 초대했지만 Google 드라이브에서 문서를 공유하지 않으면 Google에서 편집할 수 없습니다.

성공적인 협업을 위해 필요한 액세스 수준이 제공되었는지 확인하세요.

### 보드 Google 드라이브에 저장하기

> **설정 기준:** 보드 소유자

**내보내기** 아이콘 > **Google 드라이브에 저장을** 클릭하면 문서 중 하나와 마찬가지로 드라이브에서 보드를 사용할 수 있습니다.

![export_menu_export_to_google_drive.png](https://help.miro.com/hc/article_attachments/21857818125714)
*Google Drive에서 보드 링크 만들기*

Google 드라이브에서 이제 저장된 보드를 클릭하면 별도의 브라우저 탭에서 열립니다. Google 드라이브에서 보드를 삭제해도 Miro에서 계속 사용할 수 있습니다. 그러나 Miro에서 보드를 삭제하면 더 이상 Google Drive에서 보드에 액세스할 수 없습니다.

:::warning
보드 소유자가 아닌 경우 아래와 같은 오류 메시지가 표시됩니다.
:::

![Google_Drive_error.jpg](https://help.miro.com/hc/article_attachments/21857834449426)*저장 권한 부족 오류 메시지*

### 플러그인 제거하기

팀의 플러그인을 제거하려면 팀 설정의 **앱 및 통합** 섹션에서 해당 플러그인을 찾고 팀 제거를 **클릭하세요**.

![uninstall_Google_Drive_app.jpg](https://help.miro.com/hc/article_attachments/21857818129042)*팀용 Google 드라이브 제거하기*

Google Drive에서 Miro의 연결을 끊으려면 프로필 설정의 **통합** 페이지를 열고 Google 드라이브 아이콘 근처에서 **로그아웃을** 클릭하세요.

![Google_Drive_log_out_in_settings.jpg](https://help.miro.com/hc/article_attachments/21857818118418)*Miro에서 Google 드라이브 연결 끊기*

### 임베디드 Google 드라이브 파일에서 사용할 수 없는 기능

**일반**

- Google 드라이브 시작 페이지
- 폴더 간 파일 이동하기
- 공유
- 도움말 검색

**Google 프레젠테이션**

- 프레젠테이션 모드

### 발생할 수 있는 문제 및 해결 방법

**업로드할 수 없는 오류**

**죄송합니다라는 오류 메시지가 표시되면 이 파일을 업로드할 수 있는 권한이 없거나 파일이 삭제된 것 같습니다. Google Drive 파일을 Miro 보드에 업로드하려고 할** 때 액세스 권한을 확인하고 다시 시도하세요. Google 관리자에게 Drive SDK API로 사용자가 Google 드라이브에 액세스할 수 있도록 허용하도록 요청하세요.

1. [Google 관리자 콘솔에](https://admin.google.com/) 로그인하세요.
2. 홈 **> 앱 > Google Workspace를 클릭하세요**. **드라이브 및 문서가** **모든 사용자에게 설정되어** 있는지 확인하세요.
3. **드라이브 및 문서 > 기능 및 애플리케이션을 클릭하세요**. **Drive** SDK 섹션에서 **Drive SDK API로 사용자가 Google 드라이브에 액세스할 수 있도록 허용이** 켜져 있는지 **확인하세요**.

![unable_to_upload.png](https://help.miro.com/hc/article_attachments/21857834454418)
*경고 메시지를 업로드할 수 없습니다*

**인증 문제**

Google 드라이브를 Miro에 연결할 수 없는 경우 **모든 Google 드라이브 파일 보기 및 다운로드 및** Google 드라이브를 연결할 때 **이 앱과 함께 사용하는 특정 Google 드라이브 파일만 보기, 편집, 생성 및 삭제할** 수 있는 Miro 액세스 권한을 제공하세요. 이를 위해 [Miro 프로필 설정](../../using-miro/managing-your-profile/01-profile-settings.md) > **통합으로** 이동한 다음 Google Drive와의 연결을 제거하고 다시 설정하세요.

![Permissions.png](https://help.miro.com/hc/article_attachments/21857818135570)
*Google 드라이브 계정에 대한 Miro 액세스*

### 자주 묻는 질문

1. *Google Drive에서 임베드된 파일을 열 수 있나요?*
   - 네, 문서를 선택하고 컨텍스트 메뉴에서 **소스** 버튼을 클릭하세요.
2. *Miro 보드 콘텐츠를 Google Drive 파일에 붙여넣을 수 있나요?*
   - [보드 콘텐츠를 텍스트나 이미지로](../../using-miro/working-on-the-board/09-copy-as-text-or-as-an-image.md) 복사해 Google 드라이브 파일에 붙여넣을 수 있습니다.
