---
title: Edit a custom label
article_id: 21690361870354
sidebar_position: 19
created_at: '2024-09-30T13:43:27Z'
updated_at: '2026-03-04T23:02:00Z'
draft: false
---

:::note
We recommend editing labels only before you associate the label with a classification level.
:::

Edit labels to update conditions, like keywords or widgets, that you want to identify and locate on Miro boards. To edit a label, perform the following steps:

:::note
To edit custom labels , you must have the [Sensitive Content Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Sensitive Content Admin role, contact your Company Admin.
:::

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Data discovery**.
3. On the **Data discovery** **Overview** page, click the Ellipsis (three dots) on the row of the label you want to edit, and then click **Edit label**.
4. On the **Edit custom label** page, edit the label details.

   |  |  |
   | --- | --- |
   | **Field** | **Description** |
   | **Label name** | **Maximum length:** 80 characters  Descriptive name for the custom label. You can use a company-internal project name as this label does not appear in the logs.  **Note:** The label name is not visible in audit logs. If you want to search/view audit logs associated with this label, you can use the label ID. |
   | **Short name** | **Maximum length:** 10 characters, alphanumeric  Short version of the label name. The short name is used to refer to this custom label in data discovery and content explorer. **Note:** The short name is not visible in audit logs. If you want to search/view audit logs associated with this label, you can use the label ID. |
   | **Description** | **Maximum length:** 500 characters  Description of the information this label is detecting. This information is useful for other admins. |
   | **Conditions** | Add keywords and widget types you want to detect and add this label to upon detection on a Miro board. You must add at least one condition.  If you add only keywords and do not select any widget checkbox, Data discovery detects all boards that contain exact matches of the keywords you provided for all supported widgets. The current release supports the following board items for keyword detection: Sticky, Card, Jira card, Code block, Comments, Frame, Table, Connector/line, Shape, Text block, Kanban board, User Story map.  You can also select to detect only code blocks, Jira cards, Azure cards, or Prototyping screens, without adding keywords. Data discovery then detects all boards that contain those widgets.  If you add both keywords and widgets as conditions, both the keyword and widget criteria need to be met for Data Discovery to detect the board. This enables you to refine your search and target boards more precisely using custom labels.  **Examples:**  - If you want to narrow down the board detection to specifically detect product development-related boards, but not marketing-related boards, and the board must contain the project name *Enterprise* *Guard*, and you want to find only the boards that also contain a Jira card (as it is product-development related), you will configure this label to contain the keyword *Enterprise* *Guard* and select the Jira card checkbox. Data discovery then finds boards that contain the keyword Enterprise Guard and a Jira card. Data discovery also finds boards that contain Jira cards with the keyword Enterprise Guard in its title or description. If a board contains only the keyword *Enterprise* *Guard* but does not contain a Jira card, the board is not detected as it does not meet both conditions specified.  - If you want to detect all boards with the word *Enterprise* *Guard* on it for all supported widget types regardless of the widget types the board contains, in the **Add keywords** section, add the keyword **Enterprise** **Guard**. You do not need to add any widget type for this example.  - If you want to detect all boards with Jira cards regardless of any specific content, in the **Add widget type** section, select the **Jira card** checkbox. You do not need to add any keyword for this example.    **To add a keyword:**  1. Click **Add keywords**.  2. Enter or paste  keywords separated by commas. **Notes:**  - Keywords support alphanumeric and Unicode characters.  - You can add up to 100 keywords or phrases. - Data discovery detects exact matches for the keywords you provide, regardless of case sensitivity. - The current release supports the following board items for keyword detection: Sticky, Card, Jira card, Code block, Frame, Table, Connector/line, Shape, Text block, Kanban board, User Story map. Notes and comments are currently not included in data discovery scans. We are working on including notes and comments in upcoming feature enhancement releases.  **Example:** To identify and label boards containing the keywords *confidential* or *internal*, add the following keywords: *confidential, internal* (use a comma to separate each keyword). Data discovery then finds all boards that include either of these keywords.  **To add a widget type:**  1. Click **Add widget type**.  2. Select the checkbox for the widget type that you want to detect on Miro boards.  **Example:** If you want to detect and label boards that contain a Jira card, select the **Jira card** checkbox. |
5. Click **Next**.
6. Review the custom label details.

   If you want to update the custom label details, click the **Previous** button.

   If the custom label details are correct, click the **Update custom label** button.

   After you update the custom label, the scan starts automatically. Results matching the selected conditions will be available after a few minutes or hours, depending on the number of Miro boards in your organization.
