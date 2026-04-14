---
title: How to configure OneLogin SSO
article_id: 360022547134
sidebar_position: 8
created_at: '2019-05-07T13:32:16Z'
updated_at: '2025-02-26T11:22:04Z'
draft: false
availability:
  plans: '[Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md), [Business](../../../plans-billing/miro-plans/06-business-plan.md)
    plans'
  roles: company_admin
---

> *💡 It is strongly recommended to configure SSO in a separate incognito mode window of your browser.* This way, you keep the session in the standard window, allowing you to switch off the SSO authorization in case something is misconfigured.

If you wish to set up a test instance before enabling SSO on production, please request it with your Account Executive or Sales representative. Only those who configure SSO will be added to this test instance.

> **⚠️ See our main SSO article** [**here**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **for rules, supported features and optional configuration on the Miro end.**

## Setting up Onelogin

### Adding and configuring the app

Configuration of OneLogin in Miro is simple as OneLogin has a pre-configured working Miro application in the **Apps** catalogue.

![Miro_in_OneLogin_apps.jpg](images/21017429898130_Miro%20in%20OneLogin%20apps.jpg)
*Miro in OneLogin application catalogue*

Click **Save** button.

![save_button.jpg](images/21017429899538_save%20button.jpg)
*Application configuration tab in OneLogin*

## Setting up Miro

After saving the configuration you will be directed straight to the application settings. Switch to the **SSO** tab to get your **Login URL** and **x509 Certificate**.

![sso_tab.jpg](images/21017416854674_sso%20tab.jpg)
*SSO tab*

Below you will see a list of URLs. Copy **SAML 2.0 Endpoint (HTTP)** URL:

![SAML_endpoint.jpg](images/21017416855698_SAML%20endpoint.jpg)

and ***paste*** it to Miro **SAML Sign-In URL** field:

![sign-in_URL.jpg](images/21017429902354_sign-in%20URL.jpg)
*Miro **SAML Sign-In URL** field*

Go back to OneLogin application SSO tab and click **View Details** to copy the **x509 Certificate**.

![view_details.jpg](images/21017416856722_view%20details.jpg)
*View Details button*

![copy_certificate.jpg](images/21017429903634_copy%20certificate.jpg)
*Copying **x509 Certificate***

Paste the certificate to the Miro **x509 Certificate** field.

![certificate_in_Miro_SSO_settings.jpg](images/21017429905042_certificate%20in%20Miro%20SSO%20settings.jpg)
***x509 Certificate** field in Miro SSO settings*

As a final step of the Miro settings add your domains and [verify them](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). You may also configure [the optional settings](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

You're all set and now your users will be able to authenticate in Miro via SSO!

If you meet any issues, please check out [our list of common cases and how to resolve them.](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)

## Testing SSO configuration in Miro

1. Complete the steps above to configure your SSO settings.
2. Click the **Test SSO configuration** button.
3. Review the results:

- If no issues are found, a confirmation message **SSO configuration test was successful** will be displayed.
- If issues are found, a confirmation message **SSO configuration test failed** will be displayed, followed by detailed error messages to guide you on what needs to be fixed.

![test-sso.png](images/19678727059090_test-sso.png)

*Testing SSO configuration in Miro*
