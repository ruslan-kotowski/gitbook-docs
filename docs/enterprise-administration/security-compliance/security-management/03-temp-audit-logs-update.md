---
title: TEMP - Audit Logs Update
article_id: 11661793265938
sidebar_position: 3
created_at: '2023-05-25T14:03:15Z'
updated_at: '2024-08-23T12:39:53Z'
draft: true
availability:
  plans: '[Enterprise plan](../../../plans-billing/miro-plans/04-enterprise-plan.md)'
  roles: company_admin
---

Audit logs allow Company admins to track all the changes made to their Enterprise plan. Logs come in extremely useful when you need to troubleshoot a problem efficiently or to get a detailed report of important events (e.g. changes to the global security settings, invitations of new users, new boards created, etc.).

:::note
Currently, the events are logged from the moment of the Enterprise subscription creation and are stored endlessly:
a) if you upgrade to Enterprise from a different plan, the events will be logged from the moment of the upgrade,
b) if you migrate some teams to the Enterprise subscription, the data of those teams will be logged only from the moment when they become a part of the subscription.
:::

## Accessing audit logs and setting custom log periods

To access audit logs, do the following:

1. Go to **Company Settings**. You can get here by doing either of the following:
   1. On the board, click the **Settings** icon, and choose **Profile settings**. You may need to select your company from the pulldown menu in the top-left corner.
   2. From the dashboard, click your avatar in the top-right corner and choose **Settings**.
2. On the left-side panel, choose **Audit logs**.
3. Filter the logs by choosing one of the default time periods or set a **Custom time period**:![audit_logs.jpg](https://help.miro.com/hc/article_attachments/5117438525586/audit_logs.jpg)*Choosing the time period filter*

Click the **View events** button to see the event details. Time is displayed in **ISO 8601**format, **local time** zone.

![log_details.jpg](https://help.miro.com/hc/article_attachments/5117480346386/log_details.jpg)*Audit Log Details window*

You can export the logs to **CSV**format. Event date and time are provided in **ISO 8601**format, **UTC**time zone. The maximum number of records to be exported at a time is 100.000 events.
To export your logs, click the **Export to CSV**button.

## Deleting audit logs

Admins can set a period of time for audit logs to be deleted. You can choose between 30 or 90 days, six months, or one year. You can also set the logs to never be deleted.

:::warning
Once audit logs are deleted, they cannot be recovered.
:::

To set a deletion period, do the following:

1. Go into your Admin Settings
   1. On the board, click the **Settings** icon, and choose **Profile settings**.
   2. From the dashboard, click your avatar in the top-right corner and choose **Settings**.
2. Click **Audit logs** from the left-side panel.
3. Under Audit logs, click the **Settings** tab.
4. Choose an option from the drop-down list of choices. You will be asked to confirm your choice.
   ![audit_logs_deletion_period.png](https://help.miro.com/hc/article_attachments/11623525907602)*Deletion period options*
   ![audit_logs_deletion_period.png](https://help.miro.com/hc/article_attachments/11623525907602)*Confirmation of logs deletion*

## Events in Audit logs

The audit logs include records about the following categories of the events:

**Administration**

- Change Company name
- Change, remove Company logo
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
- Change app settings

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
- Upload a file, download a file, export a board - please note that tracking these events is enabled upon request; [reach out to Miro Support](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)

**Templates**

- Open a template
- Create, delete, restore a template
- Rename a template
- Change a Template owner

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

Please note, the audit log **does not** record information related to changes on boards.

### Frequently asked questions

Is there a way to automatically pull Audit Logs?

Yes, you can configure the [Miro app for Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md) to access Miro logs from Splunk.
