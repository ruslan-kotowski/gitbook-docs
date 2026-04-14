---
title: Request management on Enterprise Plan
article_id: 360017237379
sidebar_position: 9
created_at: '2020-10-27T12:09:40Z'
updated_at: '2026-02-19T11:00:31Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: access-request-management
availability:
  roles: company_admin
  notes: 'Relevant for: Enterprise Plan'
---

In Miro, requests for licenses, team and organization access, and Single sign-on (SSO) are sent to Company Admins via email by default. With advanced request management features, Company Admins can tailor how these requests are received and handled.

### Type of request

Request types fall into four categories:

- Requests to join your organization
- Requests to join a team
- Requests for a license
- Requests related to SSO issues

Learn about the different [request scenarios](#request-scenarios) for Enterprise Plan.

### Request management options

Company Admins have a variety of request management options, allowing them to customize processes according to the type of request:

:::note
The options to email all Company admins, or specific Company admins, include Team admins.
:::

- [Email all company admins](#email-all-company-admins)
- [Email specific company admins](#email-specific-company-admins)
- [Create a service desk ticket](#create-a-service-desk-ticket)
- [Redirect to a custom URL](#redirect-to-a-custom-url)

## Configuring request management

:::note
To [manage license requests directly in Miro](04-license-requests-on-enterprise-plan.md), select either **Email all company admins** or **Email specific admins**. You will receive all future license requests in your License request settings.
:::

### Email all company admins

All Company Admins will receive an email notification when a user makes an access request.

1. Under **Company** settings go to **Users** > **Access requests** > **Request management**.
2. Click on the **Type of request**you wish to manage.
3. A pop-up will open. Click the dropdown and select **Email all company admins**.

:::note
The options to email all Company admins, or specific Company admins, include Team admins.
:::

### Email specific company admins

Company Admins can specify up to 5 email addresses. Only the specified emails will receive the request. The emails do not need to belong to Miro users.

1. Go to **Company** settings > **Users** > **Access requests** > **Request management**.
2. Click on the **Type of request** you wish to manage.
3. A pop-up will open. Click the dropdown and select **Email specific company admins**.
4. Add up to 5 emails. Click **Add** each time you enter an email address in the email field.

:::note
The options to email all Company admins, or specific Company admins, include Team admins.
:::

### Create a service desk ticket

Automatically create a service desk ticket every time a user makes an access request. This feature is currently supported for **ServiceNow** and **Jira Service Management**.

ServiceNow Jira Service Management

1. Configure the email settings for ServiceNow. Create a catalog item for Miro in ServiceNow. Open ServiceNow, go to **System Properties** > **Email Properties** and enable receiving inbound emails

2. [Create an inbound email action](https://docs.servicenow.com/bundle/tokyo-servicenow-platform/page/administer/notification/task/t_CreatingAnInboundEmailAction.html). In the **From** field under the line **Only emails from this sender will trigger this inbound action**, type in [notification@miro.com](mailto:notification@miro.com).

3. [Set field values from the email body](https://docs.servicenow.com/bundle/rome-servicenow-platform/page/administer/notification/reference/r_SetFieldValsFromTheEmailBody.html) to configure additional settings and set up the process of converting a Miro email into a ServiceNow ticket. For example, you can assign a newly created ticket to a particular person.

4. Go to Miro, open **Company** settings > **Users** > **Access requests** > **Request management**, and select **Create a ticket in ServiceNow**.  In the email field, enter your ServiceNow email address.

1. Configure the email settings for Jira Service Management. From your service project, select **Project settings** > **Email requests**. [Choose your email service provider and follow the prompts to link Miro](https://support.atlassian.com/jira-service-management-cloud/docs/receive-requests-from-an-email-address/).

2. Go to Miro, open **Company** settings > **User management** > **Access requests** > **Request management**, and select **Create a ticket in Jira Service Management**. In the email field, enter your Jira Service Management email address.

### Redirect to a custom URL

The requester will be redirected to a URL of your choice for next steps.

1. Under **Company** settings go to **Users** > **Access requests** > **Request management**.
2. Click on the **Type of request**you wish to manage.
3. A pop-up will open. Click the dropdown and select **Redirect to a custom URL**.
4. Enter the redirect link in the **custom URL** field.

## Request scenarios

The below scenarios outline how different requests are triggered in Miro. Review the scenarios to decide how you would like to manage each request type.

|  |  |
| --- | --- |
| **Requests to join your organization** | - When a new user requests to join a team that is a company-managed subscription with [domain control](../canvas-25-admin-features/domain-control/01-domain-control.md) (unless domain control is set to capture new users). |
| **License requests** | - When a [Free Restricted user](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) requests a Standard or Full (legacy) license. - When a member requests a Standard or Full (legacy) license for a Free Restricted user, unless Members are allowed to invite new users to the subscription in the [invitation settings](03-invitation-settings-on-enterprise-plan.md). - When a Standard or Full (legacy) user requests an Advanced license. - When a member tries to invite or give edit access to a user with a Free Restricted license. |
| **Requests to join a team** | - When a non-admin user tries to share a board with a user that is *not* a member of the team, guest invites are turned off in the [invitation settings](03-invitation-settings-on-enterprise-plan.md), and only admins can invite new members to the team. - When a member who is not allowed to invite new members tries to grant an owner or [co-owner](../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) role on a particular board to a user who is not a member of the team. - When an Enterprise user requests to join a team [discoverable for users in their organization](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md#team-discovery). - When a [guest](../../using-miro/sharing-boards/07-collaboration-with-guests.md) invited to particular boards in a team requests to join the team |
| **Requests related to SSO issues** | - When a user has not been given access to Miro in IdP and has issues logging in via SSO. |

## Frequently asked questions

**Why am I still getting emails even though I’ve configured my settings to create tickets?**

If Team Admins are allowed to invite new users to a team in [invitation settings](03-invitation-settings-on-enterprise-plan.md), they will receive invitation requests related to this team via email, even though request management settings are set differently. Company Admins who are also a Team Admin will also still receive these emails.

**How do Team Admins know if there’s a request to join their team?**

If they are allowed to invite users to their teams, Team Admins will get an email about requests regardless of the request management settings.
