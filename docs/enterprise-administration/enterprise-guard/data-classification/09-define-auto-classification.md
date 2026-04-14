---
title: Define Auto-classification
article_id: 16494707596050
sidebar_position: 9
created_at: '2024-01-19T19:01:08Z'
updated_at: '2025-11-25T15:40:35Z'
draft: false
---

To support you in protecting your sensitive content, Enterprise Guard includes the auto-classification feature—an automated data classification process, categorizing Miro boards based on the level of its sensitive content. Auto-classification represents a significant advancement in the way you manage and protect your sensitive data. Automating the classification process helps your organization maintain a higher level of data security, comply with regulatory requirements, and provide a better security admin experience. The transition from manual to automatic classification is a strategic move towards a more accurate, secure, and efficient data security framework.

For more information on auto-classification and example scenarios, see [Auto-classification overview](../../canvas-25-admin-features/data-classification/03-auto-classification-overview-and-scenarios.md).

## Define auto-classification

This is the second step of the auto-classification and guardrails configuration flow. In this step of the flow, you will configure the auto-classification sensitivity label applicable for each classification level. The board classification is automatically applied to all new boards and existing boards matching the defined criteria. This is done after you review the impact and decide to publish updates.

## Prerequisites

- [You must enable data discovery](../../canvas-25-admin-features/data-discovery/13-activate-privacy-related-data-discovery.md).
- You must complete the first step of the auto-classification and guardrails flow, [1: Define classification levels](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md).
- You must know the sensitivity labels that you want to assign to each classification level based on your security and governance requirements.
- You must have the [Sensitive Content Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Sensitive Content Admin role, contact your Company Admin.

## Assign sensitivity labels for auto-classification

To assign sensitivity labels to a classification level, perform the following steps:

1. On the **Define auto-classification** page, click the **Edit** icon of the classification level for which you want to assign the sensitivity labels. For example, if you want to assign the auto-classification sensitivity labels for the **CONFIDENTIAL** classification level, click the Edit icon on the row of the **CONFIDENTIAL** classification level.
2. Select the checkbox for each sensitivity label that you want to assign to this classification level. For example, if you want to auto-classify all boards that contain the GDPR-related sensitive data, select the **GDPR General Data Protection Regulation** checkbox. You can assign one or more sensitivity labels per classification label.
3. Click **Done**.
   The board classification is automatically applied to all new boards and existing boards matching the defined criteria. This is done after you review the impact and decide to publish updates.
4. When you are done with assigning sensitivity labels for various classification levels, proceed to [Complete auto-classification configuration](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md#complete-auto-classification-configuration).

## Complete auto-classification configuration

After you finish assigning sensitivity labels for auto-classification, click **Next**. Your configuration is saved, but it will only take effect after you click **Publish** on the [**Review impact**](https://help.miro.com/hc/articles/16494764223378) page.

You can then proceed with either of the following next steps:

- [Define guardrails](../../canvas-25-admin-features/data-classification/05-define-guardrails.md). This is optional. If you want to define guardrails a later point in time, click **Next**.
- [Review impact](https://help.miro.com/hc/articles/16494764223378). This the last step of the workflow and it is mandatory.
