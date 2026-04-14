---
title: Set up Miro Insights
article_id: 30122381753106
sidebar_position: 1
created_at: '2025-10-10T10:26:28Z'
updated_at: '2025-11-25T15:54:01Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Connecting your tools to Miro Insights is a crucial first step for getting real value. Integrations allow Miro Insights to automatically pull in customer feedback and relevant data from across your systems. This guide is for Company Admins who will enable these connections.

If you're a team member looking to use Miro Insights after it's set up, see the article on [Using Miro Insights](../use-miro-insights).

## Prerequisites

To set up Miro Insights integrations you need to meet the following requirements:

- Must be a **Company Admin in Miro**.
- Must have **Admin or API access on the external platform** you’re connecting.

:::note
Ensure your **Miro plan includes Miro Insights**. If Miro Insights is an add-on or in limited release, your account must be eligible. Also, some integrations might require specific editions of the external software. For example, certain CRM API access is available on higher-tier plans.
:::

## Prepare your data sources

Before connecting your data sources to Miro Insights, it's important to prepare your data and establish a clear taxonomy. This preparation will ensure you get the most accurate, actionable insights from the platform.

### Clean and optimize your data

Before syncing data with Miro Insights, clean and optimize your data sources:

- Remove duplicates and outdated items.
- Clean up inconsistent or irrelevant feedback.
- Ensure data quality in your source systems.
- Address major data inconsistencies or gaps beforehand.

### Establish your taxonomy

While Miro Insights comes with basic AI-generated categories, it's recommended to define your own standardized taxonomy before rollout. This ensures consistency and improves the quality of insights from the start.

Consider including these standard categories:

- Feature requests
- Bugs
- UX pain points
- Customer segments
- Priority levels
- Business units
- Strategic initiatives

Best practices for taxonomy:

- Use terminology that matches your team's language.
- Create clear guidelines for how and when to use each category.
- Share the taxonomy with your team to ensure consistent use.
- Regularly review and refine categories as needed.
- Consider mapping to your strategic initiatives and OKRs.

:::tip
Reach out to Miro Insights support for help defining your taxonomy. They can provide examples and best practices based on other customers in your industry.
:::

## Connect an integration

When your data is ready, you can connect your integrations. Miro Insights supports a variety of popular tools across CRM, support, sales calls, project management, and chat platforms.

In the **Integrations & Automations** settings tab, you can view and manage all your connected integrations. Each integration is listed with its connection status and options to configure or disconnect.

To connect an integration:

1. From the **Miro Insights** app, select the **Settings** icon at the top of the left sidebar.
2. In the **Settings** panel, go to the **Integrations & Automations** tab.
3. Select **Connect** next to the integration you want to add.
4. **Authorize access**. A pop-up will prompt you to authorize Miro Insights to access that tool.
   This typically involves logging into the external service and granting permissions. For example, when connecting Salesforce, you must log in with your Salesforce admin account and approve the integration. For Slack, select a workspace and authorize the Miro Insights Slack app. Follow the on-screen prompts for each.
5. **Configure import settings**. Once connected, the integration will appear as “Connected” with additional settings options. Here you can set:
   - **Import conversations from**: For conversation-based sources like Gong or Zendesk, you might choose a date. This prevents pulling in old data unless you want it.
   - **Automatic import rules**: Toggle whether new items should be auto-imported. You can enable this so that new calls or tickets flow in continuously. If you leave it off, you might import items manually or selectively.
   - **If AI detects requests with**: Some sources let you filter by [AI detection confidence](#ai-filtering).
   - **Detect issues**: Enables Miro Insights to automatically identify and extract issues from customer feedback. These issues can include usability challenges, performance problems, security concerns, etc.

Other options may vary by integration. For example, in Jira, you can select which project(s) to pull features from or map custom fields.

### AI filtering

Some integrations let you **filter by AI detection**. This means Insights will scan a call transcript and only create a feedback item if it’s reasonably sure a product request was mentioned. This reduces noise from unrelated conversations. You can adjust the confidence threshold or turn this off to import everything.

### Tag or field filters

In tools like Zendesk, you can specify a tag. For example, “feature_request”, then only tickets with that tag will be ingested. In Jira, you can select a specific project or issue type to import as features.

### Issue syncing

For project tools like Jira, you may have options to map fields. The screenshot above shows an example “Push feature dollar value to custom field” – you could select a custom field in Jira to populate with the calculated dollar impact from Miro Insights, closing the loop back to engineering. This step is optional but can be powerful.

Connect all the systems that are relevant. We recommend at minimum connecting one CRM and one support or feedback source to start, so you get both account context and raw feedback. You can always add more later.

Once done, you have successfully connected your integrations to Miro Insights. The system will begin syncing data. Initial sync might take a little time if there's a lot of historical data (you'll see last synced timestamps next to each integration). You can monitor the sync status in the Integrations list – it shows the last synced time and gives a Disconnect option if ever needed.

