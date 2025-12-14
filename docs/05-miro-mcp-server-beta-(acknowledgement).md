---
title: Miro MCP Server Beta (Acknowledgement)
article_id: 31621611644306
created_at: '2025-12-05T13:40:33Z'
updated_at: '2025-12-08T12:30:22Z'
draft: false
position: 4
---

Your use of the Miro [MCP Server][1] Beta is subject to Section 16 (Trial and Beta Access) of Miro’s [Master Cloud Agreement][2], or similar Beta provision in the agreement applicable between you and Miro. Some of the setup and functionality of Miro MCP Server may change throughout the Beta. Please review our MCP [documentation][3] or access our [Help Center][4] carefully.

## **Miro MCP Server**

Miro’s MCP Server, when connected and authorized by a user, allows a third-party AI Agent to interact with content on Miro boards that the authorized user has [access][5] to.

Our MCP Server has a set of [tools][6] that allow the AI Agent to read and write content on selected Miro boards. Miro MCPs current design requires that users need to be explicit with which boards the third party AI Agent should be reviewing. The AI Agent will not be able to discover or read boards that the user hasn’t included in their prompts. Should this change in future iterations of Miro MCP, our documentation will be updated to reflect it.

## **Managing Miro MCP Server in your organization**

Once you have been approved for Miro’s MCP Server Beta, Miro will whitelist your Organization for access to MCP.

This Beta feature may contain bugs, errors, or other stability issues. Miro makes no commitments, representations, or warranties regarding the performance, availability, or fitness for any particular purpose. Miro’s service levels, security obligations, support obligations, and indemnities under the MCA (or other service agreement) do not apply.

Implementing Miro MCP into your organization requires an [Administrator][7] to install the Custom MCP App Access our documentation to see [here][8] how to install an App. When installing the App into your Miro environment, it’s important to consider how users within your organization can interact with the App. You can:

  1. **Enable the App for the entire Organization:** This means any user within your Organization can choose to access, connect and start using MCP with boards that they have access to. All Miro boards in your Organization may potentially be accessed via Miro MCP. Users will be able to prompt using boards in your Organization and will receive errors for boards that are inside separate organizations, unless they are made public. More information on board settings [here][9].
  2. **Enable the App for specific Teams:** If you enable Miro MCP only on a specific Team, only the users in that Team will be able to access and connect to Miro MCP. All Miro boards in your specific Team may potentially be accessed via Miro MCP.. More information on board settings [here][9].

## **Authorizing Miro MCP Server as a user**

Once Miro has been enabled for your Organization or for a specific Team, users will be able to connect to Miro MCP.

  1. Users can follow the detailed instructions for the different tools in our [documentation][10].
  2. Once a user has added Miro MCP to their tool of choice, they’ll be prompted to follow a standard [OAuth 2.1 flow for MCP Servers][11].
  3. Users will need to select a Team they are a member of that has had the Miro MCP App enabled. It is important that Administrators have authorized Miro MCP for the [selected Team][8].
  4. Once authorized, the user will be redirected back to their third party tool and can check to make sure the connection is completed, by accessing and viewing the Miro MCP Tools.
  5. Users will then be able to prompt their AI Agent to access the Tools in Miro’s MCP Server to perform actions on their behalf. These prompts must contain the Board URL for the AI Agent to understand which board it should be accessing, via the MCP Server. These prompts and the results are dictated by the end user and the LLM being the AI Agent respectively, not Miro.
    1. Actions performed by the AI Agent with Miro MCP Server include:
      1. Accessing and summarizing Board data
      2. Creating Miro Formats
    2. As Miro moves its MCP Server into Public Beta and General Availability, we may include additional Tools, allowing more actions to be done by the AI Agent.

## **Considerations**

Miro’s MCP tool was built following the standards outlined on [Anthropic’s][12] MCP documentation. According to the MCP Server Standards all data being sent to the MCP Server is being prepared by the MCP Client on the users side. Most modern tools allow the preview of data before it's being sent to the remote MCP Server and provide explicit grant for the tool-calling.

This is a Beta feature and we will be making improvements throughout the Beta to our MCP Server and the Tools that are available to customers. We will do our best to proactively update Beta customers and will keep our [documentation][3] up to date for what is available in our MCP Server.

## **Miro MCP Server Tools**

Tools are the actions that help an AI Agent interact with Miro. Certain tools inside Miro’s MCP Server will leverage Miro AI for better results, see table below. Here is the list of current Tools available and what they are used for. Check out our [documentation][10] for a list of tools as this list will change over time.

Tool name | Description | Uses Miro AI credits
---|---|---
board_get_items | Find specific items on a board | No
board_get_image_download_url | Download images from board | No
board_get_image_data | Find images on a board | No
context_get_board_docs | Summarize a board's information | Yes
draft_diagram_new | Create a new Diagram on a selected Miro Board | Yes

   [1]: <https://modelcontextprotocol.io/docs/getting-started/intro>
   [2]: <https://miro.com/legal/master-cloud-agreement/>
   [3]: <https://developers.miro.com/docs/miro-mcp>
   [4]: <https://help.miro.com/hc/en-us/>
   [5]: <https://help.miro.com/hc/en-us/articles/360017571514-User-access-levels-on-Enterprise-Plan>
   [6]: <https://modelcontextprotocol.io/specification/2025-06-18/server/tools>
   [7]: <https://help.miro.com/hc/en-us/articles/14766440626834-Understand-admin-roles-and-their-privileges>
   [8]: <https://help.miro.com/hc/en-us/articles/4404659741458-App-management>
   [9]: <https://help.miro.com/hc/en-us/articles/360017572194-Board-access-rights>
   [10]: <https://developers.miro.com/docs/connecting-miro-mcp-to-ai-coding-tools>
   [11]: <https://modelcontextprotocol.io/specification/2025-06-18/basic/authorization#communication-security>
   [12]: <https://modelcontextprotocol.io/docs/develop/build-server>
