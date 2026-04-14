---
title: Planner for Azure DevOps
article_id: 15280547945618
sidebar_position: 10
created_at: '2023-11-23T14:12:19Z'
updated_at: '2026-04-07T13:32:07Z'
draft: false
availability:
  notes: 'Available for: Education plan, Enterprise plan, Business plan'
---

> Available for: Education plan, Enterprise plan, Business plan

During team and company planning events like Program Increments (PI), Big Room, Roadmapping and Sprints, development teams discuss and align with each other.

With planner for Azure, facilitators and teams can run and participate in planning events on a Miro board, while also syncing updates to their Azure board in real-time — saving hours of manual work.

## How to create a planner for Azure DevOps

:::note
To use planner for Azure DevOps, first [set up your Azure integration](03-azure-cards.md).
:::

1. Navigate to the [creation toolbar](../../getting-started/start-here/your-first-board/05-toolbars.md#creation-toolbar) on the left side of your board.
2. Click **More apps** (**+**) and search ‘Planner’.
3. Click **Planner**.
4. A cursor will appear on the board. Click anywhere to place a blank planner.
5. The data source of your planner will default to the integration you have authorized. If you haven't yet authorized an integration, it will default to Jira. You can easily change this to Azure DevOps by clicking the dropdown labeled **Jira** and selecting **Azure DevOps**.
6. If you haven’t yet authorized your Azure DevOps account in Miro, you'll be prompted to log in.
7. Once you're logged in, click the **Azure project**dropdown and select a project to connect to the planner.
8. Next click the **Teams** dropdown and select a team.
9. The first **Columns** field is your *column type*. **Iteration** is automatically selected. More Azure fields are coming soon.
10. Use the second **Columns** dropdown to further refine which iterations you want to display.

## How to work with the planner

Drag Azure cards across columns to update them. For example, dragging a Azure card from Iteration 1 to Iteration 2 in the planner will update it in both Miro and Azure.

Participants can comment on Azure cards to track ongoing discussions and notes.

![Comment-on-an-Azure-Planner.png](images/21016020674450_Comment-on-an-Azure-Planner.png)*Commenting on the planner*

## Planner syncing

### From Miro to Azure

When you drag a card between custom fields in Miro, Azure is updated automatically. This may take a few seconds.

### From Azure to Miro

To make sure your planner remains up to date with changes you make in Azure, select the planner and click the **Sync** button in the context menu.

![Syncying-the-planner-with-Azure.png](images/21016020674962_Syncying-the-planner-with-Azure.png)*Syncing the planner with Azure*

The fields supported for Azure currently are:

- Iteration (aka sprint).
- Assigned-to.
- All other fields that fit the following criteria:
  - Editable (i.e. not readonly).
  - String (text) values.
  - A list of pre-defined values that can be set (i.e. not free-flow text).
  - Valid for Azure work items (some Azure fields have other usages).

# Not seeing your team's sprints?

Make sure that your iterations in Azure are mapped back to your team so that you can visualize them in the planner.

1. Go to your **Project** in Azure.
2. At the bottom of the right-hand side menu, click **Project settings** icon.
3. Go to the **Boards** section, and click **Team configuration**.
4. Click the **Iterations** tab at the top of the screen.
5. Click **+ Select iteration**. Make sure you have added all the iterations related to your team.

![Adding-iterations-Azure-Devops.png](images/21016020675858_Adding-iterations-Azure-Devops.png)*Adding iterations to Azure*

## Dependency mapping

Participants can visually map dependencies between tasks on the planner. Learn more about [Dependencies for Azure](../../using-miro/facilitation-tools/08-dependencies-for-azure-devops.md).

## Known limitations

### Dragging cards into Planner

Dragging cards from the Miro canvas into the Planner is not fully supported.

When you drag a card into the Planner, Miro attempts to update the card with the target column and row values. If the update succeeds, no error is shown. However, there are cases where the update may not work as expected. In these cases, you won't see an error message, but the card's field values may not have changed in Azure DevOps. Always verify that the changes are reflected in Azure DevOps after dragging cards into the Planner.

### Epics as parent work items

Azure DevOps only supports **Epics** as parent work items. Other work item types cannot be set as parents.
