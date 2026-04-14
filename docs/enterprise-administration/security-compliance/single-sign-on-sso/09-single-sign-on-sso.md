---
title: Single sign-on (SSO)
article_id: 360017571414
sidebar_position: 9
created_at: '2019-02-11T10:08:59Z'
updated_at: '2026-01-07T13:25:39Z'
draft: false
availability:
  plans: business, enterprise
  roles: company_admin
---

With SAML-based single sign-on (SSO), users can access Miro through an identity provider (IdP) of their choice.

## How SAML SSO works

1. When a Miro user tries to log in to Miro using SSO, Miro sends a SAML (Security Assertion Markup Language) request to the identity provider (IdP)
2. The identity provider validates the user’s credentials and sends a response back to Miro to confirm the member's identity
3. Miro acknowledges the response and grants access, allowing the member to log into their Miro account

## What happens after enabling SSO?

**Enabling SSO for the first time**

The first time you set up SSO, existing users can keep working in Miro without interruption. However, the next time they log out, their session expires, or they try to log in from a new device, they will need to sign in via SSO.

Other login options will be disabled for users, including standard login + password, Google, Facebook, Slack, AppleID and O365.

**Idle session timeout**

If you have enabled [Idle Session Timeout](../../security-integrations/security-management/02-idle-session-timeout.md), users are automatically logged out of their Miro profile and will need to authorize via SSO again.

**Multiple teams and organizations**

If your users have multiple Miro teams or organizations, you can configure them to use the same identity provider (IdP) for authentication.

**Who is required to sign in with SSO**

SSO sign in is required for active users that are part of your Enterprise subscription *and* have a domain listed in your SSO settings.

