---
title: Domain control
article_id: 360034831793
sidebar_position: 1
created_at: '2019-08-23T19:17:18Z'
updated_at: '2026-03-27T15:52:06Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: business, enterprise
  roles: company_admin, system_admin
---

Domain control empowers Company Admins to manage user access within their subscription. By utilizing Domain control, admins can enforce corporate security compliance and maintain oversight over managed user activities within their domains.

Learn how to set up and manage Domain control within your organization.

**With Domain control, Enterprise plan admins can:**

- Conduct audits to identify users who are associated with a managed domain that is not included in your subscription, and invite them to join.
- Prevent users within a domain from creating unauthorized subscriptions.
- Automatically add newly registered users to designated teams.
- [Block deactivated users](../../user-management/02-block-deactivated-users.md) to prevent their access to Miro using their corporate email address.

**Business plan admins:**

- Can use automated domain verification to manage domains. Only newly added domains will be automatically verified.
- Cannot change Domain control policies.
- Cannot request a domain audit.

![domain-policies-business.png](images/21046889202834_domain-policies-business.png)

*Domain policies can be viewed under Managed domains for Business plan users*

Business plan users will need to upgrade for other advanced features.

:::note
Bulk domain management is not currently supported.
:::

## Primary domain

Your primary domain determines how Miro identifies internal and external users in your organization. To learn how to view, change, or manage your primary domain, see [Manage your primary domain](https://help.miro.com/hc/en-us/articles/34249718672274).

## Set up Domain control

### Step 1: Add domains

1. Open your Miro dashboard.
2. Click on your profile picture in the top-right corner.
3. Select **Settings** from the dropdown menu.
4. On the left pane, navigate to **Security & compliance**, and click **Managed domains**

   > ✏️ On Business plans, **Managed domains** is found under **Account**.
5. Click **+ Add a domain** and enter the full domain name (e.g., yourcompany.com).
   ![Managed-domains-settings.png](images/21017318776338_Managed-domains-settings.png)
*Managed domain settings*

:::note
If you have enabled [**Block deactivated users**](../../user-management/02-block-deactivated-users.md), then all deactivated users associated with a newly verified domain are blocked automatically.
:::

### Step 2: Verify domains

1. After adding a domain, you will receive a verification code within your **Managed domain** settings. Copy this code.

   ![Complete-domain-verification.png](images/21017318779282_Complete-domain-verification.png)
*Copying the verification code*
2. If you manage your DNS records, update your DNS settings by adding a TXT record with the verification code as its **Value**. (If someone else manages your DNS records, forward them the verification code with instructions to update the DNS records.)
3. Log into your domain provider’s website (GoDaddy, Amazon, Cloudflare, etc), and navigate to the **DNS** **records** section.
4. Create a new **TXT-record** with the following specifications:
   **Value/Answer/Description:** *“miro-verification=[INSERT VERIFICATION CODE]”*
   **Name/Host/Alias:** Leave this blank or type @ to include a subdomain.
   **Time to live (TTL):** “86400” (this can also be inherited from the default configuration).

   ![Creating-new-TXT-record.png](images/21017318775314_Creating-new-TXT-record.png)
   *Creating a new TXT-record*

:::note
You can update the TXT record through the administration console or dashboard of the domain's hosting DNS provider. View the [list of DNS providers](https://support.google.com/a/topic/1409901).
:::

### Step 3: Check domain verification

1. After updating the DNS record, check the status of your domain verification immediately in your **Managed domain** settings by clicking **Check verification**.
2. If the domain is not verified immediately, Miro will automatically check for the verification code every 2 hours for the next 30 days.

### Step 4: Notification of verification status

1. Once your domain is successfully verified, you will receive an email notification confirming the verification status.
2. Please do not remove the DNS-record after verification, as it may be needed for future verifications.
   ![Check-domain-verification.png](images/21017348597650_Check-domain-verification.png)
*Checking domain verification*

## Rules when verifying domains

- You will need to create a separate TXT record for each top-level domain and each subdomain you use. Follow steps 1-4 above for each domain or subdomain you wish to verify.
- Your domain must be an exact match.

  > ✏️ Subdomains are not allowed.
- Ensure that all zones used in the verified domain configuration are included.
- The Fully Qualified Domain Name (FQDN) should match your domain address. For example, [www.mycompanydomain.com](http://www.mycompanydomain.com).
- If you use both internal and external DNS, we recommend verifying both to ensure comprehensive domain control.

## Managing users and access

### Edit domain settings

Domain settings determine how existing and newly registered users within your domain(s) are managed.

1. Once a domain is verified, click the three dots (**...**), and select **Edit domain settings**.
   ![Edit-domain-settings.png](images/21017318773138_Edit-domain-settings.png)
*Editing domain setting*
2. You will see options for handling new users to your domain:

- **Auto-capture new users**: Automatically add users who sign up to Miro with a managed domain email to this domain’s subscription with its default license type. You can also define which teams the users will be added to (required).
- **Block users from creating their own subscriptions**: Prohibit managed users within your domain(s) from creating any new teams outside of your subscription. However, these users can still be invited to teams in your domain(s) and collaborate externally.

  ![Managed-domain-settings.png](images/21017318773778_Managed-domain-settings.png)
*Options for handling new users to your domain*

  > ✏️ If you enable **Block users from creating their own subscriptions**, then users cannot self-register unless invited, or auto-capture or JIT is enabled.

### Internal and external users

When a domain is claimed, user details include an **Internal** or **External** classification.

![](images/33613933595794_image.png) *User details show whether the user is external or internal to your verified domain*

Internal users have an email address from a domain claimed by your Enterprise account. For example, `user@acme.com` where `acme.com` is one of your verified domains.

External users have an email address outside any domain claimed by your Enterprise account. For example, `user@not-domain.com` where `not-domain.com` is not one of your verified domains.

:::note
User details are visible in the user profile. In Admin Console, user details are also visible in the user list, where you can optionally filter by **Internal** or **External** classification.
:::

Internal or external classification is automatic and based on whether the user's domain is claimed and verified by your Enterprise account.

## Self-serve teams to Enterprise plan consolidation

As a Company Admin you can bring all teams created from your domains into your Enterprise plan. This ensures enhanced security, collaboration, and streamlined management by unifying all teams in one place. Additionally, you can also audit domains to identify and consolidate users and teams that are part of your managed domain but currently outside your subscription.

For more information, [see the Team Consolidation documentation](../../managing-enterprise-teams-and-content/06-self-serve-teams-to-enterprise-plan-consolidation.md).

## Email change requests

If your enterprise has claimed a domain, any user associated with this domain will be unable to change their email address in Miro without the approval of the Company Admin. When attempting to change their email, users will receive the following error message: **You cannot change your email to or from a domain belonging to an organization**. It is recommended that users contact their Company Admin, who will then reach out to Miro support for assistance.

## Frequently asked questions

Can I use Domain control with a subdomain?

Yes, subdomains are treated as separate entities from primary domains. Follow the setup process for each subdomain you want to verify.

How do I use SSO with domain control?

You will need to set up Domain control before enabling [SSO](../../security-integrations/single-sign-on-sso/09-single-sign-on-(sso).md) authentication.

What if my domain name changes or I want to add a subdomain?

If your domain name changes, remove the domain and restart the verification process with the new domain or any subdomains you add.

Where do I find the DNS records for my domain?

To locate the DNS records for your domain, you'll need to access your domain registrar's platform where you registered your domain. If you're unsure who your domain registrar is, you can find this information by using **who.is** to search for the domain. Once you have identified your registrar, log into their website and navigate to the section usually labeled **Domains** or **DNS Management**. Here, you will find the DNS settings or records for your domain.

Why can’t I see **Managed domains** within my **Security & compliance** settings?

If you are unable to see the **Managed Domains** option, it could be due to two reasons:

- You are not subscribed to an Enterprise Plan which includes this feature.
- You do not have the Company Admin role required to access this setting.

Please verify your plan details and role with a Company Admin for further assistance.

Can I delete the TXT record for my domain once it’s been verified?

While deleting the TXT record after verification will not immediately affect the operation of your domain control, it is strongly advised to retain this record. Keeping the TXT record in place is crucial for potential re-verification processes in the future. Removing the TXT record could complicate these processes and require you to undergo the verification steps again.
