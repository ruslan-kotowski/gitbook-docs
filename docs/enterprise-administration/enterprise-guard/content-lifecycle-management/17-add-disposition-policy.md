---
title: Add disposition policy
article_id: 19551031552018
sidebar_position: 17
created_at: '2024-06-14T19:49:31Z'
updated_at: '2025-12-08T16:13:30Z'
draft: false
---

:::note
To add disposition policies, you must have the [Data Governance Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Data Governance Admin role, contact your Company Admin.
:::

To add a disposition policy, perform the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Content lifecycle**.
3. Click the **Disposition** tab.
   The **Disposition policies** page appears.
4. Click **Add disposition policy**.
5. Enter or select the appropriate information for each field. The following table lists each field and its description.

   |  |  |
   | --- | --- |
   | **Field** | **Description** |
   | **Name**  **(required)** | Name of the disposition policy.  Max length: 60 characters. |
   | **Description**  **(optional)** | Description of this disposition policy.  Max length: 300 characters. |
   | **Disposition period**  **(required)** | Specify when boards are automatically moved to Trash. Choose a number, select **Months** or **Years**, and then choose whether the period is calculated from the board’s **last modified** date or **last access** date.  If you specify the disposition period in Months, you must select a disposition period between 1 and 120 months.  If you specify the disposition period in Years, you must select a disposition period between 1 and 10 years.  For example, if you want boards to be moved to Trash when they haven’t been modified for a year, you can select 1 year and choose **Last modified**. |
   | **Scope**  **(required)** | Select the scope for this disposition policy. The scope indicates the boards for which this disposition policy is applicable. You can set the scope of a disposition policy for all boards in an organization or for specific board classification levels.  **Set the disposition policy for all boards in the organization** If you want to set the scope of the disposition policy for all boards in the organization, in the **Scope** list, select **All boards in organization**.  **Set the disposition policy for one or more teams in the organization** If you want to set the scope of the disposition policy for one of more teams in the organization, perform the following steps:  1. In the **Scope** list, select **Team**. 2. Click the **Enter team** box and select each team for which you want to apply the disposition policy. A check mark appears beside the team you selected to associate with the disposition policy.   ✏️ - You can select multiple teams for a disposition policy. However, any given team can only be associated with one disposition policy at a time.  - You can select any team, including deleted teams, as a scope when setting the disposition policy.   - A team that is selected as the scope for a disposition policy cannot be permanently deleted until the team is removed from the scope.  **Set the disposition policy for a board classification level**  ✏️ To set the scope of the disposition policy to a specific board classification level, you must ensure that the Data Classification feature is turned on. Once a disposition policy uses a board classification level, you cannot turn off the Data Classification feature. For more information, see the documentation on [Data Classification](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  If you want to set the scope of the disposition policy for a specific board classification level, perform the following steps:  1. In the **Scope** list, select **Classification**. 2. Click the list beside the **Classification** list and then select the classification levels for which you want to apply the disposition policy. You can also search for the Classification levels, and then select the Classification levels.  A check mark appears beside the classification levels you selected to associate with the disposition policy.  ✏️ **Notes:** - You can select multiple classification levels at once. - You cannot set the same classification level for different disposition policies. If a specific classification level is already associated with a disposition policy, the classification level appears grayed out.  - Once a disposition policy uses a board classification level, you cannot turn off the Data Classification feature.  -  Once a classification level is associated with a disposition policy, you cannot delete that specific classification level. - When a board is governed by both all boards in organization scope and classification scope disposition policies, the policy with the longer disposition period is applicable. |
6. Click **Next**.
   The **Review impact page** appears.
7. Review the impact of the disposition policy. The review impact page provides the following information:
   - **Summary:** disposition policy configuration, such as the policy name, disposition period, and the scope.
   - **Policy impact:** number of boards that will be governed by this policy.
8. To save the configuration and apply the disposition policy, click **Publish**.
   The **Turn on disposition notification** dialog box appears.
9. **Disposition notifications** allow users to receive advance alerts before a board is automatically moved to the Trash due to inactivity. These alerts help users take action if they want to retain their content.

   If you want to enable disposition notifications:

   a. Click **Notify**.

   b. Configure how many days in advance the notification should be sent — any value between **1 and 30 days**.

   If enabling notifications would result in **some boards being immediately moved to Trash** (because they are already past the threshold), you’ll be asked whether to notify users about those specific boards. You can choose:

   - **Yes** – to notify board owners and co-owners even if the board is being moved to Trash right away.

   - **No** – to move the boards without sending a notification for this immediate action.

   Once enabled, users with boards in scope of any disposition policy with notifications turned on will:

   - Receive a notification in their Miro **notification feed** during the configured inspection window.

   - Be able to open the board directly from the notification.

   - See a **banner** on the board warning of the upcoming auto-trash, with an option to **Keep board** if they wish to retain it.

:::note
Creating, updating, or deleting a policy triggers the disposition policies process, which can take up 24 hours to complete. However, updating the name or description of a policy happens immediately as these actions do not trigger the disposition policies process.
:::

#