- Users accessing Miro from domains not added in your SSO settings are not required to log in with SSO, and should instead log in using the standard login methods.
- Users from a verified domain, who are not part of your Miro Enterprise subscription, need to sign in via single sign-on (SSO) only if [just-in-time (JIT) provisioning](../../user-management/13-user-provisioning-on-enterprise-plan.md#just-in-time-provisioning-jit) is enabled. These users will automatically be added to a pre-configured team and will be required to use SSO for login.
- [Managed users](../../user-management/06-managed-users-on-enterprise-plan.md), which is any user inside your verified domain(s), including any managed user who is also a member of a team outside of your Enterprise subscription. To restrict access to specific teams, update your [domain control](../../canvas-25-admin-features/domain-control/01-domain-control.md) settings.

  > ✏️ For an Enterprise subscription, an organization can have verified and unverified domains. For verified domains, users become managed users who must authenticate with SSO. For unverified domain users in the same organization, email and password are required for authentication.

**Managing user details**

User data is automatically attributed in Miro by your identity provider upon successful login. Some parameters like name and password cannot be changed. Other parameters like department and profile pics are optional.

- Miro Usernames are updated after every successful user authentication. For more information on how to set up Miro usernames, see the [advanced SSO settings](#optional-advanced-sso-settings). If you need to change a user's email address, you can do so only via [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md). If you do not use SCIM, please [reach out to the Support Team](https://help.miro.com/hc/requests/new?referer=help-center-article).

![sso-settings-2.png](images/21027132582290_sso-settings-2.png)
*Domain selection in SSO settings*

> **💡**To prevent a lockout, create a 'break the glass' user with an email that has a domain outside of the domain listed in the SSO settings, like acmebreaktheglass@gmail.com. Otherwise, you can contact support, and they can disable SSO for the whole organization.

## Configuring SSO

### Identity providers (IdP)

Use any identity provider of your choice. Below are the most popular identity provider platforms:

- [OKTA](../../security-integrations/single-sign-on-sso/07-how-to-configure-okta-sso.md)
- [Entra ID](../../security-integrations/single-sign-on-sso/05-how-to-configure-entra-id-sso.md) by Microsoft
- [OneLogin](../../security-integrations/single-sign-on-sso/08-how-to-configure-onelogin-sso.md)
- [ADFS](../../security-integrations/single-sign-on-sso/02-how-to-configure-adfs-sso.md) by Microsoft
- [Auth0](../../security-integrations/single-sign-on-sso/03-how-to-сonfigure-auth0-sso.md)
- [Google SSO](../../security-integrations/single-sign-on-sso/06-how-to-configure-google-sso.md)
- [Jumpcloud SSO](https://support.jumpcloud.com/support/s/article/single-sign-on-sso-with-miro)

### How to configure your IdP

> **💡** If your Enterprise organization would like to add [multiple identity providers](../../security-integrations/single-sign-on-sso/01-adding-multiple-identity-providers.md) (IdPs), sign up for our [private beta](https://coda.io/form/Miro-Multi-IdP-Private-Beta-Sign-Up_dkoTJMza_jV).

1. Go to your identity provider's configuration section and follow the provider's instructions to configure single sign-on.

2. Add the following metadata. We recommend skipping any optional fields and leaving any default values as they are.

#### Specs (metadata)

|  |  |
| --- | --- |
| **Protocol** | SAML 2.0 |
| **Binding** | HTTP Redirect for SP to IdP HTTP Post for IdP to SP |
| **The service URL** (SP-initiated URL)  Also known as Launch URL, Reply URL, Relying Party SSO Service URL, Target URL, SSO Login URL, Identity Provider Endpoint, etc. | https://miro.com/sso/saml |
| **Assertion Consumer Service URL**    Also known as Allowed Callback URL, Custom ACS URL, Reply URL | https://miro.com/sso/saml |
| **Entity ID**    Also known as Identifier, Relying Party Trust Identifier | https://miro.com/ |
| **Default Relay State** | must be left *empty* in your configuration |
| [**Signing Requirement**](https://developers.onelogin.com/saml/examples/response) | An unsigned SAML Response with a *signed* Assertion  A signed SAML Response with a *signed* Assertion |
| **SubjectConfirmation Method** | "urn:oasis:names:tc:SAML:2.0:cm:bearer" |
| Identity Provider SAML-response must contain **Public key x509 certificate** issued by the Identity Provider.  View detailed [SAML examples](https://www.samltool.com/generic_sso_res.php). Download the [Miro SP metadata file](https://drive.google.com/file/d/1BN58fiwC062F5MC-PsO3QN7JlCbKNCSJ/view) (XML). | |

:::warning
Encryption and Single Log Out are not supported.
:::

#### User credentials

Any additional fields outside the below are not required. We recommend skipping any optional fields and leaving any default values as they are.

|  |  |
| --- | --- |
| Required user credential attributes | |
| **NameID**(equals a user’s email address)  Also known as SAML_Subject, Primary Key, Logon Name, Application username format, etc. | &lt;NameID Format="urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress"&gt; |
| **Optional attributes to be sent with the assertion**  (updated with every new authentication via SSO, used when present/available) | - "DisplayName" or "http://schemas.microsoft.com/identity/claims/displayname" (used as preferred name)   [mceclip0.png](http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname)   - “FirstName”, "GivenName" or "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname"; - “LastName”, "Surname" or "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname"; - “ProfilePicture“ - The encoded URL of the image |

### How to enable SSO in your Miro settings

Business Plan Enterprise Plan

1. Go to your **Company** settings > **Security** > **Single sign-on**
2. Toggle on **SSO/SAML**

*![security-sso.png](images/20889990489874_security-sso.png)*

1. Go to your **Company** settings > **Security & Compliance** > **Authentication** > **Single sign-on**
2. Toggle on **SSO/SAML**

*![sso-enterprise.png](images/20937366644626_sso-enterprise.png)*

:::warning
Enabling SSO in your settings does not immediately enable SSO for users. SSO login is available after your [domains are verified](../../canvas-25-admin-features/domain-control/01-domain-control.md). Then, when you configure SSO in [the next section](#how-to-configure-sso-in-your-miro-settings), ensure that you add your verified domains.
:::

### **How to configure SSO in your Miro settings**

After toggling on the SSO/SAML feature in single sign-on settings, fill in the following fields:

1. **SAML Sign-in URL** (in most cases it opens your Identity Provider's page where your end-users are to enter their credentials)
2. **Public Key x.509 Certificate** (issued by your Identity Provider)
3. All domains and subdomains allowed or required (ACME.com or ACME.dev.com) to authenticate via your SAML server
4. Add your verified domain(s). For **Users from these domains will sign in using SSO**, click ***Select a domain***, and select any of your domains to add to the list.

![sso-settings.png](images/20937366648082_sso-settings.png)
*Miro SSO settings*

### Expiration and renewing your SSO/SAML certificate

If your Public Key x.509 Certificate has expired, SSO will continue to work, but it is strongly recommended to renew it in order to continue using Miro securely. Public Key x.509 Certificates ensure the security, privacy, authenticity, and integrity of information shared between your identity provider and Miro.

These certificates are only valid for a period of time which can be specified (and verified) with your identity provider. Please check with your identity provider to verify the expiration date.

:::note
Miro sends admins email reminders 60, 30, and 7 days before their SSO certificate expires. Admins also receive a one-time email after the certificate expires.
:::

There are two steps to this process:

1. Renew the certificate with your identity provider. Please check their instructions on how to do this.
2. Add the renewed certificate to your Miro SSO configuration.

#### Adding renewed certificates to Miro

:::warning
We recommend replacing your x.509 certificate during less busy periods in your organization (for example on the weekend or after business hours) to avoid login disruptions.
:::

1. Go to your **Company settings** > **Authentication** > **Single sign-on**
2. Delete the content inside the **Key x.509 Certificate** field
3. Paste the new key inside this field
4. Scroll down and click **Save**
   ![sso-gif-2.gif](images/21027132584850_sso-gif-2.gif)
*Renewing an x.509 certificate in Miro*

## Testing your SSO configuration

Test your SSO configuration before enabling it to reduce the chances of login issues for your users.

1. Complete the steps above to configure your SSO settings.
2. Click the **Test SSO configuration** button.
3. Review the results:

- If no issues are found, a confirmation message **SSO configuration test was successful** will be displayed.
- If issues are found, a confirmation message **SSO configuration test failed** will be displayed, followed by detailed error messages to guide you on what needs to be fixed.

![sso-test.png](images/20937366649618_sso-test.png)
*Testing SSO configuration*

## Optional advanced SSO settings

The optional settings section is used by advanced users who are familiar with SSO configuration.

### Just In Time Provisioning for new users

Make it easier for your users to get started with Miro right away, without having to wait for an invitation or going through a lengthy onboarding process. And ensure free teams are not created outside of your managed subscription (requires domain control). SSO is required to enable the Just-in-Time (JIT) provisioning of new users. All users provisioned under JIT are assigned the default license of your subscription:

|  |  |  |
| --- | --- | --- |
| **Subscription type** | **License type** | **Behavior when licenses run out** |
| Business Plan | Full License | Users are not automatically added; JIT feature stops working. |
| Enterprise Plan (without [Flexible License Program](../../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)) | Full License | Users provisioned under [Free Restricted](../../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) license |
| Enterprise Plan (with Flexible License Program activated) | Free or Free Restricted License | Depends on the [default license](../../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md) settings |

### How to enable Just-in-Time provisioning

When you activate Just-in-Time provisioning, it will automatically apply to all new users who register to Miro. However, existing Miro users will still need an invitation to join your plan.

1. Go to your SSO settings
2. Tick the box **Automatically add all newly registered users from the listed domains to your Enterprise account**
3. **Choose a default team for newly registered users** from the dropdown
4. Click **Save**

When you list specific domains in your single sign-on (SSO) settings, any users who register with those domains will be automatically added to your Enterprise subscription. They will be assigned to the team you have selected in your Just-in-Time (JIT) settings.

![Copy of user_provisioning_jit_provisioning.png](images/21017528391698_Copy%20of%20user_provisioning_jit_provisioning.png)*Enable Just in Time provisioning feature on the Enterprise integrations page*

All *newly registered users* from the domains that you list in the settings will be automatically added under your EnterpriseUmbrella to **this particular team**when they sign up with Miro.

:::warning
On the Enterprise plan this team will also be shown in the list of discoverable teams if you enable [Team Discoverability](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md#team-discovery).
:::

### Setting DisplayName as the default username

By default, Miro will use **FirstName** + **LastName** attributes. Alternatively, you can request to use **DisplayName** instead. In this case, Miro will use **DisplayName** *when it's present* in the user's SAML response.

If the **DisplayName** is not present, but **FirstName** + **LastName** are, Miro will use **FirstName** + **LastName.** Please get in touch with Miro Support to make **DisplayName** your preferred SSO Username.

If neither of the three attributes is present in your SAML communication, Miro will show the user's email address as Username

|  |  |
| --- | --- |
| **Setting** | **Default Username** |
| Miro Username | FirstName + LastName |
| Alternative Setting | DisplayName (if present in the user's SAML request) |
| Fallback | FirstName + LastName (if DisplayName is not present) |
| Preferred SSO Username | DisplayName ([contact Miro Support](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)) |
| No attributes present | Email address displayed as Username |

If you see something different than expected you may need to authenticate via SSO, or it's possible that the SAML-response does not contain the values needed to update.

### Syncing user profile pictures from IdP

:::warning
Generally it's recommended to enable this option if you do not enable SCIM, or your IdP does not support the **ProfilePicture**attribute (for example, **ProfilePicture** is not supported by Entra). In other cases, it is recommended to pass **ProfilePicture** via [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) with immediate updates.
:::

When this setting is turned on:

- profile picture set at IDP side will be set as profile picture in the user’s Miro profile
- users won’t have the ability to update or remove their profile picture themselves

As with the user name attribute, users will not be able to change their data on the Miro end immediately, but the data *sync* is not immediate, the IDP side sends the update to Miro only with the user's *next* SSO authentication (provided that “Sync user profile photos from IDP” setting is still active at that point).

If the profile picture is set in IDP and you wish the attribute to be passed in SAML communication, Miro will expect the following schema:

```
<saml2:Attribute Name="ProfilePicture" NameFormat="urn:oasis:names:tc:SAML:2.0:attrname-format:uri">
<saml2:AttributeValue
xmlns:xs="http://www.w3.org/2001/XMLSchema"
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">https://images.app.goo.gl/cfdeBqKfDKsap1icxecsaHF
</saml2:AttributeValue>
</saml2:Attribute>
```

## SSO and data residency

If you use [Data Residency](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md) support from Miro and have a dedicated URL (workspacedomain.miro.com) then you must adjust your identity provider's configuration.

:::note
For organizations with data residency in Australia and the United States, social login is unavailable. For more information about data residency, see [Data residency at Miro](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md).
:::

To do this, you will need to add your organization ID to the URL.

You can find your organization ID from the Miro dashboard by clicking on your **Profile** in the upper right corner > **Settings** > it's shown in the URL in the address bar.

|  | Standard value | Value under Data Residency |
| --- | --- | --- |
| **Assertion Consumer Service URL**(aka Allowed Callback URL, Custom ACS URL, Reply URL): | https://miro.com/sso/saml | https://workspace-domain.miro.com/ sso/saml/ORGANIZATION_ID |
| **Entity ID**(Identifier, Relying Party Trust Identifier): https://miro.com/ | https://miro.com/ | https://workspace-domain.miro.com/ ORGANIZATION_ID |

## Setting up Multi-factor authentication (2FA) for users outside SSO

Two-factor authentication (2FA) provides an added layer of security. With 2FA, users are required to complete an extra step during login to verify their identity. This additional measure ensures that only authorized individuals can access your subscription.
Learn more in our [Two-factor authentication admin guide](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md).

## Frequently asked questions and resolving possible issues

My domain addresses are not accepted in the SSO settings - `DomainName is busy` message.

For security reasons, we support an organization's domain(s) in *one Company umbrella (Enterprise subscription) only*. It is possible that your domains are already set up in another Business Plan or [Enterprise Plan](../../../plans-billing/miro-plans/04-enterprise-plan.md), preventing you from enabling SSO with the desired domain. You may wish to check it with your colleagues beforehand.

My domain is not appearing in the dropdown for available domains.

You first need to claim and verify your domains in [Managed Domain settings](../../canvas-25-admin-features/domain-control/01-domain-control.md).

We need to change the email addresses of our end-users / We changed the emails of our users, and now they are unable to access their boards.

If your company is changing its domain name and, therefore the email addresses of the end-users need a change of their SSO credentials, please [reach out to our Support Team](https://help.miro.com/hc/requests/new?referer=help-center-article)for assistance.

We would like to use a separate gateway (for instance, MFA, like Duo Dag) for the SSO procedure.

You can certainly do that. Miro will support your preferred solution for as long as it works under SAML 2.0.

We enabled SSO, but user profiles' data (names, profile pictures - if supported by your IdP) in Miro are not synchronized with those in the IdP.

Miro user name and profile picture are updated after every successful user authentication *if* SAMLResponse contains new non-empty values. For more information on how to set up Miro username, see [Advanced optional SSO settings](#optional-advanced-sso-settings).

What is the process for changing SSO providers?

When changing SSO providers, you will need to configure the new IDP from scratch as you would in a first-time setup.

If one or all of your users encounter an error when trying to sign into Miro, please check [this list of common errors](../../../using-miro/tools/troubleshooting/10-i-can't-log-in-via-sso.md) and how to resolve them.
