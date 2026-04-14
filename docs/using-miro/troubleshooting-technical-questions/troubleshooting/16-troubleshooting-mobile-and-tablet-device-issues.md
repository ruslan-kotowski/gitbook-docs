---
title: Troubleshooting mobile and tablet device issues
article_id: 360021113559
sidebar_position: 17
created_at: '2021-04-16T08:25:42Z'
updated_at: '2025-11-25T16:04:39Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

If you face any issues when working in Miro on mobile or tablet, first of all, try to *reinstall the app, and reload your device*. If that doesn’t help, see the possible reasons below.

| **Mobile Issues** | | |
| --- | --- | --- |
| **Issue** | **Possible reason** | **Solution** |
| The mobile app on iOS crashes and doesn't work properly | The iOS version is too old | Please update your iOS version or use another device. Our Mobile app for iOS is supported by version 12 or higher |
| I can successfully log into the desktop app, but on mobile I am stuck on the Miro logo | Authentication data are corrupted (bad cache) | Go to **App settings > Storage > Clear storage** or reinstall the Miro app on your device |
| I get "Something went wrong" error when authenticating via SSO on the Mobile app | 1. The network connection is secured, and something blocks the requests  2. Chrome is added to ADFS' WIAsupportedUserAgents list and incorrectly directs the user  3. It is possible that this specific device cannot access the company's SSO environment | 1. Try and authorize having connected to a different network  2. Reach out to your system administrator and ask to remove Chrome from the list  3. Check with your IT department if there are any restrictions regarding specific devices which are allowed to use SSO |
| I cannot find files imported from boards in the mobile file system | When you download a file from a board on mobile, it is "hidden" for you for some time | Please wait until the file appears in the folder with the downloaded files |
| When I log into Miro on mobile, I see the message "No accounts available" and cannot access my profile | You were removed from or [left](../../managing-your-profile/06-how-to-leave-a-team.md) all your teams. | Please log into Miro on desktop or tablet, and create a new team or ask another user to invite you to a Miro team |
| I cannot edit Miro boards in a browser on mobile | This is a known limitation at the moment | Please switch to our [Mobile app](../../../getting-started/apps-for-devices/08-mobile-app.md), tablet, or desktop |
| I cannot export my board using the Mobile app | This is a known limitation at the moment | Please switch to another device. Learn more about Miro export on [this page](../../import-and-export/export/03-how-to-export-your-board.md) |

| **Tablet Issues** | | |
| --- | --- | --- |
| **Issue** | **Possible reason** | **Solution** |
| Disappearing toolbar and weird behaviour when using Miro on iPad | Our app uses WebView to render the visuals, and one of the rules related to memory management is that the rendering process is not allowed to use more than 25% of RAM memory of the device. After this mark, the app gets limited and stops loading properly without giving any error messages or crashes | - Close all unnecessary background applications before using Miro - Work on boards that are *smaller*in size - Finally, try to switch to *another device* (desktop) with better RAM |
| I can successfully log ito the desktop app, but on tablet, I am stuck on the Miro logo | Authentication data are corrupted | Go to **App settings > Storage > Clear storage** or reinstall the Miro app on your device. |
| Error message “Sorry, you cannot copy so many objects as once” when pasting objects on iPad | You exceeded the amount of data that could be put in a buffer on iPad | Please copy and paste fewer widgets at once |
| I cannot edit [Google docs uploaded to my board](../../../integrations-apps/google/05-google-drive.md) on tablet | This is currently a known limitation | As a workaround, you can open the document via the Google Doc app if you click on the **Source** icon |
| I use Apple Pencil on iPad. When I double-tap to switch between pen and eraser, nothing happens | Switching between pen and eraser by double-tapping is a native feature supported by 2nd generation of Apple Pencils, rather than something developed by Miro specifically. It is supported in the Tablet app only | Please make sure that your Apple Pencil supports the feature and switch to the [Tablet app](../../../getting-started/apps-for-devices/11-tablet-app.md) |
| On iPad the following 2 things do not work:   - zooming when operated via the mouse wheel - board navigation when operated by two-finger swipes on the trackpad | This is a known limitation connected with the OS restrictions on iPad | Unfortunately, there is no solution for this yet. |
