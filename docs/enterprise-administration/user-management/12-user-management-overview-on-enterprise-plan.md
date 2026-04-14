---
title: User management overview on Enterprise Plan
article_id: 360017571474
sidebar_position: 12
created_at: '2019-02-11T10:09:06Z'
updated_at: '2026-02-26T14:12:09Z'
draft: false
availability:
  plans: '[Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) plan'
  roles: company_admin
---

You can easily manage user permissions of dozens, hundreds, or thousands of Miro users within your plan. Admins can track and filter user lists and view user roles, activity rate, and license consumption. Use bulk actions like inviting, adding, and removing users, assigning roles and licenses, and moving users between teams. Save time and gain additional transparency into how your Miro plan functions by mastering quick administrative operations in Miro.

All the corporate users who belong to domains that are claimed and verified via Domain control are [Managed users within your Enterprise organization](06-managed-users-on-enterprise-plan.md).

## Active users section

To open Team settings, click the team name in the upper left corner of your dashboard and then click the **Team members** icon.

Company settings will open with a list of users on the chosen Team. In this section, Company and Team admins can add or remove users from the team, and promote or revoke the Team admin role.

Company admins can also convert a guest to a member with a Standard or Full (legacy) license. To revoke or downgrade an Advanced, Standard, or Full (legacy) license, Company admins can instead give the member a [Free restricted](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) license.

:::note
Employees who share a verified domain are members with an Advanced, Standard, Full (legacy), Free, Free Restricted license. For Enterprise plans, only users from an external domain can be added as guests.
:::

:::note
Team Admins can invite new team members if this is allowed in [Invitation settings](05-manage-user-invitations-on-enterprise-plan.md).
:::

To see the full list of the users in your Enterprise subscription, go to **Company settings**. On the left-hand side, under **Users**, select **All users** to open the list of Active users (you can also switch to the **Deactivated users** and **Invitations** tabs from this screen). You'll see the list of all users added or invited to teams or boards within that particular subscription, as well as their **Last activity** date.

:::note
To get to Company settings from Team settings, click **Company** in the upper-left corner.
:::

As a Company Admin, you can download a full list of users in your organization along with their last log-in. Find the **Download CSV** button above the list of Active users.

In the **Active users** section, you will see the entire list of users along with their Role, License, Teams, and Activity.

The **Role** defines the access levels within the plan. While Company Admin is the most powerful role with the ability to manage the plan, a guest can only access the boards that they are invited to. Learn more in [the article about access levels.](11-user-access-levels-on-enterprise-plan.md)

The **License type** shows if a user is consuming a Advanced, Standard, Full (legacy), or Free license.

The **Teams**is the number of teams within the plan a user is added to.

**Last** **activity** shows when a user has opened any board within the subscription. Filter active/inactive users by selecting dates on the calendar or use one of the preset options: 30, 60, 90, or 180 days. We define an active user as someone who has used Miro within the last 90 days

### Changing single user status

As a Company Admin, you can change the role, the license, and the number of teams for any user or group of users. You can also [deactivate a user](01-deactivated-users.md) and then [remove them](10-remove-users-on-enterprise-plan.md). To access these options, click the **three dots** (**...**) icon next to any team member's row.

:::tip
The advanced user management system helps you manage the resources you’ve purchased more effectively. If you have [Flexible Licensing Program](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) activated, you can release licenses of inactive users by converting them to Free Restricted.
:::

### Filters

If you have dozens, hundreds, or thousands of Miro users **search**by email and name or **filter the list**by a specific criteria to find anyone quicker. You can also hide invited users to see only registered Miro users in your plan.

Once filters are applied, you can bulk select up to 50 users on the list and use bulk actions.

### Bulk actions

The**bulk actions**button helps you manage user groups faster. Select several users to apply necessary changes in bulk.

You can select users one by one by checking boxes on the left or apply filters and select up to 50 users at once.

#### Bulk manage active users

In the **Active users** list, select the list of users to apply one of the actions below.

1. Bulk manage team membership.
   1. Add or move users to a team.
   2. [Create a new team](../managing-enterprise-teams-and-content/09-create-a-new-team-on-enterprise-plan.md) and add users.
2. Bulk manage Licenses and Roles.
   1. Switch to Advanced Member. Advanced licenses are not supported under the Flexible Licensing Program (FLP) and always operate on a non-FLP (hard limit) model. You can only assign up to the number of Advanced licenses your organization has purchased. Organizations using FLP for Standard can continue to do so while keeping Advanced on a hard limit, allowing a mixed licensing model: Standard can remain on FLP (unlimited Free licenses with automatic downgrade to Free Restricted), while Advanced stays fixed to the purchased license quantity. Users who need Advanced features must be explicitly assigned an Advanced license or follow your organization’s upgrade or request flow.
   2. Switch to Standard Member or Full Member (legacy).
   3. Switch to Basic Member.
   4. Switch to Guest or Team Guest.
   5. Switch to Free Restricted (available for [FLP Enterprise subscriptions](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)).
3. Change the billing group or create a new one.
4. Revoke Restricted.
5. Bulk [deactivate users](01-deactivated-users.md)

#### Bulk manage invitations

Switch to the Invitations tab to see invited users (non-registered users that were sent invitations to join your subscription less than 30 days ago and have not registered with Miro yet). Select the list of invitees to apply one of the actions below.

1. Bulk manage team membership.
   1. Add users to several teams with or without removing from the current ones.
   2. Add users to a new team ([create a new one](../managing-enterprise-teams-and-content/09-create-a-new-team-on-enterprise-plan.md)).
2. Bulk [deactivate](01-deactivated-users.md) users.
3. Bulk change user licenses.

#### Bulk delete from a team

In the **Teams** list select the Team where you would like to delete users. Once you select the users, you can bulk delete them from the team.

### User info

User info is an individual and editable status card for each user within your plan. Opposite to bulk management, you can see the status and manage a person individually. Each user has a **User profile** with a picture, name, email, number of boards, number of projects, number of templates, current teams, and license. To open a user card, click the **three dots** (**...**) icon on their row and select **User info**.

:::note
User details include an **Internal** or **External** classification. Internal users sign in with an email address from a verified domain. External users do not. For more information, see [Domain Control: Internal and external users](../canvas-25-admin-features/domain-control/01-domain-control.md#internal-and-external-users).
:::

Company Admins can change the team membership and grant Admin rights to a user directly from the card. Note that Admins cannot change such user details as name, profile picture, email - instead, the users can do that in their Profile settings. If you use [SSO](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), the data is automatically attributed by your identity provider upon successful login.

### Frequently asked questions

1. *I’m getting a lot of requests from users to add them to different teams. I want to stop receiving these notifications.*
   - Your [Team privacy](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) is probably disabled, which means that Enterprise users can discover new teams to join within the organization. If you want to stop receiving these requests, you can either:
   - Toggle-on the privacy, so users are not able to discover new teams in the organization or
   - Make the teams completely open, so users don't need to have your approval to join the team
2. *A lot of users are getting a Standard license or Full (legacy) assigned but I didn’t assign any. Why?*
   - For each team, you can define who should be able to invite users to a specific team. Make sure to configure your [invitation settings](03-invitation-settings-on-enterprise-plan.md). You can also activate the [Flexible Licensing Program](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) and set the default (Free or Free Restricted) license that users will get upon joining your plan.
