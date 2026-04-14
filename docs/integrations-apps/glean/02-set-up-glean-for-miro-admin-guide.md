---
title: Set up Glean for Miro (admin guide)
article_id: 27581463837330
sidebar_position: 2
created_at: '2025-06-23T10:52:57Z'
updated_at: '2026-01-02T09:57:07Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  roles: company_admin
  plans: business, enterprise
  platforms: desktop, browser
---

As a Company Admin, you can install and configure the Glean integration for your organization. This brings Glean's AI-powered search capabilities directly into Miro, helping your team find information across more than 100 source systems to improve productivity.

## Prerequisites

1. You are a **Miro Org Admin** and a **Glean Admin**.
2. In Glean, **register an OAuth Client ID.** Read [Glean documentation](https://developers.glean.com/api-info/client/authentication/oauth) for more details.
3. Enable the user-level privacy setting **Allow chat history to be saved up to 30 days**.

## Install the Glean app

To begin, install the Glean app from the Miro Marketplace to the relevant teams in your organization.

1. Go to your **Company** settings and click **Apps & Integrations**.
2. Under the **Apps** tab, click **Add apps** to open the Marketplace.
3. Search for "Glean". You can also find it by pasting its client ID in the search bar: `1202342442818548396`.
4. From the app profile, select where to add the app: either for **All teams** or select **Specific teams...**.
5. Review the permissions page. The Glean app is developed and maintained by Miro and does not require specific permissions.
6. Select **Add** to complete the installation.

## Single Sign-On Setup (Okta)

If your organization uses Okta as its Single Sign-On (SSO) provider, you need to create an Okta OpenID Connect (OIDC) Web application before proceeding with the next sections.

1. Create a new Okta app using the steps mentioned in the documentation [here](https://help.okta.com/en-us/content/topics/apps/apps_app_integration_wizard_oidc.htm).
   1. Select **OIDC - OpenID Connect** as the Sign-in method.
   2. Select **Web Application** as the Application type.
   3. Ensure that the **Refresh Token** is enabled in the **Grant type** > **Core grants** settings.
   4. Add `https://integrations.miro.com/api/external-auth/oauth2/callback` as the **Sign-in redirect URIs**.
   5. Select **Save**.
2. Copy the **ClientId** and **Client Secret** from the Client Credentials section. These will be required in the next sections to complete the integration setup.

## Configure Single Sign-On (SSO)

Follow these steps to configure the app:

1. From the **Apps & Integrations** page, navigate to **Manage apps**.
2. Find "Glean" in your list of installed apps and click its **Settings**. If you do not see the app, search for it by client ID (`1202342442818548396`) and approve it first.
3. In the configuration settings, selectthe **SSO provider**.
   1. Okta
   2. Azure
   3. Google
4. Enter the required SSO details.
   1. Okta: **Glean Base URL, Okta app details (Auth Server URL**, **Access Token URL**, **Client ID**, **Client Secret)**.
   2. Azure: **Glean Base URL**.
   3. Google: **Glean Base URL**.
5. Click **Save** to apply the configuration.

:::note
If you are using Azure, ensure your Microsoft Entra admin has selected "Consent on behalf of your organization" for the Glean app in the Microsoft Entra admin center to allow users to authenticate correctly.
:::

## Configure Glean admin console

Before using Glean in Miro, you need to configure OAuth token-based access in your Glean admin console.

1. Open your **Glean Admin console** and navigate to **Settings** > **Third-party access (OAuth)**.
2. In the **IDP-Configured OAuth** section, enable **Enable IDP OAuth for API access**.
3. Click **Manage Settings**, select your **SSO provider**.
4. Fill in the provider details based on your SSO provider.
   - **Okta**
     - Authorization Server URL: `https://<subdomain>.okta.com`
     - Allowed client ID(s): Client ID of the Okta app created in the previous section.
     - Rest of the form fields can be left empty.
   - **Azure**
     - Issuer subdomain: `https://login.microsoftonline.com/<tenant-id>/v2.0`
     - Allowed client ID(s): `a49fdb25-3b5f-4d3b-bedf-6da7be2b4bf4`
   - **GSuite**
     - Allowed client ID(s): `1062019541050-pf2ndc9f3o4lrmkupj3cj0fep5hkecns.apps.googleusercontent.com`
5. Select **Save** to apply the settings.

> ⏰ **Note:** It may take up to 30 minutes for changes to take effect in the Glean admin console.

## Use the Glean app

Once you have installed and configured the app, users in the designated teams can begin using it. The first time a user opens the Glean app in Miro, they will be prompted to authenticate.

1. Open a Miro board and click the Glean icon in the toolbar to open the side panel.
2. Click **Connect Glean** to start the authorization.
3. An SSO authorization dialog will appear.
4. After successful authentication, the Glean user interface will appear, ready for use.

## Security

For more information about data and security, see this [security document](https://docs.google.com/document/d/1lGLF7eASQb2uMRmMEAaH-GzFhyz4UKfwMeqSQOSYPdM/edit?tab=t.0#heading=h.gu9ng058yy7y).
