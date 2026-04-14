---
title: License requests on Enterprise Plan
article_id: 17693037972370
sidebar_position: 4
created_at: '2024-03-15T08:43:14Z'
updated_at: '2026-02-19T10:46:59Z'
draft: false
availability:
  plans: enterprise
  roles: Company Admin or User Admin
---

Manage all license requests from a single location. By receiving license requests directly in Miro, you can simplify license usage and approval processes within your organization.

## License requests settings

Within your **Access requests** settings, you'll find an overview of all current **License requests**. These license requests are initiated when a user requires an upgrade from a Free Restricted to an Advanced, Standard, or Full (legacy) license.

License request details include:

- The name of the user the license request is for
- The name of the billing group (if any) the user will be assigned to
- The name of the requester
- The date of the request

Requests can be submitted either by the individual in need of the license upgrade or on behalf of someone else. Learn about the different [license upgrade scenarios](#license-upgrade-scenarios) for Enterprise Plan.

:::note
To receive license requests directly in Miro, update your [Request management](09-request-management-on-enterprise-plan.md) preferences.
:::

## How to accept or deny license requests

:::note
All requests will automatically expire and be removed after 30 days.
:::

1. Go to your Miro settings.
2. Click **Company**.
3. Under **Users**, click **Access requests**.
4. Select the **License requests** tab. Here you can view all pending license requests.
5. Under the **Actions** column, click the checkmark (**✓**) to accept, or the cross (**x)** to decline the request.
6. (optional) To bulk accept license requests, next to the **Name** column, click the checkbox to select all requests, and click **Bulk approval**.
7. When you accept or decline requests, a modal will open with the requester details along with who the license request is for.
8. Click **Approve** to approve the request, or **Deny** to decline the request. When you accept or deny a request, it will be removed from your license request overview.
9. Once the license request is approved, the user will be upgraded from a Free Restricted to an Advanced, Standard, or Full (legacy) license.

## License upgrade scenarios

Certain actions or events in Miro prompt users to submit license upgrade requests. The scenarios outlined below describe how these requests are initiated for Enterprise Plan users. Upon approval, the user's license will be upgraded from a Free Restricted to an Advanced, Standard, or Full (legacy) license. Users will retain their membership in the same teams they were previously a part of.

:::note
To view your current license usage, go to **User management** > **Active users**.
:::

|  |  |  |
| --- | --- | --- |
| **User type** | **Action** | **Scenario** |
| **Existing Members (Free Restricted license)** | Create a board or project | Free Restricted user tries to create a new board or project within a team |
| Edit access | Free Restricted user requests edit access to a board |
| Invited to edit | An existing Member requests edit access for the Free Restricted user |
| Board owner | Free Restricted user is assigned the [board owner](../../getting-started/start-here/05-roles-in-miro.md#roles-on-boards) role by a Team Admin |
