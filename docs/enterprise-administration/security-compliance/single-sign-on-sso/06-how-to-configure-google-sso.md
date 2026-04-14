---
title: How to configure Google SSO
article_id: 4716499382546
sidebar_position: 6
created_at: '2022-03-18T18:12:44Z'
updated_at: '2025-11-25T16:08:20Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: business, enterprise
  roles: company_admin
---

:::tip
It is strongly recommended to configure SSO in a separate incognito mode window of your browser. This way, you keep the session in the standard window, allowing you to switch off the SSO authorization in case something is misconfigured.
:::

Configuring Miro within your organization is easier than ever with the integration app Google has created inside the Google Workspace Admin Console. This app allows you to configure Google SSO for use with Miro, as well as [SCIM user provisioning](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md).

This article focuses on configuring Google SSO for use with Miro.

If you wish to set up a test instance before enabling SSO on production, please request it with your Account Executive or Sales representative. Only those who configure SSO will be added to this test instance.

:::tip
See the Miro [SSO article](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)  for rules, supported features and optional configuration settings.
:::

Read more on [setting up Google SSO with Miro](https://support.google.com/a/answer/14100608#zippy=%2Cstep-set-up-google-as-saml-identity-provider) on Google's Help Center.

## Setting up Google SSO for Miro using SAML

Setting up Google SSO to authenticate to Miro can be completed in four steps:

1. Setting up Google as SAML identity provider
2. Setting up Miro as SAML service provider
3. Turning on Miro for users
4. Testing authentication

Setting up Google as SAML identity provider

1. From your Google Workspace Admin Console, click **Apps > Web and mobile apps**
2. In the Apps panel click the **Add app** drop-down, choose “Search for apps” and type “Miro”
3. Choose “Miro Web (SAML)” and click **Select**
4. In the “Google Identity Provider details”, under Option 2 verify that “SSO URL”, “Entity ID”, and “Certificate” are all filled in, then click **Continue.** You will copy these values later when you configure Miro
5. In the “Service provider details”, add the following values:
   **ACS URL:** https://miro.com/sso/saml
   **Entity ID:** https://miro.com/
   **Start URL:** blank
   **Signed response:** leave unchecked
   **Name ID:** EMAIL
6. Click **Continue**
7. In “Attribute mapping” under “Google Directory attributes” choose **First Name**, then choose **Last Name**, making sure they map to the App attributes
8. Click **Finish**. You will now see your Miro app added to Google Workspace
   ![google_sso_configuring_google_settings.gif](images/21017515989394_google_sso_configuring_google_settings.gif)*Setting up Google SAML identity provider*

Setting up Miro as SAML service provider

1. Open an Incognito tab in your browser and log into the Miro dashboard (miro.com/app/dashboard)
2. Click your avatar in the top-right corner and click **Settings**
3. From your Company settings, click **Authentication.** If you are a Business plan customer, this setting is in **Security**.
4. Click the toggle to “Turn on SSO to set up SCIM provisioning”
5. You will be taken to the Authentication section of Company settings. Click the **SSO/SAML** toggle. You will be prompted to click **Turn on** to enable SSO for your organization
6. For the **SAML Sign-in URL**, return to your Google Workspace Admin Console and within the Miro app, click **DOWNLOAD METADATA.** This panel gives you the option to copy the values needed
7. Under **SSO URL**, click the **Copy** button. Go back to Miro and paste the value in **SAML Sign-in URL**
8. Repeat this process for **Key x.509 Certificate** using the Certificate in Google
9. Add your **Domain** information. Ensure you’ve already [set up and verified your domain](../../canvas-25-admin-features/domain-control/01-domain-control.md)
10. Click **Save![google_sso_configuring_miro_authentication.png](images/21017515990802_google_sso_configuring_miro_authentication.png)***Configuring SSO authentication settings in Miro*

Turning on Miro for users

1. Return to the Google Workspace Admin Console
2. If needed, click **Web and mobile apps** from the Apps menu and select **Miro**
3. Click **User access**
4. Click **ON for everyone** and click **Save![google_sso_turning_on_miro.gif](images/21017528995474_google_sso_turning_on_miro.gif)***Turning on the Miro app for all users*

If you’d like to turn on Miro for specific organizational units, click the group in the Organizational Units first, then click **ON.** You may need to click **OVERRIDE** or **INHERIT** additionally.

Testing authentication

1. In the Google Workspace Admin Console, launch the Miro app if needed
2. In the Miro section, click **TEST SAML LOGIN**
3. A new tab should appear with Google SSO sign-in options
   [GIF]
4. To test authentication in Miro, open a new Incognito tab and launch the Miro dashboard (miro.com/app/dashboard)
5. You should see a sign-in page. Click **Sign in with Single Sign On** and login with your account credentials.
   ![google_sso_testing_authentication.gif](images/21017528996882_google_sso_testing_authentication.gif)*Testing Google SSO authentication with Miro*

Alternatively, you can test in Miro:

1. Complete the steps above to configure your SSO settings.
2. Click the **Test SSO configuration** button.
3. Review the results:
   1. If no issues are found, a confirmation message **SSO configuration test was successful** will be displayed.
   2. If issues are found, a confirmation message **SSO configuration test failed** will be displayed, followed by detailed error messages to guide you on what needs to be fixed.![test-sso.png](images/19662118715282_test-sso.png)*Test SSO configuration from Miro*

> **⚠️** If you’ve previously configured SSO for your org and need to re-configure it, it's strongly recommended to turn **off** SSO in Miro before continuing in Google Admin Console; otherwise, you could lock yourself out of Miro. To prevent a lockout, create a 'break the glass' user with an email with a domain outside the domain listed in the SSO settings, like acmebreaktheglass@gmail.com. Otherwise, you can contact support, and they can disable SSO for the whole organization.

If you would like to configure user provisioning with Google, instructions can be found in the article “[Setting up automated provisioning with Google](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md)”.
