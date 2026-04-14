---
title: User permissions for boards embedded in third-party apps
article_id: 4411883577618
sidebar_position: 1
created_at: '2021-12-08T10:13:42Z'
updated_at: '2025-11-25T16:07:55Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  roles: board_owner, Board co-owners
  plans: free, starter, business, enterprise, education
  platforms: browser, desktop
---

Miro offers several integrations that enable you to easily collaborate with boards in third-party environments, such as [Microsoft Teams](../microsoft), [Confluence](../atlassian/01-miro-for-confluence.md), Notion, and Google Meet. You can discover other supported apps in the [Miro Marketplace](https://miro.com/marketplace/category/embed-miro/). When embedding boards, you can set different levels of user access and manage these permissions from within Miro.

## Understand embed access

When sharing a board in an external app, you can provide view, comment, or edit access specifically to users within that app for one-time collaboration, regardless of their Miro access. These users won’t need a Miro profile to access the board within the app. This allows you to set specific board access rights for users of the app who are not registered with Miro without making the board publicly available.

For maximum security, we advise against using this method outside of one-time collaboration (such as a workshop) and recommend that your organization allocates Miro access appropriately to those who require it.

![embed_Miro_in_Zoom.gif](images/21020254296722_embed%20Miro%20in%20Zoom.gif) *Setting up access rights for a board embed*

The board becomes accessible only within the app where it was embedded. The level of access that you set for a board embed within the app does not affect the sharing settings of the board outside the app. For example, if a [private board](../../using-miro/sharing-boards/15-make-a-miro-board-private.md) is embedded into a Microsoft Teams channel with "Anyone can view" access, users in that Microsoft Teams channel can view the board without a Miro sign-in. If the same users try to access the board outside the Microsoft Teams channel by following the board link, they will not have access.

However, board sharing settings on the Miro side take precedence over the access level set in the external app. For example, if a board is [shared publicly on the Miro side](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#sharing-boards-via-a-public-link), it will be available for anyone in Microsoft Teams even if you have embedded the board as Private.

## Manage and revoke embed access

You can easily track, manage, and revoke access to boards embedded in supported external apps.

To manage and revoke access for embedded boards:

1. Click the **Share** button to open the sharing settings of a Miro board.
2. Select **Sharing settings**.
3. Open the **Embeds** tab.
4. You will see the external applications where the board is embedded, including the integration name, when and by whom it was embedded, and the board access settings within the app.
5. To revoke access to the board within an app, click **Revoke access** next to the app. Note that this action is irreversible.

ol

![remove_an_access_link.gif](images/21020265344914_remove%20an%20access%20link.gif)
*Removing an access link*

After embed access is revoked, board access will be limited in the app. Note that the board may still be accessible within the app if it is shared on the Miro side. For example:

- If anyone could **edit** the board within the application and the same board is [publicly shared](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#sharing-boards-via-a-public-link) for **viewing** on the Miro side, then anyone will still be able to **view** the board within the app.
- If the board is private and only shared [with other users via email](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#inviting-via-email), the embedded board will require **sign-in** to access it within the app.

## Embedding rules and limitations

Please note the following rules and limitations when embedding boards:

- You cannot embed a board if it's [inactive](../../using-miro/tools/troubleshooting/15-the-board-is-locked.md) or you have view-only access on the board.
- Boards stored in [free teams](../../plans-billing/miro-plans/09-free-plan.md) cannot be embedded with comment access.
- For [Enterprise plan](../../plans-billing/miro-plans/04-enterprise-plan.md) users, your access settings will follow organization-wide access controls which might imply that some sharing options may be restricted. Learn more: [Managing Enterprise sharing policy for embed integrations](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- For some old links, you will only see the level of access and application, but not who created the board or when it was embedded.
- If you want to limit the ability to embed Miro boards inside external apps for your Enterprise organization, please refer to [Managing Enterprise sharing policy for embed integrations](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- Managing embedded board access links is not yet supported on mobile and tablet devices.

Learn more about [embedded board access for users on Free Restricted licenses](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md#free-restricted-board-access).
