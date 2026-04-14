---
title: Add a legal hold to a case
article_id: 22120471564946
sidebar_position: 8
created_at: '2024-10-21T23:29:24Z'
updated_at: '2025-11-25T16:22:33Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Creating a legal hold is a critical process for [eDiscovery Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) when litigation or an investigation is expected. Legal holds ensure that relevant Miro boards are preserved and protected from alteration, deletion, or removal. This is essential for maintaining compliance with legal and regulatory requirements, preventing the loss or modification of critical data, and safeguarding key evidence throughout the duration of the legal matter. A legal hold allows admins to lock down data, ensuring that all relevant Miro boards are available for review whenever necessary.

Creating a legal hold involves identifying the relevant users and Miro boards associated with a case and applying the hold to prevent any modifications. Admins can manage multiple holds within a case, ensuring that all necessary data is grouped and preserved in an organized manner. This process helps maintain data integrity and accountability, ensuring that the organization is fully compliant and prepared for the legal process.

Miro boards under legal hold can still be accessed and edited, but all versions are preserved. If content is deleted, it will still be available within the legal hold. The number of content items under hold might increase based on future user actions. After a board is placed on legal hold, all the versions of the board are retained indefinitely, until the legal hold is released.

To create a legal hold, perform the following steps:

:::note
You must have the [eDiscovery Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) to perform this task. To request for the eDiscovery Admin role, contact your Company Admin.
:::

1. Go to your Miro settings.
2. On the left pane, under **Enterprise Guard**, click **eDiscovery**.
3. On the **eDiscovery** page, click the **Cases** tab.
4. On the **Create case** page, click the case within which you want to add a legal hold.
5. Click **Add legal hold**.
6. On the **Add legal hold** page, enter or select the appropriate information for each field. The following table lists each field and its description.

   |  |  |
   | --- | --- |
   | **Field** | **Description** |
   | Legal hold name  **(required)** | Name of the legal hold.  Max length: 60 characters. |
   | Criteria  **(required)** | Type of content included for this legal hold. This release supports only all content. |
   | **Users who own, co-own, accessed, modified, or created content**  **(required)** | Add the users you want to put on legal hold. Click the field to search by name or email. You can add up to 200 users at once.    **Notes:**  - When a user under legal hold opens, modifies, or interacts with a board in any way (renaming or adding content), that board is flagged and preserved. For example, if the board’s name is changed or content is updated, it will be automatically placed on legal hold. Additionally, board ownership and board creation are put on hold.  - When a legal hold is created, it applies to boards that custodians created, owned, or co-owned at the time of the hold. Additionally, any boards custodians access and modify after the hold is in place are also included. Historical board access and update details are not available in this release. |
7. Click **Next**. The **Review impact** page appears.
8. Review the impact of this legal hold creation, such as the number of existing boards that will be held and the users that owned, co-owned, accessed, modified or created the boards.

   **Notes:**
   - Boards under hold can still be accessed and edited but all version will be preserved. If content is deleted, it will still be available within the hold. The number of content items under hold might increase based on future user actions.

   - When a user under legal hold opens, modifies, or interacts with a board in any way (renaming or adding content), that board is flagged and preserved. For example, if the board’s name is changed or content is updated, it will be automatically placed on legal hold. Additionally, board ownership and board creation are put on hold.

   - When a legal hold is created, it applies to boards that custodians created, owned, or co-owned at the time of the hold. Additionally, any boards custodians access and modify after the hold is in place are also included. Historical board access and update details are not available in this release.
9. After you review the impact of the legal hold you are creating, click **Add legal hold**.
   The case page appears displaying the legal hold it contains and the information about each legal hold, such as the name of the legal hold, the type of content affected by the legal hold, the number of users in this legal hold, the date when the legal hold was created, the status of the legal hold, and the number of boards that are held on legal hold.
