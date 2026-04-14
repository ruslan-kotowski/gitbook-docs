---
title: 'Board history: versions'
article_id: 360021668819
sidebar_position: 12
created_at: '2021-05-17T11:56:55Z'
updated_at: '2026-01-06T19:02:16Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: activity-list
availability:
  roles: board_owner, Board co-owners, Board editors who are members of the team where
    the board is located [if they are allowed to copy the board content](#limit-or-disable-restoring-previous-board-versions)
  plans: starter, business, enterprise, education
  platforms: browser, desktop, Tablet app
---

All versions of your Miro boards are automatically saved in your board history. You can review and recover changes at anytime.

### Key features

- Boards are backed up every hour if a change has been made, as well as at the end of each collaborative session
- Saved board history versions are stored for *90 days*
- The original board is *not* changed. The restored version is created as a *separate* board and its title is by default dated

:::warning
Occasionally, unforeseen network issues might prevent a board from backing up. Make sure you have a stable internet connection for consistent backups.
:::

### Restore a previous version of a board

To restore a previous version:

1. In the Board bar, select the vertical **three dots**.
   The **Main** menu opens.
2. Select  **Board** > **History**.
   The **History**panel opens. The **Activity** tab is open by default.
3. Select **Versions**.
4. Select a version.
   The **Restore as a separate board** modal opens.
5. (Optional) Follow the on-screen instructions.
6. Select **Restore**.

### Limit or disable restoring previous board versions

- The feature is available to [board owners](../sharing-boards/01-board-access-rights.md#board-access-rights), co-owners, and can be enabled for [editors](../sharing-boards/01-board-access-rights.md) that are members of the team where the board is located
- The feature depends on the [board content settings](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md): the option is available for team members only if the board owner allows team members to copy the board content. This can be configured on the board **Share** button > **Sharing settings** > **Permissions**
- [Content Admin permissions](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md) on the [Enterprise plan](../../plans-billing/miro-plans/04-enterprise-plan.md) - when enabled, - allow Company Admins to access board **Versions** even when it's disabled by the content settings by [reassigning the board ownership to themselves](../sharing-boards/01-board-access-rights.md#transferring-board-ownership-to-another-board-collaborator)

If you don't have permission to use the option, you will see the corresponding message in the **Versions** tab. Reach out to the board owner to get the feature enabled.

## FAQ

**I have recently [upgraded my team](../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md). Can I restore a board version that was created when my team was on Free plan?**

Yes, after your upgrade you can restore versions created while you were on a Free plan.

**I do not have versions in the board history. Why?**

Please note that the feature is not supported in [free teams](../../plans-billing/miro-plans/09-free-plan.md). Besides, please make sure that your role on the board allows you to restore versions (you should be the [board owner](../sharing-boards/01-board-access-rights.md#board-access-rights), [co-owner](../sharing-boards/06-co-owners-of-boards-and-spaces.md), or [editor](../sharing-boards/01-board-access-rights.md) and be a member of the team where the board is located). Additionally, the board owner/co-owner should allow team members to copy the board content.
If you deleted an object, you can also restore it - check out [this guide](../working-on-the-board/18-restoring-board-content.md).
