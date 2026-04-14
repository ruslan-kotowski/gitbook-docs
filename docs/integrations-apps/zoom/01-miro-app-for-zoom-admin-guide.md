---
title: Miro app for Zoom (admin guide)
article_id: 360022039379
sidebar_position: 1
created_at: '2021-05-28T04:43:09Z'
updated_at: '2025-02-26T11:51:29Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: zoom
availability:
  plans: desktop version
  notes: '*For Zoom Business and Enterprise plans, admin may need to pre-approve the
    Miro app'
---

The Miro app for Zoom enables teams to build an all-in-one digital meeting room and effectively collaborate during meetings and workshops using Miro from within Zoom. The app provides Miro’s collaboration capabilities from within Zoom and makes onboarding guest users especially easy. For Miro newcomers, we offer whiteboarding with registration-free access.

This guide can be used by Zoom and Miro Admins to enable the experience for their users.

:::note
Check out the [User guide for Miro app for Zoom](02-miro-app-for-zoom-user-guide.md).
:::

## How to enable the app experience in Zoom

### Enable Discovery of Apps

1. Sign in to the Zoom web portal as an admin with the privilege to edit account settings.
2. In the navigation panel, click **Account Management** then **Account Settings**.
3. Click the **Zoom Apps** tab.
4. Verify that **Zoom Apps Quick Launch Button** is enabled. This allows users on your account to see the Zoom Apps button ![mceclip0.png](images/21017682787474_mceclip0.png) on the desktop client.
5. If the setting is disabled, click the toggle to enable it. If a verification dialog displays, click **Turn On** to verify the change.

In addition, Zoom has additional documentation on how to enable Zoom apps only for specific groups or users. For more visit the Zoom help center [here](https://support.zoom.us/hc/articles/360061555152).

![Zoom_apps_quick_launch.jpg](images/21017682788114_Zoom%20apps%20quick%20launch.jpg)
*Enabling Zoom Apps Quick Launch Button*

This will enable Zoom Apps in the top bar in Zoom’s main client and the bottom bar in meeting clients for users of your account.

### How to pre-approve the app in Zoom

If you are a Zoom admin for a Zoom Business or Enterprise plan, you may need to pre-approve the Miro app [here](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA) in order for users to have access to it.

![pre-approve_Miro_app.jpg](images/21017653155474_pre-approve%20Miro%20app.jpg)*Pre-approving the Miro app*

### Selecting users on the account that can install the app

In addition to pre-approving the Miro app, you can select which users or groups are able to install it.

![allow_users_to_install_the_app.jpg](images/21017682790418_allow%20users%20to%20install%20the%20app.jpg)
*Selecting users and groups that can install the Miro app*

Once you have approved the Miro app and installed it on your company account, users will be able to access and install from the Zoom client.

See [Zoom’s documentation](https://support.zoom.us/hc/articles/360061555152) for more information.

## How to enable the app experience in Miro

> **Set up by:** Company Admins on Enterprise plan

If you are on [Enterprise plan](../../plans-billing/miro-plans/04-enterprise-plan.md) and you limited the installation only for approved apps then please make sure to include the Miro app for Zoom in your approved app list in **Company settings > Apps > Manage apps**. You can do this by pasting the clientID 3074457354625507111 into the search and enabling the app for installation.

![approve_Zoom_on_Enterprise_plan.jpg](images/21017653161874_approve%20Zoom%20on%20Enterprise%20plan.jpg)
*Approved apps in Company settings*

## How users can install the app

Users can find the Miro app for Zoom on the [Zoom Marketplace](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA) or the [Miro Marketplace](https://miro.com/marketplace/zoom-app/).

The first step in the installation process is to authorize the Miro app for Zoom.

![install_Miro_app_for_Zoom.jpg](images/21017653157778_install%20Miro%20app%20for%20Zoom.jpg)
*Allowing Miro to access your Zoom account*

Once authorized the app will redirect users into their Zoom desktop app and show the newly installed Miro app. **Note that they will need to be logged into their Zoom account to add the app**.

Miro users will need to **sign in** to see their boards. This will redirect them to their system browser where we request them to sign in to Miro or directly authorize the app in Miro. They can choose to install the app for any team that they have access to.

![install_Zoom_for_a_Miro_team.jpg](images/21017682793362_install%20Zoom%20for%20a%20Miro%20team.jpg)
*Install the app for one of your Miro teams*

Users will then be redirected back into the Zoom desktop app where they will see their Miro dashboard including all their existing teams and boards.

![Miro_dashboard_in_Zoom.jpg](images/21017653159442_Miro%20dashboard%20in%20Zoom.jpg)*Users will be able to select a board from their dashboard and open it within Zoom*

## Understanding board sharing access settings

Users can define the appropriate permissions for sharing a board within a Zoom meeting. They can choose between four options: **Anyone in Zoom can edit/comment/view** or **Private** (which means that the sharing settings will be the same as what is set on the Miro side).

![board_embed_sharing_settings.jpg](images/21017682795154_board%20embed%20sharing%20settings.jpg)

*Configuring access settings for your board*

The access setting options will follow organization-wide access controls. If you have restricted public link sharing for board embeds on [Enterprise plan](../../plans-billing/miro-plans/04-enterprise-plan.md), that option will not be available to users. Learn more: [Managing Enterprise sharing policy for embed integrations](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).

![publi_editing_is_turned_off.jpg](images/21017653160722_publi%20editing%20is%20turned%20off.jpg)
*Public editing is turned off by Company Admin*

## Frequently asked questions

1. *What data is the Miro app for Zoom accessing?*
   - Miro app for Zoom is requesting user profile information to associate a board to a given user. Our app does **not** access meeting content, such as video, audio, chat and/or meeting files and hence does not appear in Zoom’s Active Apps Notifier.
2. *Can the app be installed on tablet or mobile devices?*
   - No, the Miro app for Zoom is only available on desktop.
3. *For what operating system does Zoom Apps work?*
   - Mac OS and Windows.
4. *What version of Zoom is required to use Zoom Apps?*
   - Version: 5.7.3.
