---
title: User experience while moving data between regions
article_id: 25075857856658
sidebar_position: 4
created_at: '2025-03-04T08:51:38Z'
updated_at: '2025-05-09T08:47:03Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  roles: all_users
  plans: enterprise
  platforms: browser, desktop, mobile
---

This article describes the user experience during a cross-region data migration, for both [automated](../../canvas-25-admin-features/data-residency/05-move-data-between-regions-–-automated-migration.md) and [manual export and import](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md) migrations.

## User experience during automated migration (BETA)

The following sections describe what to expect before, during, and after an automated movement of data between regions.

### Before automated migration

Two weeks before migration, all users in your Enterprise organization receive the following notifications:

- **In-product banner**
  Displays the migration date and expected duration in the local timezone
- **Email notification**
  Outlines the upcoming scheduled maintenance for all users in your Enterprise organization

:::note
If you are a member of multiple Miro accounts, then your other accounts remain accessible during migration.
:::

### During automated migration

An automated migration requires approximately 8 hours of downtime.

During an automated migration, you are unable to access your Enterprise organization data, including boards, teams, and settings.

The Miro dashboard shows a notification that says a data migration for your organization is in progress. During the migration process, you will not have access to organization boards, teams, or settings.

:::tip
If you are a member of multiple organizations, then you can switch to another organization from your dashboard and continue using Miro.
:::

### After automated migration

When the migration successfully completes, you receive a confirmation email. A message appears on your Miro dashboard that confirms the successful migration.

If the migration is unsuccessful, then you receive an email notification. You can continue using Miro in the EU region, signing in from [miro.com](https://miro.com).

### Board redirects after automated migration

Any board that you have bookmarked in your previous region automatically redirects to your new region, and uses an updated URL.

## User experience during manual export and import

Users must manually export board backups from their source region, and import their backups to the target region.

**More information:** See [Move data between regions – Manual export and import](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md).

## Cross-region collaboration

Users at Miro are regional. To collaborate with users in organizations outside your region, you must have a user profile in each region respectively.

For example, if you are an EU-region user and want to collaborate with users in an AU-region organization, then you must create a seprate user profile at [au.miro.com](https://au.miro.com/).
