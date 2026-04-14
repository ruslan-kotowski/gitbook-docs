---
title: Custom Shapes for Diagramming
article_id: 20352896814866
sidebar_position: 16
created_at: '2024-07-24T19:52:05Z'
updated_at: '2026-04-07T14:09:20Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: Desktop and interactive displays
backstage_link:
  entity_kind: capability
  entity_id: custom-shapes
---

Custom shape packs enable you to tailor diagrams to specific industry or project needs, improving clarity and relevance.

## Accessing and uploading custom shapes

Access the custom shapes menu by clicking the **Shapes and lines** tool on the creation toolbar and selecting **More shapes.** From here, upload custom shapes directly from the panel by clicking **Browse and upload shapes**. Alternatively, you can add shapes by hovering over the **My Shapes** title and then clicking the **Add shapes** icon.

Each shape pack can contain up to 100 shapes of max 50KB per file in SVG format.

![custom-shapes-add-shapes.png](images/22251929558034_custom-shapes-add-shapes.png)

*Ways to add custom shapes*

### Preparing custom shapes for upload

To ensure a smooth diagramming experience when mixing Miro's built-in shapes with your own custom shapes, follow these sizing guidelines:

- Icons in Miro's built-in shape packs have a default size of **80x80px** to fit Miro's grid. For consistency, design your custom shapes at a similar size.
- SVG shapes use the size specified in their code (the `width` and `height` attributes). If your SVG specifies a size smaller than 80x80 (for example, `width="32" height="32"`), Miro scales it up to 80x80, which may produce inconsistent results when diagramming.
- To control the exact size of your shapes on the board, set the desired `width` and `height` values directly in your SVG file before uploading.
- If your shapes have a non-square aspect ratio (for example, wide rectangles or tall icons), specify the intended dimensions in the SVG and Miro will respect them.

## Edit a custom shape pack

First, click **More shapes** and select **Manage shapes.**From here you can:

- Rename your custom shape pack.
- Reorder the list of custom shapes.
- Toggle **Show shape name on board**.
- Rename custom shapes.
- Delete custom shapes.

Click the **three dots** (**...**) to rename the shape pack and toggle on or off the **Show shape name on board**. New shapes added to the board will now display their name. Additionally, when this toggle is on, edit custom shape names by double clicking on the text in the **Manage shapes** menu.

![custom-shapes-my-shapes.png](images/22251929564946_custom-shapes-my-shapes.png)

*You can edit the name of a shape pack and select whether to show the name*

Reorder the shapes by clicking and dragging the shapes.

To delete a custom shape from your shape pack, select a shape and click **Delete** at the bottom of the **Manage shapes** panel. Hold the shift key to select multiple shapes and delete them all at once.

### Share a custom shape pack

Custom shape packs can be shared with all users inside your organization. Use the dropdown in the **My Shapes** panel to share the custom shape pack.

![custom-shapes-access.png](images/22251929568786_custom-shapes-access.png)

### Using shapes from a custom shape pack

As long as the shape pack is selected in the **More shapes** menu, icons within it will appear in the **Diagramming** panel.

![ScreenRecording2024-09-26at9.31.42PM-ezgif.com-optimize.gif](images/21789157995410_ScreenRecording2024-09-26at9.31.42PM-ezgif.com-optimize.gif)

*Accessing custom shapes through the **More shapes** panel*

## Frequently asked questions

**How do I access custom shapes other users have shared with my organization?**

You'll need to enable the individual custom shape packs in order to use them. You can find the list of available custom shapes in the diagramming shapes side panel. Click the checkbox next to each pack to enable/disable the custom shapes.

**Can admins restrict which custom shape packs are shared within an organization?**

Users with the content admin role can manage any shared custom shape packs, including editing, removing, or unsharing them. This is done in the **Manage shapes** dialog, accessed through the diagramming shapes panel.
