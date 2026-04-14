---
title: Data discovery dashboard overview
article_id: 26806897106834
sidebar_position: 2
created_at: '2025-05-19T11:10:19Z'
updated_at: '2025-11-25T15:51:28Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

The Data Discovery dashboard provides a centralized view of sensitive information detected across your organization's boards. It enables admins to monitor, classify, and manage data risks by identifying privacy-related or business-sensitive content. The Data Discovery dashboard includes the following metrics:

:::note
All metrics in Enterprise Guard exclude boards of trashed teams and boards under legal hold.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Title** | **Description** | **Domain** | **Appears in Overview dashboard** | **Has historic metric** |
| Number of sensitive boards | Number of boards that have at least one built in label, keyword label, or privacy label assigned | Data Discovery | ✅ | ❌ |
| Number of boards which has business sensitive items | Number of boards that have at least one built in label, or keyword label assigned | Data Discovery | ✅ | ✅ |
| Number of boards which has privacy related sensitive items | Number of boards that have at least one privacy label assigned | Data Discovery | ✅ | ✅ |
| Number of boards that have a label assigned per label | For each individual label in the three categories (built in, keyword or privacy) count the number of boards that have that label assigned. | Data Discovery | ❌ | ❌ |
| Count of enabled privacy-related labels | Count of enabled privacy-related labels | Data Discovery | ❌ | ❌ |
| Count of enabled keyword labels | Count of enabled keyword labels | Data Discovery | ❌ | ❌ |
| Count of enabled business sensitive labels | Count of enabled business sensitive labels | Data Discovery | ❌ | ❌ |

## Understand errors, empty states, and historical changes

Understanding how to interpret empty states and error messages is essential for accurately reading Enterprise Guard dashboard metrics.

### Understand behavior of historical data when settings change

If Data Discovery is disabled after data has been collected, historic metrics will still show values from the active period. For example, if you disable Data Discovery in May and Data Discovery was active in April:

- April values will continue to appear on the dashboard.
- The May graph will display **no data available**, as data collection has stopped.

## View data discovery results

The Data Discovery cycle runs at least once every hour and scans all board updates for privacy-related, business-sensitive related, or custom business-sensitive related information based on your data discovery configuration. This includes boards that were already scanned in the previous data discovery cycle.

The data discovery results appear below the metrics charts. You can view information such as the label name, status, type, classification, number of boards, and so on.

For more information on reviewing boards with privacy-related documentation, [see this article](../../canvas-25-admin-features/data-discovery/16-review-boards-with-privacy-related-information.md).

For more information on reviewing boards with business-sensitive and custom-business sensitive data information, [see this article](../../canvas-25-admin-features/data-discovery/14-review-boards-with-business-sensitive-and-custom-business-sensitive-information-beta.md).

For more information on reviewing boards with custom business-sensitive labels, [see this article](../../canvas-25-admin-features/data-discovery/15-review-custom-business-sensitive-labels-and-data-discovery-results.md).

:::note
- To view Data Discovery results, you must have the [Sensitive Content Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Sensitive Content Admin role, contact your Company Admin.

- While we are continuously working with our technology partner and customers to improve the sensitive content detection system, we cannot guarantee that it will find and flag 100% of the sensitive data on your boards. Our sensitive content detection system uses patterns and other criteria to determine the probability of a match. There may be times when the system incorrectly flags data on your boards as likely sensitive (a false positive) or fails to flag data as sensitive (a false negative). Various factors contribute to these occurrences, including the proximity of related terms or the formatting of sensitive data.

For more information on how you can suppress false positive matches, see [Suppress a sensitive content match](../../canvas-25-admin-features/data-discovery/11-suppress-a-sensitive-content-match.md).
:::

##

##
