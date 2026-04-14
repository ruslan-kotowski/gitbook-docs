---
title: Issues with confirmation code or password reset emails
article_id: 360017731373
sidebar_position: 13
created_at: '2019-02-11T10:14:22Z'
updated_at: '2024-10-25T14:25:54Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

If you didn’t receive a confirmation code or password reset email, there could be a number of reasons why. The information below can help resolve the situation by giving you options to try.

## Common reasons codes or emails don't arrive

Two of the most common reasons why you may not be getting password reset emails, or be able to request a new confirmation code are:

1. Your company is using a firewall, and the firewall is blocking emails from miro.com domains. Ask your IT administrator to allow emails from [miro.com](http://miro.com/) domains. If you are the administrator, see the section below for instructions on how to allowlist Miro's domains.
2. Your company uses SSO. See the section below for instructions on how to address this.

## How to resolve lost emails/confirmation code issues

1. If your company uses SSO, you need to log in with your corporate SSO credentials. If you try to reset your password with Miro, you will simply be redirected back to the SSO login page. If this happens, try using your corporate SSO credentials. If that doesn't work, continue troubleshooting below.
2. A firewall may be preventing the email from reaching your inbox. Please reach out to your system administrator and ask them to allowlist our domains and subdomains: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com and realtimeboard.com*, *.realtimeboard.com.

   Here is the list of dedicated IPs: 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. Read more on [allowlisting Miro emails.](../../tools/troubleshooting/02-allowlist-miro-mailers.md)
3. Make sure there are no typos in the email you submitted. If you find a typo, [register a profile again](../../../getting-started/start-here/02-how-to-register-with-miro.md)/reset your password using the correct email address.
4. Check the **Spam, Promotions,** **Junk, Social**, and **Updates** folders in your email provider.
5. You can also register or log in using alternative sign-up/sign-in options: log in or sign up with Google, Slack, Office 365, Apple, or Facebook.
   > ⚠️ Note that alternate logins are **not** connected to corporate SSO logins. If you're using Miro in a corporate environment, please use the credentials your Miro Admin has set up for you.

   ![new-sing-in-third-party.png](images/20486895217170_new-sing-in-third-party.png)
   *Available authentication methods*

If you can’t sign up or log in using other authentication methods:

- Check to see if your inbox is full and you haven’t reached your email storage limit. If it’s full, you may need to delete some emails in order to receive new ones. After deleting emails, go back to our registration page and click **Send code again.**
- You should receive the email right away. If not, you may need to wait up to 24 hours.
- If you're using your corporate SSO credentials and cannot login, you can read about [common SSO errors and how to resolve them](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

### Other confirmation issues

My code is invalid

If the code you entered is **invalid:**

1. Check your inbox and make sure that you're entering the code you most recently received. If the code is still invalid, click **Send code again** and enter the code from the new email.
2. Another way to finish the registration is to click **Confirm your email** in the email with the confirmation code. In this case, you don't need the confirmation code.
   ![confirm email button.png](images/21017725339026_confirm%20email%20button.png)
   *The option to confirm your email*

I exceeded the email confirmation attempts

If you failed to confirm your email after 4 attempts, you’ll see  **Email confirmation attempts exceeded** on the registration page.

Wait 60 seconds and click **Send code again** - this will generate a new code for you. Enter the code and finish the registration.

I accidentally closed the tab where I enter the confirmation code

[Log in](https://miro.com/login/) using the email and password you entered during the registration, and you'll be redirected to the [confirmation page](https://miro.com/email-confirm/) again.

:::note
If you don't confirm your email, you’ll receive reminders after 12 and 24 hours. If your email is not confirmed within 7 days, your **profile is deleted**. You’ll be able to register a new profile using the same email address.
:::

:::note
Confirmation codes can only be sent via email.
:::

:::note
If you’re still having issues, [contact Miro Support](https://miro.com/contact/recover/).
:::
