---
title: Team invitation settings
article_id: 13205512707858
sidebar_position: 3
created_at: '2023-08-21T13:54:06Z'
updated_at: '2025-06-23T13:54:36Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
availability:
  roles: team_admin, company_admin
  plans: free, starter, education, business, enterprise
  platforms: browser, desktop, mobile
---

Admins can specify which team members can invite new members to their free or paid plan. For example, admins can enable only admins to invite new members.

Optionally, admins can also allow all team members to invite new members.

:::note
For paid plans, when an invitee accepts an invitation from an existing team member, including admins, a license is automatically added to your subscription.
:::

If you enable admins only to add new team members, then existing, non-admin members do not have the option in Miro to invite new members.

:::tip
For Business and Enterprise plans, Company admins can [configure invitation settings](../get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md#team-admin-company-admin) for each team individually inside their subscription.
:::

## Manage team invitation settings

To manage team invitation settings on a Free, Starter, or Education plan, ensure that you have the Team admin role.

To manage team invitation settings on a Business, or Enterprise plan, ensure that you have the Company admin role.

### Free, Starter, and Education plans

As Team admin, follow these steps:

1. From your Miro dashboard, click your avatar in the top-right, and select **Admin Console**.
2. Go to **Security** > **Permissions**.
3. Under **Invitation**, select who can invite users to your team.
4. (Optional) To provide a team link that anyone can follow to join, toggle **Enable team invite link** to the on position.

:::note
For Starter and Education plans, if team members are not allowed to invite new members, then any member who sends an invitation to edit sees a pop-up with **Ask admin to give edit access** pre-selected. The team member can send their invitation, but the invitee is added as a guest or commenter, pending admin approval for edit access. Only team members can edit boards.
:::

### Business plan

As Company admin, follow these steps:

1. From your Miro dashboard, click your avatar in the top-right and select **Admin Console**.
2. Click **Teams**.
3. Under **Team name**, select a team.
   The team settings panel opens.
4. Click **Settings**.
5. Under **Invitation**, select who can invite users to this team.
   > ⚠️ Your licenses are automatically increased when a new user is added. If you allow anyone to invite new users, then anyone can incur new licenses added to your subscription.
6. Select **Allow** or **Don't allow** for [guests](../../using-miro/sharing-boards/07-collaboration-with-guests.md).
7. In the top right click the **X** to close the team settings panel.
   Your settings are saved.

:::note
If guests are not allowed, then a team member who tries to invite a guest sees a pop-up informing them that guests are not allowed.
:::

### Enterprise plan

To learn about team invitation settings on an Enterprise plan, see [Team permissions on Enterprise plan](../../enterprise-administration/managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md).
