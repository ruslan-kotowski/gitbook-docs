---
title: Connect to Jira on-premise with third-party authorization servers using OAuth2.0
article_id: 25692796700306
sidebar_position: 9
created_at: '2025-03-31T08:02:36Z'
updated_at: '2026-03-20T14:10:12Z'
draft: false
availability:
  roles: company_admin
  plans: enterprise
---

> *✏️* Connecting Jira using an authorization server is only enabled at the organization level.

This article provides the steps for connecting Miro to Jira with a third-party, on-premise authorization server using OAuth2.0.

To learn the technical details about this configuration, see the reference article for [Jira on-premise with third-party authorization using OAuth 2.0](https://help.miro.com/hc/articles/26726425696530).

## Prerequisites

- Ensure that you have the following permissions:
  - Miro Company admin
  - (Optional) Jira System admin, if you want to use automatic webhooks.
- On your authorization server, create an OAuth 2.0 app.
- Configure the redirect URL in your OAuth 2.0 app to the following URL:
  https://integrations.miro.com/api/external-auth/oauth2/callback
- Ensure you have the following details from your OAuth 2.0 app ready to set up in Miro:
  - Authorization URL
  - Token URL
  - Client ID
  - Client secret
  - Scope

## Connect to Jira on-premise with third-party servers using OAuth 2.0

1. On your Miro dashboard, select your avatar in the top-right and go to **Admin console** | **Settings**.
2. Go to **Apps and integrations ![icon-plug.svg](images/26725418032914_icon-plug.svg)**> **Apps** > **Manage apps** tab.
3. Ensure that **Allow only apps from the list below** is enabled.
4. Under the **App** column, for **Jira Cards** select **Settings**.
5. Click **Add new connection**.
6. Under **Jira setup**, click **Jira Data Center**.
7. Under **Authentication method**, select **OAuth2.0 via a third-party authorization server**.
8. Under **Jira URL**, enter your Jira instance URL.
   > *✏️* You can add your external Jira base URL, or your internal Jira URL. If you use an internal Jira URL, then you must specify your external API gateway URL in step 10.

   > *✏️* In general, using an internal URL enables you to adjust the navigate-to-source functionality.
9. (Optional) To make this connection the default connection for all teams in your organization, tick **Make Default**.
10. (Optional) If you use an API gateway to make requests to Jira, then for **Jira API Gateway base URL**, enter your external API gateway URL.
11. Enter the following details from your OAuth 2.0 app:
    - Authorization URL
    - Token URL
    - Client ID
    - Client Secret
    - Scope
12. (Optional) To get real-time updates from Jira in Miro, tick **Create webhook automatically**.
    > *✏️ You can manually add the webhook later.*
13. Click **Connect**.
14. Follow the authentication flow for your authorization server. If prompted, log in to your environment.
    When your connection completes, your Jira instance is listed under **Connected instances** with the following tag: **Auth server**.

## Ensure your team can authenticate

Now that you have connected your Jira instance at the organization level, you can start using Jira at the team level.

1. On your Miro dashboard, select your avatar in the top-right and go to **Admin console**.
2. Select **Teams** > **Your team**.
   The **Your team** slider opens.
3. Select the **Apps** tab.
4. From the apps list select **Jira cards**.
5. Under **Admin settings**, verify whether your Jira configuration shows the **GLOBAL CONNECTION** label, and shows the correct Jira instance URL, then do one of the following:
   - If yes, you have completed this procedure. You can skip to [What next?](#what-next)
   - If no, select **Change configuration** > **Global Organization Settings** > **your Jira instance**.
6. Select **Save settings**.

## What next?

Each team member must authorize their user account. To ensure that each user obtains access and refresh tokens, when a team member attempts a Jira-related action on a Miro board, they will be prompted to authorize their account.

## FAQ

**Which authorization servers can I use?**

You can use any authorization server that supports standard OAuth 2.0 protocols for on-premises environments. For example, Azure Active Directory (Entra ID) and Okta.

**Can I use the same authorization server for multiple organizations?**

Yes, but you must manually add the server to each organization.

**Can I update the client secret for an authorization server?**

No. If you need to change the client secret, then you must disconnect and reconnect your instance.

**Can organization and team admins still use native authorization in Jira?**

Yes. Depending on the selected configuration, admins can continue to use the native authorization flow in Jira.

**What happens if a team is already connected to another Jira instance?**

You can update teams to your organization [default Jira settings](https://help.miro.com/hc/articles/26438407676434).

**Does Miro control mapping between authorized users to Jira users?**

No. Mapping between authorized users and Jira users is the responsibility of the customer environment via their API gateway. Miro does not control this gateway.

**How do I know if OAuth 2.0 via a third-party authorization server is the right solution for my organization?**

If all of the following items are true, then OAuth 2.0 via a third-party authorization server is a good fit:

- Your Jira instance is hosted on-premises.
- External access to Jira is only possible with an API gateway.
- The API gateway enforces authorization using a custom authorization server.
- You must connect Miro to Jira without exposing the Jira public base URL.

**What problem does this solution solve?**

This solution is designed for organizations that host Jira on-premises and route external API traffic through an API gateway. In this setup, Jira isn't publicly accessible, and access is controlled via a custom authorization server. Instead of having a public base URL for Jira, this solution allows you to connect your on-prem Jira instances by configuring Miro to authenticate via your own authorization server.
