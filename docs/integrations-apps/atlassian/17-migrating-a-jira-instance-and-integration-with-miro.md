---
title: Migrating a Jira instance and integration with Miro
article_id: 24905405160338
sidebar_position: 20
created_at: '2025-02-25T10:19:27Z'
updated_at: '2026-03-20T14:10:12Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  roles: Company admin with Jira System Admin role
---

This article explains what you need to know about updating your Jira integration with Miro, after you have migrated a Jira instance, including best practices and the procedure.

:::note
As of February 15, 2024 Atlassian has deprecated their Server products and moved support to Cloud. After you migrate your instance(s) of Jira to Cloud, to ensure that your Jira integration with Miro persists, follow the procedure in this article.
:::

## What you need to know about migrating a Jira instance

Ensure that you understand the following migration details:

- Migrating your Jira instance changes your Jira base URL. If you do not update your Jira integration with Miro, the integration breaks.
- Miro executes a support workflow that updates the URL for each existing Jira card in Miro. To initiate the workflow, you must notify your Miro contact person. For more information, see [How to migrate a Jira instance](#how-to-migrate-a-jira-instance).
- After migrating to Cloud, you must reconnect to Miro on OAuth 1.0.
  > ⚠️ You can update to OAuth 2.0 after the Miro support workflow is complete.
- If you use [Planner for Jira](https://help.miro.com/hc/articles/10648975837970), you must rebuild your planner after updating your integration.

### Best practice

Before you start to migrate your Jira instance, you can reach out to your Miro contact person in advance and specify your case. Miro support can help you plan a smooth transition when you are ready to update your Jira integration with Miro.

After you have successfully migrated your Jira instance, notify your Miro contact immediately. The earlier Miro updates your integration, the faster your team can begin using the integration without conflict.

:::warning
To update your integration, Miro changes only the Jira base URL, not the project key. If you plan to migrate a Jira instance, avoid making updates that change project keys. For example, renaming a project, or moving an issue between projects. Changing project keys will require you to re-create your Jira cards manually in Miro.
:::

## How to migrate a Jira instance

Migrating your Jira instance changes your Jira base URL. This procedure explains how to ensure that your Jira integration with Miro persists.

**Procedure**

Follow these steps:

1. In Jira, complete your Jira instance migration.
2. Reconnect your Miro Team(s) to each new instance respectively. To learn how, see [Set up and disable Jira Cards (OAuth 1.0)](https://help.miro.com/hc/articles/360019501754)
   > ✏️ You must reconnect with OAuth 1.0.
3. Notify your Miro contact person.
   1. Confirm that steps 1-2 are complete.
   2. Verify that your new base URL is connected with OAuth 1.0.
   3. Provide the new base URL and list of teams where the update is required.
      Miro support updates each existing Jira card URL.
4. (Optional) If migrating to Cloud, when Miro support confirms that each existing Jira card URL is updated, you can switch your integration to OAuth 2.0.

   You have successfully updated your Jira integration with Miro.
