---
title: Import OmniGraffle diagrams to Miro
article_id: 33541520646674
sidebar_position: 11
created_at: '2026-02-23T15:00:35Z'
updated_at: '2026-02-26T09:55:26Z'
draft: false
---

Easily import your diagrams from OmniGraffle into Miro and start collaborating in one unified tool. As OmniGraffle and Miro use different object models and styling systems, imported boards may not look exactly the same as the original files. You may need to review and adjust formatting after import. For more information, see the [Understand OmniGraffle object mapping in Miro](#understand-omnigraffle-object-mapping-in-miro) and [Known limitations](#known-limitations) sections.

## Before you begin

- Ensure you can create boards in Miro.
- Use OmniGraffle 7.25.1 (September 2025) or later. To verify your version, go to **OmniGraffle > About OmniGraffle**.
- Review hidden content and layers before import. Hidden and layered elements are also imported and will appear on the board. If elements overlap, rearrange them after import.
- Convert gradient fills to solid colors before export. Gradients are not supported.

## Import an OmniGraffle file to a Miro board

1. Open OmniGraffle, export the diagram in the
   **.graffle Single File (Zipped)** format, and save the
   file
   to your device.

:::note
We support only the
:::
   **Single File (Zipped)** format. The
   **Package**
   and **Legacy** formats are not supported. If you have
   an
   unsupported exported file saved earlier, you can open the file in
   OmniGraffle,
   and then export to the **.graffle Single File (Zipped)**
   format.
2. Open the Miro board where you want to add the diagram.
3. Drag and drop the **.graffle Single File (Zipped)** format
   file onto the Miro board.

## Bulk import multiple OmniGraffle files to the Miro dashboard

1. Open your Miro dashboard.
2. Click **+ Create new** in the top-right corner.
3. Click **Import** > **Import from OmniGraffle**.
4. In the import dialog, under **Import to**, select the Space where you want to create the Miro boards for your imported OmniGraffle files.
5. Drop your **.graffle** files into the upload area, or click **browse** to select files from your computer.

:::note
We support only the **Single File (Zipped)** format. The **Package** and **Legacy** formats are not supported. If you have an unsupported exported file saved earlier, you can open the file in OmniGraffle, and then export to the **.graffle Single File (Zipped)** format.
:::
6. Click **Import [X] files**, where **[X]** is the actual number of files you are importing.
7. When you see the message **We’re importing your boards**, click **Back to dashboard**.

### After you start the import

- The import runs in the background.
- New boards appear in the Space you selected during the import process once processing is complete.
- You’ll receive an email notification once the boards are created, including a direct link to the Space so you can quickly access them.

## Verify imported content

After import completes, verify the following:

- The expected number of boards was created.
- Content is readable and properly positioned.
- Connectors are attached correctly.
- Text formatting appears as expected.
- Key visual sections are intact.

For diagrams that will evolve over time, consider rebuilding highly complex areas using native Miro objects for better long-term editability.

## Frequently Asked Questions (FAQ)

Can I import multiple files at once?

Yes. You can import multiple **.graffle Single File (Zipped)** format files at once. For more information, see [Bulk import multiple OmniGraffle files to the Miro dashboard](#bulk-import-multiple-omnigraffle-files-to-the-miro-dashboard).

Where are the boards for my bulk import?

The boards for your bulk import are created in the Space you selected during the [import process](#bulk-import-multiple-omnigraffle-files-to-the-miro-dashboard). You can also click the link on the email notification you received when the boards were created to quickly access them. Lastly, if you did not specify the Space during the import process and you do not have the email notification handy, you can search for your boards in the **Imported files** Space.

Will my diagram look exactly the same after import?

Most of the time, yes, but not always. Fonts, connectors, and complex formatting may change during import. For more information, see the [Known limitations](#known-limitations) and [Understand OmniGraffle object mapping in Miro](#understand-omnigraffle-object-mapping-in-miro) sections.

How long does the import take?

The processing time depends on file size and complexity. You receive an email once your boards are created, including a direct link to the Space so you can quickly access the boards.

How do I know if my bulk import succeeded or failed?

**If your bulk import succeeded**, you’ll receive an email notification once the boards are created, including a direct link to the Space so you can quickly access them.

**If your bulk import failed**, you’ll receive an email informing you about the files for which there were import errors.

Next steps:

- Contact your Miro administrator or the Miro support team, and inform them about this error.
- If possible, provide a **redacted** version of the OmniGraffle file to your Miro admin, as this will help in troubleshooting your import error.

Can I undo an import?

You cannot undo an import. You can delete the created boards, if needed.

## Troubleshooting

I don’t see the Import from OmniGraffle option within the Import menu

- Confirm you have permission to create boards in Miro.
- Clear your cache, refresh your browser, and try again.
- Contact your Company Admin to confirm that the feature is enabled for your organization.

My file won’t upload

- Ensure that you export the OmniGraffle file as a **.graffle Single File (Zipped)** format.

:::note
We support only the **Single File (Zipped)** format. The **Package** and **Legacy** formats are not supported. If you have an unsupported exported file saved earlier, you can open the file in OmniGraffle, and then export to the **.graffle Single File (Zipped)** format.
:::
- Try uploading a single file instead of multiple files at once.
- Split larger OmniGraffle diagrams into smaller items.

I didn’t receive an email

- [Check spam or filtered inboxes.](../../using-miro/tools/troubleshooting/02-allowlist-miro-mailers.md)
- Check the selected Space for newly created boards.

Layout looks incorrect

- Reapply fonts if substitutions occurred.
- Reconnect connectors or lines manually.
- Edit critical sections using native Miro shapes if needed.

## Understand OmniGraffle object mapping in Miro

| Miro native shape feature | Available for imported OmniGraffle shapes |
| --- | --- |
| **Styling shapes**  You can customize the look of your shapes using various styling options to make them fit your needs and add a personal touch to your boards. Select a shape to change its style, color, and transparency. You can select several shapes at once and style them all. You can also style the borders by choosing the color, transparency, thickness, radius of rounded corners, and type. | Thickness ✅  Opacity/transparency ✅  Colour ✅  Multiselect features (except) transparency ❌  (Transparency can be set on multiselect)  Border color ✅  Border transparency ✅  Border thickness ✅  Border type ✅ (dotted)  Border radius of rounded corners ❌ |
| **Changing shape size or rotation**  Use the white nodes to change the dimensions of a shape. Drag the arrow icon to rotate the shape. | ✅ |
| **Converting shapes**  You can convert a shape into a card, text box, sticky note, or any other shape. | ❌ |
| **Send shape back or bring to front**  Send the shape back and bring to front - click the three dots on the context menu and choose an option. Or use shortcuts **Pg Up** and **Pg Dn** (for Windows)/**fn + ↑** and **fn + ↓** (for Mac). | ✅ |
| **Adding text to shapes**  To add text to a shape, select it and start typing. Shapes have a limit of 6,000 symbols. Feel free to use different text formatting options: you can change the text size, font, style, alignment, color and highlight the text.  **Note:** Bullet points are not supported in shapes. Use text instead. | 🟠  You cannot add new text to shapes imported from OmniGraffle. However, if an imported shape already contains text, you can edit that text as usual (font, size, colour, alignment, and highlight). |
| **Quick diagram creation**  As soon as you select a shape, a sticky note, or a card and hover over a blue dot near the object, it will show you where a new shape or a connection line will be created. Click the dot to create the line or the object. If you wish to connect the object to the one which is different from the suggested, drag the dot and draw a connection line. | ✅  Replicates the same shape |
| **Object dimensions**  Use object dimensions to create the same size shapes across your board with precision. You can enable object dimensions in your board settings. | ✅ |

## Known limitations

In this release, when importing OmniGraffle files into Miro, you may notice differences in structure, styling, or behavior due to differences between the two platforms.

### Shape and geometry mapping

**Limitations**

- OmniGraffle shapes are imported into Miro as SVGs or custom shapes, which do not support Miro’s switch type feature. If a shape cannot be recognized and no fallback geometry exists, it defaults to a rectangle.

**Workarounds**

- Replace critical shapes with native Miro shapes after import to restore full editing and QDC support.
- Try using Miro’s in-built shape and prototyping libraries with hundreds of shapes for many use cases.
- Review complex diagrams after import and manually adjust shapes that defaulted to rectangles.

### Visual fidelity and styling

**Limitations**

- Gradients are not supported. Gradient fills are flattened during import.
- Shadows are not supported and are removed during import.
- Unsupported fonts default to a system font.

**Workarounds**

- Use solid fill colors instead of gradients before export.
- Remove shadow effects in OmniGraffle prior to export if visual precision is critical.
- Use widely supported system fonts to reduce font substitution.
- Review typography and spacing after import and adjust styles directly in Miro.

### Connectors and annotations

**Limitations**

- Line captions may not be detected or positioned correctly after import.
- Lines may appear split, slightly misaligned, or pass through shapes.
- Directional arrows within grouped stencil shapes may occasionally be lost during conversion.

**Workarounds**

- Manually reposition text labels on connection lines after import.
- Reconnect or reroute Miro connectors if alignment issues occur.

### File formats

**Limitations**

- We support only the **Single File (Zipped)** format. The **Package** and **Legacy** formats are not supported.
- PNG exports are imported as flat, non-editable images.

**Workarounds**

- Use the **Single File (Zipped)** export format for best results.
- If you have an unsupported exported file saved earlier, you can open the file in OmniGraffle, and then export to the **.graffle Single File (Zipped)** format.
- Avoid PNG exports if you need editable objects.

### Bulk import behavior

**Limitations**

- Email notifications for bulk imports may occasionally fail due to hard bounces.
- After a bulk import completes, imported content may not immediately appear on the board.

**Workarounds**

- Check spam or email filtering rules if notifications are not received.
- Refresh your browser after bulk import completion.
