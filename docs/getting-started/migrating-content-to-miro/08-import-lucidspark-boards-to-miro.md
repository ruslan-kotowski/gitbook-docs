---
title: Import Lucidspark boards to Miro
article_id: 9549014537490
sidebar_position: 7
created_at: '2023-01-12T09:05:07Z'
updated_at: '2026-01-19T14:30:13Z'
draft: false
availability:
  roles: Any user with edit access to both Lucidspark and Miro boards
  plans: free, starter, business, education, enterprise
  platforms: browser, desktop
---

Migrate your Lucidspark content seamlessly into Miro for a more robust collaboration experience. This guide outlines how to import your boards and what to expect during the process.

:::warning
Editing imported content is one-way. Changes made in Miro will not sync back to Lucidspark.
:::

:::note
Lucidspark boards under Free or Restricted licenses can be migrated.
:::

## How to import Lucidspark boards via PDF export

Follow these steps to import your Lucidspark boards into Miro using the PDF export method:

1. Ensure that you export the **Lucidspark** content that you want to import to Miro as a PDF.
2. On the Miro **Home** dashboard, click **+ Create new**.
3. Select **Import**, then **Import from Lucidspark**.
   The **Import from Lucidspark** modal opens. You can bulk import several Lucidspark PDFs.
4. Follow the on-screen instructions provided in the modal.
5. Select **Import boards**.
6. Review the imported content and make any necessary adjustments. While Lucidspark and Miro have similar functionalities, there still may be differences in styling and formatting options. Refer to [How Lucidspark objects appear in Miro (Bulk PDF Import Method)](#lucidspark-object-mapping-bulk-import) for guidance on how objects are translated.

## Alternative method: Copy and paste content

As a quicker alternative for smaller amounts of content, you can directly copy elements from an open Lucidspark board and paste them onto a Miro board.

:::note
Any user with edit access to both the Lucidspark and Miro boards should be able to copy content from Lucidspark and paste it into Miro. For details on how objects are translated with this method, see [How Lucidspark objects appear in Miro (Copy/Paste Method)](#lucidspark-object-mapping-copy-paste).
:::

## How Lucidspark objects appear in Miro (Copy/Paste Method)

This table provides a comprehensive comparison of how objects are translated when you copy content directly from Lucidspark and paste it into Miro.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Azure Cards | Azure cards are migrated as Miro Cards: 1. Setup Azure integration in Miro. 2. Convert the Miro Cards to [Azure cards](../../integrations-apps/microsoft/03-azure-cards.md). |
| Collaborators and sharing | 🟠 Can be recreated manually |
| Comments | 🟠 Can be recreated manually |
| Connectors & Dividers | Connectors |
| Containers | Shapes |
| Documents from Files and URLs | 🟠 Can be recreated manually |
| Documents URLs (PDF) | Embedded documents |
| Draw | Images |
| Dynamic Tables | Tables |
| Emojis | Images |
| Frames | Frames |
| GIFs from Toolbar | Images |
| GIFs from Files | Images |
| GIFs from URLs | GIFs |
| Images | Images |
| Jira Cards | Jira cards are migrated as Miro Cards:  1. Setup Jira integration in Miro 2. Convert the Miro Cards to [Jira cards](../../integrations-apps/atlassian/03-jira-cards.md). |
| Lucid Cards | Cards |
| Mindmap | Mindmap |
| Shapes | Shapes |
| Sticky note | Sticky notes |
| Tables | Tables |
| Text | Text |
| Timeline | 🟠 Can be recreated manually |
| Videos and other URLs | Previews |

## How Lucidspark objects appear in Miro (Bulk PDF Import Method)

This table provides a comprehensive comparison of objects between Lucidspark and Miro after bulk importing your content via PDF.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Azure Cards | Images |
| Collaborators and sharing | 🟠 Can be recreated manually |
| Comments | 🟠 Can be recreated manually |
| Connectors & Dividers | Connectors |
| Containers | Shapes |
| Documents | 🟠 Can be recreated manually |
| Draw | Lines |
| Dynamic Tables | Shapes and Connectors |
| Emojis | Images |
| Frames | Frames and Shapes |
| GIFs | Images |
| Images | Images |
| Jira Cards | Shapes |
| Lucid Cards | Shapes |
| Mindmap | Shapes and Connectors |
| Shapes | Shapes |
| Sticky note | Sticky notes |
| Tables | Tables/Shapes and Connectors |
| Text | Text |
| Timeline | Shapes and Connectors |
| Videos and other URLs | 🟠 Can be recreated manually |

## Limitations of the import

While Lucidspark and Miro offer similar functionalities, be aware of the following differences and limitations when importing content:

- Miro Text boxes can accommodate up to 6,000 characters, including spaces. Any additional text will be cropped.
- Colors and styles are mapped to the nearest matches in Miro.
- Opacity values from Lucidspark are not accurately extracted during import.
- Miro sticky notes do not support rotation, color palette adjustments, or text bulleting that may have been applied in Lucidspark.

## Getting help

:::note
For further questions and support around Lucidspark migration, please contact [Miro Support](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) or reach out to your Miro Customer Success Manager directly.
:::
