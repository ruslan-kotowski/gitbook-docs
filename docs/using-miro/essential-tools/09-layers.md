---
title: Layers
article_id: 20258488000786
sidebar_position: 8
created_at: '2024-07-19T16:48:16Z'
updated_at: '2025-11-25T15:44:35Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: layers
availability:
  roles: board_owner, Board co-owners, board_editor
  plans: free, starter, business, enterprise, education
  platforms: browser, desktop, Interactive displays
---

Layers give the ability to organize separate sections of content on the board, crucial for managing the complexity of diagrams and allowing for more precise and structured work.

## Accessing Layers

To access the **Layers panel**:

1. Click on the **Media, Tools and Integrations** (![icon-tools.svg](images/29032025125650_icon-tools.svg)) icon in the Creation toolbar.
2. Search for **Layers**, then click on the Layers tool.
3. You can keep the Layers tool in the Creation toolbar by right-clicking on the **Layers** icon and then selecting **Pin to toolbar**.

![layers-new-entry-point.png](images/22431635505426_layers-new-entry-point.png)

*The Layers menu is revealed by clicking on the Frames and layers icon*

When you click on the **Layers icon**, a panel will open on the right side of the canvas. Here, you can activate a Layer, name your existing Layers, or create new Layers.

![layers-panel.png](images/21594007565842_layers-panel.png)

*The Layers menu will appear on the right side of the Canvas*

### Who can use Layers

Functionality within Layers is based on user role.

- Viewers and commenters (including guests with those permissions) cannot access Layers.
- Editors (including guests with editor permissions) can create, edit, hide, and unhide Layers.
  - Editors invited by email also have the ability to lock and unlock Layers.
- Board owners and co-owners have all the abilities Editors have as well as being able to lock and unlock Layers and use the Protected Lock.

## Using Layers

Content can be selected and added to a new or existing layer, helping you keep related content organized.

1. Select the content you want to add to a new or existing layer.
2. Click on the **Layers** menu.
3. To add the content to a new layer: click on **+ Move to a new layer**. You can then rename the new layer.
4. To move the content to an existing layer: click on the **three dots** (**...**) next to the Layer name and choose **Move selection to layer**.

![layers-move-to.gif](images/21594007570962_layers-move-to.gif)

*Adding content to an existing layer*

When adding content that you want to be included in a particular layer, select the Layer first. New content will be added to that Layer automatically.

You can also add content to a new or existing Layer by:

1. Select the content you want to add.
2. Click the **three dots** (**...**) menu in the contextual menu.
3. Select the **Move to Layer** option.

![](images/21593982256018_803bbedc-722c-45ef-afb8-e9c46ba8a857.png)

*The **Move to layer** option can be found under the three dots (**...**) in the contextual menu*

Layers can be hidden, locked, renamed, or duplicated to suit your needs.

1. Click or hover over the Layer name in the Layer Menu.
2. To **Hide** a Layer: Click the **Eye icon** to hide the Layer. The icon will change from an open eye to a closed eye. Any content in the selected Layer will disappear from the canvas. (Note that the hidden content will disappear from canvas for all users, and will remain hidden on page reload.)
3. To unhide the Layer, click on the **Closed Eye icon**. Hidden content will reappear on the canvas.![layers-eye.png](images/21593982258450_layers-eye.png)
   *Hiding a layer is done with the Eye icon*
4. To **Lock** a Layer: Click the **Lock icon** to lock the layer. The icon will change from an open lock to a closed lock. When a Layer is locked, no edits can be made to the content within that Layer (including moving or deleting content).
5. Click the **Closed** **Lock icon** again to unlock the Layer’s content.![layers-lock.png](images/21594007576466_layers-lock.png)
   *The Lock icon is used to lock or unlock a Layer*
6. To **Duplicate** a Layer: Click on the three dots (**...**) on the right-hand side of the Layer.
7. Click on **Duplicate Layer**.
8. A second instance of your Layer will appear on the board, directly over the top of the original Layer.
9. To move the duplicated Layer, make sure that Layer is selected in the Layer Menu, then click on the Layer’s content on the canvas and drag to the desired location.
   ![layers-three-dots.png](images/21593982264594_layers-three-dots.png)
   *Duplicating a layer is done through the three dots (...) menu*

To rename a Layer:

1. Double-click on the Layer name in the Layer Menu.
2. Edit the name of the Layer.
3. Press Enter.

## Layers in Diagram format

Layers within the Diagram format function independently from canvas layers. This separation is designed to streamline the diagramming process and prevent confusion between general board content and the specific components of a diagram. To learn more about the specifics of how layers work within diagrams, please see our detailed article on the [Diagram format](../formats/diagramming/02-miro-diagrams.md).

- **Canvas vs. Diagram Layers**: While canvas layers are used for general purposes, such as presentations, layers within a Diagram are managed separately to organize the diagram's own elements.
- **Parenting**: Once an element is part of a Diagram, it cannot be added to a canvas layer because it is parented by the Diagram format itself.

## Reorder layers

Layers can be reordered in the panel, which affects which Layer’s content is displayed on top. To reorder the Layers, simply drag them within the Layers panel to whatever order you prefer.

This is a powerful tool for creating diagrams where you might need two versions of the same parts of a diagram, with slightly different content. By placing the Layers directly on top of each other, you can alter which one is displayed by reordering the Layers.

## The Default Layer

The Default Layer is always visible and new widgets are added to the Default if no other Layer is active. When you’re not working on any particular Layer, you’ll be working on the Default.

The Default Layer differs from other Layers because it cannot be hidden or locked.
