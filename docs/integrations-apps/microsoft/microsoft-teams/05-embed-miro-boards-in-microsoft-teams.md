---
title: Embed Miro boards in Microsoft Teams
article_id: 360017572514
sidebar_position: 5
created_at: '2019-02-11T10:13:30Z'
updated_at: '2025-04-24T13:52:02Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ms-teams
availability:
  plans: all Miro plans
---

Embed Miro boards into Microsoft Teams channels and seamlessly share them with team members. Keep your Miro boards at hand and rest assured that your entire team is on the same page.

:::note
Check how you can embed Miro boards into Microsoft Teams Meetings: [Miro for Microsoft Teams Meetings (Admin guide)](01-miro-for-microsoft-teams-admin-guide.md), [Miro for Microsoft Teams Meetings (User guide)](02-miro-for-microsoft-teams-user-guide.md).
:::

### Installing the plugin

First, you need to find **Miro** in **Microsoft Teams Store** or just follow the [direct link](https://teams.microsoft.com/l/app/8216e453-3db5-48ee-a3d6-5122f505c8a3).

:::warning
Please note that your tenant admin on the Microsoft Teams side should enable the Miro app within your 3rd party apps catalogue for Teams. Unless Miro is approved, it won't be listed among the apps in Microsoft Teams Store.
:::

Click **Add** to install the plugin.

![Miro_plugin_installation.jpg](images/21019790725266_Miro%20plugin%20installation.jpg)
*Miro plugin installation*

Once having installed the Miro plugin, you'll be redirected to the chat where you will be able to configure getting Miro notifications. To learn more, please check out [this article](10-miro-notifications-in-microsoft-teams.md).

However, at that moment, you can already start embedding Miro boards into a Microsoft Teams channel without any additional configuration.

### Embedding boards into Microsoft Teams channels

> **Set up by:** [board owners](../../../using-miro/sharing-boards/01-board-access-rights.md#board-access-rights) and [board editors](../../../using-miro/sharing-boards/01-board-access-rights.md) who are members of the team where the board is located

You can embed your boards into Microsoft Teams channels by creating a new tab. Click the plus icon. You will get a picker with various apps. Find Miro in the list of apps and select it. If you are not authorized in Miro in the same browser or within the desktop app, you will need to log in. Click **Get Started** and sign in or [register with Miro](../../../getting-started/start-here/02-how-to-register-with-miro.md).

![embed_in_MS_teams.gif](images/21019734975122_embed%20in%20MS%20teams.gif)
*The modal that prompts you to authorize your Miro profile*

Once authorized, you will see a picker with Miro boards - the picker will show those boards that you have access to on the Miro side. Please note that you can be authorized in Miro and in Microsoft Teams under different emails.

Сhoose a board that you would like to add to your Microsoft Teams channel.

![MS_teams_embed_picker.jpg](images/21019734978322_MS%20teams%20embed%20picker.jpg)
*The picker with Miro boards*

Note that only board owners and board editors who are team members can embed Miro boards. If you pick a board on which you don't have the needed level of access, you will see a warning message.

![unable_to_embed_boards.jpg](images/21019790732690_unable%20to%20embed%20boards.jpg)
*The warning message that your access level does not allow you to embed a board*

Next, you can set permissions for the rest of the meeting participants and give or restrict access to the board. You can choose from these permission types:

- **Anyone can edit** (no sign-in required)
- **Anyone can comment** (no sign-in required)
- **Anyone can view** (no sign-in required)
- **Private**

![sharing_level.jpg](images/21019790733586_sharing%20level.jpg)
*Access settings for an embedded board*

:::note
Note that the sharing settings that are set for a board in Miro can also define the board access within Microsoft Teams. If the board is shared publicly in Miro, it will be available for anyone in Microsoft Teams even if you have embedded the board as **Private**. However, if your board is [private](../../../using-miro/sharing-boards/15-make-a-miro-board-private.md) on the Miro side and you embed it with **Anyone can view/comment/edit** access, board access in Miro will not be affected. [Learn more](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).
:::

:::note
For [Enterprise plan](../../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md) Miro users, your access settings will follow organization-wide access controls which might imply that some sharing options may be restricted. Learn more: [Managing Enterprise sharing policy for embed integrations](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

:::warning
**Anyone can comment** option is not supported if you embed a board located in a [free team](../../../plans-billing/miro-plans/09-free-plan.md).
:::

Once the board is embedded, you can start interacting with it right away.

![Miro_embed_in_MS_teams.jpg](images/21019734972562_Miro%20embed%20in%20MS%20teams.jpg)
*Board embedded into a Microsoft Teams channel*

:::note
Users of Microsoft Teams that use Miro on the Microsoft Teams mobile app can *view and comment* on boards depending on set permissions. For editing boards, we highly advise users to install our native [Mobile app](../../../getting-started/apps-for-devices/08-mobile-app.md) for which we have optimized the user interface.
:::

![Miro_in_MS_Team_on_mobile.jpg](images/21019734976146_Miro%20in%20MS%20Team%20on%20mobile.jpg)
*Miro board in MS Teams on mobile - press **Open in the app** to install Miro native mobile app*

### Frequently asked questions

1. *Does each team member need to have a Miro profile to view embedded boards in Microsoft Teams?*
   - If you choose **Anyone can view/comment/edit** when embedding the board, even non-registered users will be able to view/comment the board. Also, if the board is [shared publicly](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#sharing-boards-via-a-public-link) on the Miro side, it will be available for anyone in Microsoft Teams.
2. **Once a board is embedded, who has the ability to change the board’s access in MS Teams (e.g. from “Anyone can view” to “Private”)?**
   - No one can change access to the attached board, not even the one who has attached it. However, anyone can click **Settings** on the tab, and then choose another (or the same) board for the same tab and select another access level for the chosen board.
3. **I am registered with Miro under two emails and would like to embed a Miro board from my second Miro profile. How can I switch the Miro profile?**
   - The picker shows boards of the user with which you're authorized in Miro in the same browser. Open Miro in another browser tab, sign out and log in to your second Miro profile.
   If you use the Microsoft Teams desktop app, sign out of the app -  this will also sign you out of Miro within the app. Then log in to the app and try to [embed a board](#embedding-boards-into-microsoft-teams-channels). You will be prompted to log in to Miro and will be able to sign in to another Miro profile.
