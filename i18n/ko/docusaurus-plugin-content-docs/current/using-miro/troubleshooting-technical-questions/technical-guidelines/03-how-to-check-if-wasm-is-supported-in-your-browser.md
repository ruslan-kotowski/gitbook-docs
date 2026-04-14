---
title: 브라우저에서 WASM이 지원되는지 확인하는 방법
article_id: 33769132852498
translation_id: 33769132852498
locale: ko-kr
sidebar_position: 3
created_at: '2026-03-04T12:47:24Z'
updated_at: '2026-03-16T13:02:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '실행 가능한 사용자: 모든 사용자 사용 가능 플랜: Free, Starter, Business, Enterprise, Education
    사용 가능 플랫폼: 브라우저'
---

WebAssembly(WASM)는 보안 정책 준수를 위해 조직에서 비활성화되거나, 이전 환경에서는 지원되지 않을 수 있습니다.

> **참고:** [WebAssembly 비교 테이블](https://webassembly.org/features/?categories=browsers)에서 브라우저에서 어떤 WASM 기능이 지원되는지 확인할 수 있습니다.

브라우저가 WASM을 지원하는지 확인할 수 있습니다.

다음 단계에 따라 진행하세요:

1. 개발자 도구를 엽니다.
   - 브라우저에서:
     - (MacOS) Chrome, Edge, Firefox: `⌘ + ⌥ + I`
     - (Linux, Windows) Chrome, Edge, Firefox: `Ctrl + Shift + I`, 또는 `F12`
     - (MacOS) Safari: **설정** > **고급**으로 이동. **메뉴 바에 개발 메뉴 표시** 및 **웹 개발자 기능 표시**를 활성화. **개발** > **JavaScript 콘솔 표시**를 엽니다.
   - Miro 데스크톱 앱에서:
     - 왼쪽 상단에서 **도움말** > **개발자 도구 열기**를 클릭합니다.
2. DevTools에서 **콘솔** 탭을 클릭합니다.
3. 콘솔 입력란에 `typeof WebAssembly`를 입력하거나 붙여넣기 합니다.
4. 키보드에서 **ENTER**를 누릅니다.
5. 결과 해석하기:
   - 콘솔이 `undefined`를 반환하면 WebAssembly가 지원되지 않거나 비활성화된 것입니다.
   - 콘솔이 `object`를 반환하면, WebAssembly가 지원됩니다.![](../../../../../../../docs/using-miro/troubleshooting-technical-questions/technical-guidelines/images/33770259460626_image.png)
     *브라우저에서 WASM을 사용할 수 있을 때, DevTools 콘솔은* `object`*를 표시합니다.*

     > **참고:** 콘솔이 `object`를 반환하지만 여전히 Miro에 접근할 수 없다면, 다른 [가능한 문제 및 문제 해결](../troubleshooting)을 검토하거나 [Miro 지원](../../tools/troubleshooting/06-contacting-miro-support.md)에 문의할 수 있습니다.
