---
title: Miro in Asana tasks
article_id: 4420591454866
sidebar_position: 3
created_at: '2022-02-15T06:32:16Z'
updated_at: '2025-02-26T11:44:31Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: asana-cards
---

**Key Features**

- Add a Miro board to any Asana task, either by creating a new board or adding your existing board
- Make it easier to attach an existing board: when the user starts typing a board name, they will see a list of their existing Miro boards
- Auto-share the Miro board with the "collaborators" in the task, sending email invites and notifications from within Asana

### How to install and authorize the Miro app in Asana

Authorize and install the Miro app from the [Asana Marketplace](https://app.asana.com/-/install_platform_ui_app?app_id=1201153108289813).

![Miro_app_for_Asana.jpg](images/21017653436434_Miro%20app%20for%20Asana.jpg)
*Click **Get started** after following the link*

Then select **Connect to Miro** and allow Miro to access your Asana account.

![grant_permission.jpg](images/21017653438354_grant%20permission.jpg)
*Allowing Miro to access your Asana account*

Choose a team to install the app for and click **Install & authorize**. The app will be installed for all members of the team, but each user in the team will need to authorize in order to attach their own Miro boards to tasks.

![install_Miro_app_for_Asana.jpg](images/21017683076114_install%20Miro%20app%20for%20Asana.jpg)
*Selecting a team*

On the next step, select the Asana projects that you would like to connect to Miro.

Once you install and authorize the app, you will be able to attach boards from this team. If you need to attach your boards from **other teams** as well, follow [this link](https://app.asana.com/-/install_platform_ui_app?app_id=1201153108289813) and install the app for the teams.

### How to attach an existing Miro board to an Asana Task

:::warning
You can only attach your own boards stored in the team(s) where [the app has been installed](#how-to-install-and-authorize-the-miro-app-in-asana).
:::

1. Select the task in which you’d like to attach a Miro board.
2. In the task details section, select the **Attach Miro Board** dropdown.
   ![attach_a_Miro_board_to_Asana_task.jpg](images/21017683077266_attach%20a%20Miro%20board%20to%20Asana%20task.jpg)
   *Attaching a Miro board to an Asana task*
3. Select **Attach Existing Board**.
4. Find the specific Miro board to import directly from Miro using by searching the board name. You can also paste the board URL directly into the form and select **Add**. You can attach your own boards only.
5. If on the board Sharing window, the option **Anyone with the link can vew/comment/edit** is activated, the board will automatically be shared with all current and future Asana collaborators for this task.

:::warning
The auto-share feature will turn off if a task is inactive for more than 30 days. Users will still be able to manually [share the board from within Miro](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).
:::

Your fellow collaborators will receive an email notification letting them know you’ve invited them to the Miro board.

:::warning
Please note, if you remove a collaborator from the Asana task, their access to the attached board will not be affected. So if you want to additionally remove the user from the board, you need to [change their access in the board sharing settings on the Miro side](../../using-miro/sharing-boards/01-board-access-rights.md#changing-access-rights).
:::

### How to create a new Miro board in an Asana Task

1. Select the task in which you’d like to attach a Miro board.
2. In the task details section, select the **Add Miro board** dropdown.
3. Select **Create New Board.
   ![attach_a_new_board_to_an_Asana_task.jpg](images/21017683078162_attach%20a%20new%20board%20to%20an%20Asana%20task.jpg)***Creating a new Miro board from within Asana*
4. Type your desired board name and invite Asana collaborators by selecting one of the checkbox options. You can choose to invite all current collaborators from the task or automatically invite all future task collaborators, which includes any Asana collaborators that interact with the task (through posting in the comment section or being added by the task creator as a collaborator).
5. Select **Create Board**.
   ![creating_a_board.jpg](images/21017653442450_creating%20a%20board.jpg)
   *Creating a new Miro board from within Asana*

Your fellow collaborators will receive an email notification letting them know you’ve invited them to the Miro board.
