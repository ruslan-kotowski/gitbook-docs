---
title: How to check if WASM is supported in your browser
article_id: 33769132852498
sidebar_position: 3
created_at: '2026-03-04T12:47:24Z'
updated_at: '2026-03-16T13:02:18Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  roles: all_users
  plans: free, starter, business, enterprise, education
  platforms: browser
---

WebAssembly (WASM) may be disabled for reasons that include compliance with security policies set by your organization, or non-support in older environments, for example.

:::tip
The [WebAssembly comparison table](https://webassembly.org/features/?categories=browsers) shows which WASM features are supported in your browser.
:::

You can check whether your browser supports WASM.

Follow these steps:

1. Open Developer Tools.
   - In your browser:
     - (MacOS) Chrome, Edge, Firefox: `⌘ + ⌥ + I`
     - (Linux, Windows) Chrome, Edge, Firefox: `Ctrl + Shift + I`, or `F12`
     - (MacOS) Safari: Go to **Settings** > **Advanced**. Enable **Show Develop menu in menu bar** | **Show features for web developers**. Open **Develop** > **Show JavaScript console**.
   - In the Miro desktop app:
     - In the top-left click **Help** > **Open developer tools**.
2. In DevTools, click the **Console** tab.
3. In the console input line, type or paste `typeof WebAssembly`.
4. On your keyboard press **ENTER**.
5. Interpret the result:
   - If the console returns `undefined`, then WebAssembly is unsupported, or disabled.
   - If the console returns `object`, then WebAssembly is supported.![](images/33770259460626_image.png)
     *The DevTools console shows* `object` *when WASM is available in your browser.*

     > **NOTE:** If the console returns `object` and you are still unable to access Miro, you can review other [possible issues and troubleshooting](../troubleshooting), or contact [Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).
