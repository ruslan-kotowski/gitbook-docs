---
title: Connect to Jira using OAuth 1.0 (Updated)
article_id: 27689156602514
sidebar_position: 12
created_at: '2025-06-27T13:18:15Z'
updated_at: '2026-03-20T14:10:12Z'
draft: false
availability:
  roles: company_admin, team_admin
  plans: starter, business, enterprise, education
  platforms: browser, desktop
---

Organizations that are not ready to migrate to OAuth 2.0 can use the following procedure to connect Miro to Jira using OAuth 1.0.

Atlassian has [deprecated OAuth 1.0](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively), and the method provided in this article is an interim solution. To avoid issues, and to align with best practices for security and compatibility, Miro strongly recommends that you migrate to OAuth 2.0 as soon as possible.

:::note
The previous OAuth 1.0 authentication method [is deprecated](https://help.miro.com/hc/articles/360019501754-Set-up-and-disable-Jira-Cards-OAuth-1-0) and will be removed on July 31, 2025.
:::

This article also explains using one Jira instance for several Miro teams, and how to disable Jira Cards at the organization and team level.

## Prerequisites

- Ensure you have the following permissions:
  - (Business, Enterprise) Miro Company admin
    (Starter, Education) Miro Team admin
  - Jira system admin

    > ✏️ To complete the procedure, you must be able to create an application link in Jira.
- In Jira, remove any existing application links to Miro.

## Procedure

To connect to Jira using OAuth1.0, follow these steps:

1. From your Miro dashboard, select your avatar on the top-right and click **Admin Console**.
2. On the left sidebar, go to **Apps and integrations** > **Apps** > **Manage apps** tab.
3. Ensure that **Allow only apps from the list below** is enabled.
4. In the **App** column, for **Jira Cards** select **Settings**.
5. In the **Default settings** tab, select **Add new connection**.
6. Under **Jira setup**, select either **Jira Cloud** or **Jira Data Center**.
7. Under **Authentication method**, select **OAuth 1.0x (Updated)**.
8. Under **Jira URL**, enter your Jira instance URL.
9. (Optional) To make this connection the default connection for all teams in your organization, tick **Make Default**.
10. Under **Setup instructions**, verify that you have the following properties:
    - URL
    - Consumer key
    - Consumer name
    - Public key
11. In Jira, create an application link.
    1. (Cloud) Go to **Settings** > **Products** > **Application Links**.
       (Data Center) In Jira admin settings go to **Products** > **Application Links**.
    2. Click **Create link**.
    3. (Cloud) For **Application type**, select **Direct application**.
       (Data Center) For **Application type**, select **Atlassian product**.
    4. For **Application URL**, paste the URL from Miro Setup instructions. See step 10.
    5. Click **Continue**.
    6. For **Application name**, name your application.

       > **⚠️** Do not enter data into any other field. You will provide Miro data in a following step.
    7. Tick **Create incoming link**.
    8. Click **Continue**.
    9. Copy and paste your Consumer key, Consumer name, and Public key from Miro Setup instructions. See step 10.
    10. Click **Continue**.
        You have created your application link.
12. In Miro, click **Connect**.
    You have connected Miro to Jira using OAuth 1.0.

## What next?

You have configured and connected your Jira integration with Miro using Jira OAuth1.0. When a user attempts a Jira-related action in Miro for the first time, they are prompted to authenticate.

**More information:** See [How to use Jira Cards](https://help.miro.com/hc/articles/360017572434).

## One Jira instance for several Miro Teams

You can install Jira Cards on the organization level, or at the team level. If you have multiple teams, then you can specify organization-level settings to avoid repetitive setup for each team. The existing application link is then used for all teams.

:::note
Connecting several Jira instances to one Miro team is not supported.
:::

For update requests, after you connect your organization or team to a Jira instance, a webhook is added to your Jira webhooks for that Miro organization or team.

:::tip
Give a unique name to each webhook per team. Go to your Jira WebHooks page and edit each newly created webhook.
:::

If you specify organization-level settings, teams that already have their own team settings retain their setup. Any team with their own setup can switch to the organization-level settings at any time.

Conversely, any team can override organization-level settings to connect to a separate Jira instance.

## Disable Jira Cards

### Organization level

To disable Jira Cards at the organization level, follow these steps:

1. From your Miro dashboard, click your avatar in the top-right and click **Admin Console**.
2. Go to **Apps and Integrations** > **Manage apps**.
3. Locate **Jira Cards**.
4. For Jira Cards, toggle **Allowed** to the off position.

:::warning
If you disable Jira Cards for the organization, then members in all Enterprise teams are unable to use Jira cards. To learn more about app management, see [App management](https://help.miro.com/hc/articles/4404659741458).
:::

### Team level

To disable Jira Cards at the team level, follow these steps:

1. From your Miro dashboard, click your avatar in the top-right and click **Admin Console**.
2. Go to **Teams**.
3. Click the row for the team you want to manage.
   The team settings panel opens.
4. Click the **Apps** tab.
5. Locate and click **Jira Cards**.
6. Click **Remove for team**.
