---
title: I can't log in
article_id: 360020993079
sidebar_position: 10
created_at: '2021-04-09T06:31:47Z'
updated_at: '2025-11-25T16:04:24Z'
draft: false
---

Follow this guide if you have issues signing into your Miro profile.

## Issues with email and/or password

My email/password isn’t working

Here are two solutions you can explore:

1. Double-check that the email/password you use to log in has no typos.
2. If the credentials you enter are correct, [reset your password](../../managing-your-profile/05-how-to-change-your-password.md).
3. If your email or password includes any of the symbols **& " < >**, please [contact our Support team.](https://help.miro.com/hc/requests/new?)

:::warning
Note that your **profile gets locked** out after 10 attempts to enter your email and password. You may need to [unlock the profile](../../tools/troubleshooting/14-profile-lockout.md) first and then reset your password.
:::

I can’t reset my password

If you don’t get a password reset email, there may be three reasons:

1. **The email is incorrect**
Make sure there are no typos in the email you submitted. If you find a typo, try the reset request again.

2. **The email is not registered with Miro yet**
In this case, the password reset link will not be sent to your email address. Register a new profile on the [sign-up page](https://miro.com/signup/). If your email is registered, you will see the corresponding message:
![mceclip0.png](images/21017695734034_mceclip0.png)

3. **There are email delivery issues**

- Open your **Spam, Promotions, Junk, Social**, and **Updates** folders and check to see if the reset request email is there.
- It also may be that a firewall is preventing the email from reaching your inbox.

  Please reach out to your *system administrator* and ask them to allowlist our domains and subdomains: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) and [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/) and add the IPS of our email-sending system to the allowlist on your end.

  Here is the list of dedicated IPs: 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. [Here is an article](../../tools/troubleshooting/02-allowlist-miro-mailers.md) with more information on the mailers you need to allowlist.

I reset my password but still can’t log in

In case you still can’t access your profile:

1. Make sure you enter the new password.
2. Log in to your browser’s private (incognito) mode or try another browser.

I log in with one email but get redirected and find myself logged in with another email

The issue may appear if you use an alternative authentication method to log in (Google, Slack, Office 365, Apple ID, Facebook).

![new-sing-in-third-party.png](images/21017725436050_new-sing-in-third-party.png)
*Alternative sign-in options on the login page*

You might have accidentally linked your Google/Office 365/etc. email address to your Miro profile registered under a different email. If that happens, try the following:

1. Remove the wrong email association by going to your **Profile settings** > **Integrations** and clicking **Log out** next to Google/Office 365/etc.
   ![remove_connection.jpg](images/21017725424658_remove%20connection.jpg)
   *Removing association with Google login*
2. Log out and log in with your email again.

:::note
Set up a connection with the Google/Office 365/Slack email which matches your Miro profile’s email to prevent the issue.
:::

## SSO login does not work

