---
title: Smartsheet app for Miro
article_id: 5753415785618
sidebar_position: 16
created_at: '2022-05-25T06:41:50Z'
updated_at: '2025-01-13T14:57:02Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: smartsheet
availability:
  plans: browser version on desktop
---

Key features:

- Export sticky notes from Miro to rows in a new or existing sheet within Smartsheet
- Import rows from Smartsheet to a Miro board as cards
- Update work in both Miro and Smartsheet with two-way sync

:::warning
To make the app work in Safari, turn off the **Prevent cross-site tracking** option in the browser settings
:::

### How to install the app

You can install the app from [Miro Marketplace](https://miro.com/marketplace/smartsheet/). Find **Smartsheet for Miro** and click **Get app**. You will be redirected to the page to select the team to which you want to add the Smartsheet app. Choose the team in the picker and click **Install & authorize.**

:::warning
**Non-admin users can't install the app if it's not allowed in [settings](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).** **⚠️ Enterprise plan Company Admins may need to approve the app in settings. [Learn more](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).**
:::

![installing_smartsheet_app.jpg](images/21017653534098_installing%20smartsheet%20app.jpg)
*Selecting a Miro team to install the app*

You can also install **Smartsheet** from within a Miro board:

1. In the Creation bar, select **Tools, Media and Integrations** (**+**).The **Tools, Media and Integrations** panel opens.
2. In the **Tools** tab, search and select Smartsheet.
   The **Smartsheet** modal opens and you'll be prompted to allow permissions

![smartsheet-entry-point.png](images/21537438852626_smartsheet-entry-point.png)
*Installing the app from within a Miro board*

**When prompted whether you want to connect your Miro and Smartsheet account, log in to your Smartsheet account and allow access to the app.**

![allow_access_to_Miro.jpg](images/21017683153682_allow%20access%20to%20Miro.jpg)
***Allowing the app to access your Smartsheet account***

### How to export Miro sticky notes or Cards into Smartsheet rows

1. Open the Smartsheet app on the toolbar. If you haven't logged in to Smartsheet yet, you will need to do this first. Then select the sticky notes you’d like to convert.
2. Select your Smartsheet workspace, sheet (new or existing), and row you’d like to add the content from the sticky notes to. You can also create a new sheet and export the stickies to the new one.
3. Finally select **Convert to Smartsheet row**. The content will now be exported to Smartsheet. The sticky notes will be automatically converted into Smartsheet cards.
   Note that the cards will not sync with Smartsheet unless you import the corresponding rows from Smartsheet to Miro (coming soon). See below how you can [import Smartsheet data to Miro](#how-to-import-smartsheet-rows-into-miro).
   ![smartsheet_export.gif](images/21017683165842_smartsheet%20export.gif)
   *Exporting sticky notes from Miro to Smartsheet*

### How to import Smartsheet rows into Miro

1. Open the Smartsheet app in Miro and change the tab from **Convert from Miro** to **Choose from Smartsheet**.
2. Click **Choose from Smartsheet** and you'll see the picker with your existing sheets. You'll have the option to filter rows based on a specific workspace and choose a sheet.
3. Select all the rows you’d like to import by checking the box and selecting **Import**.
4. The rows will be imported as cards.
   ![import_from_smartsheet.gif](images/21017683161874_import%20from%20smartsheet.gif)
   *Importing data from Smartsheet to Miro*
5. You can edit the rows right within Miro: select a card, click the expand icon, apply changes, and click **Save changes**. Any updates to the cards will be reflected in Miro and Smartsheet.
   ![edit_Smartsheet_card.gif](images/21017683164818_edit%20Smartsheet%20card.gif)
   *Editing a Smartsheet card in Miro*
