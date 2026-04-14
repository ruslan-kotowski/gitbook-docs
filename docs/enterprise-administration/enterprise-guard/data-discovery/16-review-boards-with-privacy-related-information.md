---
title: Review boards with privacy-related information
article_id: 15431051181458
sidebar_position: 16
created_at: '2023-11-29T16:31:14Z'
updated_at: '2025-11-25T15:39:35Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

The Data Discovery dashboard allows [Sensitive Content Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) to review occurrences of privacy-related data detected by data discovery and validate results.

:::note
To review boards with privacy-related data, you must have the [Sensitive Content Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Sensitive Content Admin role, contact your Company Admin.
:::

To review a board with privacy-related data, perform the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard**, click **Data discovery**.
3. On the **Data discovery** **Overview** page, scroll to the section below the metrics, and then click the board count for the category of boards you want to review.
   A new page appears with the list of boards and their information.
4. Click the board you want to review.
   A slide-out panel appears on the right of the screen.
5. The slide-out panel allows you to perform the following actions:
   - **Show or hide** **privacy-related** **information:** By default. privacy-related information is blacked out. If you want to view privacy-related information, click the **Show sensitive information** toggle to turn it on.
   When privacy-related information is visible, you can hide the privacy-related information by clicking the **Show sensitive information** toggle to turn it off.

   - **Filter** **privacy-related** **information based on the data category:** To view privacy-related information that belong to a specific label, click the **Privacy-related information** tab, and then click the appropriate sensitivity label below the tab.

   **- Suppress false positive matches:** In the process of privacy-related data discovery, you might encounter situations where the system generates matches that, while technically accurate, may not be relevant or regarded as sensitive data based on various security policies and specific needs of an organization. Suppressing a match that does not pose a security or privacy risk becomes crucial for tailoring the data discovery process to an organization’s specific data security and privacy requirements.

   There may also be times when the system incorrectly flags data on your boards as likely sensitive (a false positive). Various factors contribute to these occurrences, including the proximity of related terms or the formatting of privacy-related data. You can also suppress false positive matches.

   When you suppress a match, the updates happen in real-time. The board classification and the applied guardrails are also updated per the Auto-classification and Intelligent Guardrails configuration.

   To suppress a false positive match, click the ellipsis beside the privacy-related data match that you want to suppress, and then select **Hide match**. Note that the updates happen in real-time. The board classification and the applied guardrails are also updated per the Auto-classification and Intelligent Guardrails configuration.
6. Click on the next board that you want to work with in the Content Explorer result list and perform the necessary actions, or close the slide-out panel by clicking the **Close** button at the top-right of the panel.
