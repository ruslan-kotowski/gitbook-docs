---
title: Importing Freehand boards to Miro
article_id: 18580556555538
sidebar_position: 9
created_at: '2024-04-26T16:34:28Z'
updated_at: '2025-11-25T15:42:02Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  roles: All users with eligible plans
  plans: starter, business, education, enterprise
  platforms: browser, desktop, mobile
---

This article explains how to import Freehand boards to Miro, including how to prepare your Freehand boards, for single and bulk imports.

:::note
Edits you make to imported content in Miro do not sync with their original content in Freehand.
:::

:::note
You can only import Freehand boards which are under Free or Restricted licenses.
:::

## Import a single board from Freehand to Miro

You can easily import individual Freehand boards into Miro by exporting them in Miro's `.RTB` file format. Here's how to do it:

1. Access the Freehand board you wish to export to Miro.
2. Download the file in .RTB, Miro's proprietary format, directly from Freehand. Navigate to the **Tools** menu and select **Export to Miro board**. The file will be saved to your default download folder. Freehand will notify you once the download is complete.
3. Open your Miro dashboard.
4. On the top-right area of the Miro dashboard, click the **+ Create new** button, click **Import**, and then click **Import backup**.
5. Choose the previously downloaded `.RTB` file from your system.
6. All content is now imported into a new Miro board in an editable format.
7. While most content will seamlessly transition, minor adjustments may be necessary due to variations in styling and formatting options between Freehand and Miro. Refer to [Understand Freehand object mapping in Miro](#object-mapping-in-miro) for guidance on potential differences.

## Bulk import multiple files from Freehand to Miro

For migrating multiple Freehand boards at once, Miro provides a bulk import process. First, ensure your Freehand boards are prepared correctly.

**Prerequisites: Prepare your Freehand boards for bulk import**

Follow these steps in Freehand to prepare your boards:

1. In Freehand, on the left-panel menu bar select **Documents**. A dropdown menu opens.
2. Select **All Documents** or **Created by Me**, and specify the timeframe for the boards you want to import to Miro.
3. For each board you want to import, select the three dots (**...**) and choose **Select**.
4. On the dialog at the bottom of your screen, select **Move**.
5. Select a space to move your boards. This consolidates them for easier processing by the bulk import tool.

   You have successfully prepared multiple files for bulk import to Miro.

To perform the bulk import of your prepared Freehand boards to Miro, follow the instructions provided in the following embedded Miro board guide:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1IT00=/?pres=1&amp;frameId=3458764590689727256&amp;embedId=507813406404&amp;&amp;autoplay=yep" width="100%"></iframe>

:::note
Important Notes for Bulk Import:
- The Freehand token used for bulk migration is valid only for two weeks from the date you received it.
- From December 31, 2024, at 11:59 PM EST onwards, Freehand and all associated migration tokens will be discontinued and invalidated. Users will no longer be able to generate new tokens or access Freehand for migration.
:::

## Review best practices

For a smooth migration experience, it's important to understand best practices and key considerations when moving your content from Freehand to Miro. Please review the detailed guidance in the embedded Miro board below:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1FWSM=/?pres=1&amp;frameId=3458764590691451227&amp;embedId=480338444592&amp;autoplay=yep" width="100%"></iframe>

## Object mapping in Miro

This table provides a comprehensive comparison of how objects from Freehand are typically imported and represented in Miro, along with notes on any manual adjustments that may be needed:

|  |  |  |
| --- | --- | --- |
| **Freehand** | **Miro** | **Touchups needed** |
| Boards | Kanban | None |
| Cards | Cards | Jira cards in Freehand will be imported as Jira cards in Miro. However, they will not be connected to the existing instance as users will need to re-authenticate their Jira accounts in Miro.    ADO, Trello, Asana cards are not supported. |
| Collaborators and sharing | Can be recreated manually | None |
| Comments | Can be recreated manually | None |
| Connectors/Lines | Connectors/Lines | None |
| Drawings/Diagrams/Shapes | Shapes, Text and Connectors | None |
| Dynamic data tables | CSV | Content can be downloaded and edited as a .CSV file from the Miro board. |
| Embeds:    Google and Microsoft Docs, YouTube, Spotify, Loom | Name of the source (e.g. Google, YouTube) and the URL for the embed | If users wish to re-embed a document they can [Upload via URL](../../using-miro/import-and-export/import/05-uploading-files-to-boards.md#adding-files-via-url-links). |
| Emoji reactions | Can be recreated manually | None |
| Frames | Frames | None |
| Grids (tables) | Tables | None |
| Grouped objects | Ungrouped objects | To regroup objects, select all relevant objects and press **Cmd/Ctrl + G**, or click **Group objects** from the context menu. |
| Images | Images | None |
| Pages | Embedded doc | Content can be downloaded and edited as a .docx file from the Miro board. |
| Prototypes | Name of the source (InVision) and the URL for the embed | If users wish to re-embed a document they can Upload via URL to re-embed. |
| Smart widgets:    Flip card, Poll, This or That, Charts, Counter, Leaderboard, Spinner, Buzzer, People, Story Points, T-Shirt Size, Timer, Action Buttons | PNG of the smart widget at time of import is created | Content is not editable. |
| Sticky notes | Sticky notes | Font sizes of text within sticky notes may need to be adjusted. |
| Timeline (Gantt) | CSV | Content can be downloaded and edited as a .CSV file from the Miro board. |
| Wireframes | Wireframes | Some objects may need to be redrawn. |

## Key limitations

Be aware of the following limitations and structural differences when migrating your content from Freehand to Miro to ensure a smoother transition:

- Miro Text boxes can accommodate up to 6,000 characters, including spaces. Any additional text will be cropped.
- Miro Sticky notes do not support color palette adjustments or text bulleting in the same way as Freehand; some formatting may differ.
- Freehand Smart widgets are imported as static images (PNGs) and are not editable in Miro.
- Comments, emoji reactions, and prototypes from Freehand are not migrated to Miro.
- The Freehand token required for bulk import is valid only for two weeks from the date you received it.
- From December 31, 2024, at 11:59 PM EST onwards, Freehand and all associated migration tokens will be discontinued and invalidated. Users will no longer be able to generate new tokens or access Freehand.

### Compare organizational structure between Freehand and Miro

To effectively plan your migration, it's important to understand how the organizational structures in Freehand correspond to those in Miro:

**Freehand organizational layers**

- Teams: Each subdomain you have access to in InVision is considered a Team. If you only have access to one subdomain, you have one team.
- Groups: Document folders that aid in grouping and sharing documents across your team.
- Spaces: An additional layer of organization within groups for your documents.

:::note
If your team utilized the Space overview capability in Freehand, you will need to manually migrate this content to Miro. We recommend copying Space overview content to a Miro board.
:::

**Miro organizational layers**

- Organizations: You typically only have access to a single organization in Miro.
- Teams: Shared workspaces where users collaborate on boards and Projects (formerly known as Spaces in some contexts, be mindful of Miro's evolving terminology; generally, Teams are the primary collaborative workspace).
- Projects: Collections of boards within a team, facilitating organization, retrieval, and sharing of boards.

Consider your InVision Groups to be roughly equivalent to Miro Projects (or what might have been conceptually similar to folders/spaces for organizing boards within a team). For each InVision Group you plan to migrate, we recommend creating a Miro Project with the same name. For example, if you had an InVision group named "Acme Corp Relaunch Project," we suggest setting up a Miro Project with the identical name, "Acme Corp Relaunch Project" within the appropriate Miro Team.

:::tip
For further questions around Freehand migration, please contact [Miro Support](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md#how-to-contact-miro-support) or reach out to your Miro Customer Success Manager directly.
:::
