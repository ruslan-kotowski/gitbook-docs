---
title: How to enable Miro's MCP Server (user guide)
article_id: 31625301583890
sidebar_position: 3
created_at: '2025-12-05T15:13:02Z'
updated_at: '2025-12-08T12:29:46Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: "For Enterprise accounts, enabling MCP requires admin approval. If you're\
    \ in an Enterprise team, refer to the\_[Admin guide for Miro MCP](../miro-mcp-server-beta/04-miro-mcp-server-admin-guide.md)."
---

> For Enterprise accounts, enabling MCP requires admin approval. If you're in an Enterprise team, refer to the [Admin guide for Miro MCP](../miro-mcp-server-beta/04-miro-mcp-server-(admin-guide).md).

You will need to have Miro MCP enabled and authorized in your team and organization before being able to connect to any MCP Client.

## Enabling MCP Server

Follow the steps based on your plan type to get started quickly.

### Free, Starter, Business and Educational Plans

- MCP is enabled by default, no signup or approval needed.
- Install and authenticate directly through your MCP Client.

### Enterprise Plans

- Contact your Admin to install the MCP app first.
- Once installed, you can connect through your MCP Client.

## Authorizing Miro's MCP Server

1. Open your AI tool. For example, in Lovable: **Settings** > **Integrations** > **Miro MCP Server** > **Connect**.
2. Follow the [OAuth authentication flow](https://developers.miro.com/docs/connecting-to-miro-mcp#miro-oauth-flow).
3. Select the team where your boards are located.

:::note
Miro's MCP Server will only be able to read boards in the team you select during the OAuth flow.
:::

## Connecting Miro's MCP Server to your AI Tool

Once Miro's MCP Server is enabled for your organization or team, you can configure it on your preferred MCP Client.

### One-step installation

Most MCP Clients offer a streamlined installation process:

1. Open your AI tool (such as Cursor, VSCode, or Lovable).
2. Navigate to the MCP or integration settings.
3. Find and select "Miro" or "Add MCP Server".
4. Enter [`https://mcp.miro.com`](https://mcp.miro.com) when prompted.
5. Complete the OAuth authentication flow.
6. Select the team where you want to use Miro MCP.

:::tip
Make sure to select the same team where your boards are located.
:::

### Manual installation

Some tools require manual configuration:

1. Open your MCP Client's settings or configuration area.
2. Find the MCP configuration section.
3. Add the following JSON configuration:

```
{
  "mcpServers": {
    "miro-mcp": {
      "url": "https://mcp.miro.com/",
      "disabled": false,
      "autoApprove": []
    }
  }
}
```

4. Save your changes and authenticate through the OAuth flow.

### Verifying MCP is active

After enabling MCP, you can verify it's working by:

1. Attempting to connect an MCP-compatible tool like Cursor or VSCode.
2. Following the OAuth authentication flow.
3. Testing a simple prompt that uses Miro MCP functionality.

:::note
Some MCP Clients may require additional authentication with their respective services.
:::

### Tool-specific guides

For detailed installation instructions for specific tools, refer to our developer documentation:

- [Cursor](https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#cursor)
- [Claude Code](https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#claude-code)
- [VSCode and GitHub Copilot](https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#vscode-and-github-copilot)
- [Gemini CLI](https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#gemini-cli)
- [Lovable](https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#lovable)
- [Windsurf](https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#windsurf)
- [Replit](https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#replit)
