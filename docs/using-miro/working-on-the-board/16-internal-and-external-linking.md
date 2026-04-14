---
title: Internal and external linking
article_id: 360017572354
sidebar_position: 16
created_at: '2019-02-11T10:12:22Z'
updated_at: '2026-01-06T19:00:57Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: unfurling
availability:
  roles: all_users
  plans: free, starter, business, enterprise, education
  platforms: browser, desktop, mobile
---

Enrich your board content by linking any object to an external website or another object on the board.

Withthe **Link to** option you can:

- Create interactive prototypes.
- Simplify navigation on the board.
- Add links to references and useful sources.
- Link [stickies](../essential-tools/14-sticky-notes.md) or [cards](../essential-tools/02-cards.md) to task tracker links.

## Link objects

1. Select the object you want to link to, then click the **three dots** (**...**) icon on the context menu
2. From the context menu, choose **Copy link**
3. Select an object you wish to link **from**, and click the **three dots** (**...**) icon on the context menu
4. Choose **Link to** or use **Option +** **Cmd + K** (*for Mac*) or **Alt +** **Cmd + K** (*for Windows*)
5. Insert the URL or click another object on the board that you want to link

:::tip
Quickly link objects using Command palette. Click the object, tap **Cmd + K** and **link to object** will appear as the first item in the menu. Simply paste your link in the text field and tap **Enter**.
:::

![linking_in_Miro.gif](images/21016057152146_linking%20in%20Miro.gif)
*Linking a sticky note to the Miro blog*

Please note that an object on the board can be linked to only *one* website or Miro object. You can create links to external websites, other Miro boards, [particular objects on boards](#links-to-objects-on-the-board).
To go to the linked URL - just click the link icon.

![Link_to_Google_Calendar.jpg](images/21016043778834_Link%20to%20Google%20Calendar.jpg)
*The link icon will show the logo of the linked site*

To delete or edit the link:

1. Click the three dots on the context menu.
2. Choose **Edit link**.![edit_link.jpg](images/21016057155218_edit%20link.jpg)*The option to edit a link*
3. Change the link or click **Delete link** on the pop-up.![change_or_delete_link.jpg](images/21016057156242_change%20or%20delete%20link.jpg)*The option to delete a link*

## Links to objects on the board

You can get a direct link to any object on the board ([frames](../essential-tools/07-frames.md), images, [shapes](../essential-tools/11-shapes.md), etc.). Share this link with your collaborators to draw their attention to the exact place on the board.

1. Click on the object your want to link to show the context menu.
2. Click the **three dots** (**...**) icon.
3. Choose **Copy link**.![copy_link.jpg](images/21016057158162_copy%20link.jpg)*Copying the link to a frame*

If the linked object is deleted, users who follow the link will see the message "*Sorry, the linked item has been deleted from this board*". It is possible to [restore deleted content](18-restoring-board-content.md) via the Activity list.

## Pasting links on the board

You can paste a link on your board using the shortcuts: **Ctrl + V** (*for Windows*) or **Cmd + V** (*for Mac*). The link will show a preview.

*![link_to_help_center.jpg](images/21016057159186_link%20to%20help%20center.jpg)
The link to Miro Help Center on a board*

To paste a link on a board without the preview, use the [text tool](../essential-tools/16-text.md) and paste the link into the text box.

## Linking text

When working with objects that include text, click the **link** icon on the context menu to insert a link into the text.

![insert_link.jpg](images/21016043786642_insert%20link.jpg)
 *The option to insert a link*

You can also select the text and use **Ctrl + V** (*for Windows*)/**Cmd + V** (*for Mac*) to paste a link.

![insert_link.gif](images/21016057161490_insert%20link.gif)
*Inserting a link into a text line*

:::note
If you link two objects on a board via the **Insert link** optionand then duplicate the board, the link on the board copy will lead to the original board. However, when you link two objects on the board via the [Link to option](#link-objects) and then duplicate the board, the link on the copy remains internal (it brings to the object on the same board).
:::

## FAQ

Can I link my board to another Miro board?

Yes, copy the link to the board (or a [particular object on the board](#links-to-objects-on-the-board)) and paste the link on the original board (or [add the link to an object](#links-to-objects-on-the-board) or [notes](../essential-tools/17-visual-notes.md)). You can also [embed Miro boards](../import-and-export/export/02-embed-a-miro-board.md).

How can I copy a link to my board?

Open the board [Share dialog](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md#how-to-invite-to-a-board) and click **Copy board link**. You can also simply copy the link from the browser address bar. If you have a board opened in [Desktop app](../../getting-started/apps-for-devices/05-desktop-app.md), click **File > Copy board link**.

How do I create a link to a specific area on my board?

You can create a [frame](../essential-tools/07-frames.md) that covers the area and [copy a link to the frame](#links-to-objects-on-the-board). Note that [users who have access to your board](../sharing-boards/05-who-has-access-to-my-board.md) will be able to navigate and see other areas of the board as well.

Can I remove all links on my board at once?

You can remove [all links that have been pasted on canvas](#pasting-links-on-the-board) in several clicks. [Select all objects](10-working-with-objects.md), choose **Filter** on the context menu, select **Preview,** and delete the selected link objects.
![filter_perviews.jpg](images/21016057163410_filter%20perviews.jpg)
*Filtering previews in selected objects*

Can I link to local files on my computer?

No. For security reasons, please upload your files to a cloud-based service and link from there.

Does Miro recognize hyperlinks of email addresses as mailto: links?

At the moment, this is not supported.
