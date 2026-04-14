---
title: Embed a Miro board
article_id: 360016335640
sidebar_position: 2
created_at: '2020-09-09T07:54:13Z'
updated_at: '2025-09-19T09:07:47Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  roles: board_editor
  plans: free, starter, business, enterprise, education
  platforms: Web, desktop, mobile
backstage_link:
  entity_kind: capability
  entity_id: comments
---

You can embed any Miro board or a specific item (frame or format) from the board in supported apps and websites so your teammates can work in context without switching tools.

Embeds inherit the board’s [Share settings](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md#how-to-invite-to-a-board):

- **Public link on** — anyone with the link can view (or, on paid and Education plans, comment or edit).
- **Public link off** — only invited collaborators can open the embed after they sign in.

[Enterprise administrators](../../../plans-billing/miro-plans/04-enterprise-plan.md) can manage public link availability in the [security settings](../../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

## Choose your embedding method

Miro offers two ways to embed boards:

- **Using supported apps**:

  - Working within platforms like Zoom, Teams, Confluence, Jira, or Notion.
  - You want native integration features and seamless workflow.
  - Users will primarily interact through that specific platform.
  - You need the simplest setup process.
- **Using embed code**:

  - Embedding in websites, blogs, or custom platforms.
  - Working with WordPress, Webflow, or other web builders.
  - You need more control over sizing and appearance.
  - The platform supports iFrames but doesn't have a native Miro integration.

## Embed a board in supported apps

Miro has a number of supported apps where you can easily share your Miro boards. Supported apps include:

- [Zoom](../../../integrations-apps/zoom/02-miro-app-for-zoom-(user-guide).md)
- [Webex](../../../integrations-apps/more-integrations/10-miro-for-webex.md)
- [Microsoft Teams](../../../integrations-apps/microsoft/microsoft-teams/02-miro-for-microsoft-teams-(user-guide).md)
- [Jira](../../../integrations-apps/atlassian/02-miro-for-jira-cloud.md)
- [Confluence](../../../integrations-apps/atlassian/01-miro-for-confluence.md)
- [Notion](https://miro.com/marketplace/notion-embed/)
- [Coda](https://miro.com/marketplace/coda-embed/)
- [Productboard](https://miro.com/marketplace/productboard-embed/)
- Medium

When you embed a Miro board into another app, you can set access rights specifically for users of the app and allow them to view, comment, or edit the board from within the app. Access to the board on the Miro side won’t be affected. Learn how [sharing and permissions work for embedded boards](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

To embed a board in one of the supported apps:

1. In the target app, type **/miro** or choose **Miro** from the insert menu.
2. Select the board.
3. Select the **Starting view**:
   - **Full board** — the entire canvas.
   - **Specific item**, such as frame or format (Doc, Diagram, Table, Timeline, or Slides).
4. Turn on **Focus mode** to create a distraction free embed. Leave it off to allow full interaction.
5. Select **access settings** for all visitors:
   - **Can view** — anyone viewing the embed can view the board.
   - **Require access** — anyone viewing the embed must have access to view, comment, or edit the board.
6. Select **Embed board**.

The embed respects the board’s sharing settings. On mobile devices all embeds are view-only.

## Embed a board with embed code

Use this option for any platform that supports iFrame, such as **WordPress** or **Webflow**.

1. Open the **Share** panel using one of these methods:
   - In the top right, select **Share** > **Embed**, or
   - In the board main menu, select **Board** > **Export** > **Embed**, or
   - On the canvas, select the item you want to embed (frame or format). For example, a Doc. Open the three-dot context menu, and select **Embed this doc**.
2. Select the **Start view**:
   - **Board** — the entire canvas.
   - **Specific item**, such as frame or format (Doc, Diagram, Table, Timeline, or Slides).
3. (Optional) **Set start area** — drag to outline an exact region of the board.
4. Decide on interaction:
   - Select **View only** to lock the view.
   - Deselect **View only** to let viewers pan, zoom, comment, or edit (if they have permission).
5. Select **Copy code** and paste it where you need it.
   If the destination accepts only URLs, select **Copy link** instead.

You can create multiple embeds for the same board, each with its own start view, start area, or focus object.

### Autoplay slides

To autoplay a Slides embed, set the **Auto-slide interval** from 1 to 30 seconds in the **Embed** tab. Autoplay is ignored when you embed a board inside another board.

## How embeds appear

- The board name is not clickable.
- The mini-map, [notes](../../essential-tools/17-visual-notes.md), and pop-ups are closed by default.
- Some menu options, such as **Set start view**, are hidden.
- All embeds are view-only on mobile.
- Third-party cookie blockers can prevent embeds from loading properly.

## Frequently asked questions

**What is the difference between a start view and focus mode?**
A start view sets the initial position, but viewers can still explore the board. Focus mode hides everything except the selected object and is always view-only.

**Can I make a focus-mode embed editable?**
No. To enable collaboration, clear **View only** and grant edit rights in the board’s share settings.

**Which widgets are supported?**
Docs, Diagrams, Tables, Timelines, Slides, and any frame.

**Can I remove the Miro logo?**
No. Branding removal is not available.

**Can I embed a board inside another board?**
Yes. Copy the embed code and paste it into the target board with **Paste iFrame code**.
