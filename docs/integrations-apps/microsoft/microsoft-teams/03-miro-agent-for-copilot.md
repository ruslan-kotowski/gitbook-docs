---
title: Miro agent for Copilot
article_id: 21399453845522
sidebar_position: 3
created_at: '2024-09-16T13:04:04Z'
updated_at: '2025-12-29T12:25:20Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  roles: All Miro users with a paid Microsoft Copilot license
  plans: All Miro plans (paid Microsoft Copilot license and compatible Microsoft 365
    plan required)
  platforms: Microsoft Teams (Desktop, Web, Mobile where Copilot is supported)
---

The Miro agent within Microsoft Copilot represents a significant advancement in bridging artificial intelligence capabilities with collaborative workflows. This integration transforms AI-generated insights into actionable, shared content within Miro, helping organizations demonstrate tangible business value from AI tools and seamlessly integrate AI outputs into daily workflows.

## Understanding the Miro agent for Copilot

The Miro agent in Microsoft Copilot is specifically engineered to augment collaboration by connecting AI-driven intelligence from Copilot with Miro's visual collaboration environment. It functions as a crucial link, enabling users to convert conversations and AI-generated information into dynamic, collaborative workflows within Miro.

Organizations frequently encounter difficulties in demonstrating tangible business value from AI tools, integrating AI outputs into daily workflows, and sustaining user adoption beyond initial excitement and pilot programs. The design of the Miro agent directly addresses these challenges, presenting a strategic solution aimed at making AI more practical and valuable within enterprise workflows.

The value proposition of this integration includes:

- **Accelerated information access:** Find relevant Miro boards and content directly within Microsoft Teams and Office 365, ensuring teams have immediate access to information they need. This streamlines workflows by reducing time spent searching for content, accelerating decision-making and project progression.
- **Transformation of ideas into collaborative workflows:** Convert AI-generated insights and ongoing conversations from Microsoft tools into flowcharts, sticky notes, and documents within Miro. The agent serves as the "action layer" for Copilot's intelligence, bridging the gap between AI-driven understanding and human-driven collaboration.
- **Enhanced team alignment:** Add visual, shared context to AI outputs, helping teams align on ideas, track changes, and progress together more effectively through a common visual understanding.

## Key features

Miro's current offering within Copilot is characterized as a "declarative agent". This design allows users to articulate their desired outcome through natural language prompts, rather than requiring specific commands. The agent interprets these prompts and executes the necessary actions, making it accessible to users without specialized technical expertise.

The key functionalities currently available include:

- **Surfacing Miro information:** Locate specific Miro boards and content seamlessly integrated within Microsoft Teams and Microsoft Word. For example, find boards used in a particular meeting or within a defined timeframe, ensuring relevant visual context is readily available during discussions.
- **Transforming ideas into Miro content:** Convert conversations and AI-generated insights from Microsoft tools into visual Miro formats, such as documents, diagrams, or sticky notes. This bridges the gap from unstructured discussions in Teams or Word to structured, visual, and collaborative formats within Miro.

| Feature | Description | Integration points | Use case | Miro output | Example prompt |
| --- | --- | --- | --- | --- | --- |
| Find Miro boards | Locate specific Miro boards or content based on criteria like meeting context or timeframe directly within Microsoft Teams and Word. | Microsoft Teams, Microsoft Word | Quickly retrieve relevant visual context for ongoing discussions or document creation, saving time and ensuring alignment without switching applications. | Existing Miro boards/content | Find the Miro board from our last marketing sync meeting. |
| Transform ideas to visuals | Convert conversations and AI-generated insights from Microsoft tools into visual diagrams or sticky notes within Miro. | Microsoft Teams, Microsoft Word | Rapidly visualize and structure ideas from discussions, facilitating brainstorming, planning, and immediate collaborative action by moving from unstructured text to organized visual formats. | New Miro diagrams, sticky notes | Turn this Teams chat about project requirements into a Miro diagram. |

## Set up the Miro agent for Copilot

To begin using the Miro agent with Microsoft Copilot, you'll first need to ensure Miro is connected to your Microsoft Teams account, and then enable the agent within Copilot. The initial setup requires a one-time authorization process to connect your Miro account.

### Connect Miro to Microsoft Teams (prerequisite)

Before you can enable the Miro agent in Copilot, you must add the Miro application to Microsoft Teams and connect your Miro account. If you haven't done this already, follow these steps:

:::note
Your Microsoft admin may need to enable this app for your organization before you can add it to Teams.
:::

1. In Microsoft Teams, select the **Apps** icon (often shown as a **+** symbol or a grid icon).
   The **Apps** panel will open.
2. In the search bar within the Apps panel, search for "Miro".
3. From the search results, find Miro and select **Add**.
   The Miro app installation modal will open.
4. Select **Add** again in the modal.
   You will be redirected to the Miro app view within Microsoft Teams.
5. From the Miro app view, follow the prompts to log in to your Miro account.
   Once logged in, your Miro account will be connected to Microsoft Teams.

   You have now successfully added the Miro app to Microsoft Teams and connected your account.

### Enable the Miro agent in Copilot

Once Miro is connected to Microsoft Teams, you can enable the Miro agent directly within Microsoft Copilot:

1. In Microsoft Copilot, locate the chat dialog box and select the plugin menu icon (this may look like a puzzle piece or similar icon indicating plugins).
   The **Plugins** dialog or panel will open.
2. In the Plugins dialog, search for "Miro".
3. Find the Miro agent in the list and toggle the switch next to it to the **on** position.

   You have now successfully enabled the Miro agent for Microsoft Copilot.

## Using the Miro agent for Copilot

Once you have completed the setup, you can start using the Miro agent with natural language prompts. The agent searches through board titles and metadata to help you find relevant content. Here are some example ways to interact with the agent:

- **Find boards by topic**
  Example prompts: "Find boards about Copilot" or "Show me boards related to project planning"
- **Search by timeframe**
  Example prompts: "Find boards created last week" or "Show me recently modified boards"
- **Transform conversations**
  Example prompts: "Turn this Teams chat about project requirements into a Miro diagram"
- **Create visual content**
  Example prompts: "Convert these meeting notes into sticky notes on a Miro board"

:::note
During your first use, you'll need to complete a one-time authorization process to connect your Miro account.
:::

## Security and compliance

The Miro agent in Microsoft Copilot is built with enterprise security and compliance requirements in mind:

- **Data privacy:** The agent operates within Microsoft's established security framework and follows enterprise data handling protocols.
- **Access control:** Users can only access Miro content they have permissions to view, maintaining existing security boundaries.
- **Authentication:** The integration leverages your existing Microsoft and Miro authentication, ensuring secure access without additional credential management.
- **Compliance:** The solution is designed to work within your organization's existing compliance policies and frameworks.

IT administrators can manage the Miro agent through standard Microsoft 365 admin controls, ensuring consistent governance across your organization's AI tools.

To learn more about technical implementation, application scopes, authentication, data flows, and permissions, see [this documentation](https://docs.google.com/document/d/14-oe6MUW5m7UURI0exfTphJKmkbrrsQkKlx9oJmgtJw/edit?tab=t.0#heading=h.wrqab64dlwec).

To learn more about adding and managing apps in Microsoft Teams, see the [official Microsoft support documentation](https://support.microsoft.com/office/add-an-app-to-microsoft-teams-b2217706-f7ed-4e64-8e96-c413afd02f77).
