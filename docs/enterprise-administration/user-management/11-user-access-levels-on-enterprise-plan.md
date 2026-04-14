---
title: User access levels on Enterprise Plan
article_id: 360017571514
sidebar_position: 11
created_at: '2019-02-11T10:09:11Z'
updated_at: '2026-02-19T10:32:42Z'
draft: false
---

The level of access a user has on your Enterprise Plan depends on their license type and Miro role. Review our guide below to see what level of access your users have.

## User access on the Flexible Licensing Program (FLP)

Refer to the [license type](#license-types) and [Miro role](#miro-roles) in the table to understand your user access rights.

On Free licenses, users are automatically upgraded as soon as they edit or create a board, are invited to edit a board, are granted board co-ownership, or are added to a [project](../../using-miro/sharing-boards/16-projects.md) as Editor.

Learn more about the [Flexible Licensing Program](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) and [license management on the Flexible Licensing Program](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

|  |  |  |  |  |  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  | **Company Admin** | | | **Team Admin** | | | **Member** | | | **Guest** | |
| Advanced Standard Full (legacy) | Free | Free Restricted | Advanced Standard Full (legacy) | Free | Free Restricted | Advanced Standard Full (legacy) | Free | Free Restricted | Free | Free Restricted |
| Manage company-level settings | **✔** | **✔** | **✔** | **✘** | **✘** | **✘** | **✘** | **✘** | **✘** | **✘** | **✘** |
| Manage team-level settings | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✘** | **✘** | **✘** | **✘** | **✘** |
| Create boards & projects | **✔** | auto-upgrade | **✘** | **✔** | auto-upgrade | **✘** | **✔** | auto-upgrade | **✘** | **✘** | **✘** |
| Edit shared boards | **✔** | auto-upgrade | **✘** | **✔** | auto-upgrade | **✘** | **✔** | auto-upgrade | **✘** | **✔** *subscription-based | **✘** |
| View & comment on shared boards | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** |

* Editing access for Guests must be enabled on the Miro side, and enabled in your company settings by your Company Admin. Ask your Miro contact person for more details.

## User access on non-flexible licensing (non-FLP)

Refer to the [license type](#license-types) and [Miro role](#miro-roles) in the table to understand your user access rights.

|  |  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- |
|  | **Company Admin** | | **Team Admin** | | **Member** | | **Guest** |
| Advanced Standard Full (legacy) | Free Restricted | Advanced Standard Full (legacy) | Free Restricted | Advanced Standard Full (legacy) | Free Restricted | Free |
| Manage company-level settings | **✔** | **✔** | **✘** | **✘** | **✘** | **✘** | **✘** |
| Manage team-level settings | **✔** | **✔** | **✔** | **✔** | **✘** | **✘** | **✘** |
| Create boards & projects | **✔** | **✘** | **✔** | **✘** | **✔** | **✘** | **✘** |
| Edit shared boards | **✔** | **✘** | **✔** | **✘** | **✔** | **✘** | **✘** |
| View & comment on shared boards | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** | **✔** |

## License types

The [Flexible Licensing Program (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) includes the added benefit of unlimited **Free** licenses, as well as the ability to downgrade licenses to Free Restricted licenses at any time.

|  |  |  |
| --- | --- | --- |
| Full (legacy)/ Standard | **Free (FLP only)** | **Free Restricted** |
| User has full [view, comment and edit](../../using-miro/sharing-boards/01-board-access-rights.md#board-access-rights) rights as well as the ability to create boards | Users can [view and comment](../../using-miro/sharing-boards/01-board-access-rights.md#board-access-rights), and are automatically upgraded to a **Full (legacy)/Standard** license once they edit or create a board, are invited to edit a board, are granted board co-ownership, or are added to a [project](../../using-miro/sharing-boards/16-projects.md) as Editor | Users can [view and comment](../../using-miro/sharing-boards/01-board-access-rights.md#board-access-rights) only, but are part of the team and can view all shared boards. They can request a license upgrade |

:::note
Advanced licenses are not supported under the Flexible Licensing Program (FLP) and always operate on a non-FLP (hard limit) model. You can only assign up to the number of Advanced licenses your organization has purchased.

Organizations using FLP for Standard can continue to do so while keeping Advanced on a hard limit, allowing a mixed licensing model: Standard can remain on FLP (unlimited Free licenses with automatic downgrade to Free Restricted), while Advanced stays fixed to the purchased license quantity. Users who need Advanced features must be explicitly assigned an Advanced license or follow your organization’s upgrade or request flow.
:::

## Miro roles

Miro roles define a user's access level to your Enterprise Plan settings.

:::note
Company Admins and Team Admins are always Members and have the same permissions that Members have.
:::

|  |  |  |  |
| --- | --- | --- | --- |
| **Company Admins** | **Team Admins** | **Members** | **Guests** |
| **can** see all teams, and manage team and company settings | **can** see and manage the settings for a specific team | **can** [view, comment and edit boards](../../using-miro/sharing-boards/01-board-access-rights.md#board-access-rights)  **can’t** manage team or company settings | **can** [view, comment, and/or edit](../../using-miro/sharing-boards/01-board-access-rights.md#board-access-rights) shared boards (based on the [Licensing model](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md))  **can’t** create or own boards, see other teams and company details, manage team or company settings, or request a license |

## Frequently asked questions

**How do I downgrade a user's license?**

On Enterprise FLP subscriptions, Company Admins can downgrade a user’s license to Free Restricted in Company settings > **Users** > **All users** or **Teams**, select the team the user is part of, then find the user in the list.

**In order to be a member of two teams, do I need to have a license in each team?**

If the teams are a part of one Enterprise subscription, you need one license only. If the teams are associated with different subscriptions, you need a license in every team.

**What license type does an admin need?**

Admins on FLP plans can have a Full (legacy), Standard, Free or Free Restricted license. Admins on non-FLP plans can have a Free Restricted or Full (legacy)/Standard license.
