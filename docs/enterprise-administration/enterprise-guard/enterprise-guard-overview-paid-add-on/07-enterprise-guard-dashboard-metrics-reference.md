---
title: Enterprise Guard dashboard metrics reference
article_id: 26718144750610
sidebar_position: 7
created_at: '2025-05-15T00:17:54Z'
updated_at: '2026-03-17T08:39:20Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

:::note
Notes on metrics:

- All metrics in Enterprise Guard exclude boards of trashed teams.
- All classification metrics exclude templates and trashed boards.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Title** | **Description** | **Domain** | **Appears in Overview dashboard** | **Has historic metric** |
| Total number of boards which are classified | Number of boards that have a classification label assigned | Classification | ✅ | ❌ |
| Number of boards per classification | Number of Boards per classification label (label name) | Classification | ✅ | ❌ |
| Number of non-classified boards | Number of boards that have no classification label assigned | Classification | ✅ | ✅ |
| Number of manually classified boards | Number of boards that have a manually assigned  classification label (not by auto classification) | Classification | ❌ | ✅ |
| Number of automatically classified boards | Number of boards that have an automatically assigned  classification label by auto-classification | Classification | ❌ | ✅ |
| Number of sensitive boards | Number of boards that have at least one built in label, keyword label, or privacy label assigned | Data Discovery | ✅ | ❌ |
| Number of boards which has business sensitive items | Number of boards that have at least one built in label, or keyword label assigned | Data Discovery | ✅ | ✅ |
| Number of boards which has privacy related sensitive items | Number of boards that have at least one privacy label assigned | Data Discovery | ✅ | ✅ |
| Number of boards that have a label assigned per label | Number of boards for  each label (built-in, keyword, or privacy) | Data Discovery | ❌ | ❌ |
| Count of enabled privacy-related labels | Number of enabled privacy-related labels | Data Discovery | ❌ | ❌ |
| Count of enabled keyword labels | Number of enabled keyword labels | Data Discovery | ❌ | ❌ |
| Count of enabled business sensitive labels | Number of enabled business sensitive labels | Data Discovery | ❌ | ❌ |
| Total number of boards | Total number of boards in all lifecycle states (active, trash, retained) | Content Lifecycle Management | ✅ | ❌ |
| Number of active boards Note this is NOT board activity but boards that are in the active lifecycle state | Total number of boards in active lifecycle state | Content Lifecycle Management | ✅ | ✅ |
| Number of trashed boards | Total number of boards in trashed lifecycle state | Content Lifecycle Management | ✅ | ✅ |
| Number of retained boards | Total number of boards in retained lifecycle state | Content Lifecycle Management | ✅ | ✅ |
| Number of boards under retention | Total number of boards that have at least one non-expired retention policy assigned | Content Lifecycle Management | ❌ | ✅ |
| Number of boards under disposition | Total number of boards that have at least one non-expired disposition policy assigned | Content Lifecycle Management | ❌ | ❌ |
| Number of boards following a retention grouped by policies policy | Number of boards in any lifecycle state that have at least one retention policy assigned | Content Lifecycle Management | ✅ | ❌ |
| Disposition number of boards following a disposition policy grouped by policies | Number of boards in any lifecycle state that have at least one disposition policy assigned | Content Lifecycle Management | ✅ | ❌ |
| Number of boards created this day/week/month | Number of boards created this week | Content Lifecycle Management | ❌ | ✅ |
| Number of boards deleted (trashed) this day/week/month | Number of boards deleted (trashed) this week | Content Lifecycle Management | ❌ | ✅ |
| Number of boards under disposition policies grouped by effective disposition policy date per month |  | Content Lifecycle Management | ❌ | ❌ |
| Number of cases | Total number of cases | eDiscovery | ✅ | ❌ |
| Number of legal holds | Total number of legal holds | eDiscovery | ✅ | ❌ |
| Number of legal holds for a specific case | Total number of legal holds for a specific case | eDiscovery | ❌ | ❌ |
| Number of boards under legal hold | Total number of boards that are under hold across all legal holds | eDiscovery | ❌ | ❌ |
| Users under legal hold and total number of their boards | Lists users under legal hold and the total number of their boards | eDiscovery | ❌ | ❌ |
