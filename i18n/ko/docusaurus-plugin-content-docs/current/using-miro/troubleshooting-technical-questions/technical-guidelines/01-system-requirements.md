---
title: "\uC2DC\uC2A4\uD15C \uC694\uAD6C \uC0AC\uD56D"
article_id: 360017731553
translation_id: 360017731553
locale: ko-kr
sidebar_position: 1
created_at: '2019-02-11T10:14:54Z'
updated_at: '2026-03-06T14:57:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

이 문서에서는 Miro를 사용하기 위한 시스템 요구 사항을 설명하며, 기기, GPU, 그리고 WebAssembly를 포함합니다.

Miro에서 작업하려면, 기기가 아래의 최소 또는 권장 시스템 요구 사항을 충족하는지 확인하세요.

하지만, 아래에 언급된 기준들은 절대적인 것이 아니며, Miro의 성능은 여러 다른 요인에도 영향을 받을 수 있음을 염두에 두십시오.

- 백그라운드 작업
- 브라우저 내 탭의 수와 탭 간 전환 빈도
- Miro를 여는 모니터의 해상도
- Wi-Fi 연결 안정성
- 보드의 사용자 수
- 기기 냉각 시스템

성능이나 접속 문제를 겪으시면, [트러블슈팅 가이드](../troubleshooting) 및 [보드 성능 최적화 팁](../../tools/troubleshooting/04-board-performance-and-loading-issues.md)을 확인하세요.

|  |  |  |
| --- | --- | --- |
|  | **최소** | **권장** |
| **CPU** | 3 GHz (2 코어/4 스레드) | 2.8 GHz (4 코어/8 스레드) |
| **RAM 메모리** | 8 GB | 16 GB (DDR4) |
| **네트워크 대역폭** | 8 Mb/s | 32 Mb/s |

**Miro는 웹 엔진을 사용하는 웹 앱이므로 권장 사양을 훨씬 초과하는 고급 하드웨어에서 실행하더라도 기대한 성능 향상을 얻지 못할 수 있습니다. 웹 엔진은 특정 운영 체제 및 CPU 아키텍처에 맞춰 설치된 소프트웨어처럼 디바이스의 풀 성능을 활용할 수 없습니다.*

Miro를 [태블릿](../../../getting-started/apps-for-devices/11-tablet-app.md)에서 편리하게 사용하려면 최소 6GB RAM이 필요합니다.

Miro는 다양한 종류의 장치에서 사용할 수 있습니다. 브라우저에서 Miro를 열거나 [데스크톱](../../../getting-started/apps-for-devices/05-desktop-app.md), [태블릿](../../../getting-started/apps-for-devices/11-tablet-app.md), [모바일 앱](../../../getting-started/apps-for-devices/08-mobile-app.md)을 다운로드하거나 [인터랙티브 디스플레이에서 Miro를 사용](../../../getting-started/apps-for-devices/07-interactive-displays.md)할 수 있습니다.

**오프라인 모드**

Miro는 *온라인* 협업을 위한 원활한 클라우드 솔루션을 목표로 하므로, 도구의 *오프라인* 모드는 현재 고려 사항이 아닙니다. 그러나 몇 가지 내보내기 옵션을 제공합니다. [자세한 내용을 알아보세요](../../import-and-export/export/03-how-to-export-your-board.md).

## GPU 및 WebAssembly 요구사항

Miro는 매끄러운 렌더링과 특정 고급 기능 지원을 위해 GPU 하드웨어 가속과 WebAssembly (WASM)를 사용합니다.

### GPU 없이 Miro 사용하기

최적의 성능을 위해 Miro는 GPU 하드웨어 가속이 필요합니다.

GPU 하드웨어 가속이 불가능한 경우, 예를 들어 일부 가상 머신에서는 하드웨어 가속이 꺼져 있는 경우 Miro는 자동으로 CPU 기반 렌더러로 전환됩니다.

:::tip
최상의 Miro 경험을 위해 가능한 경우 하드웨어 가속을 활성화 상태로 유지하세요.
:::

GPU 하드웨어 가속이 없을 경우, 다음과 같은 성능 변화를 경험할 수 있습니다:

- 일부 GPU 의존 기능을 사용할 수 없거나 자리표시자로 표시될 수 있습니다
- 특히 미디어가 많은 큰 보드에서 팬 및 줌 기능이 느려질 수 있습니다
- 핵심 보드 기능이 기대한 대로 작동하지 않을 수 있습니다
- CPU 사용량 증가

### WebAssembly (WASM) 없이 Miro 사용하기

일부 Miro 기능은 WebAssembly (WASM) 모듈에 의존합니다.

대부분의 최신 브라우저는 WASM을 기본적으로 활성화합니다. WASM이 사용 불가능한 경우, 예를 들어 기업 정책에 따라 차단되거나 브라우저에서 비활성화된 경우, 혹은 오래된 환경에서 지원되지 않는 경우, Miro는 가능한 경우 자동으로 JavaScript 기반 렌더링 경로로 전환됩니다.

**추가 정보:** [브라우저에서 WASM 지원 여부 확인 방법](https://help.miro.com/hc/articles/33769132852498)을 참조하세요.

:::tip
최고의 Miro 환경을 위해 WebAssembly를 활성화하세요. 관리 환경에서 WASM이 차단된 것으로 의심되면 IT 팀과 확인하세요.
:::

WASM이 없을 경우, 다음과 같은 성능 변화가 있을 수 있습니다:

- WASM이 필요한 기능이 초기화되지 않고 숨겨지거나 플레이스홀더로 표시될 수 있습니다
- WASM 기반 기능에 의존하는 보드가 완전히 로드되지 않거나 전혀 로드되지 않을 수 있습니다
