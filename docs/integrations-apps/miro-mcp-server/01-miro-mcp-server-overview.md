---
title: Miro MCP Server overview
article_id: 31624028247058
sidebar_position: 1
created_at: '2025-12-05T14:41:20Z'
updated_at: '2026-03-05T08:22:41Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: free, starter, business, enterprise, education
---

Miro's Model Context Protocol (MCP) Server is a gateway that allows AI tools to connect with Miro boards, enabling seamless interaction between your visual workspace and external AI systems. This powerful integration lets AI assistants read from and write to your Miro boards, creating a bridge between visual collaboration and AI capabilities.

### What is Miro MCP Server?

Miro's MCP Server is a secure gateway that gives AI tools secure access to Miro boards within your organization. It enables AI assistants to:

- Read and understand content from your Miro boards.
- Generate diagrams based on code or text descriptions.
- Transform visual information into code and other formats.

:::tip
Think of MCP as a universal translator that helps different AI systems communicate with Miro.
:::

### MCP Server + Clients

MCP provides the underlying infrastructure, while MCP Clients are specific integrations with AI tools:

- **MCP Server:** The secure gateway that enables communication between Miro and external AI tools.
- **MCP Clients:** Specific implementations that connect particular AI tools (like Cursor, VSCode, or Lovable) to Miro.
- **OAuth 2.1 Security:** Enterprise-grade authentication ensures secure access to your content.

:::note
Enterprise accounts require admin approval before users can install and use Miro's MCP Server.
:::

### How it works

1. **Connection:**
   1. In Enterprise plan, an admin enables Miro MCP for their organization or team.
   2. In all other plans, MCP access is enabled but needs to be authorized via an MCP Client (i.e. Cursor, Claude Code etc).
2. **Authorization:** Users connect their preferred AI tools to Miro through OAuth.
3. **Interaction:** AI tools can then read from and write to boards the user has specified.
4. **Creation:** Users can request AI tools to generate diagrams or code based on board context.

:::note
For more technical details and examples, visit our [developer documentation](https://developers.miro.com/docs/miro-mcp).
:::

### MCP tools

For a complete list of tools, read our [developer documentation](https://developers.miro.com/docs/miro-mcp-prompts).

### Explore the Miro MCP world

- Check our [developer documentation on MCP](https://developers.miro.com/docs/miro-mcp).
- Check out this [youtube playlist](https://www.youtube.com/playlist?list=PLmiHe0R4hbzSGgHWYFYwvbAKTvFPRvG2a) with fun tutorials on what you can do with Miro MCP.
