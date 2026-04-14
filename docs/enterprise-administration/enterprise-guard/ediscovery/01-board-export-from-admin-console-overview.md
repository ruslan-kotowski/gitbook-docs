---
title: Board Export from Admin console overview
article_id: 26259747401362
sidebar_position: 1
created_at: '2025-04-24T14:18:00Z'
updated_at: '2025-11-25T15:50:56Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

eDiscovery Admins can now directly export boards under legal hold from the Admin console.
This capability enables eDiscovery Admins to:

- Initiate board exports from the Admin console.
- Monitor export job progress in real time via the **Exports** tab within each case.
- Filter export jobs by status and creator and see which boards are included.
- Get a full content log for each board exported.
- View a list of exported boards and their metadata (classification, owner, export state).
- Download exported boards individually, directly from the Admin console.
- Complete the export workflow without relying on APIs or integrations.
- Cancel queued export jobs, or jobs in progress.

:::note
To export boards and manage export job operations, you must have the [eDiscovery Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Sensitive Content Admin role, contact your Company Admin.
:::

## **Board export capabilities**

- Each **export job** can contain up to **1,000 boards**.
- **Export limits** by plan:

  - **Enterprise Guard:** Up to **100** active export jobs.
  - **Enterprise:** Up to **10** active export jobs.
- **Parallel processing limits**:

  - **Enterprise Guard**: Up to **5** export jobs processed in parallel.
  - **Enterprise**: **1** export job processed at a time.
- **Content logs with export jobs:** Exports can optionally include a full content log for each exported board.
- **Filters for export jobs**: Filter export jobs and see which boards are included.
- **Cancel ongoing and queued export jobs**: Manage export bandwidth efficiently.
  > ✏️ When you cancel an export, all boards in progress will complete and be available for download. Any boards not started will not be exported.

- **Download Access**: Results are downloadable for **14 days.**
- **Admin Console Scope**: Only exports initiated via the Admin Console appear in the **Exports** tab. API-based export jobs are not included in the Admin console list.
