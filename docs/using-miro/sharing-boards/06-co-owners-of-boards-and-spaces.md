---
title: Co-owners of boards and Spaces
article_id: 360021580759
sidebar_position: 6
created_at: '2021-05-12T07:36:28Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
availability:
  roles: board_owner, Board co-owners, Space owners, Space co-owners, team_admin,
    company_admin
  plans: business, enterprise
  platforms: browser, desktop, mobile
---

The Co-owner role enhances collaboration by allowing board owners to delegate responsibilities for preparing and facilitating work on a board, whether for live or asynchronous sessions.

A co-owner ensures a seamless workflow even if the primary board owner is unavailable, as co-owners can perform nearly all owner-level actions, from managing board settings to controlling content visibility. A co-owner helps distribute the workload and provides a reliable backup for board management.

To learn which permissions a co-owner has for a board or Space, see [Co-owners reference.](#co-owners-reference)

## Enable the co-owner role for the organization

As Company admin, follow these steps:

1. From your Miro dashboard, click your avatar in the top-right and click **Admin Console**.
2. Go to **Security** > **Sharing** > **Roles and permissions**.
3. Toggle **Allow Co-owner role** to the on position.

Admins can now enable the co-owner role for their teams.

## Enable the co-owner role for a team

As Company admin or Team admin, follow these steps:

1. From your Miro dashboard, click your avatar in the top-right and click **Admin Console** | **Settings**.
2. Go to **Teams** > **\{team name\}** > **Settings**.
3. Under **Collaboration settings**, toggle **Enable Co-owner role on boards and Spaces** to the on position.

## Add co-owners to boards

As owner of a board, or an existing co-owner, follow these steps:

1. From your Miro dashboard, do one of the following:
   1. For a board click the three-dots (**...**) and click **Share**.
   2. Open a board, then click **Share** in the top-right.
2. Enter the email address for the user(s) you want to add as co-owner.
3. For their access rights, click **Is co-owner**.
4. (Optional) Add a custom message.
5. Click **Send invitations**.

:::note
You can assign the co-owner role only to team members. To add a co-owner from outside the team, first invite them to join the team.
:::

## Add co-owners to Spaces

As owner of a Space, or an existing co-owner, follow these steps:

1. From your Miro dashboard, do one of the following:
   1. For a Space in the sidebar, click the three-dots (**...**) and click **Share**.
   2. Open a Space, then click the label at the top that shows the number of members.
2. Click **Manage access**.
3. For a Space member, update their access rights to **Co-owner.**

:::note
You can assign the co-owner role only to Space members. To add a co-owner from outside the Space, first invite them to join the Space.
:::

:::note
A Space co-owner has Editor permissions for all content inside that Space.
:::

## Co-owners reference

### Board co-owner permissions

In addition to all Editor permissions, a board co-owner has the following permissions:

- **Manage board content settings and collaboration tool settings**
  Control who can copy board content and manage tools like the timer, voting, video chat, screen sharing, and attention management
- **Hide and reveal frames**
  Control the visibility of frame content during presentations or workshops.
- **Add protected lock**
  Prevent accidental moving or deletion of content during collaboration.
- **Add board password**
  Secure public boards by requiring a password for access.
- **Download a board backup**
  Create archived copies of boards. Co-owners can also restore boards from backups.
- **Add co-owners**
  Grant co-owner status to other users.
- **Change board details**
  Modify cover and rename the board
- **Share the board**
  Modify access rights for the team and other users on the board
- **Configure advanced board sharing permissions**
  Specify whether the board can be shared outside the team or organization

:::note
On Enterprise plans, board Co-owners and Content admins can move boards using the [Miro REST API](https://developers.miro.com/reference/update-board), which differs intentionally from the Miro UI experience, where only Owners can move their boards.
:::

A board co-owner cannot perform the following operations:

- Delete the board
- Move the board to another team
- Change the board owner

### Space co-owner permissions

In addition to all Editor permissions, a Space co-owner has the following permissions:

- Rename the Space
- Share the Space
- Modify access rights for the team and other users in the Space
- Add co-owners to the Space

A Space co-owner cannot perform the following operations:

- Delete the Space
- Change the Space owner

## FAQ

**I do not have the option to assign a co-owner. Why?**

The co-owner feature is available on Business and Enterprise plans. Your Company Admin must activate this feature in the team or company settings. Only existing team members can be promoted to co-owners. Ensure the user has been invited to the board via email before attempting to assign the co-owner role.

**I’m an admin with content admin permissions enabled. Why can’t I add board co-owners?**

Admins with Content Admin Permissions (CAP) need to first add themselves as an owner to the specific board. Once they are a board owner, they can then assign co-owners.

**Should I additionally pay for co-owners invited to my boards?**

Only existing team members can be designated as co-owners. If the user you want to make a co-owner is not already part of your team, you will first need to invite them to the team, which may involve purchasing an additional seat, depending on your plan and current user count. After they are a team member, you can assign them the co-owner role.
