---
title: How to set up webhooks for Jira Data Center
article_id: 360017731113
sidebar_position: 14
created_at: '2019-02-11T10:13:13Z'
updated_at: '2026-04-07T16:01:41Z'
draft: false
availability:
  roles: Jira System Admins
  plans: All Miro plans (for Jira Server/Data Center integration via OAuth 1.0)
  platforms: browser, desktop
---

To ensure your [Jira Cards](03-jira-cards.md) on a Miro board stay up-to-date, Miro must receive messages from Jira whenever data changes occur. These Jira events are transmitted to Miro via a webhook.

This guide provides two ways to create webhooks for Jira Server and Jira Data Center using OAuth 1.0 and OAuth2.0.

## Create a webhook automatically

When [setting up your Jira Cards integration](12-deprecated-–-set-up-and-disable-jira-cards-using-oauth-1.0.md), if you are connecting to Jira Server or Jira Data Center, you can leave the option **Create a webhook automatically** activated. This is the recommended method.

:::note
Automatic webhook creation requires you to be logged into Jira as a Jira System Administrator.
:::

![jira-webhooks-server-config.png](images/21304245707026_jira-webhooks-server-config.png)
*Jira Cards settings, Step 2: "Create a webhook automatically**"** is enabled*

After the webhook is created automatically, it is a good practice to go to your Jira WebHooks page and edit the webhook to give it a unique name. This is especially important if you plan to connect several Miro teams to your Jira instance.

:::note
For OAuth2.0 connections, the Miro-side connection is set at the company level. One webhook is created for all Miro teams.
:::

:::note
For OAuth 1.0 connections at the Miro team level, a webhook is created per team. At the Miro company level, one webhook is created for all teams.
:::

## Create a webhook manually

If you prefer or need to create the webhook manually, follow these steps.

### Get the webhook URL from Miro

1. In the Jira Cards settings in Miro (Step 2, when connecting to Jira Server/Data Center), uncheck the option to **Create a webhook automatically**.
2. Copy & paste your organization's **Jira URL** and click **Connect and save settings.**
   ![jira-webhooks-configure-jira-url-cropped.png](images/21304245708818_jira-webhooks-configure-jira-url-cropped.png)
   *Jira Cards settings, Step 2: "Create a webhook automatically" is disabled*
3. Allow the integration to connect in Jira when prompted.
4. After these steps, Miro will provide you with the **WebHook URL**:
   ![webhook_URL.jpg](images/21016928565010_webhook%20URL.jpg)*Webhook URL provided by Miro*

:::note
If you are not a Jira System Administrator, please copy the **WebHook URL** provided by Miro and send it to your Jira System Administrator so they can create the webhook on the Jira side using the instructions below.
:::

### Create the webhook in Jira

Below are the steps to create a WebHook in Jira using the URL obtained from Miro. You can also refer to the official Atlassian documentation for [Jira Server](https://developer.atlassian.com/server/jira/platform/webhooks/) and for [Jira Cloud](https://developer.atlassian.com/cloud/jira/platform/webhooks/) (though this article focuses on Server/Data Center).

1. To navigate to the **WebHooks** page in Jira, go to **Jira Administration** > **System** > **Advanced >** **WebHooks** (the exact path may vary slightly depending on your Jira version). Alternatively, you can often use a direct link by appending `/plugins/servlet/webhooks` to your Jira instance URL (e.g., `https://YourJiraInstanceName/plugins/servlet/webhooks`).
2. Click **Create a WebHook** in the top right corner of the WebHooks page.
3. Enter a descriptive **Name** for the WebHook (e.g., "Miro Integration Webhook").
4. Set the WebHook status to **Enabled**.
5. Paste the **WebHook URL** copied from the Miro settings into the URL field.
   ![system_webhooks.jpg](images/21016941532050_system%20webhooks.jpg)
   *System Webhooks configuration in Jira*
6. In the **Events** section, under **Issue**, select the events **updated** and **deleted**.
7. Click **Create** to save the webhook.
   ![Jira_Webhook_settings.jpg](images/21016941533074_Jira%20Webhook%20settings.jpg)
   *Jira WebHook event settings*
8. After the webhook is created in Jira, return to **Step 2** in the Jira Cards settings in Miro, ensure your **Jira URL** is correctly filled in, and click **Connect**.

Now the webhook is created and configured. Jira Cards on your Miro boards will update automatically when changes are made in Jira.

## Organization-level webhooks

If your organization uses [organization-level Jira settings](04-connect-teams-in-organization-to-default-jira-settings.md), the webhook setup works differently from team-level connections:

- **Single webhook for the organization**: When you connect Jira at the organization level, a single webhook is registered for the entire organization. This replaces the need to have separate webhooks per team.

- **Reduced webhook count**: For organizations that previously had one webhook per team (sometimes dozens), switching to org-level settings consolidates these into a single webhook, which can reduce load on your Jira instance.

- **Team overrides use the org webhook**: When teams use the global organization connection, they share the same webhook created at the org level.

:::note
If your team-level webhooks were restricted with JQL filters (for example, to specific projects), the org-level webhook either needs to reflect all those JQL filters or have no filter at all. Review your JQL requirements before migrating to org-level settings.
:::

In the **Organization Admin Settings** after the connection is set up, you will find the **Webhook URL** under **Connected instances**. Copy the **Manual webhook** and paste it into your Jira environment.
