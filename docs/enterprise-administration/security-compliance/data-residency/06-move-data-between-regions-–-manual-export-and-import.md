---
title: Move data between regions – Manual export and import
article_id: 24778387087122
sidebar_position: 6
created_at: '2025-02-20T09:07:00Z'
updated_at: '2025-11-25T15:49:48Z'
draft: false
availability:
  roles: board_owner, Board co-owners, Content admins, company_admin
  plans: enterprise
  platforms: browser, desktop
---

This article describes the manual export and import method for moving data between regions. To learn more about your options for moving data between regions, including automated migration, see [Move data between regions](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Prepare for a manual export and import to a new region

As Company admin, the following best practices help you prepare for a manual move to a new region:

- To initiate a new organization in your target region, reach out to your dedicate Miro contact.
- To ensure that you can manage all users in your domain, verify all domains that you own with DNS verification.
- Turn on the **Block own subscriptions** domain control policy, which ensures that users do not accidentally create free Miro subscriptions in your old region.
- Consolidate teams and/or organizations into a single organization with a single subscription.
- Audit which integrations your organization uses and needs in the new region, then plan a timeline to reconfigure each integration in your new region.
- Audit all settings that your organization uses currently, then plan a timeline to reconfigure each setting that you require in your new region.

## Manually export and import data to a new region

Miro provisions a new Enterprise organization in the target region. Users must export their boards as board backups from the source region, and then import their backup to the target region.

**More information:** See [How to save board backup](../../../using-miro/import-and-export/export/05-how-to-save-board-backup.md).

Only users with the following permissions can manually export and import content:

- Board owner
- Board co-owner
- Company admin
- Content admin

:::note
All board sharing is lost. Users must restore their sharing permissions after uploading their backup in the target region.
:::

To begin their manual import of content, users can log in to their new regional URL, namely one of the following:

- (Australia) [au.miro.com](https://au.miro.com/)
- (United States) [us.miro.com](https://us.miro.com/)

:::note
As a user, before you log in for the first time, verify whether your organization uses Single sign-on (SSO). If you use SSO, then wait for your Company admin to reconfigure SSO settings for your new region.
:::

## What to do after a manual export and import

After a cross-region data migration, ensure you do the following:

- Immediately reconfigure SSO, if applicable, for the new regional subdomains. For example, au.miro.com.
  > ✏️ Your users are unable to sign in to the new region until SSO is reconfigured on the IDP side.
- Reconfigure SCIM for the new regional subdomains. For example, au.miro.com.
- Verify that **Block own subscriptions** in domain control settings is turned on.
- Validate all other organization, domain control, and team settings.
- Re-install and configure each Enterprise app and integration, like SIEM, SAM, eDiscovery, Smarsh, and Okta.
- Invite users to the organization in the new region.

## Manual export and import data to new region FAQ

**How does a manual move to a new region work?**

Admins effectively re-setting up the org and all its teams, team settings, and users again, and end users manually downloading board backups from the old org and uploading them into the new org.

**Who is eligible, and who is not?**

Enterprise customers are eligible to move their data to another region. For more information, reach out to your Miro contact person.

**What data is included in a manual move?**

Only boards moved by users. For more information, see [Manually export and import data to a new region](#manually-export-and-import-data-to-a-new-region).

**Is there additional cost?**

No. Miro can provision a new organization in Australia or the United States per the standard Enterprise contract.

**How long does a manual move take?**

The duration of a manual move depends on how much time users need to export their saved boards as backup, and import their backup content to the target region.

**How does Miro ensure that my organization's data is removed from the source region?**

Notify Miro support after you complete your manual export and import to your new region, including reconfiguration, and all users have imported their backups to the target region. Miro support will then delete your organization and all data from the source region.
