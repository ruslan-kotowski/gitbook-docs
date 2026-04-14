---
title: Enterprise two-factor authentication (2FA) – admin guide
article_id: 7935391125394
sidebar_position: 1
created_at: '2022-10-04T08:57:18Z'
updated_at: '2026-01-13T13:35:36Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  roles: company_admin
  notes: 'Relevant for: Enterprise Plan'
---

## Two-factor authentication (2FA) for organizations

2FA adds an extra layer of security to online profiles, going beyond just username and password. Enterprise Company Admins can mandate an additional proof of identity when users access their organization's Miro subscription. This requirement is applicable for all logins using email and password.

For companies using SSO, 2FA includes only non-SSO external collaborators. For companies not using SSO, 2FA extends to all users.

:::note
This article explains two-factor authentication (2FA) for Enterprise plans. For all other plans, see [Two-factor authentication (2FA)](../../../administration/security-compliance/01-two-factor-authentication-2fa.md) in Administration.
:::

## Setting up enforced 2FA for your organization

:::note
Before activating two-factor authentication (2FA), it's important to inform all impacted users, including both members within your organization and external collaborators. To ensure a smooth transition, we suggest sharing our [2FA user guide](../../security-integrations/two-factor-authentication-2fa/02-enterprise-two-factor-authentication-2fa-–-user-guide.md) to assist them through this process.
:::

## How to enable 2FA for your users

1. Go to Admin console > **Security** > **Authentication**.
2. Toggle on **Enforce 2FA for non-SSO users**.

![2FA-enable.png](images/24790277317394_2FA-enable.png)*Enforcing 2FA authentication for non-SSO users*

### Trusting 2FA devices

When enabled, your 2FA users will be shown a checkbox which allows them to skip 2FA each time they sign in on that device for the next X days, where "X" is the time frame set by the administrator. You can allow user devices to be trusted for 7 to 90 days. By default, trusting 2FA devices is enabled, though you can disable the feature in your Admin console.

![2FA-trusted-devices.png](images/24790277323410_2FA-trusted-devices.png)

:::warning
If trusting 2FA devices is disabled, users will have to enter a 2FA code on every sign in. This will slow down the sign in experience.
:::

2FA will be required again after the trusted period passes.

2FA will not be skipped if users sign in on a new device or browser or if they clear their browser cookies.

## Resetting 2FA for users

If a user loses access to their 2FA method, admins can reset their 2FA. Once a user requests that their 2FA method be reset, the appropriate admin will receive an email notification.

:::note
Admins can reset two-factor authentication only for users whose email domains are verified in their organization, if the admin initiates the reset. If the user requests a reset, then any admin in the organization can approve it.
:::

To reset the 2FA method for the user:

1. Go to **Admin console** > **Users** > **Active users** tab.
2. Find the user who needs their 2FA method reset.
3. Click the **three dots** (**...**) icon on the user's row.
   ![reset-2fa.png](images/24650686629138_reset-2fa.png)
   *Resetting two-factor authentication in the Admin console*
4. Click **Reset two-factor authentication**.
   A dialog will open asking for confirmation.
5. Click the **Reset 2FA** button in the dialog.
6. A confirmation message will appear at the top of your screen confirming that reset instructions have been sent to the user.

## Impact on user experience

- Non-SSO users will be prompted to set up their second factor during their next login. This process will not log them out from any ongoing sessions.
- Users are required to configure 2FA using their mobile device along with a time-based one-time password (TOTP) application, such as Microsoft Authenticator, Google Authenticator, or Authy.
- For users using 2FA, there is a limit of 3 attempts to enter a valid TOTP code. If this limit is exceeded, they will need to start the authentication process again.
- While 2FA login is available on mobile and tablet apps, the initial registration process is supported exclusively on browser and desktop applications.

## Important to know

Enforcement of 2FA only applies to *users authenticating with their email and password or via magic links (sent via email)*.

- 2FA is not enabled for external collaborators who authenticate using SSO.
- If an external collaborator to your Enterprise organization is already authenticating using SSO from their home organization, they will continue to access all the teams and boards in Miro using SSO.
- When a user authenticates through a third-party login integration (e.g., Google, Microsoft, Slack), they will maintain access to all Miro teams and boards via that login method. Admins have the option to encourage these users to set up a second factor within their respective login integration. However, Miro's authentication flow will not prompt these users to set up a second factor.

## Audit logs

Administrators can track users who have set up 2FA, along with 2FA login successes and failures with the following audit log events:

- `mfa_setup_succeeded` - if a user has successfully set up their second factor
- Update to `sign_in_succeeded` event to include MfaFactorType attribute if a successful login is completed with 2FA
- Update to `sign_in_failed` event to include MfaFactorType attribute if a login with 2FA was unsuccessful due to the user exceeding the maximum number of attempts (non-technical failure)
