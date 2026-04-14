---
title: Jira Cards
article_id: 360017572434
sidebar_position: 5
created_at: '2019-02-11T10:13:09Z'
updated_at: '2026-03-20T14:10:12Z'
draft: false
availability:
  plans: starter, business, education, enterprise
  roles: all_users
  platforms: browser, desktop, mobile
  notes: 'Jira: Jira Cloud, Jira Server (on-premise), Jira Data Center'
---

Jira Cards enable you to work with Jira issues directly within Miro boards. This integration streamlines your team's workflow by bringing Jira issues into your collaborative workspace for retrospectives, story sizing, backlog prioritization, story mapping, and other team activities.

![Jira cards in user story mapping](images/21017348097170_Jira%20cards%20in%20USM.png)

## Import Jira issues to your board

You can import Jira issues to your board in two ways:

1. Copy the Jira issue URL and paste it on the board.
2. Click the **Tools, Media and Integrations** (**+**) icon on the Creation toolbar, select **Jira Cards**, choose one or more issues, and click **Add**.

When importing issues for the first time, you'll need to connect your Jira account:

1. Click **Authorize** in the dialog box that appears.
2. Log in to your Jira account with your credentials.
3. Authorize the connection between Miro and Jira.

After authorization, you'll see all Jira issues you have access to in the Jira Cards picker.

:::note
Users who haven't authorized their Jira account will see a simplified card view without assignee avatars.
:::

## Create new Jira issues

You can create Jira issues directly from Miro in two ways.

### Create using the Jira app

1. Click the **Tools, Media and Integrations** (**+**) icon on the Creation toolbar
2. Select **Jira Cards**.
3. Click **Create issue**.
4. Fill in the required fields.
5. Click **Create**.

### Convert existing items to Jira issues

You can convert existing sticky notes or cards on your board into Jira issues.

1. Select up to 50 sticky notes or cards.
2. Click the **Convert to** > **Jira** in the context menu.
3. Set the default values (issue type, priority, assignee, etc.).
4. Click **Convert**.

:::warning
Note:

- Cards in the USM Tasks line cannot be converted to Jira issues.
- During conversion, tags and Start date from Miro Cards will not be preserved.
- Assignee information needs to be set again after conversion.
:::

## View and edit Jira issues

:::warning
Editing Jira Cards is not supported in the Desktop or Mobile app.
:::

You can view Jira cards in two ways:

- Side view
- Centered view

### Edit issues in Miro

1. Click the **Open in side panel** or **Open in center panel** icon.
2. Make your changes.
3. Click **Update** to save.

### Change issue status

1. Click the **Workflow** icon.
2. Select the desired **Status** and **Comment**.
3. Click **Update** to save.

### Edit in Jira

1. Select a card and click the **Source** icon.
2. Edit the issue in Jira in the new browser tab.
3. Changes will sync automatically to the Miro card.

## Synchronization between Miro and Jira

|  |  |
| --- | --- |
| **Jira instance update vs Miro card update** | **When does the update occur?** |
| Update in Jira via OAuth 1.0 and OAuth 2.0 | Miro Jira Card is updated immediately via [Webhook](https://help.miro.com/hc/articles/360017731113). |
| Update in Miro | Miro Jira Card is immediately updated and the corresponding Jira issue is updated simultaneously. |

## Customize Jira Cards

### Change card colors

1. Select one or more Jira Cards.
2. Click **fill color** in the context menu.
3. Choose your desired color.

### Configure custom fields

1. Click the **Tools, Media and Integrations** (**+**) icon on the Creation toolbar
2. Select **Jira Cards**.
3. Select **Configure cards**.
4. Select the fields you want to display.
5. Click **Save**.

:::note
Important notes about fields:

- Settings apply only to the current board.
- Default fields (Assignee, Issue type, Priority, Status) cannot be removed.
- Fields may not appear if they have no value or are not available for the issue type.
- Some field types (like color custom fields) are not supported.
:::

## Search for Jira issues

The Jira Cards picker shows recent tasks first and offers several sorting options:

- Issue type
- Priority
- Key
- Summary
- Assignee
- Status

Use keywords to find specific issues or use **Jira Query Language** (JQL) for complex searches:

1. Select the **Advanced search** toggle in the search bar.
2. Enter your JQL query.

The results will update based on your query.

## Related articles

- [Jira Cards FAQ](https://help.miro.com/hc/articles/360013463739)
- [Set up and uninstall Jira Cards](https://help.miro.com/hc/articles/360019501754)
- [Set up webhooks for Jira Cards](https://help.miro.com/hc/articles/360017731113)
- [Troubleshoot Jira Cards issues](https://help.miro.com/hc/articles/360017572654)
