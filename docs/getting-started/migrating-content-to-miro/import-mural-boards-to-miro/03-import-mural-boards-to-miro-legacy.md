---
title: Import Mural boards to Miro (legacy)
article_id: 9549320965138
sidebar_position: 3
created_at: '2023-01-12T09:20:54Z'
updated_at: '2025-11-25T16:09:50Z'
draft: false
availability:
  roles: Users with edit access to both Mural and Miro
  plans: free, starter, business, education, and Enterprise plans (for copy-paste);
    Starter, enterprise
  platforms: browser, desktop
---

:::warning
Please note that this article is set to be archived. For the most up-to-date information on importing Mural content to Miro, please see the [Mural to Miro import guide – PDF](02-mural-to-miro-import-guide-–-pdf.md) or the [Mural to Miro import guide – Copy-paste](01-mural-to-miro-import-guide-–-copy-paste.md).
:::

You can seamlessly transfer your content from Mural to Miro, allowing you to continue your collaborative work with familiar content in a new environment. This guide outlines two methods for importing your Mural boards: by copying and pasting content directly, or by using the bulk import feature with PDF files.

:::warning
Editing imported content is a one-way process. Changes made in Miro will not be synchronized back to Mural.
:::

:::note
Mural boards under a Full or Free Restricted license can be migrated to Miro using these methods.
:::

## Import Mural content by copying and pasting

You can manually copy content from a Mural board and paste it into a Miro board. This method is suitable for migrating individual boards or specific content selections.

:::note
Any user with edit access to both the source Mural board and the target Miro board can perform this action.
:::

1. Open the Mural board that contains the content you wish to export.
2. Select all the content you want to move. You can use the keyboard shortcut **Ctrl + A** (Windows) or **Command + A** (Mac) to select everything on the board.
3. Right-click on the selected content and choose **Copy**, or use the keyboard shortcut **Ctrl + C** (Windows) or **Command + C** (Mac).
4. Open an existing Miro board or create a new one where you want to import the content.
5. Right-click on an empty area of the Miro board and select **Paste**, or use the keyboard shortcut **Ctrl + V** (Windows) or **Command + V** (Mac).
6. Review the imported content on your Miro board. You may need to make adjustments, as there can be differences in styling and formatting options between Mural and Miro. Refer to the [How Mural objects appear in Miro (Copy-paste)](#how-mural-objects-appear-in-miro-copy-paste) section for more details on object mapping.

## Import Mural boards in bulk using PDF export

For migrating multiple Mural boards, you can use Miro's bulk import feature, which accepts PDF exports from Mural.

> This bulk import feature is available for users on Starter, Business, Education, and Enterprise plans.

1. Access the Mural boards you wish to export.
2. For each Mural board, click **Download as** and save the board as a **PDF** file.
3. Open your Miro dashboard.
4. In the upper-right corner, click the **+ Create new** button, and then choose **Import**.
5. Select **Import from Mural** from the options.
6. In the modal window that appears, you can either click **Browse** to open your system's file picker and select your PDF files, or you can drag and drop your PDF files directly into the modal.
7. (Optional) Use the **Add your boards to a space** dropdown menu to select a specific [Space](../../../using-miro/spaces/01-spaces.md) in Miro where your imported boards will be added. If you do not select a space, the boards will be added to your main Team area by default.
8. Click the **Import boards** button to begin the import process.
9. A modal window will inform you that the boards are being imported. You will receive an email notification once the import is complete and your new Miro boards are ready to use.
10. After import, review the content on your new Miro boards. Refer to the How Mural objects appear in Miro (Bulk import via PDF) section for guidance on how Mural objects are translated.

## How Mural objects appear in Miro (Copy-paste)

This table provides a comparison of how Mural objects are typically translated when you copy and paste content into Miro.

|  |  |
| --- | --- |
| **Mural Object** | **Equivalent Miro Object (Copy-Paste)** |
| Areas | Frames |
| Collaborators and sharing | 🟠 Can be recreated manually in Miro |
| Comments | 🟠 Can be recreated manually in Miro |
| Connectors | Connectors |
| Documents from Files or URLs | 🟠 Can be recreated manually in Miro |
| Documents from URLs (PDF) | Embedded documents |
| Draw | 🟠 Can be recreated manually in Miro |
| GIFs and images from Toolbar | 🟠 Can be recreated manually in Miro |
| GIFs and images from Files | 🟠 Can be recreated manually in Miro |
| GIFs from URLs | GIFs |
| Images from URL | Images |
| Mindmap | Mindmap |
| Shapes | Shapes |
| Sticky Notes | Sticky Notes |
| Tables | Tables |
| Text | Text |
| Videos and other URLs | Previews (for supported URLs) |

## How Mural objects appear in Miro (Bulk import via PDF)

This table shows how Mural objects are generally converted when you import Mural boards as PDF files into Miro.

|  |  |
| --- | --- |
| **Mural Object** | **Equivalent Miro Object (Bulk Import via PDF)** |
| Areas | Frames and Shapes |
| Collaborators and sharing | 🟠 Can be recreated manually in Miro |
| Comments | 🟠 Can be recreated manually in Miro |
| Connectors | Connectors |
| Documents | 🟠 Can be recreated manually in Miro (often imported as images) |
| Draw | Lines (imported as part of the PDF image) |
| GIFs | Images (static representation from PDF) |
| Images | Images |
| Mindmap | Shapes and Connectors (if recognized) or as part of the PDF image |
| Shapes | Shapes and images |
| Sticky Notes | Sticky Notes (text may be part of an image if not recognized) |
| Tables | Tables/Shapes and Connectors (if recognized) or as part of the PDF image |
| Text | Text (may be part of an image if not recognized) |
| Videos and other URLs | 🟠 Can be recreated manually in Miro (links may not be active) |

## Limitations and considerations

While Miro strives to make the import process as smooth as possible, be aware of the following limitations when migrating content from Mural:

- **Text limits:** Miro Text boxes can accommodate up to 6,000 characters (including spaces). Any text exceeding this limit will be cropped upon import.
- **Sticky note shapes:** Circular sticky notes from Mural will be converted to square sticky notes in Miro.
- **Colors and opacity:** Colors and opacity levels from Mural are mapped to the nearest available matches in Miro. Some visual differences may occur.
- **Sticky note formatting:** Miro sticky notes do not currently support rotation, custom color palette adjustments beyond the standard set, or text bulleting within the sticky note itself.

### Compare Mural and Miro content structure

Understanding the differences in how content is organized in Mural versus Miro can help you plan your migration more effectively.

|  |  |
| --- | --- |
| **Mural Element** | **Miro Equivalent** |
| Workspace:  - Created by Company Admins - Managed by Team Admins | Team:  - Created by Company Admins - Managed by Team Admins |
| Rooms:  - Created by users within a Mural Workspace - Managed by users | Spaces:  - Created by users within a Miro Team - Managed by users - Cannot be nested |
| Folders:  - Created by users within a Mural Workspace - Managed by users - Can be nested in Rooms | Projects (can be used for organization, but Miro Spaces are the primary container within a Team. Miro does not have a direct equivalent to Mural's nested folders within Rooms.) |
| Murals (boards):  - Created by users within a Mural Workspace - Managed by users | Boards:  - Created by users within a Miro Team - Managed by users |

## Further assistance

:::note
For further questions and support regarding Mural migration, please contact [Miro Support](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) or reach out to your Miro Customer Success Manager directly if you have one.
:::
