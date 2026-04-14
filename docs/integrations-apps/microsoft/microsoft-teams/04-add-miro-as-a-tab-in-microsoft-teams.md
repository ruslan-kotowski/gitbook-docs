---
title: Add Miro as a tab in Microsoft Teams
article_id: 4411292563602
sidebar_position: 4
created_at: '2021-12-01T04:50:21Z'
updated_at: '2025-11-25T16:07:47Z'
draft: false
availability:
  plans: free, starter, business, education, enterprise, and all Microsoft 365 plans
---

Users can add Miro boards to Microsoft Teams meetings, channels, and calendar events to seamlessly collaborate and share access with other team members.
In this article, you will learn how to use Miro within:

- Microsoft Teams meetings
- Microsoft Teams calendar events
- Microsoft Teams channels and chats

## Add Miro in Microsoft Teams meetings

- Users who join a meeting in MS Teams via mobile or tablet can only view an attached Miro board and cannot edit or comment on it.
- Any Microsoft Teams user who has authorized the Miro app can add Miro to the meeting. Any Teams user with a Miro profile can share a board to center stage.
- Microsoft does not support the ability for guest users to use apps in a Teams meeting, users must be logged into Teams in order to use any apps (including Miro).

1. Click on the dropdown **More actions.**
2. Select **+Add an app.**
3. Search for Miro and click on the Miro icon.
4. Here, you will be asked to sign up or sign in to your Miro profile.
5. Select which board you want to share or choose to create a new, blank Miro board.
6. Set permissions for the rest of the meeting participants and give or restrict access to the board. You can choose from these permission types:

- **Anyone can edit** (no sign-in to Miro required)
- **Anyone can comment** (no sign-in required, not supported for boards located in a Free team)
- **Anyone can view** (no sign-in required)
- **Private** (only those who have previously had access to the board can collaborate)

“**Anyone can edit, comment or view**” allows anyone in your Microsoft Teams tenant to access the board. This includes:

- Other Miro users from outside your organization
- Users who do not have a Miro profile
- Users in your organization that are not logged in to Miro

:::note
Sharing settings that are set for a board in Miro can also define the board access within Microsoft Teams. If the board is shared publicly in Miro, it will be available for anyone in Microsoft Teams even if you have pinned the board as [Private](../../../using-miro/sharing-boards/15-make-a-miro-board-private.md). However, if your board is private on the Miro side and you pinned it with Anyone can view/comment/edit access, board access on the Miro side will not be affected. [Learn more](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).
:::

:::note
For Enterprise Plan Miro users, your access settings will follow organization-wide access controls. Public link sharing for embeds needs to be enabled by admins in **Company settings** > **Security**. Learn more in [Managing Enterprise sharing policy for embed integrations](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

If you need to change access rights for an embedded board, remove the tab and re-add it with a different access level.

Now you can access the Miro board any time during the meeting in the specific tab. If you create multiple boards, there will be a single tab for each board.

If you click on Miro, you will see the Miro tab pop up on the right side with the board you have attached to this meeting.

You can select the **Share-to-Stage** button to send the board to all the participants and collaborate together at the same time. You can stop sharing the board any time by clicking the **Stop presenting** button at the top.

## Pin boards to Microsoft Teams calendar events

:::note
Outlook calendar is not yet supported.
:::

- Teams calendar events must be saved and have at least one attendee before a Miro board can be attached to the meeting.
- There is no way to remove a Miro board from a Teams meeting invite ([Microsoft reference article](https://support.microsoft.com/en-gb/office/remove-a-tab-in-microsoft-teams-c18c875c-0738-40ec-a228-61d7eb27f745#:~:text=In%20one%2Don%2Done%20and,the%20tab%20and%20select%20Remove.)). Users have to delete the invite and create a new one without a board.

1. First, schedule a new Microsoft Teams calendar meeting. Make sure to add a name for the meeting and invite attendees.
2. Click **Send** to share the invitation.
3. Once the meeting is saved, click on the meeting again and select **Edit**, so you can attach a Miro board.
4. You will be able to pin Miro as a tab using the plus sign at the top of the screen (**+**).
5. On the next screen, you will be prompted to add the Miro app. Either search for Miro in the search bar or select Miro if you already see it.
6. Select **Add** so you can add Miro.
7. You will be asked to sign in to your Miro profile inside Teams.
8. Once you sign in to Miro, you will be asked to select which board you want to add to the meeting. You can search and select an existing board or create a new blank board.
9. Here, you can also set permissions for the rest of the meeting participants and give or restrict access to the board. Then s**elect Save so you can attach the selected Miro board to the Teams meeting. Y**ou can choose from these permission types:

- **Anyone can edit** (no sign-in required)
- **Anyone can comment** (no sign-in required)
- **Anyone can view** (no sign-in required)
- **Private**

## Pin boards to Microsoft Teams channels and chats

> **Required role:** [Board owners](../../../using-miro/sharing-boards/01-board-access-rights.md#board-access-rights) and [board editors](../../../using-miro/sharing-boards/01-board-access-rights.md#board-access-rights) who are members of the team where the board is located

You can pin boards to Microsoft Teams channels by creating a new tab.

1. Click the plus icon (+).
2. A picker will open with various apps.
3. Find Miro in the list of apps and select it.
4. If you are not authorized in Miro in the same browser or within the desktop app, you will need to log in. Click **Get Started** and sign in or [register with Miro](../../../getting-started/start-here/02-how-to-register-with-miro.md).
5. Once authorized, you will see a picker with Miro boards - the picker will show those boards that you have access to on the Miro side. Please note that you can be authorized in Miro and in Microsoft Teams under different emails.
6. Сhoose a board that you would like to add to your Microsoft Teams channel. If you pick a board on which you don't have the needed level of access, you will see a warning message.
7. Set permissions for the rest of the meeting participants and give or restrict access to the board. You can choose from these permission types:

   - **Anyone can edit** (no sign-in required)
   - **Anyone can comment** (no sign-in required)
   - **Anyone can view** (no sign-in required)
   - **Private**
   > ✏️ Users of Microsoft Teams that use Miro on the Microsoft Teams mobile app can view and comment on boards depending on set permissions. For editing boards, we highly advise users to install our native [Mobile app](../../../getting-started/apps-for-devices/08-mobile-app.md) for which we have optimized the user interface.

   ## Frequently asked questions

Does each team member need to have a Miro profile to view embedded boards in Microsoft Teams?

If you choose **Anyone can view/comment/edit** when embedding the board, even non-registered users will be able to view/comment the board. Also, if the board is shared [publicly](../../../using-miro/sharing-boards/08-collaboration-with-visitors.md) on the Miro side, it will be available for anyone in Microsoft Teams.

Once a board is embedded, who has the ability to change the board’s access in MS Teams (e.g. from “Anyone can view” to “Private”)?

No one can change access to the attached board, not even the one who has attached it. However, anyone can click **Settings** on the tab, and then choose another (or the same) board for the same tab and select another access level for the chosen board.

I am registered with Miro under two emails and would like to embed a Miro board from my second Miro profile. How can I switch the Miro profile?

The picker shows boards of the user with which you're authorized in Miro in the same browser. Open Miro in another browser tab, sign out and log in to your second Miro profile.

If you use the Microsoft Teams desktop app, sign out of the app - this will also sign you out of Miro within the app. Then log in to the app and try to [embed a board](05-embed-miro-boards-in-microsoft-teams.md#embedding-boards-into-microsoft-teams-channels). You will be prompted to log in to Miro and will be able to sign in to another Miro profile.
