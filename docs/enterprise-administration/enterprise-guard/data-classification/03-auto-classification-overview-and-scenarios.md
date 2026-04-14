---
title: Auto-classification overview and scenarios
article_id: 15431302000914
sidebar_position: 3
created_at: '2023-11-29T16:42:42Z'
updated_at: '2025-11-25T15:39:41Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

To support you in protecting your sensitive content, Enterprise Guard includes the auto-classification feature—an automated data classification process, categorizing Miro boards based on the level of its sensitive content. Auto-classification represents a significant advancement in the way you manage and protect your sensitive data. Automating the classification process helps your organization maintain a higher level of data security, comply with regulatory requirements, and provide a better security admin experience. The transition from manual to automatic classification is a strategic move towards a more accurate, secure, and efficient data security framework.

## Understand auto-classification scenarios

### Prerequisites

To use the auto-classification feature, you must:

- [Enable data discovery](../../canvas-25-admin-features/data-discovery/13-activate-privacy-related-data-discovery.md).
- [Define classification levels](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md).

### Example Auto-classification and Guardrails configuration

You must [configure Auto-classification and Guardrails](https://help.miro.com/hc/articles/15853672236946) based on your security and governance requirements. The following table lists the configuration used for all example scenarios on this page and is intended only for explanatory purpose only.

|  |  |  |  |
| --- | --- | --- | --- |
| **Board classification** | **Sensitivity order** | **Auto-classification criteria** | **Guardrails** |
| PUBLIC | 1  (least sensitive) | None | None |
| INTERNAL (Default) | 2 | TELECOM | - Block public sharing |
| CONFIDENTIAL | 3 | GDPR  PCI DSS | - Block public sharing  - Block sharing with teams |
| RESTRICTED | 4 (most sensitive) | HIPAA  CREDENTIALS | - Block public sharing  - Block sharing with teams  - Block sharing with organization |

*Table 1: Example configuration intended for explanatory purpose only.*

## Manual update of board classification to override auto-classification

Only Board owners, co-owners, or editors of the board can update the board classification to override the auto-classification level. If the board owner, co-owners, or editors update the board classification to a less-sensitive classification level, they must select or provide a reason for the change, and this information is added in the audit logs.

### Manually update to a lower sensitive classification level

**Scenario**
Consider a scenario where John Smith is the owner of a board that was auto-classified as **Confidential**, which has the sensitivity order **3** per our configuration.

John takes a look at the information and decides to update the classification level to **Internal**, which has the sensitivity level **2**, a lower classification level compared to the board's auto-classification level of **Confidential**, level **3**.

:::note
Only board owners, co-owners, or editors of the board can manually update the classification level.
:::

**Result**

As John is the board owner, he is able to update the board classification to a lower sensitive classification level, **Internal**, level **2**. In this scenario, John is prompted for the reason why he wants to change the board classification level to a less sensitive classification level (Figure 1). John can select the reason and click **Update**.

The board classification level is updated and information about this update is added to the Audit logs.

### Manually update to a higher sensitive classification level

**Scenario**

Consider a scenario where John Smith is the owner of a board that was auto-classified as **Confidential**, which has the sensitivity order **3** per our configuration.

John takes a look at the information and decides to update the classification level to **Restricted**, which has the highest sensitivity level **4**, a higher classification level compared to the board's auto-classification level of **Confidential**, level **3**.

:::note
Only board owners, co-owners, or editors of the board can manually update the classification level.
:::

**Result**

As John is the board owner, he is able to update the board classification to a higher sensitive classification level.

The following table summarizes various scenarios and their results considering that the board was auto-classified at some point earlier and then a board owner, co-owner, or editor manually updates the board classification.

|  |  |  |
| --- | --- | --- |
| **Auto-classification level** | **Board owner action** | **New classification level** |
| CONFIDENTIAL | **Update to lower classification level**  John, the board owner manually updates the board classification to  **INTERNAL**, which has the sensitivity level 2, a lower classification level compared to the board's auto-classification level of CONFIDENTIAL, level 3. | As John is the board owner, he is able to update the board classification to a lower sensitive classification level, **INTERNAL**.  In this scenario, the board owner is prompted for the reason why he wants to change the board classification level to a less sensitive classification level. John can select the reason and click **Update**.  The board classification level is updated to **INTERNAL** and information about this update is added to the Audit logs. |
| CONFIDENTIAL | **Update to higher classification level**  John, the board owner, decides to update the board classification to **RESTRICTED**, which has the highest sensitivity level 4, a higher classification level compared to the board's auto-classification level of CONFIDENTIAL, level 3. | As John is the board owner, he is able to update the board classification to a higher sensitive classification level. |

*Table 2: Scenarios and resulting auto-classification levels*

## Auto-update of board classification

The data discovery cycle runs every hour If the board content changes, wherein either highly-sensitive data is added or removed, the boards that have these updates will be auto-classified once again, based on the board's updated content and the last non-auto classification level. The following sections provide example scenarios for auto-updates of the classification level.

### Highly-sensitive data removed from the board

After the next data discovery cycle is complete, the board classification is automatically updated to the applicable sensitivity level.

**Example scenario board content**

The board contains highly-sensitive data that contained information belonging to the following sensitivity labels: CREDENTIALS, HIPAA, GDPR, PCI DSS. Therefore, after the data discovery cycle is complete, auto-classification classified this board as **RESTRICTED**, level 4, which is the highest sensitive order based on our example auto-classification configuration. The following table describes the following information:

- **Last non-auto classification:** This is the last non-automatic classification of the board that could have either been done [manually](../../canvas-25-admin-features/data-classification/03-auto-classification-overview-and-scenarios.md#manual-update-of-board-classification-to-override-auto-classification), via a [default board classification](../../canvas-25-admin-features/data-security/02-data-classification.md), or the [update board classification](https://developers.miro.com/reference/enterprise-dataclassification-board-set)/[bulk update board classification](https://developers.miro.com/reference/enterprise-dataclassification-team-boards-bulk) APIs.

- **Auto-classification:** The classification level that auto-classification applied to the board after the data discovery cycle was completed.

- **Action taken:** The action taken, updates made to the board content, after auto-classification.

- **New classification:** The new classification considering the action taken and all other aspects, such as the board content and the last non-auto classification.

|  |  |  |  |
| --- | --- | --- | --- |
| **Last non-auto classification** | **Auto-classification** | **User action** | **New auto-classification level** |
| INTERNAL (via default board classification) | RESTRICTED | All sensitive data removed from the board | After the next data discovery cycle is complete, the board classification is automatically updated to **INTERNAL** level, as the board no longer contains any sensitive information, but the earlier non-auto classification was INTERNAL, which was classified via the default board classification. |
| CONFIDENTIAL | RESTRICTED | All sensitive data removed from the board | After the next data discovery cycle is complete, the board classification is automatically updated to **CONFIDENTIAL** level, sensitivity order 3, even if the board no longer contains any sensitive information because the earlier non-automatic classification level was CONFIDENTIAL, level 3. |
| UNCLASSIFIED | RESTRICTED | CREDENTIALS and HIPAA, which is RESTRICTED level, sensitivity order 4, content is removed from the board. | After the next data discovery cycle is complete, the board classification is automatically updated to **CONFIDENTIAL** level, sensitivity order 3, as: - the board no longer contains CREDENTIAL and HIPAA information, but the board still contains PCI DSS sensitive data, which maps to **CONFIDENTIAL** level. - the board was not classified before auto-classification. |
| RESTRICTED | RESTRICTED | CREDENTIALS and HIPAA, which is RESTRICTED level, sensitivity order 4, content is removed from the board. | After the next data discovery cycle is complete, the board remains in the  **RESTRICTED** level, sensitivity order 4, even if the board no longer contains any CREDENTIAL and HIPAA information because the earlier non-automatic classification level was RESTRICTED, level 4. |
| UNCLASSIFIED | RESTRICTED | All sensitive data removed from the board | After the next data discovery cycle is complete, the board classification is automatically updated to **UNCLASSIFIED** level, as the board no longer contains any sensitive information and the board was not classified before auto-classification. |

*Table 3: Scenarios and resulting auto-classification levels*

### Highly-sensitive data added to the board

After the next data discovery cycle is complete, the board classification is automatically updated to the applicable sensitivity level based on the highest level of sensitive data found.

|  |  |  |
| --- | --- | --- |
| **Last auto-classification level** | **User action** | **New auto-classification level** |
| PUBLIC | Collaborator added credit card number. | **CONFIDENTIAL** PCI DSS |
| INTERNAL | Collaborator added authentication token. | **RESTRICTED** Credentials |
| RESTRICTED | Collaborator added authentication token. | **RESTRICTED** Remains the same. |
| INTERNAL | Collaborator added Germany driver's license number. | **CONFIDENTIAL**  GDPR |
| CONFIDENTIAL | Collaborator added MAC address. | **RESTRICTED**  Credentials |

*Table 4: Scenarios and resulting auto-classification levels*
