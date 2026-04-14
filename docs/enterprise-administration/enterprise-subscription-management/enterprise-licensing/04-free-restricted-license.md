---
title: Free Restricted license
article_id: 360011746739
sidebar_position: 4
created_at: '2020-02-05T07:29:16Z'
updated_at: '2026-02-19T10:40:27Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  plans: enterprise
---

When new users join a Miro subscription, depending on the [Enterprise licensing model](02-enterprise-licensing.md) they can be assigned a Free Restricted license.

## When are users assigned a Free Restricted license

**On the Flexible Licensing Program (FLP)**, a user can be assigned the Free Restricted license when:

- The default license for new users is set to Free Restricted
- A Company Admin invites the user and selects the Free Restricted license for them in the invitation window
- A Company Admin converts the user to Free Restricted in **Company settings > Active users**

:::note
Learn more about the [Flexible Licensing Program (FLP)](03-flexible-licensing-program-flp.md) and [managing licensing on FLP](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

**On non-flexible licensing (non-FLP)**, a user can be assigned the Free Restricted license when:

- The user is being auto-captured (by [Domain control](../../canvas-25-admin-features/domain-control/01-domain-control.md) or [Just-in-Time provisioning](../../user-management/13-user-provisioning-on-enterprise-plan.md)) in an organization that has insufficient Advanced, Standard, or Full (legacy) licenses during their registration in Miro.
- The user is invited to a team in the organization that has insufficient Advanced, Standard, or Full (legacy) licenses.

When multiple users are invited at the same time, they receive licenses by order of their email addresses in the list of invitees. If the organization has insufficient licenses, users at the end of the list will receive a Free Restricted license. In this case, the inviter would receive a pop-up notification about limited access for some users.

## How Free Restricted licenses work for users

Free Restricted users can view and comment on boards in the teams they participate in, and can request edit access and Standard license or a Full (legacy) license from Company Admins. They can also discover and join teams in the organization along with other members.

:::note
Company Admins can [configure request management settings](../../user-management/09-request-management-on-enterprise-plan.md).
:::

### Free Restricted board access

The following view, comment or edit access permissions apply to users with a Free Restricted license:

|  |  |
| --- | --- |
| **How the board was shared** | **Access level** |
| Public link | Free Restricted users can view and/or edit  depending on the access level granted. |
| Team or Company link | Free Restricted users can view and/or comment depending on the access level granted. |
| [Embedded link](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md) | Free Restricted users can view and/or comment depending on the access level  granted.   Free Restricted users will not be able to edit or request editing access, even if edit access is granted via the embed permissions. |

## How to manage Free Restricted licenses

> **Who can do it:** Company Admins

On all subscriptions, the Company Admin can upgrade a user license from Free Restricted to a Standard or Full (legacy) license in the **Active users** section of their Team or Company settings.

**Flexible Licensing Program (FLP)**

On FLP subscriptions, the Company Admin can also downgrade an Advanced, Standard, or Full (legacy) license to a Free Restricted license at any time.

When a user with a Free Restricted license is requesting editing access, Company Admins receive the request based on their [request management settings](../../user-management/09-request-management-on-enterprise-plan.md).

:::note
Learn more about [license management on the Flexible Licensing Program](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

## Frequently asked questions

**What happens to my Free Restricted licenses when I add more Standard or Full (legacy) licenses to my non-FLP plan?**

Your existing Free Restricted users are not automatically upgraded to the new Standard or Full (legacy) licenses. Company Admins can upgrade licenses manually.
