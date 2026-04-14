---
title: Trash management
article_id: 13359286699666
sidebar_position: 9
created_at: '2023-08-29T08:11:06Z'
updated_at: '2026-01-06T19:02:16Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
availability:
  roles: '[Board Owners](../../getting-started/start-here/05-roles-in-miro.md#roles-on-boards-and-spaces),
    [Company Admins](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md#team-admin-company-admin)'
  plans: '[Starter](../../plans-billing/miro-plans/08-starter-plan.md), [Education](../../plans-billing/miro-special-pricing/03-education-plan.md),
    [Business](../../plans-billing/miro-plans/06-business-plan.md), [Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)'
---

With the improved trash management experience, admins have more visibility and control over the lifecycle of Miro boards, helping them to align with more restrictive compliance regulations that require content deletion after certain periods.

:::warning
Trash management is only available on paid plans. Customers on Free plan can restore boards by following the board’s link. These boards can be restored within 90 days of deletion.
:::

## How to access Trash

Trash is a common bucket where you can explore and manage all the boards that have been deleted. You can see trashed boards by **board name**, **team**, **project**, **owner**, **who deleted** the board, and **when**. Trash is also searchable by board name.

:::note
Board owners can only view their own boards in trash. Company Admins with Content Admin Permissions can view all boards across their organization in trash.
:::

1. Go to your dashboard: **miro.com/app/dashboard**.
2. Click your profile avatar in the upper right.
3. Click the Trash icon.
   ![trash-location.png](images/23853113452690_trash-location.png)
   *Trash in your Miro Dashboard*

## How to delete boards

:::note
Only board owners and Company Admins can delete boards.
:::

1. In your Dashboard, navigate to the team with the board(s) you wish to delete.
2. Find the board you wish to delete, click the **three dots** (**...**) menu at the far-right and select **Delete**.
3. You will be asked to confirm that you wish to delete the board. Click the **Delete** button.
4. Your board will now be moved to Trash.

You can also delete boards directly from the board itself using the info card. Read more about [deleting a board from its info card](07-how-to-delete-a-board.md).

## How to permanently delete boards

1. Navigate to **Trash**.
2. Find the board you wish to permanently delete, click the **three dots** (**...**) menu at the far-right and select **Delete permanently**.
3. You will be asked to confirm that you wish to delete the board permanently. Check the box to “Delete 1 board permanently”, then click the **Delete permanently** button.

:::warning
Once you permanently delete a board, you cannot retrieve it.
:::

## How to restore boards from Trash

1. Navigate to **Trash**.
2. Find the board you wish to restore, click the **three dots** (**…**) menu at the far-right and select **Restore**.
3. You will be asked to confirm that you wish to restore the board. Click the **Restore board** button.
4. Your board will be moved back to the team it was deleted from.

## FAQs

I’m a Miro Company Admin. My user has informed me they deleted a board accidentally. How can I recover this?

Use the steps in “[How to restore boards](#how-to-restore-boards-from-trash)” above. Please note that only board owners and Company Admins with “Content Admin Permissions” can restore boards.

Can I bulk delete/restore boards?

Bulk actions are not currently supported, but are planned for a future release.

Will team members be notified of a board’s deletion?

Team members will not be notified of a board’s deletion, nor will they be notified of a board’s permanent deletion.

Are there public APIs for deletion/restoration available?

Public APIs are not currently supported, but are planned for a future release.
