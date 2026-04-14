---
title: How to change your email
article_id: 360011781980
sidebar_position: 4
created_at: '2020-02-12T11:22:44Z'
updated_at: '2026-01-06T19:04:10Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-details-dialog
---

Learn how to change the email associated with your Miro profile. Changing your profile email does not affect your access to boards and teams.

In order to change your email, you should have a profile password. If you've signed up to Miro using another service (Google, Slack, Microsoft, Apple or Facebook) and do not have a password, go to **Profile settings** > **Password** and click **set a password using Miro's password recovery**.

![set_password.jpg](images/21016927953298_set%20password.jpg)
*The option to set up a password in Profile settings*

## How to change your Miro profile email

1. Go to [Profile settings](01-profile-settings.md) > **Profile details** and click **Change email** in the **Email Address** section
2. Enter a **New email address** and the **Current password**, and click **Update email**

   ![Change_your_email.gif](images/21016940902546_Change%20your%20email.gif)
   *The option to change your email in the Profile settings*
3. The confirmation link will be sent to the new email address. Open the email and click **Confirm your email address**
4. Miro will open in your browser. If you initiate the email change in the Miro app (Tablet or Desktop), you may need to sign in with your **old** email address to confirm the change
5. A notification that **Your email has been changed** will be sent to your old email address

   ![email_change_confirmation.jpg](images/21016940900882_email%20change%20confirmation.jpg)
   *The email with the link to confirm the new email address*

## Changing your email on Enterprise plans

### Single sign-on (SSO) enabled emails

You cannot change your email in your Profile settings if you use [Single sign-on](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) to log in to Miro. Your email will need to be changed on your identity provider’s side by your IT department, as well as on the Miro side. Please [reach out to the Miro Support Team](../tools/troubleshooting/06-contacting-miro-support.md#how-to-contact-miro-support) for assistance.

### Enterprise emails

If the email address that you're trying to change is claimed by an Enterprise subscription using [Domain Control](../../enterprise-administration/canvas-25-admin-features/domain-control/01-domain-control.md), you’ll see the error **You cannot change your email to or from a domain belonging to an organization**.
Changes to Enterprise emails must first be authorized by Miro. Please [reach out to the Miro Support Team](../tools/troubleshooting/06-contacting-miro-support.md#how-to-contact-miro-support) for assistance. Once your request is approved by Miro support you can then log in to Miro with your new email.

## Common errors when changing your email

**Password in user profile not set**

1. Log out and go to the [password recovery page](https://miro.com/recover/)
2. Enter the email you use to log in to Miro and click **Continue**
3. We’ll send you the password reset instructions. Click the link in the email, create a new password and click **Continue**
4. Once your password is set, log in to Miro using your email and the newly created password. You can then update your email in the Profile settings

**I did not get a confirmation email**

Check your Spam, Promotions, Junk, Social, and Updates folders to see if the confirmation email is there. A firewall may be preventing the email from reaching your inbox.

Please reach out to your system administrator and ask them to allowlist our domains and subdomains: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com and realtimeboard.com*, *.realtimeboard.com.

Learn more about [how to allowlist Miro mailers](../tools/troubleshooting/02-allowlist-miro-mailers.md).

**Clicking the email link to confirm my new email brings me to the registration page**

When you click the link to confirm your new email address, make sure that you are authorized in Miro under your old email address.

If you continued on the registration page and signed up with your new email address, you’ll have two profiles and cannot change your old email to the new one. In this case, log in with your new email address and [delete the profile](07-how-to-delete-your-profile.md) (please make sure you do not delete any content that you may need). Then log in with your old email and change it to the new one in your Profile settings.
