---
title: Configuring Enterprise mobility management (EMM) on Android
article_id: 13888848676498
sidebar_position: 3
created_at: '2023-09-21T14:45:02Z'
updated_at: '2025-11-25T15:38:11Z'
draft: false
availability:
  notes: 'general: steps on how to configure your company''s EMM/MDM solution using
    three examples from specific software: VMWare (Workspace ONE), Ivanti Neurons
    (formerly MobileIron Cloud), and Intune (Microsoft Endpoint Manager). If you use
    a different solution, then for exact steps we recommend consulting the documentation
    of your EMM provider.'
---

The EMM allows Company admins to configure and distribute Miro to users in their organization in a centralized and unified way. Miro supports provisioning the following settings to the end-user devices:

- Disabling Sign-up flow.
- Limiting supported authentication providers (e.g., social networks, email providers, etc.).
- Restricting username to a specific value or list of allowed email domains.
- Advanced SSO configuration.

## How to configure

### Add Miro to the app directory of your organization

For most, enabling EMM configuration will require adding Miro to your organization's application catalog. This process might differ from one EMM provider to another. Still, usually, you will add Miro to your application catalog directly from the Google Play Store and set a distribution policy based on device groups, user groups, etc.

#### Examples

**VMware Workspace ONE**

The general VMware Workspace ONE deployment guide can be found [here](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications).

1. Click **Add** then **Public Application.**
2. Select **Android** from the Platform drop-down menu and **Search App Store** for the Source.
3. Enter “**Miro**” in the **Name text box** and click next.
4. Select the Miro app and press **Approve** if prompted.
5. Publish the app by clicking **Save & Assign**.
6. Configure assignments and distribution settings according to your organization's preferences.

**Ivanti Neurons**

The general Ivanti Neurons deployment guide can be found [here](https://help.ivanti.com/mi/help/en_us/cld/admin/ivanti/92/all/Managing_Google_Play_apps.htm).

- 1. Go to **Apps > App Catalog** and click **Add.**
  2. Select the “**Google Play Store**” and your country as the source.
  3. Search for “**Miro**” and select “**Miro: Online whiteboard**” from the list of available applications.
  4. Configure distribution settings and policies according to your organization's preferences.

**Intune (Microsoft Endpoint Manager)**

The general Intune deployment guide by MS can be found [here](https://learn.microsoft.com/mem/intune/fundamentals/deployment-guide-platform-android).

1. Go to **Apps > All apps** and click **Add**.
2. Select **Store App > Android store app** as the **App type**.
3. On the **App Information** page, populate the details from the [Miro listing on the Google Play Store](https://play.google.com/store/apps/details?id=com.realtimeboard).
4. Configure distribution settings and policies according to your organization's preferences.

Configure distribution settings and policies according to your organization's preferences.

### Pre-populating application settings

Miro uses [AppConfig](https://www.appconfig.org/) as the unified way of configuring and securing customers’ data which provides an easy way to configure enterprise mobile applications. Many EMM solutions support AppConfig format or accept it in a “compatibility mode.” For exact limitations applicable in your case, please consult the documentation of your EMM provider.

#### Examples

**VMWare Workspace ONE**

The general VMware Workspace ONE deployment guide can be found [here](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications).

1. Go to **Resources > Apps**.
2. Click **Assign** in the **Install Status** column in the **Miro: Online whiteboard** app row.
3. Define the **Name, Assignment Groups** and **App Delivery Method** of the distribution.
4. Enable **Managed Access** and **Send Configuration**
5. Define the application configuration.

**Ivanti Neurons**

The general Ivanti Neurons deployment guide can be found [here](https://help.ivanti.com/mi/help/en_us/cld/admin/ivanti/92/all/Using_the_Android_enterprise_App_Configuration.htm).

1. Go to **Apps > App Catalog**.
2. Navigate to “**Miro: Online whiteboard**” settings.
3. Go to **App configurations > Managed Configurations for Android**.
4. Click **Add** to create **App Restrictions**.
5. Define the **Required** and **Runtime** **Permissions**.
6. Select distribution profile in **Distribute this App Config** section.

**Intune (Microsoft Endpoint Manager)**

The general Intune deployment guide by MS can be found [here](https://learn.microsoft.com/mem/intune/apps/app-configuration-policies-use-android).

1. Go to **Apps > App configuration policies > Add > Managed devices** to create a new application configuration.
2. Define the name of your configuration profile.
3. Select **Android Enterprise** as the **Platform**.
4. Select **Miro: Online whiteboard** as the **Target app** by clicking **Select app**.
5. Select **Use configuration designer** as **Configuration settings format**.
6. Define application configuration.
7. Select distribution profile for the configuration.

## Full list of supported settings

### Limiting “Sign in with …” / “Sign up” options

Should the “Sign up” option be enabled, all “Sign in with …” settings will affect the signup flow.

:::warning
Any key not explicitly set to "true" (or absent) is considered as set to “false”. Hence the authentication option is available (default behaviour).
:::

| Key | Type | Allowed values |
| --- | --- | --- |
| **Facebook** miro.authentication.facebookRestricted | Boolean | true/false |
| **Google** miro.authentication.googleRestricted | true/false |
| **Microsoft Office 365** miro.authentication.office365Restricted | true/false |
| ****Slack****  miro.authentication.slackRestricted | true/false |
| **Sign up** miro.authentication.signUpRestricted | true/false |
| **Sign in with Magic link** miro.authentication.magicLinkRestricted | true/false |
| **Enterprise workspace** miro.authentication.enterpriseWorksSpaceDisabled | true/false |

### Username restrictions

Customers who want to improve security while keeping plain password authentication can use the following options.

| Key | Value | Description |
| --- | --- | --- |
| **Predefined username** miro.policy.authentication.username | **Value type:** string | The field is locked and can’t be changed by the user |
| **Whitelisted domains** miro.policy.authentication.allowedDomains | **Value type:** array  **Value:** @miro.com, @yourdomain.com  *Some provider do not support **array** data type. Should that be the case, please use the type **string** and JSON array as a value. ["@miro.com", "@yourdomain.com"] | Only emails corresponding to one of the listed domains are allowed. |

### SSO configuration

To improve organization security and simplify the authentication process for end users, organization administrators can configure SSO policy using the following example.

:::warning
Make sure that the SSO policy in the application config corresponds with the SSO settings of the Miro organization. Mismatching those policies might result in a “locked out” situation when users can’t log in. Miro cannot validate the settings before enforcing these on target devices.
:::

|  |  |
| --- | --- |
| Configuration key | miro.policy.sso |
| Configuration value type | string |
| Policy object | \{ "authenticationRestricted" : false, "email": "user@domain.com", "allowedDomains": ["domain1.com", "domain2.com"], "forceSsoLogin": true \} |

| Policy object attributes | | | |
| --- | --- | --- | --- |
| Parameter | Type | Description | Note |
| authenticationRestricted | boolean | Whether the "Login with SSO" button is enabled on the main page. | **The key is ignored when other configuration options are provided.** |
| email | string | Email predefined for SSO login. | The field is locked and can’t be changed |
| allowedDomains | boolean | Keep SSO as the only available method for authentication. | An end user is immediately taken to the “Login with SSO page”. Options other than **email** and **allowedDomains** are ignored. No other authentication methods are available. |
