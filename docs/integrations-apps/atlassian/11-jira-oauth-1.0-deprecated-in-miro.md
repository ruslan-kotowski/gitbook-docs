---
title: Jira OAuth 1.0 deprecated in Miro
article_id: 28738797627538
sidebar_position: 13
created_at: '2025-08-13T12:11:22Z'
updated_at: '2026-03-20T14:10:12Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  roles: company_admin
  plans: starter, business, enterprise, education
  platforms: browser, desktop
---

Jira OAuth 1.0 authentication is deprecated from August 2025.

If your organization has already updated to Jira OAuth 2.0, you can ignore this article. No action is needed from your Company admin. You can verify with your [Company admin](#find-your-company-admin) that your organization is using OAuth 2.0.

:::warning
If your organization has not updated to OAuth 2.0, then your Jira integration with Miro, including Jira Cloud, Server, and Data Center, can be disrupted.
:::

Only Company admin(s) can upgrade teams in their organization.

In case of disruption, syncing between Miro and Jira stops until your organization updates to OAuth 2.0 authentication. Existing Jira cards remain on your Miro boards.

Disruption means that import is unavailable, and cards do not get updates, details cannot be loaded, and creating and updating a planner is unavailable.

To avoid disruption, Miro recommends that your Company admin(s) update to Jira OAuth 2.0 immediately.

:::tip
Admins can [Check your OAuth version](#check-your-oauth-version).
:::

## Why is OAuth 1.0 deprecated?

Atlassian has deprecated and no longer supports the OAuth 1.0 authentication protocol.

**More information:** See (External) [OAuth 1.0a for REST APIs (Deprecated)](https://developer.atlassian.com/cloud/jira/platform/jira-rest-api-oauth-authentication/).

## Check your OAuth version

As an Enterprise team admin, or a Starter or Business plan admin, you can check whether your team is using OAuth 1.0 or OAuth 2.0.

Follow these steps:

1. From your Miro dashboard, click your avatar in the top-right and select **Admin Console**.
2. Go to **Teams** > **[Team name]**.
3. Click **Apps**.
4. Find and click **Jira cards**.
5. Go to **Admin settings** > **Jira configuration**.
   The configuration indicates which OAuth version your team is using.
6. (Optional) Repeat steps 1-5 for other teams you want to verify.
7. Notify your Company admin(s) about any teams not using OAuth 2.0.

## Find your Company Admin

To identify your Company admin(s), follow these steps:

:::note
(Enterprise) If team privacy is enabled, non-Company admins are unable to view members lists.
:::

1. Go to **Team profile settings** in Miro.
2. Open the **Members** page.
3. Click **Additional Roles**.
4. Find users with the **Company Admin** role.

:::tip
To ensure your team upgrades to OAuth 2.0 and avoids possible disruption, share this article with your Company admin(s).
:::

## Upgrade to OAuth 2.0 for Company admins

As Company admin, you have the following resources to help you upgrade your organization to OAuth 2.0:

- [Connect to Jira Cloud using OAuth 2.0](https://help.miro.com/hc/articles/8588617184402)
- [Connect to Jira Data Center using OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
- [Connect teams in organization to default Jira settings](https://help.miro.com/hc/articles/26438407676434)

## Interim solution

If OAuth 2.0 isn't an option for your organization right now, Miro provides an [interim solution using OAuth 1.0](https://help.miro.com/hc/articles/27689156602514).

However, Miro recommends upgrading to OAuth 2.0 for the most secure and future-proof authentication method which follows Atlassian’s current standards.

## Additional help

If you or your Company admin have questions, contact [Miro Support](https://help.miro.com/hc/articles/360020185799).
