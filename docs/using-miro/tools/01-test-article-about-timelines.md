---
title: Test article about Timelines
article_id: 28554936286738
sidebar_position: 1
created_at: '2025-08-05T08:58:50Z'
updated_at: '2025-08-05T08:59:16Z'
draft: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: amplitude
availability:
  plans: Desktop, mobile, interactive displays
---

Timeline is an interactive planning tool that strategically aligns stakeholders and teams. Create, manage, and share your timeline directly from a Miro board. Use Timeline to roadmap your project, add visibility, and hit milestones more efficiently. You can view the Timeline in terms of days, weeks, months, or quarters.

## Key features

- **Customize an interactive timeline** anywhere on your Miro board.
- **Add and delete records** inside the Timeline widget.
- **Drag and drop Miro Cards** into the Timeline widget.
- **Create groups of records** to organize information logically.
- **Resize each time bar** to change dates for individual records.
- **Scale the Timeline view and time bars** automatically when you adjust dates.
- **Include multiple Timeline widgets** with different data sources on the same Miro board.
- **Share your timeline** with team members and stakeholders.
- **Map and visualize dependencies** between records using Blocked by" and Blocking fields amongst projects.

## Add Timeline to your board

:::warning
Guest editors do not have the ability to add or edit Timeline.
:::

