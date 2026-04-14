---
title: How to disable Miro Desktop app pop-up in your browser
article_id: 360019244239
sidebar_position: 5
created_at: '2021-01-29T12:48:31Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

If you have [Miro Desktop App](../../../getting-started/apps-for-devices/05-desktop-app.md) installed on your device, when opening a Miro board in a browser, you can see the pop-up that suggests you open the board in the app.

![browser_pop-up.jpg](images/21017042611090_browser%20pop-up.jpg)
*The browser pop-up that leads you to Miro Desktop app*

If you'd like to disable the pop-up, please follow the instructions below.

- [For Mac users](#for-mac-users)
- [For Windows users](#for-windows-users)
- [Safari browser](#safari-browser)

### For Mac users

**Step 1.** Delete (uninstall) the Desktop app from your computer.

**Step 2.** Rollback the setting ‘Always open URL in the Miro App’ in your browser. Here's how you can do that in Chrome and Firefox.

*For Chrome:*

1. Close all Chrome + Miro windows before starting (use **C****md + Q** to quit the browser).
2. Open Finder on your Mac > press **Command + Shift + G** > enter the following path into the search box: **~/Library/Application Support/Google/Chrome**. Open your Chrome profile folder, find **Preferences**.

   There may be several folders with the file, please try the next suggestions:

   - open and search **Preferences**inside **Default** folder, if you have only one profile in Google Chrome
   - open and search **Preferences**inside **Profile X** folder, if you have several profiles in Google Chrome, where **X**  is a number from the profile list
   - open and search **Preferences** inside each folder (**Default, Guest Profile, Profile X**), if they exist
3. Open **Preferences** in a text editor.
4. Search for **`https://miro.com":\{"miroapp":true\}`** .
5. Remove **`https://miro.com":\{"miroapp":true\}`** .
6. Save changes.
7. Restart Chrome browser.

If you use several Google profiles, you will need to edit Preferences in all catalogs. For this, on step 2, you will need to open **~/Library/Application Support/Google/Chrome** and change **Preferences** in folders **Profile 1, Profile 2**, etc.

*For Firefox:*

1. Open browser settings.
2. In the **General** section scroll down to **Applications.**
3. Find **miroapp** and change **Use Miro** (default) to **Always ask** by selecting the option in the drop-down menu.

### For Windows users

**Step 1.** Delete (uninstall) the Desktop app from your computer.

**Step 2**. Use the script available via [this link](https://desktop.miro.com/platforms/Miro_DeleteAppSchema.reg) to clear the value from the Windows registry*.* Once this is done, the notification should not appear in your browser. If the pop-up is still there, follow step 3.

**Step 3.** Rollback the setting ‘Always open URL in the Miro App’ in your browser. Here's how you can do that in Chrome and Firefox.

*For Chrome:*

1. Close all Chrome + Miro windows before starting.
2. *N*avigate to **PC** > **Users > \{current_user\} > AppData > Local > Google > Chrome > UserData > Default > Preferences.**
3. Open **Preferences** in a text editor.
4. Search for **`https://miro.com":\{"miroapp":true\}`** .
5. Remove **`https://miro.com":\{"miroapp":true\}`** .
6. Save changes.
7. Restart Chrome browser.

If you use several Google profiles, you will need to edit Preferences in all catalogues. For this, navigate to **PC** > **Users > \{current_user\} > AppData > Local > Google > Chrome > UserData** and change **Preferences** in folders **Profile 1, Profile 2**, etc.

*For Firefox:*

1. Open browser settings.
2. In the **General** section scroll down to **Applications.**
3. Find **miroapp** and change **Use Miro** (default) to **Always ask** by selecting the option in the drop-down menu.

### Safari browser

If you need to disable the pop-up in Safari, please delete the Miro Desktop app from your device.
