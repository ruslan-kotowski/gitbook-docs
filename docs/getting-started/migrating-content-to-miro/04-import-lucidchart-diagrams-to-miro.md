---
title: Import Lucidchart diagrams to Miro
article_id: 11840840023058
sidebar_position: 6
created_at: '2023-06-06T08:50:22Z'
updated_at: '2025-11-25T15:37:28Z'
draft: false
availability:
  roles: all_users
  plans: starter, business, enterprise, education
  platforms: browser, desktop
---

You can import your diagrams from Lucidchart into Miro to collaborate with your team and use Miro's extensive features. This guide shows you two ways to import your content: from a Miro board or directly from your dashboard.

:::warning
Editing imported content is a one-way process. Any changes you make in Miro will not be synchronized back to Lucidchart.
:::

:::note
You can migrate Lucidchart boards that are under a Free or Restricted license.
:::

## Import from a Miro board

Follow these steps to import your Lucidchart diagrams while you are working on a Miro board.

1. In Lucidchart, export the diagram you want in **VSDX** format and save the file to your device.
2. Open the Miro board where you want to add the diagram.
3. On the creation toolbar on the left, click **Shapes** (![icon-shapes.svg](images/25121485636114_icon-shapes.svg)), select **More shapes**, and then click the **Import diagram** icon at the top right of the diagramming panel.
4. In the import dialog, drag and drop the `.vsdx` file you exported from Lucidchart, or click **Choose file** to select it manually. You can import multiple files at once.
5. Click **Import**. A new board is created for each imported `.vsdx` file.

:::note
While most content transfers smoothly, you may need to make minor adjustments to styling and formatting. See the [How Lucidchart objects appear in Miro](#how-lucidchart-objects-appear-in-miro) section for more details.
:::

## Import from the Miro dashboard

You can also import your diagrams directly from your Miro dashboard without opening a board first.

1. In Lucidchart, export your diagram as a `.vsdx` file by going to **File > Export >** `.vsdx`.
2. Go to your Miro dashboard.
3. Click the **Create new** button, select **Import**, and then choose **Import from Lucidchart**.
4. In the window that opens, either drag and drop your `.vsdx` file(s) or click **Browse** to select them.
5. (Optional) Use the **Choose Space** dropdown to select a [Space](../../using-miro/spaces/01-spaces.md) for your imported boards. If you don't choose one, the boards will be added to your main team space.
6. Click **Create boards** to begin the import.
7. A message will confirm that the import is in progress. You'll receive an email notification when your new Miro boards are ready.

## How Lucidchart objects appear in Miro

Due to differences between the platforms, some Lucidchart objects are converted into different types of objects in Miro. This table provides a comprehensive comparison.

|  |  |
| --- | --- |
| **Lucidchart** | **Miro** |
| Block | Text, Shapes |
| Containers | Shapes |
| Documents | 🟠 Can be recreated manually |
| Diagram Key | Text, Shapes |
| Frames | Frames and Shapes |
| GIFs | Images |
| Hotspot | Link to |
| Images | Images |
| Line | Connectors |
| Org Charts | Shapes, Images |
| Shapes | Shapes |
| Smart Containers | Shapes |
| Smart Table | Shapes |
| Sticky Note | Sticky notes |
| Tables | Shapes |
| Text | Text |
| Timeline | Shapes |
| Visual Activities | Shapes |
| **Other properties** | |
| Authors | 🟠 Can be recreated manually |
| Collaborators and sharing | 🟠 Can be recreated manually |
| Comments | 🟠 Can be recreated manually |
| Grouping | Imported |
| Icon Sets | Attached to Shapes |
| Layers | 🟠 Can be recreated manually |
| Link To | Imported |
| Lock | 🟠 Can be recreated manually |
| Notes/Annotations | 🟠 Can be recreated manually |
| **Shapes** | |
| **Lucidchart Shape Packs** | **Miro Shapes** |
| AWS Architecture | Shapes > AWS |
| Azure | Shapes > Azure |
| BPMN 2.0 | Shapes > BPMN |
| Circuit Diagrams | Imported and editable, but not available in the Miro shape library |
| Data Flow | Shapes > Data Flow |
| Dynamic Shapes | Imported and editable, but not available in the Miro shape library |
| Enterprise Architecture | Imported and editable, but not available in the Miro shape library |
| Enterprise Integration | Imported and editable, but not available in the Miro shape library |
| Entity Relationship | Shapes > ERD |
| Equations | Imported and editable, but not available in the Miro shape library |
| Floor Plans | Imported and editable, but not available in the Miro shape library |
| Flowchart Shapes | Shapes > Flowchart |
| Geometric Shapes | Shapes |
| Google Cloud Platform | Shapes > GCP |
| Kubernetes | Shapes > Kuberenetes |
| MindMaps | MindMaps |
| Network Infrastructure | Imported and editable, but not available in the Miro shape library |
| Process Engineering | Imported and editable, but not available in the Miro shape library |
| Salesforce Architecture | Shapes > Salesforce |
| Server Rack Diagrams | Imported and editable, but not available in the Miro shape library |
| Site Maps | Imported and editable, but not available in the Miro shape library |
| Standard Shapes | Shapes |
| Tech Clipart | Imported and editable, but not available in the Miro shape library |
| UI Mockups | Imported and editable, but not available in the Miro shape library |
| UML | Shapes > UML |
| Value Stream | Shapes > Value Stream Mapping |
| Venn Diagrams | Imported and editable, but not available in the Miro shape library |

## Limitations

While Lucidchart and Miro offer similar functionalities, some differences may exist:

- Miro Text boxes can accommodate up to 6,000 characters, including spaces. Any additional text will be cropped.
- Miro Sticky notes do not support rotation, color palette adjustments, or text bulleting.
- Some shape packs available in Lucidchart are not in Miro. These can still be imported, and users can duplicate and edit these shapes. However, they won't be available via Miro's shape library.
- Comments, notes, and annotations cannot be migrated from Lucidchart to Miro as Lucidchart does not export them.

:::note
For further questions and support around Lucidchart migration, please contact [Miro Support](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) or reach out to your Miro Customer Success Manager directly.
:::
