---
title: Miro plugin for Sketch
article_id: 360017731173
sidebar_position: 13
created_at: '2019-02-11T10:13:46Z'
updated_at: '2025-02-26T12:15:38Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Miro plugin for Sketch enables an easy and quick way to get images from Sketch right to the board. Send your artboards to Miro and easily update them in one click. Sync all your images whenever you make a change without uploading them again.

### Enabling the plugin

1. Download the Sketch plugin from GitHub: follow [this link](https://github.com/miroapp/sketch_plugin) > **Code** > **Download ZIP**:

![Download_from_Github.jpg](images/21017592683026_Download%20from%20Github.jpg)

2. Extract the contents of the zip archive > double-click the RealtimeBoard.sketchplugin bundle to install the plugin.

![plugin_installed.jpg](images/21017605731986_plugin%20installed.jpg)
*Miro plugin for Sketch is installed*

3. To switch it on, open Sketch, go to **Plugins >** **Manage plugins** and tick the box **Miro by Miro**.

![Miro_plugin_in_Sketch.jpg](images/21017605733522_Miro%20plugin%20in%20Sketch.jpg)
*Miro plugin is activated in Sketch*

4. After that, you need to authenticate with your Miro credentials. To do this, click **Plugins -** **Miro:** **Log into Miro, Log out of Miro**.

![Log_in_to_Miro_in_Sketch.jpg](images/21017592678546_Log%20in%20to%20Miro%20in%20Sketch.jpg)
*Log in to Miro*

5. Type in your email and password or click **Use company credentials** if you log in via SSO.

![Miro_login.jpg](images/21017605735314_Miro%20login.jpg)
*The authentication window to sign into Miro*

### Adding Sketch artboards to Miro

To add a Sketch artboard to Miro, go to **Plugins:** **Miro -** **Sync all artboards with Miro**.

The dialog window will give you the option to choose between boards on which you have an editor role via email invitation or [project](../../using-miro/sharing-boards/16-projects.md)/team access.

> *⚠️ Please note that boards on which you have [visitor](../../using-miro/sharing-boards/08-collaboration-with-visitors.md) role won't be available.*

Select a board by a) clicking one of the suggestions in the dropdown or b) typing in the name of the board. After that click to add **all**or **selected artboards**. Tick the box if you want to **open Miro after sync**:

![select_a_board.jpg](images/21017592680338_select%20a%20board.jpg)
*Selecting a board for syncing*

Click **Sync**and the artboards will appear on your board.

![artiboards_in_Miro.jpg](images/21017605731474_artiboards%20in%20Miro.jpg)
*Please note that you can send artboards only to **existing boards** in Miro*

:::warning
Note that copying and pasting artboards directly is available in the Miro *browser* version only.
:::

### Synchronising Sketch artboards with Miro

In order to sync the artboards that were already added to Miro and after that altered in Sketch, go to **Plugins -** **Miro:** **Sync all artboards with Miro**. The board you've previously synced the artboards to will be automatically selected in the dialog window, just choose whether you want to sync **all**or only **selected artboards**. Tick the box if you want to **open Miro after sync**:

![syncing_boards.jpg](images/21017605737362_syncing%20boards.jpg)
*Syncing artboards with Miro*

### Disabling the plugin

To stop synchronizing Sketch and Miro, go to **Plugins >** **Manage plugins** and untick the box **Miro by Miro**.

![disable_Miro_sync.jpg](images/21017605738898_disable%20Miro%20sync.jpg)
*Miro plugin is disabled in Sketch*

### Possible issues and how to resolve them

|  |  |  |
| --- | --- | --- |
| **Error message / issue** | **Possible causes** | **Solution** |
| 1. "An error occurred. There was an error during syncing. Please retry" | 1. You are using an outdated version of Sketch.  2. Your Sketch artboard is huge (there is a very big image in the Sketch artboard). | 1. Update to the newer version of the Sketch plugin.  2. Check the image size and decrease it if needed. |
| 2. "Connection error. Something went wrong" | 1. The plugin is unable to connect to Miro API.  2. The rate is limited by Miro API.  3. There are other possible issues with the network. | Log out and log in to your Miro profile within Sketch, and try to sync the artboard again. |
| 3. "There was an error during syncing. Please retry" | The issue may be caused by changes in your network settings. | [Record console logs](#how-to-record-sketch-logs-for-miro-support) and [send a bug report to the Miro Support team](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md). |
| 4. Sketch plugin freezes and works unexpectedly when trying to sync multiple artboards with Miro | This happens when you have a huge Miro board and try to sync multiple artboards via the Sketch plugin. | Create a new Miro board in Miro and sync a single artboard at a time with it. |
| 5. The boards aren't showing in the search results in Sketch | This happens when a board was moved to another [project](../../using-miro/sharing-boards/16-projects.md) in Miro or if you don’t have a seat in the project where the board is located | 1. Check if a board that doesn't appear in the sync list in Sketch was moved to another project in Miro.  2. Check if you have a seat in a project where a board is located. |
| 6. Sketch doesn’t replace existing artboards on a Miro board - they are duplicated on the canvas rather than replaced | This happens when a board that is synchronized with Sketch has been [moved](../../using-miro/managing-boards/04-how-to-move-a-board.md) [to another Miro team](../../using-miro/managing-boards/04-how-to-move-a-board.md). In this case, the images will be duplicated at the first synchronization. Further on, they will be replaced. | Delete the previous artboards from the Miro board. The duplicates will be further replaced. |

#### How to record Sketch logs for Miro Support

1. [Open Spotlight Search](https://www.howtogeek.com/356942/how-to-view-the-system-log-on-a-mac/) (click the magnifier icon on the upper right corner of the screen) > **Console**:

![spotlight_search.jpg](images/21017605742098_spotlight%20search.jpg)
*Spotlight search*

2. Type in**sketch-rtb-error** in the console search field and search by message / any:

![search_in_Sketch.jpg](images/21017605743762_search%20in%20Sketch.jpg)
*Console search*

3. Click the line with the message in the console's lower section, take a screenshot, and share it with us.

![error_message.jpg](images/21017592686610_error%20message.jpg)
*Console error message*
