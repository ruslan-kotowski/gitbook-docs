---
title: How to configure OKTA SSO
article_id: 360023901054
sidebar_position: 7
created_at: '2019-05-31T11:32:41Z'
updated_at: '2025-11-25T16:05:05Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: '[Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md), [Business](../../../plans-billing/miro-plans/06-business-plan.md)
    plans'
  roles: company_admin
---

> *💡 It is strongly recommended to configure SSO in a separate incognito mode window of your browser.* This way, you keep the session in the standard window, allowing you to switch off the SSO authorization in case something is misconfigured.

If you wish to set up a test instance before enabling SSO on production, please [reach out to the Support Team](https://help.miro.com/hc/requests/new?referer=help-center-article) for assistance. Only those who configure SSO will be added to this test instance.

> **⚠️ See our main SSO article** [**here**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **for rules, supported features and optional configuration on the Miro end.**

## Setting up Okta

### Adding and configuring the app

Click the **Applications** tab and choose to **Browser App Catalogue**:

![browse_app_catalog.jpg](images/21016928758930_browse%20app%20catalog.jpg)
*Applications section in Okta*

Find our preconfigured app for easy setup and click to **Add** it:

![Miro_pre-configured_app.jpg](images/21016928759570_Miro%20pre-configured%20app.jpg)
*Miro in the Okta app catalogue*

Give the app in your gallery the label you prefer (other steps are optional) and click **Next** to switch to the **Sign-On options** tab:

![general_settings.jpg](images/21016928760466_general%20settings.jpg)
*Miro app's general settings*

In the **Sign-On Options** all the values we expect are already filled and no additional data are required.

:::warning
You may add customized values if you prefer, but make sure that the **Default Relay State** is kept *empty*: our standalone apps employ redirection to the end-user's browser during the authentication procedure and generate unique RelayState values for that. If you use a Default value, Okta will overwrite our data and your users will only be able to access Miro's browser version, but not any standalone apps (desktop, tablet, mobile).
:::

![sign-on_options.jpg](images/21016941715730_sign-on%20options.jpg)
*Sign-on methods*

Click to **Finish**. You will be able to go back and edit any fields later if need be.

### Username format

:::tip
The **Application username format** is by default set to **Okta Username** which is okay if your Username is in the email format. Alternatively set the Username to **Email.**
:::

:::warning
Email is the primary ID by which the user is recognized in Miro and should not be updated on the Okta's end unless you have SCIM enabled. If you don't use SCIM but need to update your end user's addresses, please reach out to our [Support team](https://help.miro.com/hc/requests/new?).
:::

### Configuring Profile Pictures (optional)

Setting up a custom attribute like ProfilePicture can be considered a separate process. Please follow this [guide](https://drive.google.com/file/d/1go4BJWzFpQS5R04WdN1Q4O5Dy93k4wGp/view) to set up the attribute on the Okta end and then [enable ProfilePicture requirement](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) on the Miro end.

## Setting up Miro

Scroll down to **SAML Signing Certificates** to get the IDP metadata. If you do not have any issued certificates, first create one.

After that click **Actions** and choose to **View IdP metadata** like so:

![view_Idp_metadata.jpg](images/21016928761234_view%20Idp%20metadata.jpg)
*Getting the IdP metadata*

You will be directed to a separate tab that containsall the information. Copy the certificate from the line starting with &lt;ds:X509Certificate&gt; and paste it to Miro SSO Settings in **Key x509 Certificate** field.

![certificate_in_Miro_SSO_settings.jpg](images/21016928761746_certificate%20in%20Miro%20SSO%20settings.jpg)
*Key x509 certificate in Miro SSO settings*

Go back to the metadata page and copy the URL from **SingleSignOnService** line after **Location=**and paste it to **SAML Sign-in URL**.

You are all set!

As a final step of the Miro settings add your domains and [verify them](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). You may also configure [the optional settings](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

If you meet any issues, please check out [our list of common cases and how to resolve them.](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)

## Testing SSO configuration in Miro

1. Complete the steps above to configure your SSO settings.
2. Click the **Test SSO configuration** button.
3. Review the results:

- If no issues are found, a confirmation message **SSO configuration test was successful** will be displayed.
- If issues are found, a confirmation message **SSO configuration test failed** will be displayed, followed by detailed error messages to guide you on what needs to be fixed.

![test-sso.png](images/19678741029138_test-sso.png)

*Testing SSO configuration in Miro*
