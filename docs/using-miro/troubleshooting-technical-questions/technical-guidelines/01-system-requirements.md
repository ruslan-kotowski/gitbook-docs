---
title: System requirements
article_id: 360017731553
sidebar_position: 1
created_at: '2019-02-11T10:14:54Z'
updated_at: '2026-03-06T14:57:18Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

This article outlines system requirements for using Miro, including device, [GPU, and WebAssembly](#gpu-and-webassembly-requirements).

For working in Miro, please make sure your device meets the following minimum or recommended system requirements.

However, please keep in mind that the parameters mentioned below are not definitive as Miro performance can be related to multiple other factors such as:

- Tasks in the background
- Numbers of tabs in the browser and how often you switch between them
- The resolution of the monitor where you open Miro
- Stability of the Wi-Fi connection
- Number of users on the board
- Device cooling system

If you experience performance/access issues, please check [troubleshooting guides](../troubleshooting) and the [tips to optimize board performance](../../tools/troubleshooting/04-board-performance-and-loading-issues.md).

|  |  |  |
| --- | --- | --- |
|  | **Minimum** | **Recommended** |
| **CPU** | 3 GHz (2 cores/4 threads) | 2,8 GHz (4 cores/8 threads) |
| **RAM Memory** | 8 GB | 16 GB (DDR4) |
| **Network bandwidth** | 8 Mb/s | 32 Mb/s |

**Please note that running Miro on high-end hardware that is way above the recommended specification may not give you the expected performance boost as Miro is a web-app that works using a browser web engine. Web engine is not capable of utilizing the full potential of the device as software that is installed locally on your computer which is designed for a particular operating system and CPU architecture.*

Minimum system requirements for comfortable usage of Miro on [tablets](../../../getting-started/apps-for-devices/11-tablet-app.md) are 6 GB RAM.

Miro can be used on different types of devices. You can open Miro in a browser, download the [Desktop](../../../getting-started/apps-for-devices/05-desktop-app.md), [Tablet](../../../getting-started/apps-for-devices/11-tablet-app.md), [Mobile app](../../../getting-started/apps-for-devices/08-mobile-app.md), or [use Miro on an interactive display](../../../getting-started/apps-for-devices/07-interactive-displays.md).

**Offline mode**

Since Miro relies on the vision of a seamless cloud solution for *online*collaboration, the tool's *offline*mode is currently not on our radar. However, we provide several export options. [Learn more](../../import-and-export/export/03-how-to-export-your-board.md).

## GPU and WebAssembly requirements

Miro uses GPU hardware acceleration and WebAssembly (WASM) for smooth rendering, and to support certain advanced features.

### Using Miro without GPU

For optimal performance, Miro requires GPU hardware acceleration.

If GPU hardware acceleration is unavailable, for example on some virtual machines, or when hardware acceleration is disabled, then Miro switches automatically to a CPU-based renderer.

:::tip
For the best Miro experience, keep hardware acceleration enabled when possible.
:::

Without GPU hardware acceleration, you may experience the following performance changes:

- Some GPU-dependent features may be unavailable or shown as placeholders
- Slower panning and zooming, especially for large boards, or boards with a lot of media
- Core board functionality may not behave as expected
- Higher CPU usage

### Using Miro without WebAssembly (WASM)

Some Miro features rely on WebAssembly (WASM) modules.

Most modern browsers enable WASM by default. If WASM is unavailable, for example blocked in compliance with enterprise policy, disabled in the browser, or unsupported in older environments, Miro switches automatically to JavaScript-based rendering paths where possible.

**More information:** See [How to check if WASM is supported in your browser](https://help.miro.com/hc/articles/33769132852498).

:::tip
For the best Miro experience, keep WebAssembly enabled. In a managed environment, if you suspect WASM is blocked, then check with your IT team.
:::

Without WASM, you may experience the following performance changes:

- Features that require WASM may not initialize and are hidden or shown as placeholders
- Boards that depend on WASM-based functionality may not fully load or load at all
