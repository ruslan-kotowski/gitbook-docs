---
title: Profile lockout
article_id: 360017571374
sidebar_position: 15
created_at: '2019-02-11T10:08:55Z'
updated_at: '2026-02-24T12:02:59Z'
draft: false
---

The profile lockout is standard forall Miro users and plans, customization is unavailable. Users trying to [authenticate through external identity providers](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-(sso).md), will not be affected by this feature.

After the wrong login to your profile, you have **10 attempts** to put a correct password in for an email-password pair. The first 5 attempts are standard with no extra complexity.

The next attempts add captcha (for web and desktop apps only). If you fail to provide the correct password **10 times in a row** for an email-password pair, your user profile gets locked for**1 hour**, during which all attempts to log in to the profile will fail even if a correct password is provided.

:::tip
During the lockout hour, you can try to log in with passwordless or social provider.
:::

Once your user profile gets locked, Miro sends you an email with a six-digit code to unlock your profile. The link in the email redirects you to the confirmation page where you would have to provide the six-digit code. If the provided code is correct, your profile gets unlocked and all the attempts reset. The email also recommends changing the password.

The locked profile gets unlocked **automatically** in 1 hour and all failed attempts reset.

### What to do if you do not receive the code

If you cannot find the email in your inbox, try these troubleshooting steps:

- Make sure there are no typos in the email you submitted. If you find a typo, try to log in with the correct address
- Open your **Spam, Promotions, Junk, Social**, and **Updates** folders and check to see if Miro confirmation email is there
- Check to see if your inbox is full to make sure you haven’t reached the memory limit with your email inbox. If it is full, you may need to delete some existing emails in order to receive new ones. After deleting emails, click **Send code again** to receive a registration email
- It may be that a firewall is preventing the email from reaching your inbox. Please reach out to your *system administrator* and ask them to allowlist our domains and subdomains: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) and [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). [Here is an article](../../tools/troubleshooting/02-allowlist-miro-mailers.md) with more information on the mailers you need to allowlist
- AOL/CompuServe users: make sure your Mail Controls are set to receive emails from the Internet. If you have Internet email blocked, please change your Mail Controls by entering **Mail Controls** on AOL or CompuServe. After that, get back to our registration form to resend your confirmation code
- Normally, the code should arrive instantly but due to the peculiarities of your mailing system, you may need to wait up to 24 hours
- If neither of the solutions help, [report the issue to Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).
