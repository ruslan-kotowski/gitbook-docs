---
title: How to install apps
article_id: 360017731093
sidebar_position: 4
created_at: '2019-02-11T10:12:46Z'
updated_at: '2025-08-05T07:54:07Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  roles: all_users
  plans: free, starter, business, enterprise, education
  platforms: browser, desktop
  notes: Team Admins can restrict installation for non-admins. Company Admins on Enterprise
    plan can further restrict to approved apps only.
---

You can extend Miro's functionality by installing apps from the Miro Marketplace. This article guides you through installing and uninstalling apps, understanding app permissions, and provides an overview of creating custom integrations.

## Install apps from Miro Marketplace

The [Miro Marketplace](https://miro.com/marketplace/) is your central hub for discovering and adding apps to enhance your Miro experience. You can install apps directly from your board or by visiting the Marketplace website.

![Miro_marketplace.jpg](images/5021611044242_Miro%20marketplace.jpg)*Miro Marketplace*

There are two primary ways for users to add apps:

1. **From your board:** Click the **Tools, Media and Integrations (+)** icon on the creation toolbar, then use the "Search integrations" search box on the Marketplace tab. If you find your app already listed, just click to add it. You can also browse available apps from this panel.
   ![marketplace-add-apps.png](images/21260776452626_marketplace-add-apps.png)*Marketplace on the Creation toolbar*
2. **From the Marketplace website:** You can also go directly to the [Miro Marketplace](https://miro.com/marketplace/) website to browse and install apps from their respective listings.

**For Company Admins:**
Company Admins on applicable plans can also install apps for their entire team through the team settings. To do this, navigate to **Team Settings** > **Apps & Integrations** > **Install apps**. This section allows for centralized management and deployment of apps across the team.

![apps_and_integrations_page.jpg](images/5021832338450_apps%20and%20integrations%20page.jpg)*Installed apps section in Team settings for Admins*

## Uninstall apps

You can manage and uninstall apps from your team settings. Note that non-admin users may have restrictions on uninstalling apps, depending on the team's configuration.

:::warning
Non-admin users cannot uninstall apps if they are not allowed to install them by an Admin in the team settings.
:::

To manage your team apps, navigate to **Team settings > Apps & Integrations**. This page lists all apps currently installed for your team or by you personally.

![apps_settings.jpg](images/5021898097682_apps%20settings.jpg)*Apps & Integrations in Team settings*

To uninstall an app, follow these steps:

1. From the **Apps & Integrations** list, select the app you wish to remove.
2. Click either **Uninstall for team** or **Uninstall for me**. The available option will depend on how the app was installed and your administrative rights.

![uninstall_an_app.jpg](images/5021797466258_uninstall%20an%20app.jpg)*The option to uninstall an app*

## App installation permissions

Team and Company Admins have various controls to manage who can install apps and which apps are available to their organization, ensuring security and compliance.

Team Admins can configure whether non-admin team members are allowed to install apps. This setting is found in **Team settings > Apps & Integrations** under the app management options.

![allow_non-admins_to_install_apps.jpg](images/5021903025170_allow%20non-admins%20to%20install%20apps.jpg)*"Allow non-admins to install apps" option in Team settings*

For users on the [Enterprise plan](../../plans-billing/miro-plans/04-enterprise-plan.md), Company Admins have access to more granular controls. They can manage **Approved apps** via **Company Settings** > **Apps**. This feature allows admins to curate a list of company-vetted applications, restricting users from installing apps not on this approved list. [Learn more about managing app discovery and installation settings for Enterprise plans](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).

![Enterprise_apps.jpg](images/5021890162962_Enterprise%20apps.jpg)*Managing approved apps in Enterprise Company settings*

## Custom integrations and developer platform

If you require specific functionality not available in the Miro Marketplace, you can create your own customized solutions using the [Miro Developer Platform](https://miro.com/api/). This platform offers robust tools, including REST APIs, web plugins, and embeds, to help you build powerful integrations tailored to your needs.

Here are key points to consider when developing custom integrations:

- **Getting Started:** You can begin building your app by [creating a Developer team](https://developers.miro.com/). Standard developer teams are intended for development and testing purposes and have certain limitations:
  - Up to 5 users in the team.
  - Up to 3 boards in the team.
  - A watermark is displayed on boards.
  - Board export functionality is not available.
- **Enterprise Plan Developers:** If your organization is on an [Enterprise plan](../../plans-billing/miro-plans/04-enterprise-plan.md), you can create a Developer team as part of your subscription. These developer teams are not subject to the limitations of standard ones and benefit from all Enterprise-grade security features. [Learn more about developer teams for Enterprise plans](../../enterprise-administration/managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md).

For additional information, support, and to connect with other developers, you can explore the [Developer Platform Forum](https://community.miro.com/developer-platform-forum-57).
