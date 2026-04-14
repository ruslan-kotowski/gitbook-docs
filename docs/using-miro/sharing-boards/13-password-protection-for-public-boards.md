---
title: Password protection for public boards
article_id: 360014617239
sidebar_position: 13
created_at: '2020-06-22T10:42:25Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
availability:
  roles: board_owner, [board co-owners](06-co-owners-of-boards-and-spaces.md), and
    Company Admins on Enterprise plans with [Content Admin](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)
    permissions
  plans: browser, [Desktop app](../../getting-started/apps-for-devices/05-desktop-app.md),
    [Tablet app](../../getting-started/apps-for-devices/11-tablet-app.md)
  notes: 'Relevant for: Starter, Business, Enterprise and Education plans'
---

Read about our password protection feature for paid plans, and learn how to set a password for your public boards.

## Passwords for public boards

Inviting visitors to your board using a public link is a great option for instant, one-time or short term collaboration with users outside of your team or company - even non-Miro users can access public boards.

When sharing public Miro boards you can add an extra layer of security by setting a password.

### Password protection based on your plan

Password protection and the level of permissions depend on your plan type.

|  |  |  |  |
| --- | --- | --- | --- |
|  | **Free** | **Starter, Business** | **Enterprise** |
| **Enable, change or remove  passwords** | ✘ | ✔  Board owners, co-owners | ✔  Board owners, co-owners, company admins* |
| **Enable mandatory passwords** | ✘ | ✘ | ✔  [Set a mandatory password](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md#require-passwords-for-public-boards-company-level) |
| **Require complex passwords** | ✘ | ✘ | ✔  [Require a complex password](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md#require-passwords-for-public-boards-company-level) |

*[Content Admin](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md) permissions must be enabled.

:::note
Learn more about our [sharing policy on Enterprise plan](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).
:::

## How to add password protection to a board

1. When you enable access for **Anyone with a link**, click on the **Set password** button.

2. Enter a strong alphanumeric password of at least 8 characters, and then click **Set**.

3. The password will be copied to your clipboard.

![3-1-720p-10fps-s4-r20.gif](images/20257248240274_3-1-720p-10fps-s4-r20.gif)
*Setting a password on a board shared by link*

:::note
Enterprise plan Admins can [set mandatory passwords for all boards within the subscription](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md#require-passwords-for-public-boards-company-level).
:::

## How password protection works for users

After receiving and opening the board link, visitors are prompted to enter the password.

![3-2-720p-10fps-s4-r20.gif](images/20257248243730_3-2-720p-10fps-s4-r20.gif)

Once they enter the password they’ll have full access to your board. They’ll only need to reenter the password every 72 hours.

If users have to log in more frequently, it’s possible the company Miro admin has enabled [Idle Session Timeout](../tools/troubleshooting/19-why-does-miro-keep-logging-me-out.md) for added security.

Please note that if a board is password-protected, it will only be shown in the Starred and Recent lists as long as they are visible to the user.

Once the session expires for the user, the boards become unavailable for them and are removed from the Starred and Recent lists. If the user opens the board via a direct link and re-enters the board password, the board will be shown in relevant lists again.

## Change the password for a public board

Changing the password will immediately revoke access for all board visitors, even if they’re currently on the board.

:::note
Users who can share a link to a password-protected board are not able to change the password unless they’re a board owner or co-owner.
:::

**To change the password for a public board:**

1. Click **Edit password** in the sharing settings, and then click **Change password**.
![3-1.png](images/20235526720658_3-1.png)
*Editing a board password in the share settings*
2. A confirmation window appears and informs you that you'll need to share the new password with existing collaborators for them to continue accessing the board. Click **Change password**.

![change_password.png](images/20022115780754_change_password.png)
*Change password confirmation window*
3. Enter a strong alphanumeric password of at least 8 characters.
Your admin may have set specific password requirements for your account. As you create your password, the required criteria will be clearly displayed to guide you.
![Password requirements are shown as you enter your password.](images/23762870609298_image.png)*Password requirements are shown as you enter your password.*

4. Click **Set password**.

:::note
Changing the password will immediately revoke access for all board visitors, even if they’re currently on the board.
:::

## Disabling a public link

You can [stop sharing a public board](03-sharing-boards-and-inviting-collaborators.md#stop-sharing-a-board) at any time, however it doesn't automatically reset the password for your board. To enable visitors to access the board with the same password, you must share the board by link again.

To learn about changing the password, see [Change the password for a public board](#change-the-password-for-a-public-board).

## I forgot the password for my board

If you forget the password you can easily [change your board password](#change-the-password-for-a-public-board) in the share settings.

:::note
Setting up password protection for boards for mobile is in our backlog.
:::
