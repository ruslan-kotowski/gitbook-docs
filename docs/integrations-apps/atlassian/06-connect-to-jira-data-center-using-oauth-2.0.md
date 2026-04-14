---
title: Connect to Jira Data Center using OAuth 2.0
article_id: 25753304280466
sidebar_position: 8
created_at: '2025-04-02T09:38:30Z'
updated_at: '2026-03-20T14:10:12Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  roles: Company admins with Jira system admin permissions
  plans: enterprise
  platforms: browser, desktop
---

:::note
Connecting to Jira Data Center using OAuth 2.0 is only enabled at the organization level.
:::

## Prerequisites

- Ensure you have the following permissions:
  - Jira system admin permissions
  - Miro Company admin role
- Create an OAuth 2.0 application link on Jira Data Center. To learn how, see (External) [Atlassian Jira applications Support](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Create%20an%20incoming%20link%20using%20application%20links).
  - Use the following redirect URL when prompted:
    https://integrations.miro.com/api/external-auth/oauth2/callback
  - To use automatic webhooks, ensure you select **Admin** for your scope.

## Connect Miro to Jira Data Center using OAuth 2.0

1. From your Miro dashboard, select your avatar in the top-right and go to (Enterprise) **Admin console**, or(Starter and Business) **Settings**.
2. On the left sidebar, go to **Apps and integrations ![icon-plug.svg](images/26513589065106_icon-plug.svg)** > **Apps** > **Manage apps** tab.
3. Ensure that **Allow only apps from the list below** is enabled.
4. Under the **App** column, for **Jira Cards** select **Settings.**
5. Select **Add new connection**.
6. Under **Jira setup**, select **Jira Data Center**.
7. Under **Authentication method**, select **OAuth 2.0**.
8. For **Jira URL**, enter your Jira instance URL.
9. (Optional) To make this connection the default connection for all teams in your organization, click **Make Default**.
10. Enter the Jira **Client ID**.
    **More information**: See (External) [Configure an incoming link](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
11. Enter the Jira **Client secret**.
    **More information**: See (External) [Configure an incoming link](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
12. Choose your scope.
    To use automatic webhooks, choose **Admin** or **System admin**.
13. (Optional) To get real-time updates from Jira in Miro, tick **Create webhook automatically**.
    > ✏️ Optionally,  you can manually add the webhook later.
14. Select **Connect**.
    > ✏️ The first time a user attempts a Jira-related action, they are prompted to authenticate. They do not need to re-authenticate.

## What next?

To view and manage your connected Jira instances, go to **Admin Console** | **Settings** > **Apps and integrations ![icon-plug.svg](images/26513589065106_icon-plug.svg)** > **Manage apps**. Then under the **App** column, for **Jira Cards** select **Settings**.

To learn how to connect your teams to the default Jira instance, see [Connect teams in organization to default Jira settings.](https://help.miro.com/hc/articles/26438407676434)

## FAQ

**Does choosing Admin for scope require that all users have admin privileges in Jira?**

No. The Admin scope means that admin is the highest scope a user can have in Miro. The scope is anyway limited per user, depending on their permissions in Jira.

**Can I connect Jira Data Center with OAuth 2.0 at the team level?**

No. Only at the organization level.
