---
title: Airtable
article_id: 360012807619
sidebar_position: 1
created_at: '2020-03-24T12:09:00Z'
updated_at: '2025-08-05T07:33:41Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  roles: All Miro users, users on paid Airtable plans
  platforms: browser
  notes: 'Miro Plans: All plans'
---

Bring the power of whiteboard visualization to your work while using Airtable! You can export data from Miro to Airtable and embed Miro boards in Airtable bases to view, comment, and edit them right within Airtable.

## Export data from Miro boards to Airtable

The Airtable Sync integration allows you to export data (e.g., sticky notes, cards) from your Miro boards and organize it in Airtable. To learn more about setting up and using this feature, please visit [Airtable's official documentation](https://support.airtable.com/docs/airtable-sync-integration-miro).

## Embed Miro boards into Airtable bases

### Install the Miro app in Airtable

:::warning
The Miro app for Airtable is **not** available in the **Safari** browser.
:::

Base editors in Airtable can install the Miro app. To do this:

1. Open your Airtable base and click **Extensions** in the top right corner.

   ![Airtable extensions button in the top right corner.](images/21017651877394_Airtable%20extensions.jpg)
   *Extensions button in the top right corner of an Airtable base.*
2. Click **Add an extension**.

   ![Add an extension option in Airtable.](images/21017647938834_add%20an%20extension.jpg)
   *The option to add a new extension.*
3. Search for "Miro" in the Airtable Marketplace and click **Add**.

   ![Miro app in Airtable Marketplace.](images/21017647933714_Miro%20in%20Airtable.jpg)
   *Miro app on the Airtable Marketplace.*

### Add existing Miro boards to Airtable bases

Once the Miro app is added to your Airtable base, click **Add a board** in the Miro app section that appears in your extensions panel.

![Add a Miro board button in Airtable.](images/21017651876498_add%20a%20Miro%20board.jpg)
*Adding a Miro board via the Miro app in Airtable.*

A Miro board picker will appear. If you are not already logged into Miro in your browser, you will be prompted to sign in or create a Miro account.

After selecting a board, set the sharing permissions for how it will appear in Airtable using the dropdown menu. You have three options:

- **Anyone can view:** Anyone in Airtable can [view](../../using-miro/sharing-boards/01-board-access-rights.md) the embedded board's content.
- **Anyone can comment:** Anyone in Airtable can [leave comments](../../using-miro/sharing-boards/01-board-access-rights.md) on the embedded board. (Note: This option is not available for boards stored in Miro [Free plans](../../plans-billing/miro-plans/09-free-plan.md).)
- **Private:** The board will adhere to its existing sharing settings as configured on the Miro side.

  > ✏️ For Miro [Enterprise plan](../../plans-billing/miro-plans/04-enterprise-plan.md) users, your access settings will follow organization-wide access controls, which might mean some sharing options are restricted. Learn more: [Managing Enterprise sharing policy for embed integrations](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).

![Sharing settings options when adding a Miro board to Airtable.](images/21017651879826_board%20access%20in%20Airtable.jpg)
*Sharing settings when adding a Miro board to Airtable.*

The embedded Miro board will then appear in your Airtable base, where you can view, comment, or edit it based on the permissions set.

![Embedded Miro board within an Airtable base.](images/21017651872402_Miro%20board%20in%20Airtable.jpg)
*An embedded Miro board in Airtable.*

To replace an embedded board with a different one, click the gear icon (**Settings**) for the Miro app in Airtable, select **Choose a board**, and pick another board from the Miro picker.

![Replacing an embedded Miro board in Airtable.](images/21017647932690_replacing%20a%20board.jpg)
*Replacing an embedded Miro board in Airtable.*

### Create new Miro boards from Airtable

To create a new Miro board directly from Airtable:

1. In the Miro app section within Airtable, click **Add board** (or **Choose a board** if one is already embedded and you are replacing it).
2. In the Miro picker, select the option to create a **New board**.

![Creating a new Miro board from the picker within Airtable.](images/21017651880466_add%20a%20new%20board%20to%20Airtable.jpg)
*Creating a new Miro board from the picker in Airtable.*

The new board will be created in your Miro account and embedded in your Airtable base.

### Remove Miro boards from Airtable

To remove an embedded Miro board from your Airtable base, you need to remove or reconfigure the Miro app extension within that base. Click the dropdown menu on the Miro app in the extensions panel and choose to remove or manage the extension.

![Deleting the Miro app from Airtable extensions panel.](images/21017647933074_deleting%20the%20app.jpg)
*Removing the Miro app from the Airtable extensions panel.*
