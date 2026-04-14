---
title: Jira cards in Tables and Timelines FAQ
article_id: 33772179950482
sidebar_position: 18
created_at: '2026-03-04T14:25:24Z'
updated_at: '2026-03-20T14:11:11Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  roles: team_member
  plans: (See [FAQ](#what-miro-licenses-support-jira-in-tables-and-timelines)) Business, Enterprise Advanced
  platforms: browser, desktop, mobile
---

## What Miro licenses support Jira in Tables and Timelines?

You must have a [Business + AI Workflows](https://help.miro.com/hc/en-us/articles/33274850111762) subscription, or an Enterprise subscription with an [Advanced](https://help.miro.com/hc/en-us/articles/33311996124306) license, to import Jira cards, convert data table rows into Jira items, and edit Jira items from a data table.

For Enterprise with a Standard license, Jira in data tables is ready only.

The legacy Business plan, and the Enterprise Full and Standard licenses, do not support Jira in Tables and Timelines.

## How do I import Jira issues to Tables and Timeline in Miro?

In Miro, drag and drop one or multiple Jira Cards directly onto a Table or Timeline.

## Which Table fields link to Jira?

From a Miro table, the following fields link to Jira:

- **System Jira fields**
  - Title
  - Description
  - End date (**Due Date** in Jira)
  - Assignee (Beta)
  - Status (Beta)
- **Custom Jira fields**
  - Start date
  - Estimate

## Which Table fields do not sync to Jira?

In a Miro table, click a cell. Fields that do not show a Jira logo are stored in Miro only and do not sync to Jira.

## Why can’t I edit a supported field?

The field may not be present on the edit screen in Jira.

To check, in Miro open the Jira card side-panel. If the field is not present in the side panel, then you must add the field to the edit screen in Jira.

## Why can't I edit a custom field?

If you are trying to edit a custom field, like **Start date** or **Estimate**, then there could be a mapping issue. If the **Start Date** or **Estimate** fields do not comply with Miro's mapping, then editing may be unavailable.

Miro applies the following checks to map these custom fields:

- **Start date**
  Fields named `Start Date`, `StartDate`, or `Target Start`.
- **Estimate**
  Fields named `Story Points`, `Story point estimate`, `Story Point`, `StoryPoints`, `StoryPoint`.

## Why does editing the Start Date or Estimate in Miro not work or update the wrong field in Jira?

Miro maps the **Start Date** and **Estimate** custom fields automatically. Your Jira configuration may include multiple custom fields that match Miro's mapping criteria, where only the first match is synced.

For example, a Jira ticket has both `Story points` and `Story point` fields for **Estimate**. Miro matches and syncs only `Story points` for the **Estimate** field. Changes to the **Estimate** field update `Story points` in Jira, but not `Story point`.

## Why can’t I import Jira cards from two Jira instances to a Table or Timeline?

Miro currently supports one Jira instance per Table or Timeline. When you import a Jira card, the Table or Timeline links to that specific Jira instance.

To import cards from another Jira instance, create a new, separate Table or Timeline.

## Why can’t I view or edit the Status and Assignee fields for my Jira records in a Table or Timeline?

**Status** and **Assignee** fields are currently available in beta. You can reach out to [Miro Support](https://help.miro.com/hc/articles/360020185799) to provide feedback.
