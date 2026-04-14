---
title: Board Export API overview
article_id: 17774560667794
sidebar_position: 13
created_at: '2024-03-19T12:52:09Z'
updated_at: '2025-07-09T17:32:16Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

[eDiscovery APIs](https://developers.miro.com/reference/enterprise-create-board-export) allow customers on the Enterprise Plan to export board data from Miro to be reviewed manually or ingested into purpose-built tools for legal, compliance, and security purposes.

The Board export API provides a ZIP file with a snapshot of the board data at the time the job runs, including export of the board content in a specified format SVG, PDF or HTML, a JSON file with a record of all comments, a JSON file with a list of all users who viewed or modified the board, video recordings of TalkTrack webcam footage associated with the board, if applicable, and a JSON with Board matadata. For large boards, the export in PDF format produces multiple PDF files depicting the complete board.

The asynchronous API design includes endpoints for retrieving information about a board export job, such as the status.

:::note
If you are on the Enterprise plan, you can only have one board export job running at a time. As an Enterprise Guard customer, you can run up to five board export jobs simultaneously with a significantly higher export speed.
:::

## Use cases

Some of the common eDiscovery use cases include:

- **eDiscovery (electronic discovery):** the process of identifying, collecting, preserving,  and reviewing electronically stored information for use in a legal matter.
- **Information archive:** a practice in which organizations maintain data outside the original system for long-term storage and record-keeping purposes. The content and metadata help customers index and search the archive and proactively monitor for compliance concerns.