## Import items manually

You can also import features and feedback items manually using a CSV file. This is useful for one-time imports or if you have a list of feature requests or feedback from another source.

To import features via CSV:

1. In Miro Insights, go to the **Backlog** view.
2. Click the **Import** button at the top right.
3. Select **Upload CSV**.
4. Select the column in your CSV data source that best matches Miro Insights’s properties.
5. Select **Import feature** to complete the process.

Your imported features will now appear in the [Backlog](../../tools/use-miro-insights/05-backlog.md) section.

To import feedback items via CSV:

1. In Miro Insights, go to the **Feedback** view.
2. Click the **Import** button at the top right.
3. Select **Upload CSV**.
4. Map the columns in your CSV to Miro Insights’s feedback properties (e.g., title, description, source).
5. Select **Import feedback** to complete the process.

Your imported feedback items will now appear in the [Feedback](../../tools/use-miro-insights/07-feedback.md) section.

## Connect unsupported tools using Zapier

If you have a tool that isn’t directly supported, you can often use [Zapier](http://zapier.com/) to forward data into Miro Insights. For instance, you could create the following Zapier workflow. When a Google Form is submitted or when a new entry in a custom database appears, create a feedback item in Miro Insights.

For detailed steps, see the article on [Using Zapier with Miro Insights](03-connect-tools-with-zapier.md).

## Additional steps

After connecting your integrations, you can do a few optional steps to ensure everything is set up properly:

### Import or verify features

If you connected a task tracker like Jira, check the Backlog in Miro Insights to see if your existing features or epics have appeared. If not, you might use the Import button in the Backlog view to upload a CSV or trigger a pull from Jira. Ensure each imported feature has a clear title and description; the AI relies on that text to match relevant feedback.

### Set up Slack commands or email forwarding

If you added Slack, let your team know how to send messages to Insights. For example, right-click a message > “Send to Miro Insights”.

For email or other channels, you might configure forwarding. Some teams set up a specific email address that auto-forwards into a tool like Intercom or a Zapier hook for ingestion.

:::tip
: It’s a good idea to periodically review your integration settings. For instance, if you notice too much trivial feedback coming in from a source, tighten the filters or raise the AI confidence threshold. Conversely, if you’re missing data you expected, ensure the integration is connected with the right scope (e.g., the correct project or tag). A well-tuned integration setup keeps your insights signal high and noise low.
:::

## Disconnect an integration

If you ever need to disconnect an integration:

1. Go to **Settings** > **Integrations & Automations**.
2. Find the integration you want to remove.
3. Select **Disconnect** next to it.
4. Confirm the disconnection in the pop-up prompt.

This will stop any future data syncs from that source.

> **Important**: In some cases, for example Gong, disconnecting may also remove previously imported feedback items. In other cases, such as Jira, existing features may remain but won’t receive updates. Review the specific behavior for each integration in the documentation or contact support if unsure.

Make sure to communicate with your team if you disconnect a major source, as it may impact the completeness of backlog and feedback in Miro Insights.

## What's next?

By connecting integrations, you’ve laid the foundation for Miro Insights to deliver rich, continuous product insights. Data will start flowing in, and the AI will start making connections.

You can now proceed to [using Miro Insights](../use-miro-insights) or learn more about ongoing administrative tasks, including general settings, team management, notifications, and API access in the [Miro Insights administration guide](02-manage-miro-insights.md).
