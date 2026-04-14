---
title: Zapier
article_id: 360025942994
sidebar_position: 18
created_at: '2019-07-04T17:26:16Z'
updated_at: '2025-02-26T12:10:13Z'
draft: false
availability:
  plans: free, starter, business, enterprise
---

Connect your favorite apps to Miro via Zapier, expanding the list of possibilities for automating your daily tasks. Move information between your apps and boards automatically so that you can focus on the most сrucial work.

## Creating a Zap with Miro

To connect Miro to other apps via Zapier, you need to have a Zapier account.

To create a Zap, click the corresponding button on the [dashboard in Zapier](https://zapier.com/app/dashboard).

![Create_Zap.jpg](images/21017005247378_Create%20Zap.jpg)
*Create Zap button*

Zapier creates an automated workflow between apps with **Triggers** and **Actions**.

:::warning
Now Miro can work only as an **Action** in Zapier.
:::

**Trigger**

A Trigger is an event in an app that launches the Zap. Once you set up a Zap, Zapier will monitor the app for that event. For the "Save new events in Google Calendar to Miro card widgets" example, the Zap is triggered only when a new event is created in Google calendar.

![new_event_trigger.jpg](images/21017005250578_new%20event%20trigger.jpg)
*Setting a Trigger event in Zap*

**Action**

An Action is an event that completes the Zap. In the previous example "Save new events in Google Calendar to Miro card widgets", new Miro cards will behave as an Action.

:::warning
Now Miro works only as an Action in Zapier.
:::

Find Miro and choose one of the three Actions there: [Copy board](#copy-board-action), [Create board](#create-board-action), [Create card widget](#create-card-widget-action).

![creating_a_Zap_with_Miro_as_an_action.gif](images/21016967717138_creating%20a%20Zap%20with%20Miro%20as%20an%20action.gif)
*Creating your own Zap with Miro as Action*

### Copy board action

It's an action designed to create a copy of a particular board. You will need to select a team where the board copy will be created.

![install_Zapier.jpg](images/21016967717522_install%20Zapier.jpg)
*Selecting a Miro team*

On the next step, choose the following parameters:

- Original board - pick a board from the team to make a copy of. You can search the board by its name or ID *(*e.g. *o9J_rxLXasqA).*If you can't find a board on the list, please try reloading the data and check once again
- Title - enter a title name for the board copy. If you leave the field blank, the board will be created with the **Untitled** name
- Description - enter text for the board description
- Team access - you can choose between **Private**, **View**, **Comment,** and **Edit** types of team access to the board
- Access via link - create rules for sharing this board with a link. You can set **Private**, **View,** and **Comment** access groups

![set_up_action.jpg](images/21016967719058_set%20up%20action.jpg)   *Setting up the Copy board action event*

### Create board action

This action will create a board with a specific title, description, and access settings.

- Title - enter a title name for the new board. If you leave the field blank, the board will be created with the **Untitled** name
- Description - enter text for the board description
- Team access - you can choose between **Private**, **View**, **Comment,** and **Edit** types of access for your team
- Access via link -  create rules for sharing this board with a link. You can set **Private**, **View,** or **Comment** access via a public link

![create_board_action.jpg](images/21016967720338_create%20board%20action.jpg)
*Setting up the Create board action event*

### Create card widget action

This action enables you to transfer information (Slack messages, for example) as a [card](../../using-miro/essential-tools/02-cards.md) widget directly inside a specific [frame](../../using-miro/essential-tools/07-frames.md) on a Miro board with custom rules.

- Board - pick a board from the team which you want to use. You can search the board by its name or ID *(*e.g. *o9J_rxLXasqA)**.* If you can't find a board on the list, please try reloading the data and check once again
- Frame - select a frame from the board you've picked. You can search the frame by its name, and if you can't find it there, please try reloading the data and check once again
- Card title - enter a title for your card
- Card title link - here you can insert a link from the connected app (for example, you can create a card with a link to a newly created task in Asana)
- Card description - create a description for your card
- Card due date - set a due date for the card
- Card border-color - pick a custom color for your card borders (for example, **#ff0000** in this field will set the card color as red).

![create_card_action.jpg](images/21017005262610_create%20card%20action.jpg)
*Setting up the Create card action event*

## Disable Zapier integration

To remove the Zapier integration from your Miro team, open the [Team settings](../../administration/get-started-as-a-miro-admin/06-manage-starter-and-education-plan.md)**> Apps & Integrations > Zapier**and click **Uninstall***.*

![uninstall_Zapier.jpg](images/21017005263890_uninstall%20Zapier.jpg)
*Zapier uninstall options*

## Frequently asked questions

1. *Do I need to have an enterprise Zapier account to use it with Miro?*
   - No, it is not required. Miro integration can be built with any Zapier plan.
2. *Where are my Zapier data stored?*
   - This is an official Miro maintained integration and all data storage practices in Miro apply here as well.
3. *Do I need to be the Team Admin in Miro to set Zapier integration?*
   - It depends on admin settings in Miro and in Zapier. By default, even non-admin team members can set up the integration.
4. *Do the cards (Trello, Asana, etc.) sync with cards imported into Miro boards?*
   - No, Zapier currently doesn't provide synchronization. For instance, if you move your Trello card from "doing" to "done", it isn't reflected on Miro's side.
5. *I cannot link Gmail to Miro via Zapier. Why?*
   - Please check your email. At the moment, users with Gmail account which ends *@gmail.com* or *@googlemail.com* cannot link Gmail to Miro, as Zapier can send Gmail information to a limited number of apps.
