---
title: How to save board backup
article_id: 360017572774
sidebar_position: 5
created_at: '2019-02-11T10:14:51Z'
updated_at: '2025-12-02T10:14:09Z'
draft: false
availability:
  roles: board_owner, Board co-owners, Company Admins with [Content Admin permissions](../../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)
    on [Enterprise Plan](../../../plans-billing/miro-plans/04-enterprise-plan.md)
  plans: starter, business, enterprise, education
  platforms: browser, desktop
---

Create archived copies of your boards by saving board backups. Backups allow you to ensure the safety of your content and share copies of your boards with other Miro users.

## Save a board backup

To create a backup:

1. Open the board and click on the **vertical three dots** (![icon-main.svg](images/27743904151698_icon-main.svg)) icon.
2. Select the **Board** submenu.
3. Then select the **Export** submenu.
4. Choose the **Download board backup** option and follow the on-screen instructions.

![backup-entry-point.png](images/21537453245330_backup-entry-point.png)
*Downloading board backup*

You can also save a backup from your dashboard. Open the board's menu by clicking the **three dots** (**...**) icon and select **Download board backup** from the options.

The **.rtb* file will be saved to your device.

:::warning
Please note that **only board owners** and co-owners can download backups of boards located in **paid** teams. If this option is greyed out in the Export menu, please check if this functionality is [available on your plan](../../../plans-billing/miro-plans/02-plans-and-features-available.md) and if you are the [owner of the board](../../sharing-boards/01-board-access-rights.md) or [board co-owner](../../sharing-boards/06-co-owners-of-boards-and-spaces.md).
:::

## Restore a board from a backup

The option to upload a board backup is available for any user in paid teams. You can send an archived copy of your board to another Miro user so that they can recreate the board copy in their paid team.

To restore a board from a backup:

1. From the [dashboard](https://miro.com/app/dashboard/), click **Create New**.
2. Select **Import**.
3. Then select **Import backup**.
   A dialogue box will appear.
4. Choose your **.rtb* board backup file.
5. After you confirm your choice, a new board with the same content will be created in the team. The board title will include **Restored**.

After restoring the board, you also have the capability to move the board to a different space within your team.

![backup-import.png](images/21537453249938_backup-import.png)
*Restoring a board from backup*

## Troubleshooting

Please note both board backup downloads and uploads are limited. For downloads, there is a limit of **1GB**. If your board is larger than that, you'll need to either split the board into smaller boards or rely on the [board versions](../../managing-boards/12-board-history-versions.md) instead of downloaded backups of the board.

As for uploads, the Miro interface can upload board backups of a maximum of **1GB**. To upload larger backup files, please contact the Miro Support team:

1. Log in to Miro and submit your request [using the Support form](../../tools/troubleshooting/06-contacting-miro-support.md#how-to-contact-miro-support).
2. Attach your backup file to your request or upload it to any cloud storage and send us the link to it (please make sure to allow anyone with the link to download the file).
3. If your backup file is less than 1GB and you still have issues uploading it, please check the troubleshooting steps [on this page](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

If you get the error: **Can't find existing resource duplicate for optimized resource 0** when trying to upload a backup, it means that the board backup contains a resource that needs to be deleted. You can [send the .*rtb* file to Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md#how-to-contact-miro-support) so that we can delete the resource data to ensure the successful upload of the backup.

:::note
If you have issues saving a backup, try the troubleshooting steps from [this article](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).
:::

## FAQ

**I don't have the option to download board backup. Why?**

Please note that only board owners/co-owners in paid teams or Company Admins with [Content Admin permissions](../../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md) on [Enterprise plan](../../../plans-billing/miro-plans/04-enterprise-plan.md) can save board backups.

**What to do if my board has been deleted?**

Check this guide: [How to restore a deleted board](../../managing-boards/08-how-to-restore-a-deleted-board.md).

**Can I make backups of several boards in bulk?**

This is not currently possible. You'll need to back up each board individually.
