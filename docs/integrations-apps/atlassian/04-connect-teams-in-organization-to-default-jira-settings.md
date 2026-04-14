---
title: Connect teams in organization to default Jira settings
article_id: 26438407676434
sidebar_position: 6
created_at: '2025-05-02T12:25:08Z'
updated_at: '2026-03-20T14:10:12Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  roles: company_admin
  plans: enterprise
  platforms: browser, desktop
---

Company admins can bulk connect teams in their organization to use global Jira settings, which overrides settings specified at the team level.

## Prerequisites

- Ensure you have the Company admin role in Miro.
- Ensure you have a default connection to a [Connect to Jira Data Center using OAuth 2.0](https://help.miro.com/hc/articles/25753304280466).

## Connect teams to default Jira settings

1. From your Miro dashboard, select your avatar on the top-right and go to **Admin Console** | **Settings**.
2. On the left sidebar, go to **Apps and integrations ![icon-plug.svg](images/26513504419218_icon-plug.svg)** > **Apps** > **Manage apps** tab.
3. Ensure that **Allow only apps from the list below** is enabled.
4. Under the **App** column, for **Jira Cards** select **Settings**.
5. Under **Add teams to default instance**, select each team that you want to connect, or click **Select all**.

   > ✏️ The list only shows teams not using global organization settings.
6. Click **Add &lt;number of teams&gt; to default**.

   > ✏️ Users not already using the global Jira instance in your organization are migrated, and must reauthenticate.

   > ✏️ Users migrated from another Jira instance get prompted to reauthenticate the first time they attempt a Jira-related action in Miro.

## FAQ

**Will teams remain using the global Jira connection indefinitely?**

No. You can change Jira settings for a given team later.

**Which teams should use the global Jira connection?**

Using organization settings is generally preferred as it requires less administration from you. If any of your team connections share the same settings as the organization, we advise onboarding teams to the default organization settings for this reason.
