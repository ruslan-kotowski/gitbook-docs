---
title: Invitation settings on Enterprise Plan
article_id: 4412315533842
sidebar_position: 3
created_at: '2021-12-13T04:56:26Z'
updated_at: '2026-02-19T10:56:01Z'
draft: false
availability:
  plans: enterprise
  roles: company_admin
---

Configure your Enterprise Plan invitation settings to manage who can invite new users to join your plan. You can customize your invitation settings to meet the requirements of your teams and wider company.

:::tip
If you’re new to Miro, learn more about [Team and Company settings](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md#team-admin-company-admin).
:::

## Team invitation settings

For smoother collaboration, allow **All team members** to invite new Members to the team. If you prefer to have more control over team invites, you can restrict this option to Company and/or Team Admins so that all invite requests are sent via [Request management](09-request-management-on-enterprise-plan.md). You can also control whether users can invite [Guests](../../using-miro/sharing-boards/07-collaboration-with-guests.md) to teams.

### How to configure team invitation settings

To manage your team invitation settings, in Admin Console go to **Teams** and select your team. Your team panel opens. Under **Invitation**, select one of the following options:

- **Company Admins only**
  Only Company Admins can add new Members to the team.
- **Company Admins and Team Admins**
  Company Admins and Team Admins can invite new Members to the team.
- **All team members**
  All team members can invite new Members to the team.

:::note
On [Flexible Licensing Program (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) subscriptions, the team invitation settings are complemented by [company invitation settings](#company-invitation-settings).
:::

### How to configure Guest invitations

Company Admins can allow or restrict the option for Members to invite [Guests](../../using-miro/sharing-boards/07-collaboration-with-guests.md). Guests can only access boards they’re invited to and do not require a license.

Update Guest invitation settings in **Teams** > select your team > **Settings** > **Allow Guests for [Name] team.**

:::note
Company Admins can enable the [automatic deactivation of Guests](#automatic-deactivation-of-guests) after 30 days of inactivity.
:::

## Invite scenarios

:::tip
Depending on the [Request management](09-request-management-on-enterprise-plan.md) settings, requests to share a board or invite a user to a team may be sent either directly to Company Admins, specific people via email, or a service desk ticket is created.
:::

**Inviting new Members to a team**

If Guests are not allowed, and Members are not allowed to invite new Members, when they try to share a board they will see the below notification and will need to submit a request.

**Granting the owner or co-owner role**

If Members are not allowed to invite new Members, and attempt to assign an owner or co-owner role to a Guest or a [Free Restricted](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) Member on a specific board, they will see the below notification and will need to submit a request.

**Inviting an external user or Guest to edit a board**

:::note
External Guests are Guests outside your company domain. They will have an external company email.
:::

If Members are not allowed to invite new Members to the team, and Guests with edit access haven’t been enabled for the team, when trying to invite an external user to edit a board users will see the below notification and will need to submit a request. After submitting the request, the invitee will be added to the board with comment access, allowing them to add comments on the board but not edit its content.

## Company invitation settings

Company invitation settings control who can invite new Members to your Enterprise subscription. All new Members are granted an Advanced, Standard, Full (legacy), Free, Free Restricted license depending on your [licensing model](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md#overview-of-licensing-models) and [default license](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

### How to configure Company invitation settings

> **Available for**: [Flexible Licensing Program (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)

To manage your Company invitation settings, go to **Company** settings > **Security** > **Sharing** > **Invitation** and select one of the following options:

**Company Admins only**
Only Company Admins can grant licenses to new Members. Team Admins and Members can only invite existing Members from the company to their teams, and they cannot activate new licenses.

**Company Admins and Team Admins**
Company Admins and Team Admins can invite new Members and add new licenses. Team Admins can only invite new Members to teams in which they are a Team Admin.

**All members**
Every member of the Enterprise subscription can add new licenses by inviting people to their team, as long as invitations are allowed for **All team members** in the [Team invitation settings](#how-to-configure-team-invitation-settings).

## How Company and Team settings work together

Company settings complement Team invitation settings. Company Admins can configure who can invite users to a specific team in the Team settings. This means that Company Admins can allow Members and Team Admins to manage their own team invitations and collaboration, but licenses are still controlled by Company Admins in the Company settings.

## Automatic deactivation of Guests

Set up the automatic deactivation of Guests after 30 days of inactivity. Use this feature to remove Guests and keep your subscription secure.

When the feature is turned on, any Guests (regardless of their domain) who have not been active in your Enterprise teams within 30 days will be automatically deactivated. It is not possible to customize the 30-day period.

This setting is applied for all teams within the organization.

Go to your **Company** settings > **Security** > **Sharing** and toggle on **Automatically deactivate Guests**.

:::tip
As soon as the setting is toggled on, the action is recorded in [Audit logs](../security-integrations/security-management/01-audit-logs.md) as **Enabled/disabled external users expiration setting**. Deactivation events will also be logged in [Audit logs](../security-integrations/security-management/01-audit-logs.md). The actor will be shown as **Miro Automation**.
:::
