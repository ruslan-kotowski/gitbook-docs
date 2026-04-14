---
title: Whiteboards.io Importer for Miro
article_id: 20624350720402
sidebar_position: 3
created_at: '2024-08-07T16:30:40Z'
updated_at: '2026-01-19T14:08:30Z'
draft: true
---

ServiceRocket’s Whiteboards.io Importer for Miro is a user-friendly solution designed to streamline importing data from the [Whiteboards.io](https://whiteboards.io/) app to [Miro](https://miro.com/app/dashboard/). Upload your Whiteboard-generated backups with haste and ease.

Get your access to the importer today. Visit `https://www.servicerocket.com/miro/whiteboards-io-miro-migration` for more details.

## **Exporting boards from Whiteboards.io**

1. Log in to [Whiteboards.io](https://whiteboards.io/).
2. On the main page, click Export boards in the warning status message.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeiEjTayvBy6uufihIKif-C14REIupCmqvKKU6_DMUVhT6lrGC01PkVkXOVJENoCmA2piy40VIRGxFT4YGIE870A9TSYnIpSDyY37H1euf5ZsiP_dbN3zMpcp5GOCIRAcsaJonD8obCfo-WSOxfax4HVtuN?key=RrckFddS6o4KjRqYlXDbPw)
*Click Export boards from the warning status message to start*

3. Next, perform the following steps to export the board.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeyDxMc_ob24RYp6Rne_MAIXICO3JRrSesUAHtsyJ0hsG3DjTC5iiNg6_b-97m97XkgtjWRbX0uDcmbyBqMz6tGEEayg0eLvmVIUzLNwTizSYtlQBQXIP5XSNMQFTX2psIIE6SnbVo74EQABRH9vDwe9SPK?key=RrckFddS6o4KjRqYlXDbPw)
*Verify the settings are correct when exporting your board*

1. 1. Select .json format only.
   2. Uncheck include media (images, videos and other files).
   3. Click Export to confirm the settings and export the board.

4. A .zip file will be successfully generated.

## **Importing Whiteboards.io boards into Miro**

1. Open your Miro board.
2. On the toolbar, click More apps > select or search for Whiteboards.io Miro Importer.
3. Click Choose File to upload the (.zip) file generated from the [Whiteboards.io](http://whiteboards.io/) app.
4. Next, select the board you want to import and click Import.
5. Once the import is complete, the system will show the board's status as COMPLETED.
6. Close the app and return to Miro’s main page. The app will import the selected boards into your team account.

## **Whiteboards.io data mapping in Miro**

Data mapping is essential to maintain data integrity, consistency, and schema differences during the transition from one app to another. The tables below list all the equivalent terminology, data structures, field names, formats, and more.

|  |  |  |
| --- | --- | --- |
| **Whiteboards.io** | **Miro** | **Notes** |
| Text | [Text](https://developers.miro.com/docs/text-1) | N/A |
| Shape | [Shape](https://developers.miro.com/docs/shape-1) | - The heart shape will be imported as a cloud shape. - The paperTape shape will be imported as a flowchart_input_output flowchart shape. - An icon will be imported as an image. |
| Card | [Sticky Note](https://developers.miro.com/docs/stickynote-1) | - Font formatting will be lost when converting to a card. - Card color will be lost and the alignment will be off. - The size of the sticky note might differ. |
| Line | [Connector](https://developers.miro.com/docs/connector_intro) | N/A |
| Frame | [Frame](https://developers.miro.com/docs/frame-1) | Child objects of the frame cannot be linked to the parent frame. |
| Free Draw | [Image](https://developers.miro.com/docs/image-1) (.svg) | N/A |
| Comments | N/A | There is no method provided in Miro to map this. |
| File | [File](../../troubleshooting-technical-questions/technical-guidelines/03-supported-file-formats.md) | File type and file format:   - Images - Tables and spreadsheets - Text documents - Presentations |
| Image | [Image](https://developers.miro.com/docs/image-1) | N/A |
| Embed iFrame | [Embed](https://developers.miro.com/docs/embed-2) | N/A |
| Card Table | [Card](https://developers.miro.com/docs/card-1) and [Frame](https://developers.miro.com/docs/frame-1) | Without the column and swimlane name. |
| Mind map | [Mind map](https://developers.miro.com/docs/mind-maps) (Experimental) | Border color is not supported. |
| GitHub Card | [Card](https://developers.miro.com/docs/card-1) | N/A |
| Jira Card | Text with Jira Issue URL | N/A |
