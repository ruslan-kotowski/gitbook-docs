---
title: Block deactivated users
article_id: 11846063620882
sidebar_position: 2
created_at: '2023-06-06T12:47:53Z'
updated_at: '2025-11-04T11:30:33Z'
draft: false
availability:
  plans: enterprise
  roles: company_admin
---

When a Company Admin [deactivates a user](01-deactivated-users.md), they lose access to the Enterprise subscription and can no longer log in with SSO. Deactivated users can continue to access other Miro subscriptions with the same email.

You can further block deactivated [managed users](06-managed-users-on-enterprise-plan.md) to prevent them from accessing any other Miro subscriptions.

## Blocking deactivated users

**When the setting is toggled on:** deactivated managed users will be blocked from accessing any Miro subscriptions. This setting applies to all users that are currently deactivated in your subscription and any users you deactivate in the future.

**When the setting is toggled off:** deactivated managed users can continue to access other Miro subscriptions with their corporate email and password.

:::tip
Enabling the **Block deactivated users** setting will impact all previously deactivated users in your subscription. Before you enable the setting, or verify new domains while the setting is enabled, we recommend first reviewing your deactivated users list to understand who will be blocked.
:::

### How to block deactivated users

1. Go to **Settings** > **Security** > **Managed domains**
2. Toggle on **Block deactivated users**
   *![Block deactivated users in the Enterprise admin console](images/23921780232082_image.png)*
   *Block deactivated users in the Enterprise admin console.*

## What do blocked users see?

Blocked deactivated managed users will be immediately logged out. When they try to log in the next time, they will see one of the following messages:

![Account](images/21017430794898_Account%20deactivated.png)*User attempted to log in with email and password*

![Email](images/21017417753746_Email%20not%20associated%20with%20an%20SSO%20account.png)*User attempted to log in with SSO*

## Unblocking deactivated users

Company Admins can unblock users in three ways:

**Reactivate or re-invite the user**

Reactivate or re-invite the user to your Enterprise subscription where the domain is verified. This user gains access to all subscriptions they are part of. If they are not actively using your Enterprise subscription, you can assign them a [Free Restricted](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) license. Learn more about inviting Members in [Manage invitations on Enterprise Plan](05-manage-user-invitations-on-enterprise-plan.md).

**Toggle off the Block deactivated users setting**

This will unblock all deactivated managed users, and they will be able to log into Miro with their corporate email. This will not give them access to your Enterprise subscription. This option only works if the user hasn’t been deleted from the subscription. Go to your **Managed domains** settings and toggle off **Block deactivated users.**

**Delete the domain**

You can delete the domain from your verified domains list. This will unblock all managed users from that domain unless they have been deleted from the subscription. To delete a domain, in your company settings go to **Security & compliance** > **Collaboration** > click **Remove** next to the domain name.

> **✏️** Blocking a user’s Miro access means they cannot log in to other Miro subscriptions with their corporate email and password, or via SSO. Unblocking doesn’t give the user access to the Enterprise subscription unless explicitly granted access.

## Blocked user scenarios

Use this table to understand more about what happens in different blocked user scenarios.

|  |  |
| --- | --- |
| **Action** | **Result** |
| **User is blocked** | |
| Company admin deactivates managed user | User is blocked |
| A Member of your Enterprise subscription tries to invite a **deactivated** managed user to their team | User remains blocked. Inviter will see a message that the user is deactivated. They cannot be invited. Admins can reactivate users. |
| Company admin deactivates and deletes a managed user | User is blocked |
| Managed user is deactivated in IdP | User is blocked |
| Managed user is removed from the Miro app/group in IdP | User is blocked |
| Company admin adds and verifies a domain while the setting is enabled | All users from the newly verified domains in the deactivated list are blocked. |
| Someone from another subscription (any other subscription apart from the one where the domain is verified) tries to invite your deactivated managed user to their subscription.   This also applies even if the managed user is deleted from your subscription. | The user remains blocked. They can be invited to other subscriptions and will receive invitation notifications but cannot log in to Miro. |
| **User is unblocked** | |
| Company admin reactivates a deactivated managed user | User is unblocked |
| Company admin invites a deactivated or deleted managed user back to the subscription. | User is invited and unblocked |
| Managed user is reactivated via SCIM | User is unblocked |
| Managed user is added back to the Miro app/group in IdP and synced via SCIM | User is unblocked |
| A Member of your Enterprise subscription invites a **deleted** managed user to their team | If the [invitation settings](03-invitation-settings-on-enterprise-plan.md) allow Members to invite new users to their teams, the user is invited and unblocked. |
| **Mixed scenarios** | |
| The verified domain is deleted from the Domain Control | Deactivated users from the deleted domain are unblocked. Deleted users remain blocked and need to be re-invited to the subscription to become unblocked. |
| The setting is disabled after it has been enabled. | All managed deactivated users are unblocked. Deleted users remain blocked and need to be re-invited to the subscription to become unblocked. |

## Frequently asked questions

**What can other subscriptions see about blocked deactivated users?**

Deactivating the user in your subscription will deactivate them only in your Enterprise subscription. Blocking will only impact the capability to log in to Miro using the corporate email. The user looks active in other subscriptions but they cannot log in with their corporate email address.

**If a user is deactivated and deleted, will they be blocked from accessing Miro once the setting is enabled?**

Users will remain blocked after you [delete them from your subscription](01-deactivated-users.md#permanently-delete-a-user). Deleting the user will have some implications - for more information review our [blocked and deactivated user scenarios](#blocked-user-scenarios). The only way to unblock a deleted user is to re-invite them to the subscription with the verified domain. If the user is deleted from the subscription prior to enabling the setting, it doesn’t apply to them.

**Does this setting impact unmanaged users?**

No. Only managed users are impacted by this setting.
