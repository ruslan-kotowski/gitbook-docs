---
title: Review boards with business-sensitive and custom-business sensitive information
  (Beta)
article_id: 24090123693586
sidebar_position: 14
created_at: '2025-01-21T15:10:56Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

The Content Explorer allows [Sensitive Content Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) to review occurrences of business-sensitive or custom business-sensitive data matches.

:::note
- To review boards with business-sensitive or custom business-sensitive data matches, you must have the [Sensitive Content Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Sensitive Content Admin role, contact your Company Admin.
- Business-sensitive data matches are tagged as either CUSTOMER, TECH, or STRATEGY and the results are listed at the top of the result list.

- Custom business-sensitive data matches are tagged with the appropriate custom labels applicable.
:::

To review a board with business-sensitive or custom business-sensitive data matches, perform the following steps:

1. If you are on the **Content Explorer** page, skip to step 2.
   If you are not on the **Content Explorer** page:
   a. Go to your [Miro settings](https://miro.com/app/settings).
   b. On the left pane, under **Enterprise Guard**, click **Content explorer**.
   c. Click **Data discovery**.
2. On the **Content explorer/Data discovery** page, click the board that you want to review.
   A slide-out panel appears on the right of the screen.
3. The slide-out panel allows you to perform the following actions:

   - For custom business-sensitive data matches only: **Show or hide** **business-sensitive information**
   By default, custom business-sensitive information is blacked out. If you want to view custom business-sensitive data information, click the **Show sensitive information** toggle to turn it on.
   When custom business-sensitive data is visible, you can hide the data by clicking the **Show sensitive information** toggle to turn it off.

   > ✏️ - Business-sensitive data matches are tagged as either CUSTOMER, TECH, or STRATEGY and the results are listed at the top of the result list.
   > - Custom business-sensitive data matches are tagged with the appropriate custom labels applicable.

   - For both business-sensitive data and custom business-sensitive data matches: **Filter information based on business-sensitive data category**
   To view business-sensitive data that belong to a specific category, click the **Business-sensitive information** tab, and then click the appropriate filter button below the tab.

   -For business-sensitive data matches only: **Suppress false positive matches**
   In the process of business-sensitive data discovery, you might encounter situations where the system generates matches that, while technically accurate, may not be relevant or regarded as sensitive data based on various security policies and specific needs of an organization. Suppressing a match that does not pose a security or business risk becomes crucial for tailoring the data discovery process to an organization’s specific data security and business requirements.

   There may also be times when the system incorrectly flags data on your boards as likely sensitive (a false positive). Various factors contribute to these occurrences, including the proximity of related terms or the formatting of business-related data. You can also suppress false positive matches.

   When you suppress a match, the updates happen in real-time. The board classification and the applied guardrails are also updated per the Auto-classification and Intelligent Guardrails configuration.

   To suppress a false positive match, click the ellipsis beside the business-sensitive data match that you want to suppress, and then select **Hide match**. Note that the updates happen in real-time. The board classification and the applied guardrails are also updated per the Auto-classification and Intelligent Guardrails configuration.
4. Click on the next board that you want to work with in the Content Explorer result list and perform the necessary actions, or close the slide-out panel by clicking the **Close** button at the top-right of the panel.
