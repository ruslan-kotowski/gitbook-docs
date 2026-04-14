---
title: Gemini Enterprise integration
article_id: 32304596526482
sidebar_position: 1
created_at: '2026-01-05T10:38:04Z'
updated_at: '2026-02-17T09:38:53Z'
draft: false
availability:
  roles: company_admin
  plans: business, enterprise
  platforms: browser, desktop
---

As Company admin, you can enable and configure the Gemini Enterprise integration for teams in your Miro organization.

The Gemini Enterprise integration enables you to connect Gemini Enterprise as a [Knowledge](../../using-miro/miro-ai/09-knowledge.md) resource in Miro. For example, use Gemini Enterprise to provide company intelligence to Sidekicks and Flows.

You can also connect Gemini Enterprise to the [standalone chat](../../using-miro/miro-ai/09-knowledge.md) app in Miro.

To use the Gemini Enterprise integration, follow these steps:

1. Enable the Gemini Enterprise app.
   1. As Company admin, go to **Admin Console**.
   2. Go to **Apps & integrations** > **Apps** > **Add apps**.
   3. Search and find **Gemini Enterprise**.
      If you cannot find the app by name, then search by the following client ID: `2392210303456548729`.
   4. In the app profile, select whether to add the app for **All teams in \{Team name\}**, or select **In** **specific teams**.
   5. Click **Add**.
2. Configure the Gemini Enterprise app.
   1. In **Admin Console**, go to **Apps & integrations** > **Apps**.
   2. For Gemini Enterprise, ensure that **Allowed** is toggled to the on position. Then click **Settings**.
   3. Add your Gemini Enterprise configuration details.
      To learn how to find the Project ID, see (External) [Locate the project ID](https://support.google.com/googleapi/answer/7014113?hl=en).
      To get the App ID, go to Gemini Enterprise > Apps, and use the value in the ID column.
      ![](images/33221858257554_image (2).png)
      *Configure the Gemini Enterprise app for use in Miro.*

      > ✏️ **Project ID** and **App ID** are required. The other fields are optional.
   4. Click **Save**.

:::note
When a team member connects Gemini Enterprise as a [Knowledge](../../using-miro/miro-ai/09-knowledge.md) resource for the first time, the member is asked to authenticate. The team member must have a Gemini Enterprise license.
:::
