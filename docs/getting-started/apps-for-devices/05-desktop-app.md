---
title: Desktop app
article_id: 360017572854
sidebar_position: 5
created_at: '2019-02-11T10:15:04Z'
updated_at: '2025-11-25T16:00:29Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
---

Launch the Miro Desktop app in seconds right from your home screen, and work on boards without distraction. The app supports all the basic features of the browser version.

:::tip
Download the Miro app from [our website](https://miro.com/apps/).
:::

## Download the Miro desktop app

### Windows

- Windows 64-bit - [download the app](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.exe)

:::note
Windows 32-bit is deprecated and no longer available.
:::

### macOS

- Macs with Apple silicon chips - [download the app](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro.dmg)
- Macs with Intel chips - [download the app](https://desktop.miro.com/platforms/darwin/Install-Miro.dmg)

To find out what kind of processor you have, follow these steps:

1. Click the Apple icon in the top-left corner of your Mac.
2. This will bring up a drop-down menu. Click on the option **About this Mac**.

The window should show you the information you need including processor type (Intel or Apple silicon).

## Deploy Miro to multiple devices

Miro offers various installer versions that IT Administrators can use to deploy Miro to users across thousands of machines. There are two basic ways to do this: install per user or per machine. Within each of those, there are versions with and without auto-updates. The version with auto-updates means your users will get the updated app version as soon as it’s published. The one without auto-updates gives you more control over the version of Miro your employees are using.

### For Windows

#### Deploy Miro to Program Files

Miro can also be installed in the Program Files directory, making it available to every user of a device, while keeping their profiles separate. A single installation on a machine means a smaller hard drive footprint at scale while still making Miro available for ever user of that machine. If you opt for the version with automatic updates, note that administrative permissions are needed to install an update.

- Windows MSI 64 bit with auto-updates - [download the app](https://desktop.miro.com/platforms/win-nsis/Miro-setup.msi)
- Windows MSI 64 bit without auto-updates - [download the app](https://desktop.miro.com/platforms/win-nsis/Miro-no-updates.msi)

#### Deploy Miro for a particular user

Miro offers various installer versions that IT Administrators can use to deploy Miro for a single user. This version can be updated without administrative permissions and installs only for the particular user(s) chosen.

- Windows MSI 64 bit with auto-updates - [download the app](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.msi)
- Windows MSI 64 bit without auto-updates - [download the app](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-no-updates.msi)

### For MacOS

- Apple silicon Mac without auto-updates - [download the app](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro-no-updates.dmg)
- Intel Mac without auto-updates - [download the app](https://desktop.miro.com/platforms/darwin/Install-Miro-no-updates.dmg)

## App system requirements

### For Windows

|  |  |  |
| --- | --- | --- |
|  | **Minimum** | **Recommended** |
| **CPU** | 3 GHz (2 cores/4 threads) | 2.8 GHz (4 cores/8 threads) |
| **RAM** | 8 GB | 16 GB (DDR4) |
| **OS** | Windows 10 or higher for the app from Microsoft Store + Microsoft .NET Framework 4.5 (Please note the ARM version of Windows is not supported) | Latest OS |
| **Network** | 8 Mb/s or faster | 32 Mb/s |

### For macOS

|  |  |  |
| --- | --- | --- |
|  | **Minimum** | **Recommended** |
| **CPU** | 64-bit Intel or Apple M1 |  |
| **OS** | MacOS 12 (Monterey) or higher | Latest OS |
| **Network** | 8 Mb/s or faster | 32 Mb/s |

Please note that the app will have several instances running on your device:

- main process
- window process (UI renderer)
- hardware acceleration
- crash handler
- + 1 process per each opened tab (because each tab has a webview)

For example, if you have 3 tabs open during your work, you will see 7 instances of Miro.exe. More information on this architecture can be found [here](https://www.electronjs.org/docs/glossary#process) and [here](https://www.chromium.org/developers/design-documents/multi-process-architecture).

## App-specific shortcuts

The desktop app has additional [shortcuts](../../using-miro/working-on-the-board/06-shortcuts-and-hotkeys.md):

- **Ctrl + R** *(for Windows)* / **Cmd + R** *(for Mac)* to reload the tab
- **Ctrl + W** *(for Windows)* / **Cmd +W** *(for Mac)* to close the tab
- **Ctrl + Q** *(for Windows)* / **Cmd + Q** *(for Mac)* to exit the app
- **Ctrl + Shift + L** *(for Windows)* / **Cmd + Shift + L** *(for Mac)* to copy board link
- **Ctrl + ~** *(for Windows)* **/ Cmd + ~** *(for Mac)* to zoom

## App actions

The following table shows which available actions in the Miro desktop app may have a different experience from the browser:

| Action | **Win & Mac apps from** [**Miro Apps**](https://miro.com/apps/) |
| --- | --- |
| Save as image (Low, Medium, High) | ✔ |
| Save as image (Vector) | ✔ |
| Save as PDF (Low) | ✔ |
| Save as PDF (Vector) | ✔ |
| Export to a spreadsheet (CSV) | ✔ |
| Video Chat | ✔ |
| Pasting from a spreadsheet | ✔ |
| Plugin for Confluence | ✔ |

### Unavailable actions

The following actions are unavailable in the Miro desktop app:

- Visitors cannot log in.

  > ✏️ Only registered Miro users can log in to the desktop app.
- No option to copy-paste from Sketch
- For some versions of Jira Server, you are unable to edit Jira Cards for security reasons.

## Spell check

If you would like to turn off the automatic spell check functionality in the Desktop app, follow these steps:

- Press **Alt** (*for Windows only*)
- Click**View** in the main navigation bar at the top
- Uncheck the **Show Spell Check** button

Note the option to disable spell check is not available in the app downloaded from Microsoft Store.

## Possible issues and how to resolve them

### How to reset the app data

In a lot of cases where an issue arises (especially if you're having difficulties with the login procedure), it helps to **reset the app data**, clearing the memory of the app.

:::tip
If the issue persists after resetting the data, you may also want to delete the app and reinstall it by [downloading the latest version](https://miro.com/apps/).
:::

#### For Windows

Press **Alt > Help**and choose to reset the application data as shown in the screenshot below:

​​
![reset app data on Windows.png](images/21016134171922_reset%20app%20data%20on%20Windows.png)
*Resetting the app data on the Desktop app for Windows*

If you cannot find the menu, you probably use the app downloaded from the MS Store. In this case, to reset the app data, open Windows **Settings** > **Apps** > **Apps and Features** > find **Miro** on the list > **Advanced options** > **Reset**.

If this does not immediately help proceed to delete all app files from **C:\Users\username\AppData\Roaming\RealtimeBoard** and **C:\Users\username\AppData\Local\Programs\RealtimeBoard**

> **✏️** If the **Appdata** folder is hidden, see [here](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) how you can reveal it.

#### For macOS

Click Miro in the top menu and choose **Reset application data** as shown in the screenshot below:

![reset app data on Mac.png](images/21016120799378_reset%20app%20data%20on%20Mac.png)
*Resetting the app data on Mac*

After that, try to log into the app again and check if the issue is solved.

If resetting does not immediately help proceed to open a finder window > press **Command + Shift + G** > paste **~/Library/Application Support/RealtimeBoard**and delete all app files.

If you use MDM for Mac

If you face an issue when the app cannot load, stuck in a loop, please make sure that your setup allows for our auto-updater to perform. `https://github.com/Squirrel/Squirrel.Mac` must have rights to:

- read, write, and execute for `Application` directory,
- read and write for `~/Application Support/Caches/` for work with `com.electron.realtimeboard.ShipIt` directory and also it works with temp directory `private/var/folders`.

If something goes wrong during the update process Squirrel creates `ShipIt_stderr.log` in `~/Application Support/Caches/com.electron.realtimeboard.ShipIt`. More information about the issue can be found there.
Please note that Skype and Slack use a similar update process so if you have already configured MDM for them you can apply the same settings for Miro Desktop app.

## Frequently asked questions

1. *Where can I download the Desktop app?*
   - Download it from [our website](https://miro.com/apps/).
2. *How can I remove the pop-up to open the Desktop app when you start Miro in a browser?*
   - Try the steps from [this article](../../using-miro/troubleshooting-technical-questions/technical-guidelines/04-how-to-disable-miro-desktop-app-pop-up-in-your-browser.md).
3. *Do you have a Desktop app version for Linux?*
   - No, at the moment, we do not have this version.
4. *How can I copy an opened board's link in the Desktop app?*
   - You can open the board **Share** menu and copy the board link from there. Another way is to click **File** in the upper-right corner > **Copy board link**. You can also use the shortcut **Ctrl + Shift + L** *(for Windows) /* **Cmd + Shift + L** *(for Mac).*
5. *When I press **Alt** while in my Windows Desktop app, the menu does not appear. How can I get it?*
   - Please note that the menu is not supported in the app downloaded from the Microsoft Store. You can reset app data via windows settings (**System > Apps & Features > Find Miro > Advanced Options > Reset**) or [install the original app version](https://miro.com/apps/).
6. *If I remove the Desktop app, will my boards get deleted?*
   - No, your content is tied to your Miro profile. You can access it in a browser, [Tablet app](11-tablet-app.md), [Mobile app](08-mobile-app.md) as well.
