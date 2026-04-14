---
title: Miro for Jira Cloud
article_id: 360017572414
sidebar_position: 4
created_at: '2019-02-11T10:12:55Z'
updated_at: '2026-03-20T14:10:12Z'
draft: false
availability:
  plans: starter, business, enterprise
  notes: Jira Cloud only
---

Visualize anything together with your team — work on the product backlog with digital sticky notes, create flowcharts, diagrams and wireframes. Attach boards to Jira issues and collaborate with your team in real-time like on a whiteboard meeting.

:::note
You can also embed Miro boards with the [Atlassian Smart link feature](#atlassian-smart-link-for-miro).
:::

:::note
Note that Miro has two types of Jira integrations: **Miro for Jira Cloud** (which allows embedding Miro boards on the Jira side) and **Jira Cards**. To learn more about Jira Cards, visit [this article](https://help.miro.com/hc/articles/360017572434).
:::

## How to install

The installation process is standard for all Jira add-ons. First, log into your Jira with administrative rights, then download the add-on [here](https://marketplace.atlassian.com/apps/1215456/miro-for-jira-cloud?tab=overview&hosting=cloud) (the app can also be found at **the Atlassian Marketplace** > **Find new apps** > **Miro for Jira Cloud**): click **Get app**and **Get it now**.
And that's all! The installation is complete.

![Miro_for_Jira.jpg](images/21016134089234_Miro%20for%20Jira.jpg)
*Jira notification about the successful installation*

Please note that as an administrator you don't need to map Miro users to Jira users during setup. Each user will have to authorize themselves in Miro within Jira.

## How to use the add-on

### Attaching boards to Jira issues

To attach a board to a Jira issue, open the issue in Jira. Click **Add Board** in the **Miro boards** section.
![add_Miro_boards_in_Jira.jpg](images/21016134090642_add%20Miro%20boards%20in%20Jira.jpg)
*The add-on button appears after the installation*

:::tip
If you don't have the Miro boards section, find it in the context menu of the issue.
:::

![Miro_boards_section.jpg](images/21016134091026_Miro%20boards%20section.jpg)
*Adding the Miro boards section to a Jira issue*

You will see a picker with Miro boards. Choose the board you wish to add (feel free to switch between your teams in the picker). If you're not authorized in Miro, you'll need to sign in first.

Set the sharing settings of the board in the drop-down menu. You can make the board available for viewing and commenting so that the users who do not have a profile in Miro can also access it.

:::note
For [Enterprise plan](https://help.miro.com/hc/articles/360017571534) Miro users, your access settings will follow organization-wide access controls which might imply that some sharing options may be restricted. Learn more: [Managing Enterprise sharing policy for embed integrations](https://help.miro.com/hc/articles/4405088016274).
:::

![embed_a_board_in_Jira.jpg](images/21016134091922_embed%20a%20board%20in%20Jira.jpg)
*Sharing settings when attaching a board to a Jira issue*

Note that you can only embed boards on which you have Editor access.

Your board is now attached to the chosen Jira issue:

![Miro_board_in_Jira.jpg](images/21016120705810_Miro%20board%20in%20Jira.jpg)
 *Miro board attached to a Jira issue*

### Creating new boards from Jira

To create a new board right from a Jira issue, click **Add board** and create a **New board** from the picker.

![create_a_new_board_from_the_picker.jpg](images/21016120706322_create%20a%20new%20board%20from%20the%20picker.jpg)
*Creating a board from the picker*

### Viewing, commenting, and editing boards

Simply click an attached board to view/comment/edit it depending on the set access rights. The board window will open as an overlay allowing you to work and collaborate as if you were in Miro.

![Miro_embed_in_Jira.jpg](images/21016120699410_Miro%20embed%20in%20Jira.jpg)
*Board's overlay in Jira*

 You can also click the source button to open the board in Miro in a new tab for your convenience.

![source_button.jpg](images/21016134094738_source%20button.jpg)
*The button to go to the Miro app*

### Detaching boards

To detach a board, simply click on the cross icon and the attachment will be instantly removed from the issue (on the Miro side the board will be unaffected).

![remove_an_attached_board.jpg](images/21016134095634_remove%20an%20attached%20board.jpg)
*The option to remove the attached board*

## How to disable the add-on

To disable the integration, open **Atlassian Marketplace** > **Manage apps** > open the page of the add-on, and click **Uninstall**:

![uninstall_Jira_add-on.jpg](images/21016134096274_uninstall%20Jira%20add-on.jpg)
*The option to **Uninstall**in the Jira add-ons section*

## Atlassian Smart Link for Miro

You can embed Miro boards into Jira issues using the Atlassian Smart Link feature. The feature allows you to automatically embed a board without the need to install a plugin.

:::note
Please note that only those users who have access to the embedded board on the Miro's side will be able to work with the preview after connecting their Miro and Atlassian accounts. If you'd like to make the preview available for all Jira users, feel free to use the Jira add-on.
:::

Go to a Jira issue and simply paste a board link or type /link to insert. If you use the feature for the first time, you will be asked to connect your Miro team. Click **Connect to preview,**authorize in Miro, and choose a team from which you will embed your boards.

![install_Atllassian_links.jpg](images/21016134098834_install%20Atllassian%20links.jpg)
*Choosing a team to embed boards from*

When you paste a Miro board's link into a Jira issue, it will turn into a Jira widget automatically. Click the link and you will see the options to display the link as a card or as an embed.

![display_as_link.gif](images/21016134099346_display%20as%20link.gif)
*The options to display a Miro board link as a link, card, or embed*

If you choose to display the board as an embed, you can change the embed size by dragging its side.

![changing_embed_size_in_Jira.gif](images/21016120700306_changing%20embed%20size%20in%20Jira.gif)
*Changing Miro embed size in Jira*

:::warning
If third-party cookies are blocked in your browser there can be unexpected issues displaying embedded boards.
:::

## Frequently asked questions

Can I hide the Miro boards section in Jira issues?

Yes, click the three dots in the upper-right corner of the section and choose **Hide Miro boards**.
![hide_Miro_boards.jpg](images/21016120713746_hide%20Miro%20boards.jpg)
*Hiding Miro boards in Jira*

Does the add-on work in Jira Next-gen projects?

Yes, you can attach your boards to such projects.

Is there an additional cost for Jira add-on?

Miro for Jira Cloud is available for all paid plans at no additional cost (Starter, Business, and Enterprise plans).

We're going to migrate Jira from one cloud instance to another. Will Miro boards embedded in Jira issues be affected?

There should be no issues with embedded Miro boards if the content is moved without changes.
