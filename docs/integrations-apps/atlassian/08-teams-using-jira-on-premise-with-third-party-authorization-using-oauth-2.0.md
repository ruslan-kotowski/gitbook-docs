---
title: Teams using Jira on-premise with third-party authorization using OAuth 2.0
article_id: 25699264170386
sidebar_position: 10
created_at: '2025-03-31T11:33:06Z'
updated_at: '2026-03-20T14:10:12Z'
draft: true
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Using a third-party server replaces the native authorization flow in Jira, and enables your organization to manage authentication externally for team members.

This article explains how to enable teams to authenticate with Jira on-premise using OAuth 2.0.

:::warning
Ensure you have completed the connection procedure for third-party authorization with OAuth2.0.[LINK].
:::

## How to setup a Jira on-premise connection with OAuth 2.0 for Miro teams

**Prerequisites**

Ensure you have completed the connection procedure for third-party authorization with OAuth 2.0[LINK].

**Procedure**

Follow these steps:

1. On your Miro dashboard, select your avatar in the top-right and go to **Admin console**.
2. Select **Teams** > **Your team**.
   The **Your team** slider opens.
3. Select the **Apps** tab.
4. From the apps list select **Jira cards**.
5. Under **Admin settings**, verify whether your Jira configuration shows the **GLOBAL CONNECTION** label, and do one of the following:
   - If yes, you have completed this procedure. You can skip to [What next?](#what-next)
   - If no, select **Change configuration** > **Global Organization Settings** > **your Jira instance**.
6. Select **Save settings**.

   You have successfully setup your Jira on-premise connection with OAuth 2.0 for Miro teams.

## What next?

Each team member must authorize their user account. To ensure that each user obtains access and refresh tokens, when a team member attempts a Jira-related action on a Miro board, they will be prompted to authorize their account.
