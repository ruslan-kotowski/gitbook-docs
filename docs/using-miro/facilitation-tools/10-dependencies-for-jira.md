---
title: Dependencies for Jira
article_id: 10649083010834
sidebar_position: 7
created_at: '2023-03-22T10:22:08Z'
updated_at: '2025-11-25T16:22:15Z'
draft: false
availability:
  plans: Desktop browser, Desktop app
  notes: '💡: ** This feature is now available for [Azure DevOps](08-dependencies-for-azure-devops.md).'
---

Map existing dependencies or create new ones between Jira cards on your [planner](../../integrations-apps/atlassian/21-planner-for-jira.md) or anywhere on your Miro board, and they'll instantly sync in Jira. With the Dependencies app you can identify, visualize, discuss, and record dependencies between teams in real-time during planning exercises.

## How dependencies work

Dependencies appear as a layer of connecting lines, and show relationships between Jira cards.

They are only visible when you open dependencies on the board. Participants can filter different dependency types to discuss blockers and relationships.

![Dependencies-app.png](images/13244544218258_Dependencies-app.png)
*Dependencies mapped between Jira cards on a Planner widget*

## How to create a new dependency

1. Go to the Creation toolbar on the left-hand side of the board.
2. Click the **Dependencies** icon. If the Dependencies icon isn't already in your Creation toolbar, you'll need to add it from **Tools, Media and Integrations** (**+**).
3. The Dependencies panel will open.
4. Click **New dependency**.
5. Click **First card** and select a Jira issue from the dropdown or via search.
6. Select the **Dependency type** based on those available in your Jira instance (for example, blocks, clones, duplicates, or relates to).
7. Click **Second card** and select a Jira issue from the dropdown or via search.
8. Click **Save draft**, or **Save to Jira**directly.

:::tip
Draft dependencies are saved only in Miro. You can create draft dependencies as suggestions to other participants and teams during planning exercises. Once they’ve been reviewed and discussed you can then either save them to Jira or delete them.
:::

![dependencies-entry-point.png](images/21537435953426_dependencies-entry-point.png)
*Creating a new dependency and saving it to Jira*

## How to view and filter dependencies

1. Go to the Creation toolbar on the left-hand side of the board.
2. Click the **Dependencies** icon. If the Dependencies icon isn't already in your Creation toolbar, you'll need to add it from **Tools, Media and Integrations** (**+**).
3. The Dependencies panel will open, and any existing dependencies will appear as lines on the board.
4. Click the **Filter** icon at the top of the Dependencies panel.
5. Use the toggles to filter by **Dependency type** and **Sync status**.
6. Use the **Show lines** dropdown to control when dependencies are displayed. Select **Always** to view all active dependencies. Choose **On selection** to see dependencies only when you click on a specific Azure card or dependency type.

Dotted lines show draft dependencies, and solid lines show dependencies that have been synced to Jira. The line color represents the dependency type.

![Filtering-dependencies.gif](images/13245295619730_Filtering-dependencies.gif)
*Filtering the dependency view* *on the Planner widget*

## How to edit, save, revert or delete a dependency

1. Go to the Creation toolbar on the left-hand side of the board.
2. Click the **Dependencies** icon.
3. The Dependencies panel will open.
4. Click the **Edit** icon next to a dependency.

![The_option_to_edit_a_Dependency.jpg](images/10866625733778_The%20option%20to%20edit%20a%20Dependency.jpg)
*Editing a dependency*

You can change the **First card** and **Second card** of a dependency, as well as the **dependency type.**

*![Editing_a_dependency.gif](images/10866808392722_Editing%20a%20dependency.gif)**Changing the First card and Dependency type*

Click **Save to Jira** to save and sync a draft dependency to Jira.

![Save_to_Jira.png](images/10868740630034_Save%20to%20Jira.png)
*Saving a draft dependency to Jira*

Click **Revert to draft** to revert a synced dependency back to draft.

![Revert_to_draft.png](images/10868741500690_Revert%20to%20draft.png)
*Reverting a synced dependency in Jira back to draft*

Click the **Trash** icon to delete a dependency.
![Delete_dependency.png](images/10868804195986_Delete%20dependency.png)*Deleting a dependency*
