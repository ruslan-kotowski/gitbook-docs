---
title: Content Lifecycle dashboard overview
article_id: 26894063726482
sidebar_position: 2
created_at: '2025-05-22T16:02:58Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
---

The Content Lifecycle dashboard provides a centralized view for administrators to monitor and manage the full lifecycle of boards—from creation to deletion—while aligning with organizational data retention policies. It provides visibility into the current lifecycle stage of each board, helping ensure appropriate content handling.

Administrators can also track boards governed by retention and disposition policies, and view historical trends for policy application. The dashboard includes a disposition forecast, allowing proactive planning for upcoming automated lifecycle actions. This enables consistent, policy-driven content governance across the organization.

:::note
All metrics in Enterprise Guard exclude boards of trashed teams and boards under legal hold.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Title** | **Description** | **Domain** | **Appears in Overview dashboard** | **Has historic metric** |
| Total number of boards | Total number of boards in all lifecycle states (active, trash, retained) | Content Lifecycle Management | ✅ | ❌ |
| Number of active boards Note this is NOT board activity but boards that are in the active lifecycle state | Total number of boards in active lifecycle state | Content Lifecycle Management | ✅ | ✅ |
| Number of trashed boards | Total number of boards in trashed lifecycle state | Content Lifecycle Management | ✅ | ✅ |
| Number of retained boards | Total number of boards in retained lifecycle state | Content Lifecycle Management | ✅ | ✅ |
| Number of boards under retention | Total number of boards that have at least one non expired retention policy assigned. | Content Lifecycle Management | ❌ | ✅ |
| Number of boards under disposition | Total number of boards that have at least one non expired disposition policy assigned. | Content Lifecycle Management | ❌ | ❌ |
| Number of boards following a retention grouped by policies policy | Number of boards in any lifecycle state that have at least one retention policy assigned per policy | Content Lifecycle Management | ✅ | ❌ |
| Disposition number of boards following a disposition policy grouped by policies | Number of boards in any lifecycle state that have at least one disposition policy assigned per policy | Content Lifecycle Management | ✅ | ❌ |
| Number of boards created this day/week/month | Number of boards created this week | Content Lifecycle Management | ❌ | ✅ |
| Number of boards deleted (trashed) this day/week/month | Number of boards deleted (trashed) this week | Content Lifecycle Management | ❌ | ✅ |
| Number of boards under disposition policies grouped by effective disposition policy date per month |  | Content Lifecycle Management | ❌ | ❌ |

## Understand errors, empty states, and historical changes

Understanding how to interpret empty states and error messages is essential for accurately reading Enterprise Guard dashboard metrics.

### Understand behavior of historical data when settings change

If Data Discovery is disabled after data has been collected, historic metrics will still show values from the active period. For example, if you disable Data Discovery in May and Data Discovery was active in April:

- April values will continue to appear on the dashboard.
- The May graph will display **no data available**, as data collection has stopped.

###
