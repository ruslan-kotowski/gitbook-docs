---
title: Tables
article_id: 22760922335506
sidebar_position: 11
created_at: '2024-11-20T17:33:53Z'
updated_at: '2026-03-13T12:26:15Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: All Miro plans
  roles: Board owners and editors
---

Tables are an interactive tool that allow you to structure your content on Miro, turning ideas into actionable plans.

## Key features

Tables includes the following key features:

- **Create custom fields**
  Organize and structure your information with custom fields.
- **Create records from Miro Cards**
  Drag and drop Miro Cards into the Table widget to create new records.
- **Create records from Sticky notes**
  See Add a Miro Card or Sticky note to a Table.
- **Create synced records from Jira cards**
  See [Add a Jira card to a Table](#add-a-jira-card-to-a-table).
- **Advanced filter and sorting capabilities**
  Filter and sort Tables to organize and prioritize records.
- **Group records**
  Organize the records in a Table by field to group information logically.
- **Create synced Tables on multiple boards**
  Copy and paste a Table to create a synced view of the same records
- **Timeline view**
  Switch to a Timeline view to see your data in a new layout.
- **Column calculations**
  Calculate aggregates like sum, average, and more for numeric fields to analyze your data at a glance.
- **Visual number formatting**
  Format numbers as progress bars with percentage or currency display and use conditional formatting rules to highlight values that meet specific criteria. See [Visual numbers in Tables](04-visual-numbers-in-tables.md).
- **Dependencies**
  Map and visualize dependencies between records using "blocked by" and "blocking" fields amongst projects.
- **Bulk actions**
  Perform actions like edit, move, duplicate, and delete on multiple records at once, or drag multiple records to the canvas as cards.

## Add a Table to your board

:::warning
Guest editors do not have the ability to add or edit Tables.
:::

1. Open a Miro board.
2. Click the **Tools, Media and Integrations** icon (**+**) on the creation toolbar.
   The Tools, Media and Integrations panel opens.
3. Search and select **Table**.
   Your cursor now shows as the Table icon.
4. Click anywhere on the Miro board to place your Table widget.

## Convert an Excel file to a Table

1. Open a Miro board.
2. Click the **Tools, Media and Integrations** icon (**+**) on the creation toolbar.
   The Tools, Media and Integrations panel opens.
3. Search and select **Upload**.
   The Upload panel opens.
4. Select **My device**.
5. Navigate to and select the Excel file (.xlsx) you'd like to upload.
6. A modal will open with options:
   1. Convert to table.
   2. Convert to grid.
   3. Add as file.
7. Select **Convert to table** and choose whether to **Use first row as headers**.
8. Click **Select**.
9. A table will be created on the board with the data from the Excel file.

:::warning
When uploading an Excel file, there is a limit of 500 rows and 30 columns.
:::

## Copying and pasting Tables

You essentially have two options when copying and pasting Tables, either within a board or between boards. The first option is to create a synced Table that will show updates in each location. The second option is to create a non-synced Table, which functions like a template.

1. Select the table you’d like to copy.
2. Click on the Context menu (![icon-main.svg](images/28592441885714_icon-main.svg)) and select Copy. Alternatively, use the Ctrl + C (on Windows) or Command + C (on Mac) keyboard shortcut.
3. Navigate to the place on the board where you want to paste your table.
4. Right click and select Paste. Alternatively, use the Ctrl + V (on Windows) or Command + V (on Mac) keyboard shortcut.
   A pop-up will open.
5. Select whether you want to create a synced Table or a new Table in the pop-up.

## Managing permissions for Tables

If you create one or more synced views of a table across Miro boards you will have to manage permissions to make sure that when you add a synced view of a Table to a new board you can see and manage who has edit and view access to that Table. Permissions to synced views of tables are managed by the Home board—the board on which the original table was created.

Upon pasting a Table on a new board as a synced view you will be shown a pop-up if not all users of the board have view or edit permissions for the Table. If you would like to view or edit the permissions of the table it will navigate you to the original board where the Table appears to make changes.

If a user on a board does not have access to the home board where the original Table was created the Table will appear in a no access state for them. If the user only has view access to the home board they will be able to see the Table on the new board but not edit any of the records or change the view by applying filters, sorts, groups etc.

## Interacting with Tables

The Table widget provides flexibility to create content you want and structure and organize it most effectively for your use case.

Upon creating a new Table on your Miro board a set of default fields will be provided that map to the existing fields found in Miro cards. You can delete, edit, or hide these fields or create your own new fields.

### Create a field

Follow these steps to create a new field:

1. Click the + icon at the top of the far right column of the Table.
   A menu opens.
   ![tables-adding-fields.png](images/25142699942930_tables-adding-fields.png)
   *Adding a new field to a Table*
2. Click on the type of field you want to create from the menu. There are options for Miro fields and Custom field types.
   An options dialog opens.
3. Enter the field information (Field name and in the case of the Select field, the Options for the drop down) in the dialog and click Save.

:::note
The Link field type is only available for Business and Enterprise plans.
:::

### Edit a field name or options

1. Hover over the field name.
   A three dots (...) icon will appear.
2. Click the **three dots** (**...**) icon.
   A menu will open.
3. Click **Edit field**.
   A dialog will open with edit options.
4. Edit the field name and/or options and click **Save**.

### Delete a field

1. Hover over the field name.
   A three dots (...) icon will appear.
2. Click the **three dots** (**...**) icon.
   A menu will open.
3. Click Delete.

:::warning
A deleted field cannot be undone. It will be deleted from the current Table and all synced versions immediately.
:::

### Hide or unhide a field

Follow these steps to hide or unhide a single field:

1. Hover over the field name.
   A three dots (...) icon will appear.
2. Click the **three dots** (**...**) icon.
   A menu will open.
3. Click **Hide field**.
   The field will be hidden.
4. To unhide the field, repeat the same steps above but click **Unhide field**.

You can also hide or unhide multiple fields at once.

Follow these steps to hide or unhide multiple fields:

1. Click on the **Hide** icon at the top of the Table.
   A list of fields in the Table will appear.
2. Select the fields you would like to hide or unhide from the list.

### Edit a record

1. Double click on the record you’d like to edit.
   The record becomes editable.
2. Edit the record and press enter.

To apply formatting or add a link to text within a record:

1. Double click on the record you’d like to edit.
   The record becomes editable.
2. Highlight the text you want to format.
   A context menu will appear.
3. Apply formatting or add a link to the text from the context menu or using [keyboard shortcuts](../working-on-the-board/06-shortcuts-and-hotkeys.md).
4. Press enter to save the record.

Text formatting can also be applied in the side panel when editing a record.

### Bulk edit multiple records

1. Click on the six dots menu next to a row you'd like to include in the bulk edit.
2. Select additional records by holding down shift and clicking the last in the range of rows to include, or hold down command/control to select individual records.
   A toolbar will appear with options for editing.
3. Edit, move, or duplicate those records simultaneously in the toolbar.

### Delete a record

1. Hover over the record you’d like to delete.
2. Click the six dots icon to open the menu.
3. Select **Delete**.

### Delete multiple records

1. Hover over the row to reveal the checkbox on the left.
2. Select the records to edit using the checkboxes on each relevant row.
   A toolbar will appear with options for editing.
3. Click the **Delete** icon in the toolbar to delete all of the selected records.

### Add comments to Tables

Make collaboration easier by adding comments directly to the parts of a Table you want to discuss.

1. Hover over the row you'd like to add a comment to.
   An Add comment icon will appear on the right of the first cell.
2. Click the **Add comment** icon.
   A side panel will open on the left.
3. In the panel, add your comment and press enter.

Once new comments have been added, a comment count will appear next to the Add comment icon for each row. Click the icon to open the comments panel.

From the comments panel, you can:

- Reply to comments.
- Add reactions to comments.
- Resolve a comment thread.
- Copy a link to the comment.
- Follow the comment thread to receive notifications.
- Delete the comment thread.
- Edit a comment you've left.

### Add a Miro Card or Sticky note to a Table

You can create records in a Table using Miro Cards or Sticky notes.

1. Select the Card or Sticky note you want to copy to the Table.
2. Drag and drop the Card or Stick over the Table.
   A blue line will appear where the new record will go.
3. A new record is created, with the content from the Card mapped to the appropriate fields.
   In the case of a Sticky note, the content will populate in the first field.

### Add a Jira card to a Table

You can drag and drop Jira cards into a Table to create Jira synced records. This means you can combine work from Miro and Jira into a Table or Timeline view to manage and track the whole team's work in one place.

1. Find the relevant Jira card on the canvas.
2. Drag the card onto the Table.
3. Drop the card on the target row within the Table.

Any changes made in Miro will be reflected in Jira and vice versa. The following fields within the Table will sync to Jira:

- Title
- Description
- Estimation
- Start date
- End date
- Assignee (Beta)
- Status (Beta)

All other fields in the Table are stored only in Miro and do not sync to Jira.

**More information:** See [Jira Cards FAQ](../../integrations-apps/atlassian/17-jira-cards-faq.md).

### Work with Jira Cards in bulk

When bulk editing Jira-synced records, only actions and fields supported by the Jira integration are available. Unsupported actions will be hidden or disabled in the bulk actions menu.

### Filter a Table

You can filter the contents of a Table by one or more fields to help narrow the view/records you would like to work with.

1. Click the **Filter icon** at the top of the Table.
   A dialog will open.
2. Select whether you want to **Add filter** or **Add filter group**.
   A dialog opens.
3. Specify the parameters of the filter: the field to filter based on, the filter logic, and the specific content for the filter.
   The Table is filtered in real-time.
4. Click anywhere outside of the filter dialog to close it.

### Sort a Table

1. Hover over the field name.
   A three dots (...) icon will appear.
2. Click the **three dots** (**...**) icon.
   A menu will open.
3. Click on either **Sort ascending** or **Sort descending**.

To remove sorting on a Table:

1. Click on the **Sort icon** at the top of the Table.
   A dialog opens.
2. Click on **Delete sort**.

### Search in a Table

1. Click the **Search** icon in the top toolbar on the Table.
2. Type in your search query.
3. The relevant results will appear as you type.
4. You can navigate results using the arrow icons in the search bar or by scrolling through the Table.
5. Click the **Clear** (**X**) icon to return to the full Table.

### Group records by field

1. Click on the **Group** icon at the top of the Table.
   A menu opens.
   ![table-group-records.png](images/25142699944338_table-group-records.png)
   *Grouping records in a Table*
2. Select the field you’d like to group records based on.
   The records in the Table will be grouped by the chosen field.

:::note
When you drag a record into an existing group, the relevant field value will be updated to match that group.
:::

To remove the grouping on a Table, follow these steps:

1. Click on the **Group** icon at the top of the Table.
   A menu opens.
2. Click **Clear grouping**.

### Synced Cards

You can drag and drop records from the Table onto your canvas to create a synced card.

1. Hover over the record you’d like to create a synced card from.
   Icons will appear on the left-hand side of the record.
2. Click and hold the dots icon and drag it onto the canvas.
   A card is created with the information from that record.
3. The card will be updated whenever the record in the Table is updated, and vice versa.

You can tell whether a card is synced to a Table via a database icon that will appear on the bottom right of the card.

If you delete a record, the corresponding synced card will remain on the board but will now appear blank.

If you delete a synced card on the canvas, the record will remain in the Table.

If you drag an existing synced card into the Table it originates from, it will not work, as it is treated as a unique record in that Table. However, you can drag an existing synced card into a new Table and it will appear in the Table as a new un-synced record.

### View a Table as a Timeline

Follow these steps to switch to Timeline view:

1. Click on the **Table** icon at the top of the Table.
   A dialog opens.
2. Select **Timeline view** (or switch back to **Table view**).

When you switch to a Timeline view, the default Start date and End date, where populated, are used to plot the records in your Table as corresponding bars in your timeline. The Title field and the assignee field are used to display the record name and assignee on the bar.

**More information:** [Timeline](15-timeline.md)

## Column calculations

> **Which plans:** Business, Enterprise

Column calculations allow you to perform aggregate functions on numeric fields in your Table, helping you analyze and summarize your data. You can calculate sum, average, count, minimum, maximum, and median values for any numeric column.

1. Open the field options menu by clicking on the column header containing data.
2. Select **Show column calculation** from the menu.
3. Choose the calculation type you want to apply:
   1. Sum: Adds all values in the column
   2. Average: Calculates the mean of all values
   3. Count: Counts the number of entries
   4. Min: Shows the smallest value
   5. Max: Shows the largest value
   6. Median: Shows the middle value
4. The calculation result will appear in a footer row at the bottom of the Table.

To remove a column calculation:

1. Click the **Calculate** option within the footer row.
2. Select **None**.
3. Repeat until the last Calculation has been set to None.

:::note
You can apply one calculation per column. When you filter or group your Table, calculations automatically update to reflect only the visible records. In grouped views, calculations appear for each group as well as an overall total.
:::

Column calculations work seamlessly with visual number formatting. When you apply visual formatting to a calculated column, the result displays as a progress bar following your formatting rules. See [Visual numbers in Tables](04-visual-numbers-in-tables.md).

## Multi-column formulas

> **Which plans:** Business, Enterprise

In addition to column calculations, you can create fields for formulas across multiple columns. Formula fields calculate across multiple columns in the same row.

To create a formula field:

1. Click the **+** icon to add a new field.
2. Select the **Formula** type.
3. Use the visual formula builder to select fields, constants, and operators (+, -, ×, ÷, (,)).
4. Your formula automatically calculates for every row.

:::note
Formula fields currently support numeric fields and constants.
:::

## Relations (Dependencies)

> **Which plans:** Business, Enterprise

This relation field type allows you to map dependencies between records in your Table using "blocked by" and "blocking" fields. This helps you track project relationships and understand how work items depend on each other.

### Create dependency fields

1. Click the **+ icon** to add a new field.
2. Choose either:
   1. **Blocked by** - To show which records must be completed before this one.
   2. **Blocking** - To show which records are waiting for this one.
3. Name your field and click Create.

### Add dependencies between records

Once you've created dependency fields, you can link records following these steps:

1. Click on a cell in the **Blocked by** or **Blocking** column.
2. Select the record(s) you want to link from the dropdown menu.
3. Click outside the cell to save.

:::note
Records can have multiple blocking and blocked by relationships. Dependencies sync across all synced Tables, ensuring consistency across your views and boards.
:::

:::warning
**Current limitations (Beta):**

- Dependencies are not yet supported for Jira-synced records or other third-party integrations
- Visual indicators for dependencies are not yet shown on synced cards
- Automatic date adjustments based on dependencies are not yet available
:::

## Relations (Nesting)

> **Which plans:** Enterprise Advanced

The nesting relation field type allows you to create hierarchy between records in your Table using **Parent** and **Child** fields.

### Create hierarchical fields

1. Click the **+** icon to add a new field.
2. Choose either:
   1. **Parent**: Use this field to link a record to its higher-level item (e.g. a feature linked to an epic).
   2. **Child**: Use this field to link a record to its lower-level items (e.g. an initiative with sub-tasks).
3. Name your field and click **Create**.

### Link parent and child records

1. Click on a cell in the **Parent** or **Child** column.
2. Select the record(s) you want to link from the dropdown menu.
3. Click outside the cell to save.

### Visualize your hierarchy

1. Click the **View Settings** icon in the Tables header.
2. Toggle **Nesting** on.

Use the **chevron** next to Parent records to reveal or hide Child records.

:::note
*Nesting and hierarchy are hidden by default. You will need to turn it on in these settings.*
:::

### Other ways to create hierarchy

1. Click **Add sub-record** via the **6-dot menu** on the left on each row.
2. Nesting will turn on by default.

   > ✏️ Parent and Child fields will be created, but hidden. To unhide these fields, go to the Hide fields menu the Table header.

   > ✏️ To turn off Nesting, go to View Settings in the Tables header.
3. You can manage hierarchies through the Parent and Child fields.
4. When nesting is on, you can also drag and drop to create hierarchies.

:::warning
*If you delete a parent record, all of that record's child records will be deleted too. Use the Undo function to reverse this if needed.*
:::

If the Parent and Child fields are not hidden, they will be visible in the side panel. You can switch to Timeline view and watch your portfolio cascade over time.

:::warning
***Current limitations:***

- *Eight-level maximum for hierarchy.*
- *Nesting is not yet supported for Jira-synced records or other third-party integrations.*
- *Visualization is not in synced cards or in Kanban view.*
:::

## Focus mode

You can edit and view your Table in focus (full screen) mode. Simply click the **diagonal arrow icon** at the top of the widget. Settings like Filter, Sort, Group, and Hide fields are located on the top right.

To return to the canvas, click **Go to canvas** at the top.

## Structured Data widget limits

Each Miro board has a maximum limit of 250 structured data widgets, which includes the total combined count of Tables, Timelines, and Synced cards. Each table is limited to 1,000 rows and 50 columns. When you reach the row limit, you'll see a message preventing additional rows from being added.

For optimal performance, we recommend keeping tables under 200 rows when using many columns, as operations like grouping, sorting, and filtering may slow down beyond this point. These limits help ensure optimal performance and reliability for your Miro boards.

### What happens when you reach the data widget limit?

When a board reaches or exceeds the 250 structured data widget limit, you may experience:

- An error message when attempting to add more structured data widgets.
- Inconsistent loading of existing data widgets.
- Potential issues with saving changes.
- Performance slowdowns.

### Tips for managing data widget limits

If you're approaching or have exceeded the structured data widget limit, try to:

**Distribute widgets across multiple boards:**

- Group related content on separate boards.
- Use meaningful board names for easy navigation.
- Create a "master" board with links to all related boards.

**Consolidate similar data:**

- Merge tables with similar structures.
- Use filtering instead of creating separate tables for different views.
