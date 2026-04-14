---
title: Relations in Timeline
article_id: 32042959413010
sidebar_position: 8
created_at: '2025-12-22T18:29:47Z'
updated_at: '2026-03-13T12:26:15Z'
draft: true
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: dependencies
availability:
  plans: Desktop, mobile, interactive displays
---

## Dependencies

> **Which plans:** Business, Enterprise

This relation field type allows you to map dependencies between records in your Timeline using connection lines. This helps you track project relationships and understand how work items depend on each other.

### Add dependencies between records

1. Hover over a timeline bar until you see connection points.
2. Click and drag from one bar to another to create a dependency line.
3. The dependency will automatically appear in both the Timeline and Table views.

:::note
Records can have multiple blocking and blocked by relationships. Dependencies sync across all synced Timelines, ensuring consistency across your views and boards.
:::

:::note
Dependencies will automatically create corresponding Blocked by and Blocking fields in your Table view.
:::

:::warning
Current limitations (Beta):

- Dependencies are not yet supported for Jira-synced records or other third-party integrations.
- Visual indicators for dependencies are not yet shown on synced cards.
- Automatic date adjustments based on dependencies are not yet available.
:::

## Nesting (BETA)

> **Which plans:** Business, Enterprise

The nesting relation allows you to create hierarchy between records in your Timeline.

### Create hierarchy between records

1. Click on timeline bar and click **Add sub-record** from the context menu.
2. Nesting will turn on by default. To turn off, go to **View Settings** in the Timeline header.
3. You can also drag and drop records to create hierarchies when Nesting is turned on.

Use the **chevron** next to Parent records to reveal or hide Child records.

Hierarchical relations can be viewed and edited in the side panel. You can switch to **Tables** layout to view your data in more detail.

:::note
Hierarchies in Timeline will also be synced with Tables. Nesting will automatically create corresponding Parent and Child fields in your Table view.
:::

:::note
Easily turn off the nesting visualization by toggling off Nesting in the **View Settings** Tables and Timeline header.
:::

:::warning
If you delete a parent record, all sub-records will be deleted too. You can reverse this using the Undo function.
:::

:::warning
**Current limitations (Beta):**

- Four-level maximum for hierarchy.
- Nesting is not yet supported for Jira-synced records or other third-party integrations.
- Visual indicators for Nesting are not yet shown on synced cards.
:::
