---
title: Miro MCP Server (admin guide)
article_id: 31625761037202
sidebar_position: 4
created_at: '2025-12-05T15:27:42Z'
updated_at: '2026-04-01T08:43:09Z'
draft: false
---

**Relevant for:** Company and team admins in Enterprise plans

As a company admin for an Enterprise subscription, you control whether Miro MCP Server is available to your organization. This setting determines whether your teams can use AI integrations that connect with Miro.

Use Miro MCP (Model Context Protocol) to connect your Miro boards to MCP‑compatible AI tools. When enabled and authorized, AI agents can read context from specific boards and (where allowed) take actions such as summarizing content or creating diagrams via a curated set of Miro MCP tools. This guide explains prerequisites, enablement, governance, and troubleshooting.

## Before you begin

- Decide scope: enable for the entire organization or only for selected teams (board‑level permissions still apply).

## Enable or disable MCP Server

To enable MCP Server:

1. Go to **Admin settings** > **Apps & Integrations** > **MCP**.
2. Choose scope.
   1. **Organization**: Any user in your org may authorize MCP for boards they can already access.
   2. **Selected team(s)**: Only users in those teams may authorize MCP; board‑level permissions still apply.
3. Toggle on. Changes take effect immediately.

To temporarily halt usage, toggle Miro MCP off in the same location (halts new tool calls).

## How access and permissions work

When you enable MCP, you allow:

- External AI agents to read board content when authorized by users
- AI tools to create or modify content on Miro boards
- Secure data exchange between Miro and third-party applications

Important security considerations:

- All access is authenticated through OAuth 2.1
- Users can only grant access to boards they have permission to view
- Enterprise security compliance is maintained
- Standard API rate limits apply to all operations
- Users in your org will be able to authenticate to the MCP Server allowing external/3rd party AI agents to read and create content on a board on their behalf

### Managing MCP in your organization

As an admin, you should consider:

1. **Communication:** Inform your teams about Miro MCP availability and use cases
2. **Training:** Provide guidance on how to effectively use MCP with different AI tools
3. **Governance:** Establish guidelines for appropriate use of AI-generated content
4. **Monitoring:** Periodically review MCP usage and adjust settings as needed

For more information on managing apps in your Miro environment, see the [App management documentation](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).

### Rollout guidance

- Start small: enable for one or two pilot teams (for example, engineering and product) and validate value/control.
- Reinforce prompt hygiene: require users to include a full board URL in every MCP prompt.

## Troubleshooting

- “I can’t see Miro MCP tools in my client”
  - Confirm MCP is enabled for the org or intended team, and the user belongs to that team.
  - Re‑run the OAuth flow and select a team with MCP enabled.
  - Verify the client supports MCP and is among the clients we’re targeting/documenting.
- “Access denied when prompting”
  - Ensure the prompt includes a full board URL; agents won’t auto‑discover boards.
  - Confirm the user already has access to that board in Miro.
- “We need to pause usage now”
  - Toggle MCP off in **Admin settings** > **Apps & Integrations** > **Miro MCP**.
