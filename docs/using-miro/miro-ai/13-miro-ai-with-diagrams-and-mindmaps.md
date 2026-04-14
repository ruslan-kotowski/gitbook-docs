---
title: Miro AI with Diagrams and mindmaps
article_id: 28782102127890
sidebar_position: 13
created_at: '2025-08-15T08:50:59Z'
updated_at: '2026-03-18T17:56:48Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: creation-toolbar
availability:
  roles: all_users
  plans: free, starter, business, enterprise, education
  platforms: browser, desktop, mobile
---

Use Miro AI to create diagrams or mindmaps from scratch. You can also digitize your hand-drawn diagrams into fully editable objects on the Miro board.

For information about Miro Prototypes, see [Miro Prototypes](https://help.miro.com/hc/articles/26654269713682).

## Create a diagram or mindmap

1. Above the Creation toolbar, select **Create with AI**.
   The **Create with AI** panel opens.
2. Click **Sidekicks library** (four-square button in the top-right) **>** **Formats** > **Diagram or mindmap**.
   The prompting panel opens.
3. Select a diagram type, or mindmap.
4. In the response box, describe the diagram or mindmap you want to create.

   > 💡 Select one of the starter prompts to begin your description.

   > 💡 Learn how Miro AI handles style and color input for diagrams. See [Style & color input for Miro AI diagrams](#style-color-input-for-miro-ai-diagrams).
5. Press **ENTER** on your keyboard, or click the response arrow.
   Miro AI generates a sketch diagram or mindmap on the board. To interrupt generation you can optionally click **STOP**, and repeat step 3.
6. Do one of the following:
   - Click **Apply to canvas**.
     Your diagram or mindmap is ready for you to edit. You have completed the procedure.
   - Click **Discard all**.
     Your sketch diagram or mindmap is erased and the **Create with AI** panel resets.
   - In the **Create with AI** sidebar, continue to describe your diagram or mindmap, and repeat step 6 until you have applied your diagram or mindmap to the board.

## Digitize hand-drawn diagrams

Miro AI includes Digitize Diagram (BETA), a feature that converts your hand-drawn diagram sketches into fully editable diagrams on your board.

Follow these steps:

1. Upload an image of your hand-drawn diagram to a Miro board.
2. Select the image.
   The context menu displays.
3. From the context menu, click **Convert to**.
4. Select **Diagram** from the menu.
   Miro AI generates a fully editable version of your diagram. Ensure that you inspect the result and make any necessary adjustments or re-alignment.

## Style & color input for Miro AI diagrams

Miro AI responds to semantic style input. For example, in your prompt you can describe an aesthetic or specify a preferred style. Miro AI generates your diagram or mindmap based on your description or preference and ensures all properties correspond. You can continue to prompt or manually edit to refine your output.

The following table shows how Miro AI gives output based on your prompt for diagrams.

| Use case | Description | AI action | Color palette | Border color |
| --- | --- | --- | --- | --- |
| **No color input** | You do not give any color preference or specification, e.g. "Create a flowchart" | System uses default color palette | Sunshine yellow, Ocean blue, and Moss green | Each element gets an appropriate, higher-contrast border color |
| **Vague color input** | You give an aesthetic preference or theme, e.g. "Create an orange diagram" | System uses your preference as input and matches color to Miro muted color palette optimized for accessibility | In this example, Miro AI generates a diagram with muted orange | In this example, Miro AI generates a matching, higher-contrast orange border |
| **Specific color input** | You give HEX or RGB values to specify brand colors, e.g. "Generate UML sequence...in color #006FF" | Overrides system defaults | Complies to values specified in request | Miro automatically creates an appropriate, higher-contrast border color based on your specified shape or color |
