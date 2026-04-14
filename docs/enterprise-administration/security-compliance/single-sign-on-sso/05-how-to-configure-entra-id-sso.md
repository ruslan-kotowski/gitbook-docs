---
title: How to configure Entra ID SSO
article_id: 360022722233
sidebar_position: 5
created_at: '2019-05-07T12:03:08Z'
updated_at: '2025-11-25T16:04:59Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: business, enterprise
  roles: company_admin
---

> *💡 It is strongly recommended to configure SSO in a separate incognito mode window of your browser.* This way, you keep the session in the standard window, allowing you to switch off the SSO authorization in case something is misconfigured.

If you wish to set up a test instance before enabling SSO on production, please [reach out to the Support Team](https://help.miro.com/hc/requests/new?referer=help-center-article) for assistance. Only those who configure SSO will be added to this test instance.

> **⚠️ See our main SSO article** [**here**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **for rules, supported features and optional configuration on the Miro end.**

## Adding and configuring the app

 1. Find the Miro pre-configured application in Entra ID Enterprise Application Gallery ([Enterprise Applications](https://portal.Entra.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/) > +New Application).

2. Create the application and click **2.** **Set up single sign-on** (or select **Single sign-on** from the left side and select the **SAML** sign-on method).

3. You will see that the **Basic SAML Configuration** is already in place:

:::warning
if after everything is set up the SSO login fails, try changing the Entity ID from `https://miro.com`to `https://miro.com/`
:::

:::warning
Sign-on URL, Relay State and Logout URL (For Single Sign-Out) must be left empty since these functionalities are not supported.
:::

The **Attributes & Claims** are also already in place:

:::warning
Note that:
a) the UPN will become the main parameter by which a user in Miro will be recognized and this parameter will not be updateable from the Entra side. When you need to update user emails in Miro without using SCIM, please [reach out to our support team](https://help.miro.com/hc/requests/new?referer=help-center-article).
b) Miro will accept [**GivenName,** **Surname**, **DisplayName** and **ProfilePicture**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Other attributes are not supported via SSO but can be transferred via [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).
:::

### Creating the Certificate

1. In Microsoft Entra,  ensure that the **SAML Signing Certificate** > **Signing Option** is either **Sign SAML Assertion** or **Sign SAML response and assertion**.

2. **Download** the **Base64** file.

## Configuring SSO in your Miro plan

1. Open the **Base64** downloaded file in a text editor, and then copy the **x509** certificate from the file.

2. In Miro, under **Security > Authentication**, paste the copied **x509** certificate into the **Key x509 certificate** box.

3. In the Microsoft Entra settings UI, copy the **Login URL**, and then go to the Miro **Security > Authentication** page, and paste it into the **SAML Sign-in URL** box.

4. In the Miro **Security >**  **Authentication** page, on the **Users from these domains will sign in using SSO** section, ensure that you add at least one company domain.

:::warning
In Miro, ensure **Sync profile photos from IdP** is not checked. Entra ID does not support syncing user profile photos. When **Sync profile photos from IdP** is not checked, users are able to set their own profile photos.
:::

5. Click **Save**.

Your SSO configuration is now complete.

## Configuring claims when UPN and Email differ

You can configure the settings to use any Entra attribute which is in the email format as the **NameID** in Miro.

### IDP- and SP-initiated logins

*For IDP-initiated login*, Entra sends Miro the value you decide to use as the **NameID** (**user.mail**in the example below).

With this flow, your end-users access Miro via the icon on their portal console (for example at `https://myapplications.microsoft.com/`). From there a request is sent to Miro and *the user is logged in using the **NameID** you defined.*Miro will expect this attribute to match the user's**email**in Miro. A mismatch will result in failed authentication.

*For SP-initiated login*, Miro will send a request specifically for the user's **UPN** and will expect it to match the user's **email** in Miro. A mismatch will result in failed authentication.

Now, the **SAML Sign-in URL** field in your Miro settingd is expected to contain the **Login URL** of the Miro app of your Entra instance. This will be the URL Miro will direct the user to from the [Miro Login page](https://miro.com/sso/login/).

When the user is directed to the Login URL from the app, the SAML request is generated. With this flow, the user is logged in with the email address that the user entered on the Miro login page and which Miro then requests from Entra requiring it to be the UPN attribute.

### How to set up

To allow your users to access Miro with their Entra's **Email** rather than **UPN** you can fill out the **SAML Sign-In URL** field in Miro with the URL of the app from the Entra console. Then the SP-initiated flow will be as follows:

1. The user accesses Miro entering their Miro email which is the email they have in Miro. Miro understands that the person should be logged into the defined user profile.
2. The user is directed to their app link that is used for the IDP-initiated login.
3. The link utilizes the **NameID**attribute *that you defined* and sends it to Miro.
4. The user is therefore logged into Miro into the previously defined user profile with the **NameID** you defined.

If you'd like to also enable auto-provisioning for Miro, check out [this article](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

If you encountered any issues during configuration, please check out [this article](../../../using-miro/tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## Entra testing tool

To get to the testing tool, choose the **Single Sign-In** tab in the settings of your application and scroll down to the bottom of the section.

Entra suggests using the test login process to check the connection and troubleshoot an error message. After the test, you will be given instructions on how to solve the situation.

Please keep in mind which credentials managed by Entra/ADFS your workstation is authenticated with. If you are trying to use a different set to log into Miro the login attempt may fail, as the Identity Provider will transfer your main set of credentials and there will be a mismatch. For instance, this can happen if you are the SSO administrator and test the login procedure under different user credentials.

## Alternatively, you can test in Miro

1. Complete the steps above to configure your SSO settings.
2. Click the **Test SSO configuration** button.
3. Review the results:
   1. If no issues are found, a confirmation message **SSO configuration test was successful** will be displayed.
   2. If issues are found, a confirmation message **SSO configuration test failed** will be displayed, followed by detailed error messages to guide you on what needs to be fixed.

##
