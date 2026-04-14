---
title: 'Board history: activity'
article_id: 360017730913
sidebar_position: 11
created_at: '2019-02-11T10:12:03Z'
updated_at: '2026-01-06T19:02:16Z'
draft: false
availability:
  plans: browser version, [Desktop app](../../getting-started/apps-for-devices/05-desktop-app.md),
    [Tablet app](../../getting-started/apps-for-devices/11-tablet-app.md)
  roles: editors who were explicitly invited to boards [via email](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md#inviting-via-email)
    or have access to the board because they are part of a [space](../spaces/01-spaces.md)
    or [team](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) in
    Miro
---

Managing your team's workflow on a single board sometimes gets a bit challenging. Activity is our take on tracking and evaluating the input that every teammate adds to your boards.

### Board Activity list

You can access the change log for a given board. In the Board bar, select the vertical three dots to access the **Main** menu, then select **Board** > **History**. The **History** panel opens, showing the **Activity** tab by default.

**Activity** is visible to editors of boards that were explicitly invited to boards [via email](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md#inviting-via-email) or have access to the board because they are part of a [space](../spaces/01-spaces.md) or [team](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) in Miro (in other words, it is visible to [guests](../sharing-boards/07-collaboration-with-guests.md) and team members with editor rights on the board). If the board is shared [via link with the company](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md#sharing-a-board-with-the-entire-company) or [via a public link](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md#sharing-boards-via-a-public-link) with visitors, **Activity** won’t be visible for them. Viewers and commenters don't see **Activity**.

If you open a board that somebody edited while you were away, you will see the option **Highlight changes** at the bottom of the Board history panel.

At the bottom of the **Activity** panel, you can enable and disable highlighting recent changes made by other users while you were away. If you enable highlighting changes, you will be automatically redirected to the most recently modified object on the board.

![board_history_activity_highlight_changes.png](images/21016134524178_board_history_activity_highlight_changes.png)*Show highlighting on changes*

The board changes are arranged in *date order* and grouped by user. All changes are recorded in the user's **local** time. There are 3 categories of changes that you will find included:

- adding and duplicating content
- editing content
- deleting content (including the [Undo](../essential-tools/16-undoredo.md) actions)

If you're looking to pin down a particular action, you can scroll down the list and look through the edits' content - all text changes are shown as references below the action's name (if it's a frame, the [frame](../essential-tools/07-frames.md)'s name will be displayed).

Clicking a record on the list, you will be automatically redirected to the corresponding object on the board and zoom in to view the change in detail (except for **Delete** records).

![board_history_activity_selecting_edits.gif](images/21016121177362_board_history_activity_selecting_edits.gif)*Click an event to jump to an updated object*

In pursuit of content optimization in every regard, we have limited the list to always displaying only the most recent change - if you modify one object several times, all the previous modifications will be erased from the list.

Whatever you are working on at the moment, all board objects, including [comments](../facilitation-tools/asynchronous-tools/01-comments.md), and uploaded files will be registered and tracked **in real time** right after you exit the edit mode - no need to re-open the menu or refresh the board. An exception is [moving objects](../working-on-the-board/10-working-with-objects.md) - you will not find any records of that on the list.

To close the **Activity** panel, simply click the cross iconin the top right corner of the panel.

If your collaborators changed something on a board while you were offline, you will see the button **See recent changes** upon entering the board. Click **See recent changes** to see all the changes highlighted in pink on the board. You will see the names of the collaborators who added/modified objects on the board and the time the updates were made. To hide highlighting, click **Hide highlighting on changes**.

If you don't click the button **See recent changes** for 30 seconds, it will disappear.

![see_recent_changes.jpg](images/21016134517394_see%20recent%20changes.jpg)*Highlighting changes on the board*

:::note
Saved board history activity is stored for 90 days.
:::

### Restoring recently deleted board content using Activity

> **Set up by:** board editors
> **Available on:** browser version, [Desktop app](../../getting-started/apps-for-devices/05-desktop-app.md), [Tablet app](../../getting-started/apps-for-devices/11-tablet-app.md)

:::tip
For the option to restore a whole version of the board from the past (a snapshot) please see [Board history: versions](12-board-history-versions.md).
:::

> **⚠️**  The feature is not available for [visitors](../sharing-boards/08-collaboration-with-visitors.md).

You can restore recently deleted objects by opening **Activity** and clicking **Restore** next to deleted widgets – the deleted objects will reappear on the board (exactly where they were before being deleted), and the board will zoom in to that part of the board.

![restore_content.jpg](images/21016134518162_restore%20content.jpg)*Restoring a deleted object*

The following content is available for restoration:

- Any content deleted from the board during their current active session and 30 minutes after the content was deleted in case the session is over
- The last 1000 objects deleted from the board – if the restoration occurs more than 30 minutes after the content was deleted
- Any content deleted from the board if the objects were selected and deleted simultaneously for an indefinite period of time – until the next 1000 objects are deleted

Please note that there can be edge cases. For more details, please refer to [this article](../working-on-the-board/18-restoring-board-content.md).

### Frequently asked questions

1. *Can I see activity history for a specific object?*
   - No, but if you click the object and choose **Info** under three dots on the context menu, you will see who and when created the object and last modified it.
2. *Can I clear the activity?*- No, this is not possible at the moment.
3. *My boards are not shared publicly in Miro, but I see visitors in the Activity. Why?*- This happens when a board is embedded into another service (for example, [Zoom](../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md)) with an **Anyone can edit. No sign-in required** option.
4. *I do not see the board history icon on my toolbar. Why?*
   - Please note that the board history is only visible to editors of boards that were explicitly invited to boards [via email](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md#inviting-via-email) or have access to the board because they are part of a space or [team](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) in Miro. The board history is not visible to viewers, commenters, or [visitors](../sharing-boards/08-collaboration-with-visitors.md).
5. *I do not see the See recent changes button. Why?*
   - The button is only shown if someone edited content while you were not present on the board. If there have been no changes since your last visit, the button is not available.
