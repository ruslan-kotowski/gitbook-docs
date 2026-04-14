---
title: How to troubleshoot and report a bug
article_id: 360017731413
sidebar_position: 8
created_at: '2019-02-11T10:14:28Z'
updated_at: '2026-04-02T09:35:12Z'
draft: false
---

If you are experiencing performance issues or can’t use Miro, learn how to report the bug to [Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).

## Before reporting a bug

1. Check the [Miro Status Page](https://status.miro.com/) for reports of potential performance degradation
2. Check if the issue is reproduced in [incognito](https://support.google.com/chrome/answer/95464) **(private) mode** and a **different browser**
3. [Disable the browser extensions](https://support.box.com/hc/articles/360044196613-How-To-Disable-Plugins-Add-Ons-Extensions-In-Multiple-Browsers). Sometimes they clash with Miro processes (e.g. Grammarly with the text widgets).
4. If you work in the Desktop app, [reset the app data](../../../getting-started/apps-for-devices/05-desktop-app.md#how-to-reset-the-app-data)
5. If you experience performance issues on a specific board, try [duplicating](../../managing-boards/03-how-to-duplicate-a-board.md) it and see if the issue persists on the copied board
6. Check our troubleshooting guides:

- [Board performance and loading issues](../../tools/troubleshooting/04-board-performance-and-loading-issues.md)
- [I can’t log in](../../tools/troubleshooting/09-i-can't-log-in.md)
- [I can’t access or edit a Miro board](../../tools/troubleshooting/08-i-can't-access-or-edit-a-miro-board.md)
- [Board export issues](../../tools/troubleshooting/03-board-export-issues.md)
- [I lost my board or content](../../tools/troubleshooting/11-i-lost-my-board-or-content.md)
- [Other guides](.)

## How to submit a bug

Provide as many details as possible - this will help us understand your issue right away so we can better help you.

1. Include a description of the issue and send screenshots, GIFs, or a [short video](https://chrome.google.com/webstore/detail/openvid-screen-recorder-c/liecbddmkiiihnedobmlmillhodjkdmb). Additionally,

- If the issue happens on a specific board - [contact Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md) and [share the board](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) with editing rights if possible
- If the issue is connected with a specific uploaded file - send us the file

2. Specify your device, operating system, and browser version
3. Provide your browser console and network logs or Desktop app logs

### How to record console logs

**How to record browser console logs**

1. While on the Miro board, **click the address bar** of your browser (use this step if the issue is reproduced on one of the boards as opposed to the settings page or the dashboard)​![mceclip1.png](images/21020264821010_mceclip1.png)
2. Press **F12** or **fn + F12** to open the browser developer tools
3. Choose **Network** tab, tick the box **Preserve logs**
4. Reload the page
5. Try to reproduce the issue again
6. Click the Download Arrow sign to **Export** the Network HAR logs
   ![network_console_logs.jpg](images/21020264822418_network%20console%20logs.jpg)
7. Switch to the **Console** tab, right-click the records and choose **Save as**​![save_console_logs.jpg](images/21020253821970_save%20console%20logs.jpg)
8. Send us the  .*log* and .*har* files. If the file size doesn’t attach to your ticket, upload the file to any cloud storage and send us the link  (allow anyone with the link to download the files)

**How to record Desktop app logs on Mac**

If you experience a bug in the Desktop app on Mac, send us the log records.

1. While in the Desktop app, click **Help** in the top-left corner. Select **Open developer tools for tabs**​​​​​​​​
   ![open_developer_tools_for_tabs.jpg](images/21020253822866_open%20developer%20tools%20for%20tabs.jpg)
2. ​Switch to **Network** tab.​​​​ Tick the box **Preserve logs**
3. Open the board you wish to troubleshoot (skip the step if you can’t access boards)
4. Reload the page with **Ctrl + R** shortcut
5. Reproduce the issue
6. Click the Download Arrow sign to export the Network HAR logs:
   ![preserve_logs.jpg](images/21020253823250_preserve%20logs.jpg)
7. Switch to the Console tab, right-click the records, and choose **Save as.**​![save_as_.jpg](images/21020253825042_save%20as%20.jpg)
8. Click **Help** again > choose **Open developer tools** and repeat steps 2 to 7. This would collect another type of log that would provide us with a different set of data, to investigate the issue further for you
9. Send us the .log and .har files. If the file size doesn’t attach to your ticket, upload the file to any cloud storage and send us the link (allow anyone with the link to download the files).

**How to record Desktop app logs on Windows**

If you experience a bug in the Desktop app on Windows, send us the log records.

1. While in the Desktop app press **Alt** > click **Help** > **Open developer tools for tabs![open_developer_tools_for_tabs_on_Windows.jpg](images/21020264830994_open%20developer%20tools%20for%20tabs%20on%20Windows.jpg)**
2. ​Switch to **Network** tab.​​​​ Check the box **Preserve logs**
3. Open the board you wish to troubleshoot(skip this step if you can’t access boards)
4. Press **Ctrl + R** to reload the page  **Ctrl + R**
5. Reproduce the issue
6. Click the Download icon to export the Network HAR logs
   ![preserve_logs.jpg](images/21020253823250_preserve%20logs.jpg)
7. Switch to the Console tab, right-click the records and choose **Save as**​
   ![save_as_.jpg](images/21020253825042_save%20as%20.jpg)
8. Open **Help** again > choose **Open developer tools** and repeat steps 2 to 7. This would collect another type of log that would provide us with a different set of data, to investigate the issue further for you
9. Send us the .log and .har files. If the file size doesn’t attach to your ticket, upload the file to any cloud storage and send us the link (allow anyone with the link to download the files).

### How to collect a browser report

When you report loading or performance issues, sharing extended browser version information helps Miro Support diagnose the problem. You can find this information by entering a specific command in your browser’s **address bar**. Below, you'll find how to access this information in different browsers.

- **Chrome**: chrome://version
- **Microsoft Edge**: edge://version
- **Firefox**: about:support (or about:version in some versions)
- **Opera**: opera://about
- **Yandex Browser**: browser://version

> **✏️** See [How to contact Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).
