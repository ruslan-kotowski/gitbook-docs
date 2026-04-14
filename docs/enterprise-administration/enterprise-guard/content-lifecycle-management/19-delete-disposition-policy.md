---
title: Delete disposition policy
article_id: 19551053395090
sidebar_position: 19
created_at: '2024-06-14T19:52:35Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Deleting a disposition policy will remove all its associated disposition dates for boards. As a result, boards that were linked to this policy will no longer be automatically moved to the Trash.

:::note
To delete disposition policies, you must have the [Data Governance Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Data Governance Admin role, contact your Company Admin.
:::

To delete a disposition policy, perform the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Content lifecycle**.
3. On the **Content lifecycle page,** click **Disposition**.
   The **Disposition policies** page appears.
4. On the **Disposition policies** page, click the disposition policy that you want to edit.
   The page displaying information related to the policy appears.
5. Click **Delete** at the top-right of the page.
6. Review the impact of the disposition policy deletion. The review impact page provides the following information:
   - **Summary:** disposition policy configuration, such as the policy name, disposition period, and the scope.
   - **Policy impact:** number of boards that will be governed by this policy.
7. To delete the disposition policy, click **Delete policy**.

:::note
Creating, updating, or deleting a policy triggers the disposition policies process, which can take up 24 hours to complete. However, updating the name or description of a policy happens immediately as these actions do not trigger the disposition policies process.
:::
