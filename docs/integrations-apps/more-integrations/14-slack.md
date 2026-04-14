---
title: Slack
article_id: 360017572494
sidebar_position: 15
created_at: '2019-02-11T10:13:25Z'
updated_at: '2025-02-26T12:10:38Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
---

Get Slack notifications of new comments and mentions on your boards and other changes related to your profile, easily share your Miro boards from within Slack, and automatically unfurl board links. Read the article to learn how to connect your Slack to Miro and get access to all the nice features.

:::note
Some Slack users are suggested to seamlessly register with Miro via Slack when clicking a link to a Miro board posted in a Slack channel. The feature is currently in beta and managed by Slack. It does not require our application to be installed in the Slack workspace.
Workspace administrators have the option to completely disable the Sign in with Slack feature in the Slack workspace settings (App Management Settings > Sign in with Slack Settings). Enterprise Grid Org and their workspaces are excluded from the launch during beta.
:::

:::note
For support with the Slack app, email [slack_integration_support@miro.com](mailto:slack_integration_support@miro.com) or visit [How to contact Miro support](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).
:::

## Enabling the app

Slack App integration is set up by a user for their own profile. To enable the integration, open your Miro [Profile settings](../../using-miro/managing-your-profile/01-profile-settings.md).

![getting_to_profile_settings.jpg](images/21017652360210_getting%20to%20profile%20settings.jpg)
*Getting to Profile settings from Miro [dashboard](https://miro.com/app/dashboard/)*

Switch to the **Integrations** tab, find **Miro Feed (Slack App)** and click **Connect**:

![connect_Slack.jpg](images/21017652361234_connect%20Slack.jpg)
*Connecting Slack App*

Another option is to enable it right in the [Notifications tab](https://miro.com/app/account/profile/notifications/):

![connect_Slack_from_notifications.jpg](images/21017648436626_connect%20Slack%20from%20notifications.jpg)
*Enabling Slack App on the notification page*

You will be redirected to authorize in Slack. Please enter your credentials and sign in to Slack.

![authorize_Slack.jpg](images/21017648438546_authorize%20Slack.jpg)
*Allowing Miro access to the workspace*

## Configuring notifications

Customize the feed that you receive by choosing the events you'd like to be notified about.

You can keep track of the following events:

- invitees sign up
- someone requests access to a team or a board
- you are invited to a project
- a board is shared with you
- there's a new comment on your board or a reply to your comment on a board
- someone @mentions you in a comment or reply

Open the [Notifications page](https://miro.com/app/account/profile/notifications/) and set up your preferences:

![notification_settings.jpg](images/21017652365458_notification%20settings.jpg)
*Notifications settings*

Keep in mind that in some cases the notification will be sent to you *only if the notifier decides* to send it out.

## Reacting to notifications right in Slack

When someone requests access to your board you can grant in right in Slack. Choose the option and click the button:

![react_in_Slack.jpg](images/21017652366482_react%20in%20Slack.jpg)
*Granting access to a board in the Slack channel*

## Unfurling board links

The latest version of Miro Slack app unfurls links to Miro boards by adding the board names, descriptions, and board thumbnails.

![unfurl_a_board_link.jpg](images/21017648441106_unfurl%20a%20board%20link.jpg)
*Board name, description, and thumbnail in Slack channel*

Reinstall your Slack integration to get access to the feature: go to Miro **Profile settings > Integrations** and click **Log out** next to **Miro Feed (Slack App)**. Then click **Connect** and [re-authorize](#enabling-the-app).

:::note
To re-authorize, you may need to receive approval from the Slack Workspace admin.
:::

To set a board thumbnail, access your Miro board and open the board information card by clicking the title in the upper-left corner of your board. On the pop-up window, click the image in the upper-left corner and upload a picture from your device or select a section from the board. The thumbnail will then appear in Slack when you share the board link.

![change_board_thumbnail.gif](images/21017652381330_change_board_thumbnail.gif)
*Setting board thumbnail*

## Sharing a board from Slack

When posting a board link in Slack you will see a notification showing the users that don't have access to the board. You can easily invite them to the board right via Slack. Feel free to [make the board public](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#sharing-boards-via-a-public-link) so that anyone with the link can view/comment it.

![share_from_Slack.jpg](images/21017652368658_share%20from%20Slack.jpg) *Sharing a Miro board from within Slack*

:::tip
If the option is not available for you, please re-install the app in settings or ask your admin to update the plugin in Slack Marketplace.
:::

## Creating a board from Slack

You can use the Miro shortcut to create a board from within Slack. Search Miro and choose **Create a board**.

![Miro_shortcut.jpg](images/21017652369938_Miro%20shortcut.jpg)
*Creating a board from Slack*

Enter a title for the board, select a Miro team, and add a short message to send along with the link to the newly created board within Slack.

![create_board_modal.jpg](images/21017648447506_create%20board%20modal.jpg)
*Setting parameters for a new board in Slack*

Once the board is created, the message will be sent to the channel/conversation along with the board link.

![new_board_message.jpg](images/21017648448530_new%20board%20message.jpg)
*A message will be posted after creating a new board from within Slack*

If some channel members do not have access to the newly created board, you'll be suggested to [share the board with them from within Slack](#sharing-a-board-from-slack).

## Disabling the app

To disable the integration, go to the **Profile settings > Integrations** and click **Log out**:

![Slack_log_out.jpg](images/21017648449554_Slack%20log%20out.jpg)
*Disabling Miro Feed*

To remove the app from Slack completely, open **Miro** channel settings in Slack, click **Configuration**.

![Miro_Slack_configuration.jpg](images/21017648451218_Miro%20Slack%20configuration.jpg)
*Configuration of the Miro App for Slack*

You'll be redirected to the Miro app Settings page. Scroll down, find your name in the list of authorized users and click **Revoke**.

![revoke_access.jpg](images/21017648452242_revoke%20access.jpg)
*Removing Miro access to Slack*

Workspace Admins will also see the option to delete the App from the *whole workspace*.

![remove_app.jpg](images/21017648453138_remove%20app.jpg)
*Removing App from Slack*

## Frequently asked questions and possible issues

*1. If a user adds Miro to Slack, will Miro be able to read their Slack channels?*
- No, Miro will just view basic information about public channels in the workspace. It means that Miro will be able to read the list of channel names and won't be able to read the channel messages.

2. *I am getting 'Something went wrong' message when trying to connect the Miro Feed for Slack.*
- Please check if your browser is allowing pop-ups from the miro.com domain. There may be an extra page asking for app permissions.

3. *I am not getting Miro-Slack notifications and re-installing the Miro app in Slack does not help. How can I fix it?*
- Please try to re-connect Miro and Slack on Miro's side (**Profile settings > [Integrations](https://miro.com/app/account/profile/integrations/)**).
