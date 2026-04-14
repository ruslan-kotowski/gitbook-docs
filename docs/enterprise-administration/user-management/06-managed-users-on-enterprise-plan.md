---
title: Managed users on Enterprise Plan
article_id: 6882052393618
sidebar_position: 6
created_at: '2022-07-29T11:04:13Z'
updated_at: '2026-02-26T14:01:27Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-management
---

For an Enterprise subscription, a managed user is any user inside one of your verified domains.

To learn more about the domain verification process, visit the article about [Domain control](../canvas-25-admin-features/domain-control/01-domain-control.md).

Note that there are different ways you can provision your corporate users into the Enterprise organization, including Domain Control, SCIM, JIT, and a manual invitation via email. [Learn more](13-user-provisioning-on-enterprise-plan.md).

Managed users can be supervised by Enterprise Company Admins, and the organization can establish policies and controls around how and what they can access in Miro, along with overall ownership over the user - e.g., assigning them to teams, managing their content, analyzing their activities, and deleting the user.

:::note
User details include an **Internal** or **External** classification. Internal users sign in with an email address from a verified domain. External users do not. For more information, see [Domain Control: Internal and external users](../canvas-25-admin-features/domain-control/01-domain-control.md#internal-and-external-users).
:::

Miro provides the following user management opportunities:

- Domain control features:
  - Gain insights on users who belong to your corporate domains but are not yet captured into the Enterprise organization
  - Auto-capture users from your domain to your Enterprise subscription
  - Restrict Managed users from creating new Miro subscriptions outside the Enterprise organization
- License management
  - Define whether a user should have [Advanced, Standard, Full (legacy), or restricted access to the plan](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) and change licenses of managed users
- User access
  - [Deactivate](01-deactivated-users.md) and [delete](10-remove-users-on-enterprise-plan.md) users from the Enterprise organization
  - Manage user access to teams within the organization
  - [Block all Miro access](02-block-deactivated-users.md) for deactivated managed users
- Reporting
  - Filter Managed users who are part of your Enterprise plan in Admin settings and download the list of users as a CSV file
