---
title: Add retention policy
article_id: 19205113739282
sidebar_position: 10
created_at: '2024-05-28T18:00:55Z'
updated_at: '2025-12-08T16:05:16Z'
draft: false
---

:::note
To add retention policies, you must have the [Data Governance Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Data Governance Admin role, contact your Company Admin.
:::

To add a retention policy, perform the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Content lifecycle**.
3. Click the **Retention** tab.
   The **Retention policies** page appears.
4. Click **Add retention policy**.
   The **Define criteria** page appears.
5. Add or select the appropriate information for each field. The following table lists each field and its description.

   |  |  |
   | --- | --- |
   | **Field** | **Description** |
   | **Name**  **(required)** | Name of the retention policy.  Max length: 60 characters. |
   | **Description**  **(optional)** | Description of this retention policy.  Max length: 300 characters. |
   | **Retention period**  **(required)** | Prevent boards from being permanently deleted for a specific period based on one of the following criteria: **Last access**, **Last modified**, or **Created at**. Select a number, choose **Months** or **Years**, and then choose which event the retention period is calculated from.  If you specify the retention period in months, you must select a retention period between 1 and 120 months.  If you specify the retention period in years, you must select a retention period between 1 and 10 years. |
   | **Scope**  **(required)** | Select the scope for this retention policy. The scope indicates the boards for which this retention policy is applicable. You can set the scope of a retention policy for all boards in an organization or for specific board classification levels.  **Set the retention policy for all boards in the organization** If you want to set the scope of the retention policy for all boards in the organization, in the **Scope** list, select **All boards in organization**.  **Set the retention policy for one or more teams in the organization** If you want to set the scope of the retention policy for one of more teams in the organization, perform the following steps:  1. In the **Scope** list, select **Team**. 2. Click the Enter team box and select each team for which you want to apply the retention policy. A check mark appears beside the team you selected to associate with the retention policy.   ✏️ - You can select multiple teams for a retention policy. However, any given team can only be associated with one retention policy at a time.  - You can select any team, including deleted teams, as a scope when setting the retention policy.   - A team that is selected as the scope for a retention policy cannot be permanently deleted until the team is removed from the scope.  **Set the retention policy for a board classification level**  ✏️ To set the scope of the retention policy to a specific board classification level, you must ensure that the Data Classification feature is turned on. Once a retention policy uses a board classification level, you cannot turn off the Data Classification feature. For more information, see the documentation on [Data Classification](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  If you want to set the scope of the retention policy for a specific board classification level, perform the following steps:  1. In the **Scope** list, select **Classification**. 2. Click the list beside the **Classification** list and then select the classification levels for which you want to apply the retention policy. You can also search for the Classification levels, and then select the Classification levels.  A check mark appears beside the classification levels you selected to associate with the retention policy.  ✏️ **Notes:** - You can select multiple classification levels at once. - You cannot set the same classification level for different retention policies. If a specific classification level is already associated with a retention policy, the classification level appears grayed out.  - Once a retention policy uses a board classification level, you cannot turn off the Data Classification feature.  -  Once a classification level is associated with a retention policy, you cannot delete that specific classification level. - When a board is governed by both all boards in organization scope and classification scope retention policies, the policy with the longer retention period is applicable. |
6. Click **Next**.
   The **Review impact page** appears.
7. Review the impact of the retention policy. The review impact page provides the following information:
   - **Summary:** retention policy configuration, such as the policy name, retention period, and the scope.
   - **Policy impact:** number of boards that will be governed by this policy. The retention policy is also applicable to trashed boards and they are included in the review impact calculation.

   > ✏️ When a board is governed by both a time-based and a classification-based retention policy, the policy with the longer retention period is applicable.
8. To save the configuration and apply the retention policy, click **Publish**.

:::note
Creating, updating, or deleting a policy triggers the retention policies process, which can take up 24 hours to complete. However, updating the name or description of a policy happens immediately as these actions do not trigger the retention policies process.
:::

#
