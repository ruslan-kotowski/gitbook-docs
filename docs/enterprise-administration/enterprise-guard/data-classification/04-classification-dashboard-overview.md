---
title: Classification dashboard overview
article_id: 26886219054354
sidebar_position: 4
created_at: '2025-05-22T11:26:15Z'
updated_at: '2025-08-18T09:36:23Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

The Classification dashboard provides a centralized view for administrators to track and manage the classification of boards across their organization. The dashboard provides a clear breakdown of classified and not yet classified boards, helping ensure comprehensive coverage and identify areas needing attention.

Administrators can also monitor the classification method used—whether manual, automatic, or unclassified—to understand how boards are being categorized. Additionally, the classification method history visualizes changes over time, offering insight into trends and the effectiveness of ongoing board classification.

:::note
Notes on metrics:

- All metrics in Enterprise Guard exclude boards of trashed teams and boards under legal hold.
- All classification metrics exclude templates and trashed boards.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Title** | **Description** | **Domain** | **Appears in Overview dashboard** | **Has historic metric** |
| Total number of boards which are classified | Number of boards that have a classification label assigned | Classification | ✅ | ❌ |
| Number of boards per classification | Number of Boards per classification label (label name) | Classification | ✅ | ❌ |
| Number of non-classified boards | Number of boards that have no classification label assigned | Classification | ✅ | ✅ |
| Number of manually classified boards | Number of boards that have manually assigned a classification label (read not by auto classification) | Classification | ❌ | ✅ |
| Number of automatically classified boards | Number of boards that have automatically assigned a classification label by auto-classification | Classification | ❌ | ✅ |

## Understand errors, empty states, and historical changes

Understanding how to interpret empty states and error messages is essential for accurately reading Enterprise Guard dashboard metrics.

### Understand behavior of historical data when settings change

If a feature, such as Classification, is disabled after data has been collected, historic metrics will still show values from the active period. For example, if you disable Classification in May and Classification was active in April with 20 boards classified:

- April values will continue to appear on the dashboard.
- The May graph will display **no data available**, as data collection has stopped.
