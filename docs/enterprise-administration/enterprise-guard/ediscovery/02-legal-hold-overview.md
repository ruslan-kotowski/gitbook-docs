---
title: Legal Hold overview
article_id: 21922434361618
sidebar_position: 2
created_at: '2024-10-11T12:20:34Z'
updated_at: '2025-11-25T15:48:02Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

The Legal Hold feature is designed to support compliance and eDiscovery processes by preserving boards that are subject to investigation or relevant to ongoing legal cases.

[eDiscovery Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) can prevent the permanent deletion of content by creating legal holds based on specific users and their actions in Miro. This functionality is essential for ensuring that relevant information is retained and secure during legal proceedings.

For example, when a user who is subject to a legal hold interacts with a board, that board is automatically placed on hold to prevent permanent deletion.

Additionally, all versions of the board are also preserved ensuring that the board's content is retained for legal purposes.

:::note
You must have the [eDiscovery Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) to perform Legal Hold tasks. To request for the eDiscovery Admin role, contact your Company Admin.
:::

## Key Benefits of Legal Hold

- **Preservation of Information:** Legal Hold ensures that all relevant data is preserved, preventing permanent deletion. This is crucial for compliance and legal investigations, as it guarantees that data presented in legal cases remains accurate and unaltered.
- **Compliance with Legal Requirements:** Legal Hold supports organizations in adhering to legal and regulatory obligations by ensuring that necessary information is retained and available when needed, helping to avoid penalties or legal challenges
- **Risk Mitigation:** By safeguarding important data, Legal Hold reduces the risk of data loss that could result in significant legal or financial consequences.
- **Audit and Monitoring:** Each time a legal hold is created or modified, an audit log is generated, providing full visibility and traceability. All audit logs in an organization are preserved indefinitely when at least one legal hold is active. This ensures accountability and transparency in managing legal holds.

## How Legal Hold Works

- **User or Board Interactions:** When a user under legal hold opens, modifies, or interacts with a board in any way (renaming or adding content), that board is flagged and preserved. For example, if the board’s name is changed or content is updated, it will be automatically placed on legal hold. Additionally, board ownership and board creation are put on hold.

  When a legal hold is created, it applies to boards that custodians created, owned, or co-owned at the time of the hold. Additionally, any boards custodians access and modify after the hold is in place are also included. Historical board access and update details are not available in this release.
- **End User Actions and Board Deletion:** While end users can delete boards, these boards are preserved if a legal hold is in place. They remain inaccessible to the end user but are retained for legal and administrative purposes.
- **Administrative Control:** eDiscovery admins can create and delete legal holds through the eDiscovery section in the settings. Legal holds can be applied to all boards a user has created, owned, co-owned, edited, or accessed. To manage multiple legal holds, admins can first create a case under which these holds are grouped.
- **Team Deletion:** If a board under legal hold exists within a team, that team cannot be permanently deleted until the hold is released. This prevents unintended data loss, ensuring that all relevant content is preserved. In cases where a team is deleted but contains a board under legal hold, the team will be marked as preserved on the deleted teams page, and its permanent deletion will be disabled until the legal hold is released.
- **Administrator and eDiscovery Perspective:** While end users cannot access or recover a deleted board that is on hold, administrators and eDiscovery teams can still interact with it. The board is preserved until the legal case is closed, at which point the legal hold can be lifted, and the board can be permanently deleted.
- **Board Export Functionality:** Boards under legal hold can still be exported using the board export functionality, allowing for easy collection of relevant data for legal cases.
- **Moving boards:** Boards under legal hold cannot be moved outside the organization. If a board is under legal hold, external teams are automatically filtered out from the list of teams to which the board can be moved.
