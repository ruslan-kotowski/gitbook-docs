---
title: Miro MCP Server overview
article_id: 31624028247058
created_at: '2025-12-05T14:41:20Z'
updated_at: '2025-12-08T12:28:43Z'
draft: false
position: 0
---

> **Available for:** All plans

Miro's Model Context Protocol (MCP) Server is a gateway that allows AI tools to connect with Miro boards, enabling seamless interaction between your visual workspace and external AI systems. This powerful integration lets AI assistants read from and write to your Miro boards, creating a bridge between visual collaboration and AI capabilities.

> ✏️ **This is a beta release of our MCP.** It is intended for evaluation and feedback purposes. The feature set and user experience may change in future releases.

### What is Miro MCP Server?

Miro's MCP Server is a secure gateway that gives AI tools secure access to Miro boards within your organization. It enables AI assistants to:

  * Read and understand content from your Miro boards.
  * Generate diagrams based on code or text descriptions.
  * Transform visual information into code and other formats.

> 💡 **Tip:** Think of MCP as a universal translator that helps different AI systems communicate with Miro.

### MCP Server + Clients

MCP provides the underlying infrastructure, while MCP Clients are specific integrations with AI tools:

  * **MCP Server:** The secure gateway that enables communication between Miro and external AI tools.
  * **MCP Clients:** Specific implementations that connect particular AI tools (like Cursor, VSCode, or Lovable) to Miro.
  * **OAuth 2.1 Security:** Enterprise-grade authentication ensures secure access to your content.

> ✏️ Enterprise accounts require admin approval before users can install and use Miro's MCP Server.

### How it works

  1. **Connection:**
    1. In Enterprise plan, an admin enables Miro MCP for their organization or team.
    2. In all other plans, MCP access is enabled but needs to be authorized via an MCP Client (i.e. Cursor, Claude Code etc).
  2. **Authorization:** Users connect their preferred AI tools to Miro through OAuth.
  3. **Interaction:** AI tools can then read from and write to boards the user has specified.
  4. **Creation:** Users can request AI tools to generate diagrams or code based on board context.

> ✏️ For more technical details and examples, visit our [developer documentation][1].

### MCP tools

The tool list may evolve during beta. Examples include:

Tool name | Description | Uses Miro AI credits
---|---|---
board_get_items | Find specific items on a board | No
board_get_image_download_url | Download images from board | No
board_get_image_data | Find images on a board | No
context_get_board_docs | Summarize a board's information | Yes
draft_diagram_new | Create a new Diagram on a selected Miro Board | Yes

### Explore the Miro MCP world

  * Check our [developer documentation on MCP][1].
  * Check out this [youtube playlist ][2]with fun tutorials on what you can do with Miro MCP.

   [1]: <https://developers.miro.com/docs/miro-mcp>
   [2]: <https://www.youtube.com/playlist?list=PLmiHe0R4hbzSGgHWYFYwvbAKTvFPRvG2a>
