---
title: Manage user invitations on Enterprise Plan
article_id: 360017571534
sidebar_position: 5
created_at: '2019-02-11T10:09:16Z'
updated_at: '2026-02-19T10:45:59Z'
draft: false
availability:
  roles: company_admin
  notes: 'Relevant for: Enterprise Plan'
---

Learn how to manage invitations to your Enterprise Plan, including how to add or remove team members, change invitation permissions, and manage Guests.

## How to invite new members

There are three ways to invite new members to a team. Depending on your [team privacy settings](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) some invitation options may not be available.

Learn more about [Invitation settings on Enterprise Plan](03-invitation-settings-on-enterprise-plan.md).

Dashboard Team settings Company settings

1. Open the teams list from your [dashboard](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md).
2. Click on the users icon next to the team name you'd like to add users to.
3. The team settings panel will open.
4. Click **Add people to team**.
5. Enter the email addresses of the people you'd like to add, or click on **Add users from Company**.
6. Choose whether you want to add them as **Free members** or **Free restricted members**.
7. Click on **Send invitations**.

1. Open your **Company settings**.
2. Go to **Teams**.
3. Click on the Team you want to add members to.
4. The team settings panel will open.
5. Click **Add people to team**.
6. Enter the email addresses of the people you'd like to add, or click on **Add users from Company**.
7. Choose whether you want to add them as **Free members** or **Free restricted members**.
8. Click on **Send invitations**.

1. Open your **Company** settings.
2. Go to **Users** > **All users** > **Active users**.
3. Click **Invite people** in the top-right corner.
4. A dialog will open.
5. Enter emails (up to 500) of the users you want to invite or click **Add users from Company** and select users from the list.
6. Click the **+ Add teams** button to select which team(s) the users should be added to.
7. Click **Send invitations**.

### What happens after inviting new team members

All invitees will receive an email notification with a link. When the invitee clicks on the link in the email, new users will be asked to sign up, while existing users can log in.

**Registered Miro users** will immediately find the new team on the left sidebar of their dashboard upon signing in.

**Non-registered Miro users** will have 30 days to activate the invite. Reminder emails will be sent on the 3rd, 7th, 14th, 21st, and 28th days. On the 30th day the invitation expires, and the user is deleted from the active user list.

## Managing invites on the Flexible Licensing Program (FLP)

> **Relevant for:** Enterprise Plan
> **Who can do it:** Company Admin

On FLP subscriptions, Company Admins have full control over the invitation flow including conflicting permissions and deactivations cases. For example, admins can first reactivate a user and then change their permissions.

**Permissions**

If a user is already enrolled in your Enterprise subscription and you extend an invitation with altered permission levels, you will have the option to modify their existing permissions, extend the invitation with their current permission settings, or exclude them from the invitation altogether.

**Reactivating a user**

If an invitee is deactivated, you will be able to reactivate them or remove them from the invitation.

**Inviting users from outside your company domains**

If you try to invite a user from a domain that is not allowed in your plan, update the allowlist and then validate the user again. You can keep the invitation flow open and update the allowlist in another window. Once you have added the domain to the allowlist, click **Validate again after updating allowlist**.

## Managing Guest invites

You can invite users to a board without adding them as a team member by inviting them as Guests.

The level of access a Guest may have (view, comment, or edit) depends on your license type and team permissions.

|  |  |  |
| --- | --- | --- |
| **License type** | **Non-flexible licensing (non-FLP)** | **Flexible Licensing Program (FLP)** |
| **Guests** | Can comment and view | External guests with an email outside your company domains can edit |

Learn more about [user roles on the Flexible Licensing Program](11-user-access-levels-on-enterprise-plan.md#miro-roles).

### Inviting external guests on the Flexible Licensing Program (FLP)

:::note
External guests are guests outside your company domain. They will have an external company email.
:::

You can invite external **Guests** with editing access on an [FLP license](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md) without adding them as a team member and using up a license:

- If the option to invite external guests with edit access is enabled for your Enterprise Plan. For more details, please reach out to your Miro contact person.
- If the invitee is already an Advanced, Standard, or Full (legacy) member of *another team* within the same Enterprise subscription. You can invite existing members to edit a specific board as a Guest.

### How to invite a Guest to a board

When sharing a board, enter the email address of the user and select **can view** or **can comment** from the dropdown.

**If you have permissions to invite members to a board**, you will see a pop-up with two options when inviting someone with edit access. One of the options is to add them as a Guest, which gives them access to the current board only. The other option is to add them as a Member, which would also give them access to other boards within the team.

To invite someone as a Guest with edit access, choose **Add them to this board only** in the dialog.

Users with a [Free Restricted](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) license cannot be invited as Guests with edit access. The Company Admin will need to revoke the Free Restricted license first.

### Team invitation settings for Guests

Company Admins can see all current Guests in their **Company settings** > **Users** > **Active users**.

Guests can only access the boards they’re invited to, and can request additional access to the team. Learn more about [collaboration with Guests](../../using-miro/sharing-boards/07-collaboration-with-guests.md).

Company Admins can **restrict Guests** in the [Invitation settings](03-invitation-settings-on-enterprise-plan.md). Admins can also [set up automatic deactivation of inactive guests](03-invitation-settings-on-enterprise-plan.md). You can also allow Guests outside your [allowed company domains](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

## Manage ongoing invitations

> **Who can do it:** Company Admin

To filter and manage all your invitations in one place go to your **Company** settings > **Users** > **Access requests**.

Under **License requests** you will see the list of non-registered emails that have received and not accepted an invitation to Miro within the last 30 days. You can also see when they were invited and who invited them.

If an invitee doesn't accept the invitation within 30 days, it expires and the user is deleted from the list. To resend the invitation, simply invite the user again.

### Revoke an invitation

If you need to cancel an invitation, click the **X** icon next to a user.

### Bulk-revoke invites

Company Admins are able to bulk-revoke invites.

Navigate to **Company settings** > **Users** > **Access requests** to see the list of invites. You can select several users by checking boxes on the left side. You can select up to 50 users at once.

:::tip
More bulk actions are available in the Active users list. Scroll down to the end of the Active users list to see invited users. Select the list of invitees to add them to teams.
:::

## Frequently asked questions

**Why didn’t the user receive the email invite?**

If a user cannot find the invite in their inbox, please ask them to check their Spam, Promotions, Junk, Social, and Updates folders. A firewall may also be preventing the email from reaching their inbox. Learn [how to allowlist Miro mailers](../../using-miro/tools/troubleshooting/02-allowlist-miro-mailers.md).
