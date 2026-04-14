---
title: Two-factor authentication (2FA)
article_id: 27356474050834
sidebar_position: 1
created_at: '2025-06-12T12:01:03Z'
updated_at: '2025-06-24T08:19:34Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  roles: team_admin, company_admin
  plans: starter, business, education, enterprise
  platforms: browser, desktop, mobile
---

Two-factor authentication (2FA) adds an extra layer of security to online accounts by requiring users to provide two unique verification methods before accessing their accounts.

Miro admins can enable 2FA for their teams, and reset 2FA for team members. Users have the option to trust a device for 30 days.

:::note
This article explains 2FA for Starter, Business, and Education plans. To learn about 2FA for Enterprise, see [Two-factor authentication (2FA) (admin guide).](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)
:::

## Enable two-factor authentication (2FA)

For Starter and Education plans, ensure that you have the Team admin role.

For a Business plan, ensure that you have the Company admin role.

Follow these steps:

1. From your Miro dashboard, click your avatar in the top-right and select **Admin Console**.
2. (Starter) Go to **Security** > **Permissions**.
   (Education) Go to **Permissions**.
   (Business) Go to **Security** > **Authentication**.
3. Under **Two-factor authentication (2FA)**, toggle **Require two-factor authentication when signing in** to the on position.

## Two-factor authentication (2FA) setup for users

For teams that have 2FA enabled, users must authenticate using an authenticator app, in addition to their email and password.

To learn how to setup 2FA as a user, see [Two-factor authentication (2FA) – user guide](02-two-factor-authentication-2fa-–-user-guide.md).

## Trusted devices

A user logging in to Miro with 2FA can choose to trust their device.

When using the trusted device to log in, the user will only be prompted to authenticate with their first factor, skipping their second factor, because the device is trusted.

![](images/27358547112978_image.png)

*Trusted device for 2FA is enabled by default.*

At sign in, **Trust this device for 30 days** is selected by default, which the user can optionally deselect.

:::note
The trust device period can only be modified on an Enterprise plan. For more information, see [Two-factor authentication (2FA) (admin guide)](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md).
:::

To untrust a device that was accidentally trusted, a user can sign themselves out of everywhere. Go to **Profile**, under **Profile settings**, click **Sign out of everywhere**.

## Reset two-factor authentication (2FA)

If a user loses access to their second factor, then they can request that their admin reset their 2FA.

To reset 2FA for users on Starter and Education plans, ensure that you have the Team admin role.

To reset 2FA for users on a Business plan, ensure that you have the Company admin role.

Follow these steps:

1. From your Miro dashboard, click your avatar in the top-right and select **Admin Console**.
2. Go to **Users** > **All users**.
3. Locate the user, then select the three dots (**...**) at the end of the row.
4. Click **Reset two-factor authentication**.
   The user receives reset instructions by email.
