---
title: Get started with Linear
article_id: 30629568232722
sidebar_position: 3
created_at: '2025-10-29T13:35:01Z'
updated_at: '2026-02-23T11:34:34Z'
draft: false
availability:
  roles: all_users
  plans: business, enterprise
  platforms: browser, desktop
---

The Linear integration in Miro enhances collaboration by enabling seamless two-way synchronization between Miro boards and Linear issues. Import, view, and edit issues directly within Miro, ensuring your workflows stay up to date and teams remain aligned and productive.

:::note
: Administrators must authorize the Linear integration for their Miro team. Team members can use the integration only after it's installed at the team level.
:::

## Prerequisites

Before you begin using the Linear integration, make sure you have:

- An active Miro account ([sign up here](https://miro.com/) if needed)
- An active Linear account
- Administrator approval if your organization restricts app installations

## Connect Linear to Miro

To get started with the Linear integration, you'll need to connect your Linear account to Miro. Open a Miro board and click **Tools > Media & Integrations (+)** in the Creation bar. Search for **Linear** and click **Connect**.

When authenticating, you can choose to:

- Use your credentials (recommended)
- Use your API key or access token

After completing the authentication process, your Linear account will begin synchronizing with Miro. This initial sync can take several minutes to hours for large accounts. You'll receive an email notification once synchronization is complete.

## Add Linear issues to your board

Once connected, you can start adding Linear issues to your Miro boards. Access the Linear issue picker through **Tools > Media & Integrations (+)** and search for **Linear**. The picker lets you filter issues by Status, Assignee, and Project before importing them as Linear Issue Widgets.

Note that the picker only displays issues you have access to in Linear.

## Work with Linear issues

### Edit issues in Miro

You can edit Linear issues directly within Miro. Click any Linear Issue widget and use the side panel icon to open the issue details. From here, you can modify properties and click **Update** to synchronize changes with Linear.

### Organize your workflow

Miro offers several tools to help organize your Linear issues effectively:

The [Table](../../using-miro/formats/14-tables.md), [Timeline](../../using-miro/formats/15-timeline.md), [Columns](../../using-miro/advanced-tools/02-columns-(formerly-kanban).md), and [User story mapping](../../using-miro/advanced-tools/07-user-story-mapping.md) tools provide different ways to structure your workflow. Simply drag and drop Linear issues into these tools to organize them according to your needs.

Note that while you can move issues in the Columns widget, this action doesn't automatically update their status in Linear.

### Navigate and customize issues

The Linear integration provides several ways to work with your issues:

To view the full issue details in Linear, click the **Source** icon in either the detail view or side panel. You can switch between side panel and modal window views using the **Switch view** icon, and use the **Fill color** icon to color-code issues for better visual organization.

## Additional features

### Action shortcuts

The Linear integration supports [Action shortcuts](../../using-miro/facilitation-tools/03-action-shortcuts-(beta).md), allowing you to quickly:

Open the Linear Issue picker or create new Linear issues with customized shortcuts.

## Uninstall the integration

You can remove the Linear integration at either the team or individual level.

For team-level removal:

1. Navigate to **Team settings** > **Apps & Integrations**
2. Locate **Linear** and click **Uninstall for team**

For individual removal:

1. Go to **Apps & Integrations** in your settings
2. Find **Linear** and click **Uninstall for me**

## Frequently asked questions

### Who can use the integration?

The Linear integration is available to authorized users in your Miro team or organization who have appropriate Linear permissions.

### Who can see Linear issues in Miro?

Any user with board access (view, comment, or edit permissions) can see imported Linear issues. No Linear authorization is required to view issues on the board.

### How do Linear permissions work in Miro?

The integration respects your Linear permissions. While you can only search, import, or edit issues based on your Linear access rights, any issues you import to a Miro board become visible to all board users. Editing these issues still requires appropriate Linear permissions.
