---
title: Board export issues
article_id: 360020567820
sidebar_position: 4
created_at: '2021-03-18T12:15:46Z'
updated_at: '2025-11-05T13:45:32Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

You can [export your Miro board](../../import-and-export/export/03-how-to-export-your-board.md) as an image, PDF, or CSV file. If you face any issues exporting your Miro board, explore the possible solutions below.

## I can't export the board

**Export button is missing on my board**

The export button is located under the **three dots** (**...**) menu, then under the **Board** submenu.

No export option in the [board menu](../../../getting-started/start-here/your-first-board/05-toolbars.md):

1. Check that the board owner/co-owner has allowed exporting the board for users in the board content settings.

   To find out the board owner’s name, click the board name in the top-left corner to open the board information card. If you’re not allowed to see this information, you can check the name of the user who invited you to the board in the invitation email.

   Reach out to the board owner and ask them to enable the option for you in the **Share** window > **Sharing settings** > **Permissions**. The owner/co-owner needs to select which category of users can [copy the board content](../../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).
   ![.gif](images/21016044218642_.gif.png)
   *Configuring who can copy the board*
2. Make sure your browser, plan, and device support exporting. You can check the availability below. If your browser, plan, or device doesn’t support the export option, we recommend switching to another browser or device or [upgrading your team](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

   |  |  |  |  |  |  |
   | --- | --- | --- | --- | --- | --- |
   |  | Free plan | | Starter, Business, Enterprise, Education plans | | Export to CSV (all plans) |
   |  | Low resolution | High resolution without watermark | Low  resolution | High resolution  without watermark |
   | Google Chrome | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Safari | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Firefox | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Opera | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Edge < 79 | ✘ | ✘ | ✘ | ✔ | ✘ |
   | [Desktop app](../../../getting-started/apps-for-devices/05-desktop-app.md) | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Tablet | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Mobile | ✘ | ✘ | ✘ | ✘ | ✘ |

**For low-quality exports**

To troubleshoot, close browser tabs and background tabs. You can also try switching browsers.

For high-quality exports, do the following:

- Hide frames you do not want to export. Content in hidden frames is not exported.
- Split the board into smaller boards for export.

**General tips**

- Put everything you want to export in frames, as only widgets inside of frames are exported.
- Avoid PDF in PDF. If you have a PDF on a board which you would like to export as a PDF, replace the PDF on the board with low-quality images.
- Convert high-resolution images to JPEG or downsize them with an external tool.
- Check the Miro Status page for relevant incidents.
- Divide the board into frames and export frames separately. Separate PDFs can later be rejoined using an external tool.
- Split large boards into smaller boards and use [Spaces](../../spaces/01-spaces.md) to help you stay organised and group boards that belong together.

**"Sorry, something went wrong when generating the PDF document"**

Try dividing the board into frames and export frames separately, as the issue could be caused by the board size.

If that does not help, check [your browser console logs](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md). If the logs contain the following message:

```
ERR_CONNECTION_ABORTED
```

*where:*

The export is blocked by security software on your device or a firewall within your network.

You or your system administrator need to configure the settings of your antivirus program and/or firewall to allow Miro to perform the export procedure.

When in doubt, [contact Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).

**Nothing happens when I try to export a board to PDF, and Miro shows no error**

This known issue occurs mostly in the Safari browser, when pop-up windows are disabled. To resolve the issue for Safari, [follow these steps](https://support.apple.com/en-gb/guide/safari/sfri40696/mac). Ensure that you enable pop-up windows for miro.com, or all websites. Return to Miro and retry to export your board.

For Chrome, [follow these steps](https://support.google.com/chrome/answer/95472?hl=en&co=GENIE.Platform%3DDesktop).

## I have issues with exported files (PDFs, images, CSVs)

**Images/PDFs are blurry on the exported document**

If uploaded images or PDFs are blurry on your saved file:

1. Set the board zoom to 100% and let the images/PDFs render before exporting the board
2. The uploaded image/PDF may be too complex or large for export. To downsize the file, convert the image/PDF to PNG format and replace it on the board. Then export the board again

Free plan supports export in low quality only. If you need to export your board in high quality, we recommend [moving it to a paid team](../../managing-boards/04-how-to-move-a-board.md) or [upgrading your team](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

**The order of the pages is not the same as the order of the frames on the board**

The order of the frames exported to PDF is the same as in the frames panel. To change the order of the frames:

1. Open the board overview in the bottom left corner
2. Drag frames to change their position on the list. You can also use [Magic organize](../../essential-tools/07-frames.md) to quickly arrange your frames in the order in which they are placed on the board
   ![move_frames.gif](images/21016057584914_move%20frames.gif)
   *Changing the order of the frames*

**The exported file is cut off**

If you **export your board as an image**, be sure to include all the content that you want to export in the selected exported area.

![save_as_image.gif](images/21016057583890_save%20as%20image.gif)
*Exporting a board as an image*

If you **export your board as PDF**, be sure to create a frame that will include all the content that you would like to export. Then [export the frame](../../import-and-export/export/03-how-to-export-your-board.md#save-as-pdf).

**The exported PDF file doesn’t contain frame names**

When you export your board as a PDF file, the frame titles are not included in the export. You can replace the frame titles using the [text tool](../../essential-tools/16-text.md) and put the text on the frames. The titles will appear on your PDF.

**The data in an exported CSV file is not structured**

At the moment, the CSV export doesn't keep board structure or relationships. However, if you export [tables](../../advanced-tools/05-grid.md) as a CSV file, the structure is saved.

If you need to export a [mind map](../../advanced-tools/03-mind-map.md) as a file with intelligent data, use the [Mindmap downloader](https://miro.com/marketplace/mindmapdownloader/?backUrl=%2Fmarketplace%2F).

**Fonts on the board differ from fonts on the exported file**

Miro export uses the fonts installed in your device's operating system. If the font is not present in your OS, a similar font from your system will be used instead. If you need the same font as on your Miro board, choose a different font on the board or install the needed font on your device.

## I can’t locate the exported file

**I can’t find the exported file on my device**

**If you use Miro in a browser**

The files will be stored in the folder where browser downloads are saved by default. You can check the download options in the browser settings.

**If you use the Miro Desktop app or Tablet app**

Check the Downloads folder on your device. You can also search your files using the board name.

**Miro creates a new folder every time I export a board**

> **Relevant for**: [Windows Desktop app](../../../getting-started/apps-for-devices/05-desktop-app.md)

It is possible that the path has been saved in the Miro app settings. To delete the path:

1. Delete the Miro Desktop app
2. On the bottom left of Windows (search bar), type **%AppData%** and open the folder **Local,** then delete the folder **RealTimeBoard**
3. Open **%AppData%** again, browse to the folder **Roaming,** and delete the folder **RealTimeBoard**

Reinstall the latest [Miro Application](https://miro.com/apps/).

If none of the solutions help, [contact Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).
