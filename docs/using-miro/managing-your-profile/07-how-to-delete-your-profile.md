---
title: How to delete your profile
article_id: 360017571354
sidebar_position: 7
created_at: '2019-02-11T10:08:54Z'
updated_at: '2026-01-07T13:30:06Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
availability:
  roles: profile owner
---

Deleting your profile from Miro will result in your information being removed from our system. Please note that a profileand a team are two different things.

- Your profile represents your data connected to your registration and email address
- A team is a space that you are a part of together with other team members where members can create content and store their boards

Every profile can be associated with several teams. If you wish to remove a team, find out how to do that [here](../../administration/team-management/06-delete-and-restore-teams.md).

:::warning
Profile deletion **cannot** be undone.
:::

:::warning
Note that profile deletion does not cancel your active subscriptions. To stop further renewals, please [cancel your subscription in settings](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md).
:::

### How to delete your profile

1. Open your [Profile settings](https://miro.com/app/settings/user-profile/).

2. Scroll to the bottom of the page and choose **Delete my profile.**

![Delete_profile.png](images/21017429126546_Delete%20profile.png)
*Deleting your profile*

3. At this point, we suggest saving [backups](../import-and-export/export/05-how-to-save-board-backup.md) or [exporting](../import-and-export/export/03-how-to-export-your-board.md) your boards before deleting them.

![profile_removal_modal.jpg](images/21017429125778_profile%20removal%20modal.jpg)*Profile removal confirmation message*

4. Shortly afterward, you will receive an email with a confirmation link. Click the link to finish. Please note that you need to be logged in to your Miro profile in the browser when clicking the **Delete profile** to successfully complete the profile deletion.

![Profile_deletion_email.jpg](images/21017416055186_Profile%20deletion%20email.jpg)
*Confirmation email to delete the profile*

### What happens to your content after profile removal

As soon as you remove your profile, your boards get deleted.

If you are the only Admin for your team, the content will be removed *completely*. The Admins rights will be granted to the member invited first chronologically.

If there are other Admins in the team you're a member of, then content will be deleted and reassigned to one of the Admins - it means that the admin will be able to [restore your boards within 90 days](../managing-boards/08-how-to-restore-a-deleted-board.md) (paid users will find them in Trash, free users will be able to restore via link).

### Frequently asked questions

1. *Can I delete my profile if I log in to Miro with* [*Single Sign-On (SSO)*](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)*?*
   - Whether you can delete your profile depends on how your account is managed. Organization admins can’t permanently delete user profiles. They can only deactivate users or remove them from an organization. For SCIM-managed accounts, profiles can’t be permanently deleted. As long as the user exists in the IdP, the profile will remain or be recreated.
2. *How can I change my email address linked to the Miro profile?*
   - Use this guide: [How to change your email](04-how-to-change-your-email.md).
3. *I do not receive the email with the confirmation link. What do I do?*
   - Please try these steps:

- Open your **Spam, Promotions, Junk, Social**, and **Updates** folders and check to see if Miro confirmation email is there
- Check to see if your inbox is full to make sure you haven’t reached the memory limit with your email inbox. If it is full, you may need to delete some existing emails in order to receive new ones. After deleting emails, request the profile deletion again
- It may be that a firewall is preventing the email from reaching your inbox. Please reach out to your *system administrator* and ask them to allowlist our domains and subdomains: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) and [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). [Here is an article](../tools/troubleshooting/02-allowlist-miro-mailers.md) with more information on the mailers you need to allowlist
- If neither of the solutions help, [report the issue to Miro Support](../tools/troubleshooting/06-contacting-miro-support.md)
