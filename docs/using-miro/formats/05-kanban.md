---
title: Kanban
article_id: 29188841316114
sidebar_position: 6
created_at: '2025-09-02T19:42:54Z'
updated_at: '2026-03-13T12:26:15Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: kanban-usm
availability:
  roles: All logged-in users
  plans: free, starter, business, enterprise, education
  platforms: browser, desktop, mobile, Interactive displays
---

The Kanban view lets you organize your tasks into columns, making it easy to track progress, spot bottlenecks, and keep your team aligned. Seamlessly switch between Kanban, Timeline, and Table views to plan, execute, and adapt in one place.

## Key features

- **Customize a Kanban board** anywhere on your Miro board.
- **Add, edit, and delete cards** inside the Kanban widget.
- **Add, edit, delete, and hide columns** inside the Kanban widget.
- **Create swimlanes** in the Kanban widget.
- **Drag and drop Sticky notes, Miro Cards, and Jira Cards** into the Kanban widget.
- **Group, sort, and filter cards** to organize information logically.
- **Switch to Table or Timeline layout** to visualize your data in different ways.
- **Include multiple Kanban widgets** with different data sources on the same Miro board.
- **View and edit your Kanban board in full screen mode** for full focus.

## Add Kanban to your board

:::warning
Guest editors do not have the ability to add or edit Kanban.
:::

1. Open a Miro board.
2. Select **Tools, Media and Integrations**(*![icon-tools.svg](images/29210901366418_icon-tools.svg)*) from the [creation toolbar](../../getting-started/start-here/your-first-board/05-toolbars.md#creation-toolbar).
3. Search and select **Kanban.**
   Your cursor now shows as the Kanban icon.
4. Click anywhere on the Miro board to place your Kanban board.

## Kanban card actions

The Kanban widget provides several controls for cards that enable you to manage your work.

### Add a card

Click the **plus sign** (**+**) in a column. A new card will appear in the column.

### Move a card

To reposition or move a card, drag and drop the card. Once a card has been move to another column, the card's column field will also change.

### Edit a card's text

Select the card, and then select the text. The blinking cursor indicates that the text is ready for editing.

To apply formatting or add a link to text within a card:

1. Double click on the card you’d like to edit.
   The record becomes editable.
2. Highlight the text you want to format.
   A context menu will appear.
3. Apply formatting or add a link to the text from the context menu or using [keyboard shortcuts](../working-on-the-board/06-shortcuts-and-hotkeys.md).
4. Press enter to save the record.

Text formatting can also be applied in the side panel when editing a card.

### Change card color

1. Click the card and a **color circle** will appear.
2. Click the **color circle** to access the color picker.
3. Select a color.

### Edit card fields

1. Select the card.
2. Click the **Open record in side panel** icon to open the side panel.
3. Edit the card fields as needed.
4. Alternatively, you can switch to the Table layout to see your Kanban cards in more detail as rows in a Table.

You can also determine which card fields you want shown in the Kanban cards:

1. In the Kanban header, click the Hide fields icon to open the menu.
2. Select which fields you want to show or hide on the Kanban cards.
   Cards are updated in real time.

### Delete a card

1. Select a card.
2. Press delete or backspace on your keyboard. Alternatively, you can click the record and delete via the trash bin icon.
3. The record is now deleted.

## Kanban column actions

There are several column actions you can take to better manage your work within the Kanban widget.

### Add a Kanban column

1. Click the **Create column** on the very right of the Kanban.
2. Alternatively, you can add a Kanban column in the **three dots** (**...**) menu beside a column name.

### Edit Kanban column

1. Click the **column name**.
2. Rename the column. You can also change the column color here.
3. Alternatively, you can rename a Kanban column name in the **three dots** (**...**) menu beside a column name.

### Hide columns

1. Click the **three dots** (**...**) icon beside the column name
2. Click **Hide column** in the menu.
3. Click the **eye** icon on the right to unhide columns

### Move columns

1. Click the **three dots** (**...**) icon beside the column name.
2. Click **Move left** or **Move right**.

Drag and drop functionality is coming soon.

### Delete columns

1. Click the **three dots** (**...**) icon beside the column name.
2. Click **Delete column**.

### Change which columns are used

1. Click the **Column field** icon in the Kanban header.
2. Select the field (among all single-select fields) you want to use as your columns.
3. Alternatively, you can edit or create a new field to use as your columns.

:::note
Currently only single-select fields are available as columns.
:::

### Create swimlanes

1. Click the **Group** icon in the Kanban header.
2. Select the fields you want to use as your swimlanes.
3. Alternatively, you can create a new field to use as swimlane.
4. To remove swimlanes, click the **Group** icon again and click **Remove grouping**.

### Focus (full screen) mode

You can edit and view your Kanban in focus (full screen) mode. Simply click the **diagonal arrow icon** at the top of the widget. Settings like Filter, Sort, Group, and Hide fields are located in the header.

To return to the canvas, click **Go to canvas** at the top.

## How to add Jira cards into Kanban (BETA)

You can drag and drop Jira cards into a Kanban to create Jira synced records. This means you can combine work from Miro and Jira into a Kanban view to manage and track the whole team's work in one place.

To add a Jira card to your Kanban, follow these steps:

1. Find the relevant Jira card on the canvas.
2. Drag the card onto the Kanban.
3. Drop the card in the target column within the Kanban.

Any changes made in Miro will be reflected in Jira and vice versa. The following fields within the Table or Timeline will sync to Jira:

- Title
- Description
- Estimation
- Start date
- End date
- Assignee (Beta)
- Status (Beta)

**More information:** See [Jira Cards FAQ](../../integrations-apps/atlassian/17-jira-cards-faq.md).
