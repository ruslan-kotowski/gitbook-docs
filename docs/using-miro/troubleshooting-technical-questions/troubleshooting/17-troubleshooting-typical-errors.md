---
title: Troubleshooting typical errors
article_id: 5132313152530
sidebar_position: 18
created_at: '2022-04-15T12:33:03Z'
updated_at: '2024-08-23T12:36:47Z'
draft: true
---

In Miro, we try to ensure the best user experience and aim to provide a stable service to all users. If you spot one of the error messages below on your Miro boards, this guide will help you understand possible reasons and a solution.

### Syncing... Please wait

The pop-up notification **Syncing... Please Wait** may appear if you are working on an extremely heavy board when bulk-moving, for instance, a lot of objects, or if there's a packet loss. The board may look simple, but if it has a lot of PDF files, high-resolution images, drawings, or tables - this can cause the performance degradation that triggers the error message.

Please try to divide your board into smaller ones by copying and cutting your content to another board and see if the issue persists. If that does not help:

- Make sure your device meets the minimum [system requirements](../technical-guidelines/01-system-requirements.md) and your browser is updated to the latest version
- If you use VPN, check if the issue persists when you turn it off
- Try to [duplicate the board](../../managing-boards/03-how-to-duplicate-a-board.md) and check if the error is reproduced on the new one

### Connection restored

Generally, **Reconnecting...**, **Connection restored** error can appear in the following cases:

- When there are some connectivity issues on your side. Makes sure your network connection meets the minimum requirements. If it is not the case, try to switch to a faster network
- When you are working on the multiple heavy boards opened in the same browser. If this appears to be your case, close all extra tabs & running applications in your browser and refresh the browser page
- It is also worth checking [your WebSocket connection](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md). If the results are negative, get in touch with your IT department and ask them to enable the WebSocket connections on port 80 and 443 (SSL)
