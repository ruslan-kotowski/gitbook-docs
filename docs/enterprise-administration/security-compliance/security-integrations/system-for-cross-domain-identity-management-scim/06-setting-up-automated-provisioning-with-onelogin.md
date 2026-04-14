---
title: Setting up automated provisioning with OneLogin
article_id: 360019893480
sidebar_position: 6
created_at: '2021-02-25T18:00:56Z'
updated_at: '2025-11-03T08:18:39Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: '[Enterprise](../../../../plans-billing/miro-plans/04-enterprise-plan.md)
    plan'
  roles: Company-level admin
---

:::warning
The guide provides steps to configure the feature. For available functionality, rules that Miro SCIM follows and possible issues and how to resolve them please first see [**here**](../../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md).
Miro's Developer documentation for SCIM can be found [**here**](https://developers.miro.com/docs/scim).
:::

Prerequisites

The Miro SCIM API is used by SSO partners to help provision, manage users and teams (groups). SAML-based SSO must be properly set up and be functional in your Miro Enterprise plan before you start configuring automated provisioning. The instructions on how to set up SSO can be found [here](../../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

## Setting up Provisioning

### Create a connector application

1. Go to **Applications** tab on the top bar of OneLogin admin center and click on the **Add App** button on the top right corner of the Application’s page.
2. In the Search section type "Miro" and choose the following app in the list marked as SAML, provisioning.

   You will be able to name the app in a specific way if you so desire.
   Click **Save** in the top right corner of the page.

### Configure the application

1. Go to **Configuration** on the left panel and **Enable** API Connection:
   Add the API **Token** to the respective field. You can obtain it from the SSO section of your Miro settings.
2. Go to **Provisioning** section on the left panel and check that you have the following settings:
:::warning
By default **Create**, **Delete** and **Update** **user** needs Admin approval before provisioning. To disable it please uncheck these options.
:::

Your Onelogin SCIM application is now configured and working.

## User Assignments

Miro SCIM Provisioning can help you to provision and de-provision users to your Enterprise subscription, as well as to automatically distribute them across teams. Users from OneLogin should be assigned to the Miro application to be automatically managed in Miro. To assign users to the application, follow the steps below (group assignments are not yet supported).

1. In **Users** directory choose a user to be assigned and provided access to Miro and click the **Applications** section on the left panel. Then click on the **plus** button in the top right corner of the page.
2. Select the **Miro** app and click **Continue.**

   You can update the user’s attributes on the following form and then click on **Save.**
3. If you disabled the Admin approvals for the application then you will see that the user is provisioned to Miro.

### Admin approval

If Admin approvals are required for provisioning you will see the status as **Pending.**

In this case, the Admin will need to approve the assignment by choosing the **Users** section on the left of the **Applications** page and clicking on the **Pending** status., and then clicking **Approve.**

:::tip
If at the moment of confirmation there are several users waiting for confirmation the admin will see an option to bulk-confirm the assignments at once:
:::

Your end-user is now assigned and is added to your Miro subscription!