Check out the article: [Possible issues with SSO login](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## Endless loading when signing in

For users who have endless loading issues after entering their Miro credentials, we recommend the following:

1. Log in on a **different browser**.
2. Log in using your browser’s **private (incognito) mode.** If the issue is not reproduced in incognito mode/another browser, clear your browser cache.

   How to clear Chrome cache

   1. Go to `https://miro.com/` and open the **Developer tools**of Chrome (**Command + Option + J** *on Mac*, **Ctrl + Shift + J***on Windows*).
   2. Choose the tab **Application > Storage**. You will see the blue button **Clear site data.**​  Click the button, and this should remove any data of Miro saved in your Chrome browser so you can start a new working session.
   ![clear_site_data.jpg](images/21017725432466_clear%20site%20data.jpg)
   *The option to clear site data in Chrome*
3. If you’re using **VPN**, toggle it off/on.
4. Check with your IT department if your company uses firewalls or a proxy that may block Miro. Follow [these guidelines](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md#if-you-use-a-firewall) to **allowlist Miro** or provide a bypass.
5. Check your Internet connection. If your network bandwidth doesn't reach the minimum of 8 Mb/s, **switch to another, preferably** **faster network**.
6. Try connecting to a **mobile hotspot**, if that's available. Then reconnect to your original network.
7. If that does not help, [submit a request](https://miro.com/contact/recover/) and [send your browser console logs to Support](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md#how-to-record-console-logs).

## Login issues on Miro desktop app

1. If you can't access Miro on the desktop app, log in using your browser. If you still can't log in, follow the [steps above](#endless-loading-when-signing-in). If you can access Miro in the browser, follow the steps below.
2. Reset the application data.

How to reset the app data on Windows

Press **Alt > Help**and choose to reset the application data as shown in the screenshot below:

​​![reset_app_data_on_Windows.jpg](images/21017725434514_reset%20app%20data%20on%20Windows.jpg)
*Resetting the app data on the Desktop app for Windows*

If you cannot find the menu, you probably use the app downloaded from the MS Store. In this case, to reset the app data, open Windows **Settings** > **Apps** > **Apps and Features** > find **Miro** on the list > **Advanced options**> **Reset**.

If this does not immediately help proceed to delete all app files from **C:\Users\username\AppData\Roaming\RealtimeBoard** and **C:\Users\username\AppData\Local\RealtimeBoard**

> **✏️** If the **Appdata** folder is hidden, see [here](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) how you can reveal it.

How to reset the app data on Mac

Click Miro in the top menu and choose **Reset application data** as shown in the screenshot below:

![reset_app_data_on_Mac.jpg](images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
*Resetting the app data on Mac*

After that, try to log into the app again and check if the issue is solved.

If resetting does not immediately help, open a Finder window > press **Command + Shift + G**> paste **~/Library/Application Support/RealtimeBoard**and delete all app files.

3. If the issue persists, ensure that you’re using the latest version of the app downloaded [from our website.](https://miro.com/apps/)

## Google/Office 365/Slack/etc. login

I can’t log in via Google/Office/Slack/etc.

1. Log in to Miro using your standard credentials (email and password). If you don’t remember or don’t have the password, [reset the password](../../managing-your-profile/05-how-to-change-your-password.md#how-to-reset-your-password).
2. Go to **Profile settings** > **Integrations**, click **Log out** next to Google/Office 365/etc. and reconfigure the connection.
   ![remove_connection.jpg](images/21017725424658_remove%20connection.jpg)
   *Removing association with Google login*

I can’t log in via Google/Office/Slack/etc. on the desktop app

Explore [these troubleshooting steps](#login-issues-on-miro-desktop-app).

I used to log in to Miro via Google/Office 365/etc., but my email service has changed. How can I log in now?

Log in to Miro using your new service credentials (email and password). If you don’t remember or don’t have the password, [reset it](../../managing-your-profile/05-how-to-change-your-password.md).

## Login issues on tablet/mobile

1. Check if you can log in to the browser version. If not, we recommend [these](#endless-loading-when-signing-in) [troubleshooting steps](#endless-loading-when-signing-in).
2. If logging in works for you in the browser, it may be the case that your device authentication data is corrupted. Go to **App settings > Storage > Clear storage** or reinstall the Miro app on your device.

## Troubleshooting tips

If you could not find a solution above, please log into Miro using **another browser** or **incognito mode**. If everything is fine in the incognito mode of your browser, clear the browser's cache and cookies and log in to Miro in the standard mode.

How to clear Chrome cache

1. Go to `https://miro.com/` and open the **Developer tools**of Chrome (**Command + Option + J** *on Mac*, **Ctrl + Shift + J***on Windows*).
2. Choose the tab **Application > Storage**. You will see the blue button **Clear site data.**​  Click the button, and this should remove any data of Miro saved in your Chrome browser so you can start a new working session.

![clear_site_data.jpg](images/21017695738386_clear%20site%20data.jpg)
*The option to clear site data in Chrome*

In case that does not help, [contact Miro Support](https://miro.com/contact/recover/). Please describe the issue in detail.

:::note
If you’re having issues registering with Miro, check out[Issues with confirmation code](../../tools/troubleshooting/12-issues-with-confirmation-code-or-password-reset-emails.md).
:::
