---
title: User Groups
article_id: 30658859384594
sidebar_position: 8
created_at: '2025-10-30T13:00:25Z'
updated_at: '2026-01-20T13:17:27Z'
draft: false
availability:
  roles: (Setup) Company admins, team_member
  plans: enterprise
  platforms: browser, desktop, mobile
---

As Company admin, User Groups enable you to manage access to content for groups of users, instead of sharing with each individual member. All members of your organization can see and share their content with User Groups that you create.

This article explains how to create, manage, and share content with User Groups. For more general information about the capability, see [User Groups overview](07-user-groups-overview.md).

:::note
To learn about managing User Groups via SCIM, contact your Miro CSM or Support.
:::

## Company admin guide

### Create a User Group

1. As Company admin, go to Admin Console.
2. Go to **Users** > **Groups**.
3. In the top-right, click **+ Create group**.
   The **Create new group** modal opens.
4. Name your group.
5. (Optional) Add a description for your new group. You can always add or edit your description later.
6. Click **Create group**.
   Your new group is added to the **Groups** view.

### Add users to a User Group

1. In Admin Console, go to **Users** > **Groups**.
2. For the User Group you want to manage, select the three-dots (**...**) at the end of the row.
3. Click **Add users**.
   The **Add users** modal opens.
4. To locate your user(s), search by name or email.
5. Tick each user you want to add.
6. Click **Add selected users**.
   Each selected user is added to your User Group.

### Add User Group to teams

1. In Admin Console, go to **Users** > **Groups**.
2. For the User Group you want to manage, select the three-dots (**...**) at the end of the row.
3. Click **Add to teams**.
   The **Add group to teams** modal opens.
4. To locate your team(s), search by name.
5. Tick each team that you want your User Group to join.
6. Click **Add**.
   Your User Group has joined each team that you selected.

   > ✏️ User Group members have edit access to all content in each team you selected.

### Edit a User Group

1. In Admin Console, go to **Users** > **Groups**.
2. For the User Group you want to manage, select the three-dots (**...**) at the end of the row.
3. Click **Edit group**.
   The **Edit group** modal opens.
4. (Optional) Rename your group.
5. (Optional) Add a description for your new group.
6. Click **Save**.

### Delete a User Group

:::warning
Deleting a User Group cannot be undone. By deleting a User Group, some users may be removed from some teams.
:::

1. In Admin Console, go to **Users** > **Groups**.
2. For the User Group you want to manage, select the three-dots (**...**) at the end of the row.
3. Click **Delete group**.
   The **Delete \{User Group name\}** modal opens.
4. Click **Delete**.
   The User Group is permanently deleted.

## User guide

### Share a board with a User Group

Team members can share a board with any User Group in their organization. The board is shared with all members in that User Group.

Follow these steps:

1. On a Miro board, in the top-right click **Share**.
   A modal opens.
2. Enter the name of your target User Group.
3. From the auto-populated options, select the User Group.
4. (Optional) Update permissions. Default: **Can edit**.
5. (Optional) Add a custom message.
6. Click **Send invitations**.
   Each user in the User Group receives an email invitation to access your board.

### Share a Space with a User Group

Team members can share a Space with any User Group in their organization, and specify permissions. The Space is shared with all members in that User Group.

Follow these steps:

1. From the Miro dashboard, for the Space you want to share click the vertical three-dots to open the **Options** menu.

   > 💡 Alternatively, in the Spaces sidebar, at the top click the vertical three-dots to open the **Options** menu.
2. Click **Share**.
   The **Share Space '\{Space Name\}'** modal opens.
3. Enter the User Group name.
4. (Optional) Update permissions. Default: **Can edit**.
5. (Optional) Add a custom message.
6. Click **Send invitations**.
   Each member in the User Group receives an email invitation to access your Space.

:::note
Members added to the User Group have access to shared Spaces automatically. For members removed from the User Group, their access is automatically revoked.
:::