1. Open a Miro board.
2. Select **More apps** (**+**) from the [creation toolbar](../../getting-started/start-here/your-first-board/05-toolbars.md#creation-toolbar).
3. Search and select **Timeline**.
   Your cursor now shows as the Timeline icon.
4. Click anywhere on the Miro board to place your Timeline widget.

## Timeline interactions

The Timeline widget provides several controls that enable you to manage your work.

### Add a record

Click the plus sign (**+**) above the records column. A new record appears on the timeline.

To reposition a record, drag and drop the record higher or lower on the timeline. You can also drag and drop the corresponding time bar on the timeline itself.

### Edit a record’s text

Select the record or timebar, and then select the text. The blinking cursor indicates that the text is ready for editing.

### Delete a record

1. Select a record or time bar for editing.
2. Press delete or backspace on your keyboard.
3. The record is now deleted.

### Change start and end dates

To change the time range shown on the Timeline, elect the **calendar icon** (![icon-calendar.svg](images/28554943314706_icon-calendar.svg)) on the upper left side of the Timeline widget to choose your start and end dates. The Timeline scales automatically to match your selection.

You can also use the dropdown to select whether to scale the Timeline to **Days**, **Weeks**, **Months**, or **Quarters**.

![timeline-dates.png](images/28554943315858_timeline-dates.png)

*Changing the Timeline scale*

To change the start and end dates for a specific record, drag either end of the time bar.

### Change record color

Click the record or time bar for a color circle to appear. Click the color circle for a color picker and select a color.

### Reposition records

In the records column, drag and drop a record to reposition it on the timeline. You can optionally drag and drop a time bar.

![timeline-rearrange.gif](images/28554936283794_timeline-rearrange.gif)

*Rearranging records on a Timeline*

### Filter records

You can filter the contents of a Timeline by one or more fields to help narrow the tasks you would like to work with. You can do this by clicking the filter icon on the top of the Timeline. You can choose whether you want to filter by one or more fields and then choose which field you want to filter by. Once a filter is applied you should see a counter on top of the filter by icon on the timeline to reference how many filters are applied.

To remove a filter follow the same steps and click the trash can next to the filter you would like to remove.

### Sort records

You can sort the contents of a timeline by clicking the sort icon at the top of a timeline then choosing which field you would like to sort records within the timeline by. You can then choose whether you want the records to be sorted in either ascending or descending order according to the field you have sorted by. Once a sort has been applied you will see a counter appear on top of the sort by icon to indicate that a sort is applied.

You can remove a sort by following the same steps and clicking the delete sort option from the drop down.

### Copying and pasting Timelines

When you copy and paste a timeline you will see a pop-up that will provide you with two options:

- To paste as a synced view of the original timeline.
- To create a new timeline using the original timeline as a template.

You can copy and paste within and across boards.

Choosing to paste as a sync view of the original timeline ensures that all the records within the new timeline remain synced with the records in the original timeline, however, you can customize the view of the new timeline without impacting the original. For example you can apply a filter, sort, group or change the layout of the new timeline without changing those properties on the original timeline. You can use this to create multiple views/layers of data of the same information all whilst the records remain synced across timelines and boards.

Choosing to paste as a new timeline will create a copy of the original timeline however the records in the new timeline will not sync back to the original. Therefore you have just used the original timeline as a template to create a new timeline with the same layout. No edits made to the new timeline will reflect on the original and vice versa.

### Group records

A group adds an additional level of hierarchy to your timeline, for example, if you want to order a roadmap by start date or end date.

To create a group, click the **Group** icon at the top of the Timeline then select which field you would like to group the records by. Choosing a group by field will separate the Timeline into relevant groups, which you can expand and collapse. To remove a group, follow the same steps and click **Clear grouping**.

![timeline-grouping.png](images/28554943317266_timeline-grouping.png)

*Grouping records on a Timeline*

:::tip
You can drag and drop a record to another group.
:::

## Add Miro Cards or Sticky notes to your timeline

The Timeline widget visualizes data from Miro Cards or Sticky notes. Simply drag and drop any card or sticky to a Timeline widget.

## Synced Cards

You can drag and drop records from the Timeline onto your canvas to create a synced card.

Follow these steps to create a synced card:

1. Hover over the record you’d like to create a synced card from.
   Icons will appear on the left-hand side of the record.
2. Click and hold the dots icon and drag it onto the canvas.
   A card is created with the information from that record.
3. The card will be updated whenever the record in the Timeline is updated, and vice versa.

   You have successfully created a synced card from your Timeline.

You can tell whether a card is synced to a Timeline via a database icon that will appear on the bottom right of the card.

If you delete a record, the corresponding synced card will remain on the board but will now appear blank.

If you delete a synced card on the canvas, the record will remain in the Timeline.

If you drag an existing synced card into the Timeline it originates from, it will not work, as it is treated as a unique record in that Timeline. However, you can drag an existing synced card into a new Timeline and it will appear in the Timeline as a new un-synced record.

## How to add Jira cards to Timelines

You can drag and drop Jira cards into a Timeline to create Jira synced records. This means you can combine work from Miro and Jira into a Timeline view to manage and track the whole team's work in one place.

To add a Jira card to your Timeline, follow these steps:

1. Find the relevant Jira card on the canvas.
2. Drag the card onto the Timeline.
3. Drop the card on the target row within the Timeline.

Any changes made in Miro will be reflected in Jira and vice versa. The following five fields within the Timeline will sync to Jira:

- Title
- Description
- Estimation
- Start date
- End date

Assignee and Status fields do not sync to Jira and are disabled in Timelines. While the content will still exist in Jira, they are not visible in Timelines. You can edit these fields in the Jira card side panel or in Jira directly.

All other fields in the Timeline are stored only in Miro and do not sync to Jira.

**More information:** See [Jira Cards FAQ](../../integrations-apps/atlassian/17-jira-cards-faq.md).

## Add milestones

You can add milestones to your timeline to keep track of upcoming dates and deadlines.

1. Hover on the timeline widget for a dotted line and flag icon to appear.
2. Click on your selected date and name your milestone.
3. Edit the milestone name by double clicking. The blinking cursor indicates that the text is ready for editing.
4. Change color by clicking and selecting a color from the color circle.
5. Change the milestone date by clicking on the milestone and then opening the calendar picker that appears above it.

## Change the layout of a Timeline

Switch the layout of your Timeline to view the same records on a table. You can do this by switching the layout of the existing widget you have on the canvas or making a copy of that timeline then changing the layout. You change the layout by clicking on the Timeline icon at the top of the table and choosing between Table or Timeline. When you switch to a Table view, settings like filtering, grouping, and sorting will be preserved and default fields may appear such as Title, Description, Status, Estimation, Priority, Theme, Start, and End Date.

**More information:** See [Tables](../formats/14-tables.md).

## Share your timeline

On your Miro board, follow these steps:

1. Select the Timeline widget that you want to share.
   The context menu appears above the widget.
2. Select the **more** (**...**) menu.
   A drop-down menu opens.
3. Select **Copy link**.
4. Share the link with anyone who has permissions to view the board.

## Relations (Dependencies)

> **Which plans:** Business, Enterprise

This relation field type allows you to map dependencies between records in your Timeline using connection lines. This helps you track project relationships and understand how work items depend on each other.

### Add dependencies between records

1. Hover over a timeline bar until you see connection points.
2. Click and drag from one bar to another to create a dependency line.
3. The dependency will automatically appear in both the Timeline and Table views.

:::note
Records can have multiple blocking and blocked by relationships. Dependencies sync across all synced Timelines, ensuring consistency across your views and boards.
:::

:::note
Dependencies will automatically create corresponding Blocked by and Blocking fields in your Table view.
:::

:::warning
Current limitations (Beta):

- Dependencies are not yet supported for Jira-synced records or other third-party integrations.
- Visual indicators for dependencies are not yet shown on synced cards.
- Automatic date adjustments based on dependencies are not yet available.
:::

## Focus mode

You can edit and view your Timeline in focus (full screen) mode. Simply click the **diagonal arrow icon** at the top of the widget. Settings like Filter, Sort, Group, and Hide fields are located on the top right.

To return to the canvas, click **Ideate on canvas** at the top.
