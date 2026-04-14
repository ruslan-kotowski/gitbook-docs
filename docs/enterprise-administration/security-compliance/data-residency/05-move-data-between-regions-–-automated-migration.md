---
title: Move data between regions – Automated migration
article_id: 24866660560402
sidebar_position: 5
created_at: '2025-02-24T08:47:08Z'
updated_at: '2025-10-29T14:40:39Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  roles: company_admin
  plans: enterprise
  platforms: browser, desktop
---

:::note
Automated migration is a paid engagement with professional services. For a quote, reach out to your dedicated Miro contact.
:::

This article explains automated data migration. To learn more about other options for moving data between regions, see [Move data between regions](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Data included in an automated cross-region migration

The following list shows what data an automated cross-region migration includes:

- Boards, board content, and board sharing settings
- Content hierarchy, including Teams, Spaces, and Spaces sections
- Organization, Team, and board settings
- Users, user profiles, and user settings, including guests
- Audit logs, data classification, and content security settings

## Prepare a for cross-region data migration

To prepare for a cross-region data migration, follow these steps:

1. To ensure that you can manage all users in your domain, verify all domains that you own with DNS verification.
2. Turn on the **Block own subscriptions** domain control policy, which ensures that users do not accidentally create free Miro subscriptions in your old region.
3. Consolidate teams and/or organizations into a single organization with a single subscription.
4. Audit which integrations your organization uses and needs in the new region, then plan a timeline to re-configure each integration in your new region.

## How a cross-region data migration works, and how long it lasts

A cross-region migration includes the following five steps:

- **Preparation**
  Typically 4-8 weeks. The Company Admin, supported by Miro, prepares their org for migration, schedules migration downtime, and communicates to end users
- **Migration**
  Typically <8 hours of downtime. The organization and its data is migrated to the new region.

  > ✏️ The Miro team coordinates with you to select the migration date. If the migration is unsucccessful for any reason, access to your source region is restored, and Miro coordinates a new migration date with you to retry the migration.
- **Verification and configuration**
  Typically 2-3 weeks. Admin must re-configure certain integrations, like SSO, in the new region. Admin and end users verify that their boards and data have landed in new region as expected.
- **Training**
  Typically 2-3 weeks. End users are trained on where to access their new Miro org.
- **Compliance**
  Within 120 days of migration date – Miro verifies that the organization’s data has been removed from the source region.

## What to do after a cross-region data migration

After a cross-region data migration, ensure you do the following:

- Immediately reconfigure SSO, if applicable, for the new regional subdomains. For example, au.miro.com.

  > ✏️ Your users are unable to sign in to the new region until SSO is reconfigured on the IDP side.
- Reconfigure SCIM for the new regional subdomains. For example, au.miro.com.
- Verify that **Block own subscriptions** in domain control settings is turned on.
- Validate your other domain control settings.
- Re-install and configure relevant apps and integrations.

## Automated cross-region data migrations FAQ

**What is a cross-region data migration?**

Cross-region data migrations automate the movement of customer data from one geographical region to another. The end result of a cross-region migration is that your in-scope Miro customer data will be stored and processed in the new region

**How does it work and how long does it take?**

See [How a cross-region data migration works, and how long it lasts](#how-a-cross-region-data-migration-works-and-how-long-it-lasts).

**Who is eligible, and who is not?**

To automate a cross-region migration you must be an Enterprise customer. However, an Enterprise customer using Enterprise Guard and EKM is ineligible. For more information, reach out to your Miro contact person.

**What data is included in an automated cross-region data migration?**

To learn what data an automated cross-region migration includes, see [Data included in an automated cross-region migration](#data-included-in-an-automated-cross-region-migration).

**What data is not included in an automated cross-region data migration?**

An automated cross-region migration does not include the following data:

- Apps and integrations, including SSO and SCIM, which must be reconfigured for the new region
- Talktracks
- In-app notifications are cleared

**Is there additional cost?**

Yes. An automated cross-region migration is a paid engagement with Miro Services. For more information, reach out to your Miro contact person.

**How does Miro ensure that my organization's data is removed from the source region?**

To remove your data from the source region after a cross-region migration, Miro adheres to the following protocol:

- Data remains in the source region for 30 days, which ensures that a reliable backup is available should there be an issue with the migration.
- After 30 days, Miro begins to delete your data from the source region.
- After a maximum of 120 days after the initial migration date, Miro has deleted all data from the source region.

**What do users see during a cross-region migration?**

To learn about the user experience during a migration, see [User experience while moving data between regions](../../canvas-25-admin-features/data-residency/04-user-experience-while-moving-data-between-regions.md).

**What happens if the migration is unsuccessful?**

If the migration is unsuccessful for any reason, Miro restores access to your source region, and coordinates a new date to retry the migration.
