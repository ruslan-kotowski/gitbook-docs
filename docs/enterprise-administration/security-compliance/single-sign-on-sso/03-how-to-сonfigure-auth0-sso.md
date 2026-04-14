---
title: How to сonfigure Auth0 SSO
article_id: 360022496573
sidebar_position: 3
created_at: '2019-05-01T18:33:32Z'
updated_at: '2025-02-26T11:43:03Z'
draft: false
availability:
  plans: business, enterprise
  roles: company_admin
---

*It is strongly recommended to configure the feature in a separate incognito mode window of your browser.* *This way you keep the session in the standard window, allowing you to switch off the SSO authorization in case something is configured incorrectly.*

If you wish to set up a test instance before enabling SSO on production, please request it with your Account Executive or Miro Sales representative. Only those who configure SSO will be added to this test instance.

## Creating the Miro application within your tenant

1. Create the application in your **Applications** list.
   ![create_application_button.jpg](images/21017725476370_create%20application%20button.jpg)
   *Auth0 Applications section*
2. Select **Regular Web Applications** application type.
   ![application_types_list.jpg](images/21017695804818_application%20types%20list.jpg)
   *Application types list*
3. Head over to the **Settings** tab and make sure that the options listed are selected exactly the way as described below.
   ![mceclip0.png](images/21017725482002_mceclip0.png)


   |  |  |
   | --- | --- |
   | **Token Endpoint Authentication Method** | POST |
   | **Allowed Callback URLs** | `https://miro.com/sso/saml` |
   | **Application Login URI** | `https://miro.com/sso/saml` |
   | **Allowed Origins (CORS)** | `https://miro.com/` |
   | **JWT Expiration** | 36000 (Set by default) |
4. Click **Show Advanced Settings:**
   ![mceclip1.png](images/21017725485074_mceclip1.png)

   and then go to **Certificates** and Copy your x509 Signing Certificate:
   ![copy_the_certificate.jpg](images/21017695807634_copy%20the%20certificate.jpg)
   *Advanced Settings tab in Auth0*
5. Switch to Miro and open your SSO settings (Business plan Admins will find the settings in the **Security** tab, Enterprise plan Admins will need to go to **Enterprise integrations** tab) and then paste the **x509 Signing Certificate** in the respective field as shown on the screenshot below:
   ![certificate_in_Miro_SSO_settings.jpg](images/21017725488402_certificate%20in%20Miro%20SSO%20settings.jpg)
   *Miro **Security** tab with SAML settings*

## Setting SAML for the application

1. Go back to the Auth0 application configuration page and choose the **Addons** tab and the **SAML2** addon:
   ![add-ons_catalog.jpg](images/21017725489682_add-ons%20catalog.jpg)
   *Auth0 add-ons catalog*You will see a pop-up window with the request settings and **Application Callback URL:
   ![add-on_settings.jpg](images/21017725490962_add-on%20settings.jpg)***Addon **Settings** tab*
2. Make sure that the **URL** is set to **`https://miro.com/sso/saml`**The request **Settings** should be set to the following:

   ```
   {
    "nameIdentifierFormat": "urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress",
    "nameIdentifierProbes": [
    "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress"
    ]
   }
   ```
3. Switch the tabs to **Usage**and copy the **Identity Provider Login URL:**![mceclip2.png](images/21017695812626_mceclip2.png)
   *Identity Provider Login URL field in Auth0*
4. Switch to Miro again and paste the URL to**SAML Sign-in URL** field.
5. Click **Save** for the settings to be applied to your Miro plan.

## Checking the configuration

You can now go back to Auth0 console and switch back to the **Settings** tab of the addon. Click **Debug** to trigger the login attempt.

![debug.jpg](images/21017695814290_debug.jpg)
*Triggering the login attempt*

This will initiate the IdP login attempt and will allow you to see the results.

In case of any difficulties - feel free to [contact our Support Team](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md#how-to-contact-miro-support).

## Testing SSO configuration in Miro

1. Complete the steps above to configure your SSO settings.
2. Click the **Test SSO configuration** button.
3. Review the results:

- If no issues are found, a confirmation message **SSO configuration test was successful** will be displayed.
- If issues are found, a confirmation message **SSO configuration test failed** will be displayed, followed by detailed error messages to guide you on what needs to be fixed.

![test-sso.png](images/19678830886418_test-sso.png)

*Testing SSO configuration in Miro*
