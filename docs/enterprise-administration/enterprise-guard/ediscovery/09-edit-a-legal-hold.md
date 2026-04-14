---
title: Edit a legal hold
article_id: 27968005251090
sidebar_position: 9
created_at: '2025-07-09T17:31:49Z'
updated_at: '2025-11-25T15:52:48Z'
draft: false
---

Editing a legal hold allows eDiscovery Admins to adjust and refine ongoing legal preservation efforts as case requirements evolve. Whether new custodians are identified, additional Miro boards become relevant, or existing boards or users are no longer in scope, editing a legal hold ensures that the correct data remains preserved and defensible throughout the legal process.

Admins can update the legal hold’s name or description and add or remove users and boards as needed. This flexibility supports dynamic legal workflows and ensures that preservation stays precise, up to date, and aligned with the scope of the legal matter—maintaining compliance while avoiding unnecessary data retention.

When a legal hold is edited:

- Boards newly added to the hold will begin having their versions preserved from that point forward.
- Boards or users removed from the hold will stop being preserved, and their versions will no longer be preserved as part of that legal hold.
- Boards that remain under hold will continue to have all versions preserved, including any deletions that occur after the hold was applied.

This approach ensures organizations can respond to legal demands with accuracy and accountability as a case evolves.

To edit a legal hold, perform the following steps:

:::note
You must have the [eDiscovery Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) to perform this task. To request for the eDiscovery Admin role, contact your Company Admin.
:::

1. Go to your Miro settings.
2. On the left pane, under **Enterprise Guard**, click **eDiscovery**.
3. On the **eDiscovery** page, click the **Cases** tab.
4. Click the case within which you want to edit a legal hold.
   The list of legal holds within the case appears.
5. Click the three dots on the row of the legal hold that you want to edit, and then click **Edit legal hold**.
6. On the **Edit legal hold** page, enter or select the appropriate information for each field. The following table lists each field and its description.

   |  |  |
   | --- | --- |
   | **Field** | **Description** |
   | Legal hold name  **(required)** | Name of the legal hold.  Max length: 60 characters. |
   | Criteria  **(required)** | Type of content included for this legal hold. This release supports only all content. |
   | **Users who own, co-own, accessed, modified, or created content**  **(required)** | Add the users you want to put on legal hold. Click the field to search by name or email. You can have up to 200 users per legal hold, including users added in legal hold updates.  **Notes:**  - When a user under legal hold opens, modifies, or interacts with a board in any way (renaming or adding content), that board is flagged and preserved. For example, if the board’s name is changed or content is updated, it will be automatically placed on legal hold. Additionally, board ownership and board creation are put on hold.  - When a legal hold is edited, it applies to boards that custodians created, owned, or co-owned at the time of the hold. Additionally, any boards custodians access and modify after the hold is in place are also included. Historical board access and update details are not available in this release.  - Boards newly added to the hold will begin having their versions preserved from the time you save the legal hold updates in step 9.  - Boards or users removed from the hold will stop being preserved, and their versions will no longer be retained as part of that legal hold.  - Boards that remain under hold will continue to have all versions retained, including any deletions that occur after the hold was applied. |
7. Click **Next**. The **Review impact** page appears.
8. Review the impact of this legal hold creation, such as:
   - The number of boards that remain under hold, will be released from hold, and added to hold.
   - The users that owned, co-owned, accessed, modified or created the boards.
   - The criteria for the hold.
   - The list of boards that remain under hold.

   **Notes:**
   - Boards under hold can still be accessed and edited but all version will be preserved. If content is deleted, it will still be available within the hold. The number of content items under hold might increase based on future user actions.

   - When a user under legal hold opens, modifies, or interacts with a board in any way (renaming or adding content), that board is flagged and preserved. For example, if the board’s name is changed or content is updated, it will be automatically placed on legal hold. Additionally, board ownership and board creation are put on hold.

   - When a legal hold is created, it applies to boards that custodians created, owned, or co-owned at the time of the hold. Additionally, any boards custodians access and modify after the hold is in place are also included. Historical board access and update details are not available in this release.
9. After you review the impact of the legal hold you are creating, click **Save legal hold**.
   The case page appears displaying the updated legal hold, such as the name of the legal hold, the type of content affected by the legal hold, the number of users in this legal hold, the date when the legal hold was created, the status of the legal hold, and the number of boards that are held on legal hold.
