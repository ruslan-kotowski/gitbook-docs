---
title: Delete retention policy
article_id: 19205219887762
sidebar_position: 12
created_at: '2024-05-28T18:02:52Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Deleting a retention policy releases retained boards associated with the retention policy. These boards can then be permanently deleted without constraints.

:::note
To delete retention policies, you must have the [Data Governance Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Data Governance Admin role, contact your Company Admin.
:::

To delete a retention policy, perform the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Content lifecycle**.
3. Click the **Retention** tab.
4. On the **Retention** **policies** page, click the retention policy that you want to delete.
   The page displaying information related to the policy appears.
5. Click **Delete** at the top-right of the page.
6. Review the impact of the retention policy deletion. The review impact page provides the following information:
   - **Summary:** retention policy configuration, such as the policy name, retention period, and the scope.
   - **Policy impact:** number of boards that will be released from retention and can be permanently deleted without constraints. The retention policy is also applicable to trashed boards and they are included in the review impact calculation.
7. To delete the retention policy, click **Delete policy**.

:::note
Creating, updating, or deleting a policy triggers the retention policies process, which can take up 24 hours to complete. However, updating the name or description of a policy happens immediately as these actions do not trigger the retention policies process.
:::
