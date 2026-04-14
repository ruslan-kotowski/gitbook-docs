---
title: How to allow or restrict copying and exporting boards and content
article_id: 360018350399
sidebar_position: 14
created_at: '2020-12-14T06:10:03Z'
updated_at: '2026-01-22T14:23:08Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
availability:
  roles: team_member, (Setup) Team admins, (Setup) Company admins
  plans: starter, business, enterprise, education
  platforms: browser, desktop, mobile
---

Company admins and Team admins can specify whether team members and non-team members can copy board content, and set the default copying setting for new boards.

Board owners and board co-owners can specify copying settings for other team members on a given board. If admins allow non-team members to copy boards, which includes visitors and guests, then board owners and co-owners can allow non-team members to copy.

If admins do not allow non-team members to copy content, then the board option to allow non-team members to copy a board is removed.

:::note
On Free plans, copying boards is enabled by default and cannot be modified.
:::

## How to set board copying permissions for a team

For a given team, a Company admin or Team admin can specify whether non-team members can copy and export boards and content, and set the default copying permissions for newly created boards.

Follow these steps:

1. Go to **Admin Console**.
2. Click **Teams**.
3. Click the row for **\{Team name\}**.
   The **\{Team name\}** panel opens.
4. Click to open the **Settings** tab.
5. Scroll to **Content Security**.
6. For **Copying Content**, specify whether only team members, or anyone in the organization, can copy board content.
7. Specify **Default setting for copying content**. Board owners can modify this setting for individual boards.
   Your settings are saved automatically.

:::note
If copying board content is not allowed for non-team members, then the option for **Anyone with board access** is removed from board settings. For example, visitors and guests are prohibited from copying content.
:::

:::note
Copying images between private boards connected to different teams is not possible. Talk to your Miro Company Admin about getting permission to access the other board in order to copy images.
:::

## How to set board copying permissions for a board

For a given board, a board owner or co-owner can specify who can copy the board.

Follow these steps:

1. On a board you own, co-own, or created, in the top-right click **Share**.
   The sharing modal opens.
2. In the bottom-right click **Sharing settings**.
3. For **Who can copy board content**, specify one option.

   > ✏️ If your Company admin or Team admin disables the option **Anyone with board access**, then the option is unavailable.
4. Click **Done**.
   Your changes are saved automatically and apply to anyone with access to the board.

## Board copying options per user type

Assuming **Anyone with board access** can copy content, the following table shows permissions per type of user.

|  | Save board as template | Copy board content | Export | Duplicate | Download files from board |
| --- | --- | --- | --- | --- | --- |
| Team members | ✔ | ✔ | ✔ | ✔ | ✔ |
| Guests | ✘ | ✔ | ✔ | ✔ | ✔ |
| Visitors with a Miro account | ✘ | ✔ | ✔ | ✔ | ✔ |
| Visitors without a Miro account | ✘ | (With edit access) ✔ | ✘ | ✘ | ✔ |

:::note
(Enterprise) If [moving boards between teams is not allowed](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md#restrict-ability-to-move-boards-to-other-teams-team-level), then the option to duplicate a board is unavailable.
:::

:::note
Some options are not available for certain categories of users even if the board owner allows anyone with the link to copy the board content
:::

## FAQ

*Why can’t I copy and paste content on a Miro board?*

The board owner or co-owner may not allow copying for your role. You can view your role in the Collaboration bar, in the top-right of a Miro board. Contact the board owner or co-owner to request copying permissions for your role.

You may also want to ensure that you are signed in to Miro. If your role has copying permissions, and you are signed in, sign in and open the board in another browser and try to copy.

*Why isn't **Anyone with board access** an available option for me?*

Your Company admin(s) or Team admin(s) have disabled this option. If you are a Company admin or Team admin, see [How to set board copying permissions for a team](#how-to-set-board-copying-permissions-for-a-team).

*How can I allow visitors to download files while restricting their ability copy or duplicate the board?*

Create a separate board with the files only, then enable copying board content for anyone with the board link. Share the board link with visitors.

Alternatively, you can embed the new board with the files, and copying enabled for anyone with the link, in the original board. For more information about embedding, [Embed a Miro board](../import-and-export/export/02-embed-a-miro-board.md).

*Why can't I find **Permissions** on the board **Share** menu?*

(Paid) Only the board owner and co-owner can specify content permissions. (Free) Content permissions cannot be modified from their default, which allows copying for all users.

*Can I specify who can upload content to my board?*

Anyone with **Can edit** rights can upload content to your board.
