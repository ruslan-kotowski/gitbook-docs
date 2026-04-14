---
title: Possible issues with Miro app for Confluence
article_id: 360021388500
sidebar_position: 21
created_at: '2021-04-29T05:44:00Z'
updated_at: '2026-03-20T14:10:12Z'
draft: false
---

Use the troubleshooting tips below if you have run into an issue when using [Confluence plugin](https://help.miro.com/hc/articles/360020712594).

|  |  |  |
| --- | --- | --- |
| **Message / issue** | **Possible causes** | **Steps to resolve the issue** |
| You have a black/blank Miro picker when trying to sign in to Miro/embed Miro boards into Confluence pages | Incorrect browser settings | Go to your browser settings and check that:   - The checkbox **Prevent cross-site tracking** is disabled - The checkbox **Block all cookies** is disabled:   mceclip0.png   - **Pop-up windows** on the Miro & Atlassian websites are allowed:   mceclip1.png |
| You have view-only permission on this board and can't share or embed it  **mceclip0.png** | You are not an editor/owner of the board | Please make sure that:   - You are an editor or the board owner - You are authorized in your browser in Miro with the correct credentials - You embed a board in Confluence in the same browser |
| After embedding a Miro board you see the message: "Miro requires access to your cookie files" | Your browser does not allow to save third-party cookies | To enable the embed, you need to enable the cookies in your browser. This mostly happens in Mozilla and Safari |
| The embedded board shows the error message "Your session has expired" |
| When you try to embed a board, you get the following message: "You are not a member of any team. Please log in to the full version of the product and create your team or let someone invite you to the existing one."  mceclip0.png | You are not a member of any team under the Miro profile authorized in the browser | Go to [Miro](https://miro.com/app/dashboard/) and create a team. If you know that you should be a member of some team(s) in Miro, please open Miro in another browser tab and make sure you're authorized with the **correct email** |
