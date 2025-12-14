---
title: What are MCP Clients
article_id: 31624733719058
created_at: '2025-12-05T14:59:14Z'
updated_at: '2025-12-08T12:29:21Z'
draft: false
position: 1
---

> **Available for** : All plans

MCP Clients are AI tools (i.e. Cursor, Claude Code, Lovable) that connect to the Miro MCP Server using the Model Context Protocol (MCP). They implement the MCP specification to establish a secure client-to-server connection and interact with Miro boards.

## How it works

  1. In Enterprise Plans, an admin enables Miro's MCP Server for their organization.
  2. Configure your MCP Client (AI tool) to connect to the Miro MCP Server.
  3. The client establishes a secure MCP connection to https://mcp.miro.com.
  4. You authorize the client via OAuth, choosing what it can access (boards, team, scope).
  5. The AI tool uses MCP to read and act on board content within the granted permissions.

## Types of clients

  * IDE Clients: VSCode, Cursor, GitHub Copilot
  * Non-IDE Clients: Lovable, Replit, Claude Code, Gemini CLI, Windsurf

## What they can do

  * Code to diagram: Convert code into visual diagrams.
  * Board to code: Turn board content into working application code.
  * Visual prototyping: Generate landing pages and UI designs from board concepts.
  * Cross-tool context: Let AI tools understand and build on your visual work across tools.

## Available clients

  * [Cursor][1]
  * [Claude Code][2]
  * [VSCode and GitHub Copilot][3]
  * [Gemini CLI][4]
  * [Lovable][5]
  * [Windsurf][6]
  * [Replit][7]

Explore all options in our [developer documentation][8].

   [1]: <https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#cursor>
   [2]: <https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#claude-code>
   [3]: <https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#vscode-and-github-copilot>
   [4]: <https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#gemini-cli>
   [5]: <https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#lovable>
   [6]: <https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#windsurf>
   [7]: <https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools#replit>
   [8]: <https://developers.miro.com/docs/miro-mcp>
