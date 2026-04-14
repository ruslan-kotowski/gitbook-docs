---
title: Deactivated users
article_id: 360025025894
sidebar_position: 1
created_at: '2019-06-19T22:16:18Z'
updated_at: '2026-02-19T10:44:30Z'
draft: false
availability:
  plans: '[Enterprise plan](../../plans-billing/miro-plans/04-enterprise-plan.md)'
  roles: company_admin
---

The advanced user management in Miro allows Company Admins to deactivate users instead of deleting them. Deactivated users stay in the plan directory and can be reactivated at any time.

## Rules

- Deactivated users will not be able to access your Enterprise account and its features.
- If you have enabled the [Block deactivated users](02-block-deactivated-users.md) setting, deactivating a managed user will block them from logging in to Miro.
- Deactivated users will not be able to use your company's SSO option to log in anymore, switching back to standard authentication methods.
- Shared boards and Spaces created by deactivated users are *not* reassigned to anyone else and are still available to collaborators (unless during deactivation, you also remove the user from their team. In this case, the boards are reassigned to a team admin. This is usually relevant for [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) operations).
- All [notifications](../../using-miro/managing-your-profile/02-miro-notifications.md) to deactivated users are blocked.
- Other users cannot share boards and Spaces with deactivated users.
- Deactivated users cannot be added to teams within your Enterprise subscription. Company Admins can reactivate deactivated users upon inviting them as members, [learn more](05-manage-user-invitations-on-enterprise-plan.md).
- Deactivated users are not billed. Their licenses are released and can be applied to another active user.
- The following attributes are not allowed to be updated for Deactivated users:

|  |
| --- |
| `userName` |
| `userType` |
| `roles.value` |

## Deactivate a user

You can deactivate a user at any time. When you deactivate a user, they're moved from an **Active** to a **Deactivated** state and stop consuming a license. This change is also reflected in the Active and Deactivated user lists in the **Users** settings.

To deactivate a user:

1. Open your **Company** settings.
2. Select **All Users** under the **Users** menu**.**
3. Click the **three dots** (**...**) icon to the right of a user you would like to deactivate.
4. Click on **Deactivate**.
   ![deactivate-users.png](images/23921781594002_deactivate-users.png)
   *The option to deactivate a user on Enterprise plan*

   You can also deactivate users in bulk. Select several users by checking the boxes on the left or apply filters and select up to 50 filtered users at once then choose **Deactivate** under **Bulk actions.**
5. Check **Reassign user's content** box if you would like to transfer the user's boards, [templates](../../getting-started/start-here/your-first-board/02-custom-templates.md), and [Spaces](../../using-miro/spaces/01-spaces.md). A new owner must be chosen for each team in which the selected user(s) had content. Reassigning users' content cannot be undone.
   ![deactivate-reassign-content.png](images/23921804187154_deactivate-reassign-content.png)
   *The option to reassign user's content when deactivating them*
6. Select **Deactivate.**

Deactivating users won’t remove their data in Miro. Permissions they have will be retained and will be restored once the users are re-activated.

:::note
Note: to deactivate a Company Admin you need to revoke Company Admin permissions first.
:::

:::note
If you see a notification **The team must have at least one Admin** when trying to deactivate a user, it means that the user is the *only* Admin in an Enterprise team or teams. To fix this, [invite yourself to these teams](05-manage-user-invitations-on-enterprise-plan.md) and [grant Team Admin rights to yourself](../../administration/user-management/06-how-to-manage-admin-roles.md). Сlick on the number of teams of the respective user to learn which teams they are a member of.
:::

:::note
If your company uses [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) solution, you can also deactivate users via your Identity Provider. When a user is deactivated by SCIM, their content is not reassigned - the reassignment option is supported only in the UI for this scenario.
:::

### Automatic deactivation for Guests

For Guests (users originally invited to your boards via an email) you can enable [automatic deactivation](03-invitation-settings-on-enterprise-plan.md).

## Reactivate a user

To reactivate a user:

1. Open your **Company** settings.
2. Select **All Users** under the Users menu item and then the **Deactivated users** tab**.**
3. Click the **three dots** (...) icon to the right of a user you would like to reactivate.
4. Select **Reactivate**.
5. Add the user to teams if necessary.
6. Confirm **Reactivate**.

![reactivate-users.png](images/23921804191762_reactivate-users.png)
*Reactivating a user*

When you reactivate a user:

- Users can sign in right away
- They will have access to shared boards, team boards, and boards they created prior to their deactivation (unless the boards were reassigned)

:::note
Note: only Company Admins can re-activate deactivated users.
:::

### Permanently delete a user

To permanently delete a deactivated user:

1. Open your **Company** settings.
2. Click on **Users** > **All users** from the menu.
3. Select the**Deactivated users** tab.
4. Click the **three dots** (**...**) icon to the right of a user you would like to delete.
5. Select **Delete**.
   ![delete-users.png](images/23921781612562_delete-users.png)
   *Deleting a deactivated user*
6. Choose whether to reassign the user's content or remove it — either choose the new owner and click **Delete user** or select **Delete user and content**.

You can also delete users using bulk actions:

1. From the Deactivated users tab, click the check box next to the users you want to delete.
2. Click on the **Delete from Company** button at the top.

:::note
Note: after deletion, users can be invited back to your plan as members or onto a board as guests by anyone having permission to [add new users](05-manage-user-invitations-on-enterprise-plan.md).
:::
