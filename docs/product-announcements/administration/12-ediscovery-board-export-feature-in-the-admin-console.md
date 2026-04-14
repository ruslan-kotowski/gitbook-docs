---
title: eDiscovery Board Export Feature in the Admin Console
article_id: 26529264912146
sidebar_position: 16
created_at: '2025-05-06T17:01:06Z'
updated_at: '2025-05-26T08:55:18Z'
draft: false
---

Enterprise Guard Admins can now use the Admin console to support eDiscovery workflows more effectively. They can:

- Export all boards under a legal hold (selective export not supported).
- View a list of export jobs (completed, ongoing, and planned) within each eDiscovery case.
- See export status for individual boards in a job.
- Download exported boards individually, available for 14 days after export.

**Export limits and behavior:**

- Each export job can include up to **1000 boards**. Jobs will not start if a legal hold includes more than 1000 boards.
- A maximum of **100 export jobs** can be active in the organization.
- Up to **5 jobs** are processed in parallel (unchanged).

**API limits (Board Export API):**

- Up to **100 export jobs** for Guard orgs and **10 jobs** for Enterprise orgs.
- Export job size limit: **1000 boards**.

These updates help streamline legal hold processes while ensuring transparency and control over board export activities.
