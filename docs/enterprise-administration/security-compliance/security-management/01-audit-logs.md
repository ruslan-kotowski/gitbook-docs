---
title: Audit logs
article_id: 360017571434
sidebar_position: 1
created_at: '2019-02-11T10:09:04Z'
updated_at: '2026-03-12T09:21:18Z'
draft: false
availability:
  plans: enterprise
  roles: company_admin
---

Audit logs allow organization admins with relevant privileges to track user activity in their Miro organization. Logs are extremely useful when investigating a problem or getting a detailed report of important events (for example, changes to the global security settings, invitations of new users, or new boards created).

:::note
Currently, the events are logged from the moment of the Enterprise subscription creation and are stored for 180 days by default:
a) If you upgrade to Enterprise from a different plan, the events will be logged from the moment of the upgrade.
b) If you migrate some teams to the Enterprise subscription, their data will be logged only when they become a part of the subscription.
:::

## Accessing audit logs

To access audit logs, do the following:

1. Go to **Company Settings**.
2. On the left panel, click **Security** > **Audit logs**.
3. You can filter the audit logs by choosing a **Date range**, an **Actor**, an **Event category**, and a specific **Event**.

Click the View events button to preview the events matching your filtering criteria. Time is displayed in **ISO 8601** format, in the **local** time zone. You can see details of a particular event by clicking on three dots in the **Details** column.

:::note
Only events that occurred during the last 90 days are available for preview.
:::

## Export audit logs

You can export logs in a **CSV** file format.

In the CSV Export file, the event date and time are provided in ISO 8601 format, UTC time zone. There is no limit on the number of records to be exported at a time; however, the more mode data you export, the longer it takes to prepare the file to download. Also, be mindful that popular applications for working with tables have their limits to the volume of data they can open.

To export logs, click the **Export to CSV** button.

The bar with your export file details will appear below. When the file is ready to download, you can click the Download CSV button. The file will be available for download for 24 hours.

:::note
Currently, only one export file is available for download per organization at a time. Clicking the **Export to CSV** button will replace the current export file.
:::

## Access audit logs via API

Admins can use the [Audit Log API](https://developers.miro.com/reference/audit-logs) or supported [SIEM Integrations](https://help.miro.com/hc/sections/4404757427090-Security-information-and-event-management-SIEM) to programmatically access and collect audit log data.

## Deleting audit logs

Admins can set a retention policy for audit logs. You can choose between 30, 90, 180, or 365 days.

:::warning
Once audit logs are deleted, they cannot be recovered.
:::

:::note
Indefinite retention for audit logs has been deprecated.
:::

To set a deletion period, do the following:

1. Go to **Company Settings**.
2. On the left panel, click **Security** > **Audit logs**.
3. Under **Audit logs**, click the **Settings** tab.
4. Choose an option from the drop-down list. You will be asked to confirm your choice.

## Events in Audit logs

The audit logs include records about the following categories of events:

**Administration**

- Change Company name
- Change, remove Company logo
- Created access request
- Declined access request
- Enable, disable user activity metrics in Analytics
- Enable, disable or change SSO/SAML settings
- Enable, disable SCIM
- Generate token for SCIM API
- Enable, disable SCIM notifications
- Enable, disable, change [allowlist](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Enable, disable sharing with guests outside of allowed domains
- Enable, disable sharing [via public link](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Enable, disable sharing [via public link for editing](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Enable, disable [team privacy](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Enable, disable, update [domain control](../../canvas-25-admin-features/domain-control/01-domain-control.md) settings
- Enable, disable [Block deactivated users](../../user-management/02-block-deactivated-users.md)
- Change [request management settings](../../user-management/09-request-management-on-enterprise-plan.md) (including changing ServiceNow email or service desk URL)
- Create, delete a team
- Change team name
- Change, remove team logo
- Change [team invitation settings](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Change [team discovery](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Enable, disable [guests for a team](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Change [default board sharing settings](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Change [default project sharing settings](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Install, uninstall an app
- [Approve, restrict an app](../../../integrations-apps/integrations-basics/04-how-to-install-apps.md)
- [Miro AI moderation](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md)

**User Management**

- Invite a new team member
- Convert a member to guest
- Convert a user to Full member
- Promote a user to Company admin, revoke Company admin
- Promote a user to Team admin, revoke Team admin
- Delete a user from a team or from a company (if a user leaves a team, they act both as an actor and an affected object)
- Revoke invitation
- Deactivate, reactivate a user
- User joins a team/Company

**Boards**

- Open a board
- Create, delete, restore a board
- Rename a board
- Change board description
- Change board cover
- Move a board to another team
- Add a board to a project, remove from a project, move to another project
- Change a Board owner
- Share a board with a Viewer/Commenter/Editor
- Remove a user from a board
- Enable, disable, change board [public link](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#sharing-boards-via-a-public-link)
- Enable, disable, change [password for a public board](../../../using-miro/sharing-boards/13-password-protection-for-public-boards.md)
- Enable, disable, change [sharing a board with Company](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#sharing-a-board-with-the-entire-company)
- Enable, disable, change [sharing a board with team](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Export a board,  download a file from a board.
- Status created
- Status updated
- Status deleted
- Upload a file (deprecated, available in [Content log](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md))

Please note, the audit log **does not** record information related to changes on boards.

**Templates**

- Open a template
- Create, delete, restore a template
- Rename a template
- Change a Template owner
- Status created
- Status updated
- Status deleted

**Projects**

- Create, delete a project
- Rename a project
- Share a project with a user, remove a project participant
- Enable, disable team sharing for a project
- Change a Project owner

**Logins**

- Sign in
- Failed to sign in
- Sign out
- Profile locked, unlocked

:::warning
Login events will include the activity of [Deactivated users](../../user-management/01-deactivated-users.md).
:::

**Profile details**

- Change profile details
- Request an email address change
- Change email address

**Blueprints**

- Create a Blueprint
- Delete a Blueprint
- Create a Blueprint section
- Delete a Blueprint section
- Change Blueprint owner

**Miro AI**

- Use Miro AI feature

### Frequently asked questions

Is there a way to automatically pull Audit Logs?

Yes, you can configure the [Miro app for Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md) to access Miro logs from Splunk.
