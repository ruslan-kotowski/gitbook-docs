---
title: Azure Cards
article_id: 360033799934
sidebar_position: 4
created_at: '2019-08-13T10:01:30Z'
updated_at: '2026-04-07T13:28:48Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  roles: all_users
  plans: business, enterprise
  platforms: browser, desktop, mobile
backstage_link:
  entity_kind: capability
  entity_id: azure-cards
---

Azure Cards allow you to import work items from Azure Boards (a part of Azure DevOps services, formerly VSTS - cloud solution) to your Miro boards. They can become essential to your remote retrospectives, story sizing, backlog prioritization, story mapping, and other team activities. You can also use them in Miro Kanban and User story mapping frameworks.

Azure Cards enhance your Miro experience by integrating directly with Azure Boards, enabling seamless workflow management for various team activities.

## Key features

The Azure Cards integration offers several key functionalities:

- Import Azure Cards using the in-app Azure Boards work items picker. This includes various sorting options.
- Search for Azure Boards work items in the in-app picker.
- Automated easy-to-read card view changes while zooming in and out.

:::note
Guarantee your Azure cards are always updated with card polling, which ensures users always get card updates even if [webhooks](../atlassian/14-how-to-set-up-webhooks-for-jira-data-center.md) fail.
:::

## Set up the Azure Cards integration

Setup is required on two levels:

1. The app must be added either on an organizational-level for all teams, or added on a team-level for specific teams.
2. After the app is added, the integration must be connected and authorized on a personal level to import Azure Cards.

This process requires specific administrative permissions in both Miro and Azure DevOps.

:::note
To successfully set up Azure Cards with Miro, **the Azure admin and Miro admin must be the same account**.

While adding Azure Cards requires Miro Team or Company Admin permissions **and** Project Collection Admin group permissions in Azure Boards, these permissions can be downgraded after the connection is complete. The admin cannot be removed, however, and must retain access to the Azure project.
:::

### Add Azure Cards for your organization or team

Miro Company Admins can add Azure Cards for all teams, while Team Admins can add it for specific teams they manage. This step makes the Azure Cards app available for connection.

:::note
To connect Azure Cards at the team level, you must be a Team Admin.
:::

1. Navigate to your **Profile settings** (click the main menu hamburger icon and choose **Profile settings**, or from the dashboard, click your avatar in the top-right corner and choose **Settings**).
2. Click **Apps** and then navigate to the **Add apps** tab on the right side.
3. Type "Azure Cards" and select it from the drop-down list. Click **Add**.
4. In the next dialogue box, choose either **All teams** or **In specific teams** (choose your team if needed), then click **Next step**.
5. On the "Review and add Azure Cards" screen, click **Add**. The app will be added for your company or team.
6. Go to the **Manage apps** tab, search for Azure Cards, and click **Approve**. The app will now be approved at the company- or team-level.
7. Next, connect your Azure organization to Miro. From the Apps panel, go to **Manage Apps.**
8. Search for "Azure Cards" in your apps list and click **Settings.**
9. In the settings panel for Azure Cards, add your **Azure instance** URL and click **Connect**. Provide your Microsoft Azure login credentials.
10. In the authorization dialog box, click **Accept** to finish connecting Azure to Miro.

### Apply custom Azure Cards settings for specific teams

If you need different settings for specific teams than the global company-level configuration, Team Admins can configure this in the Team **Apps & Integrations** area.

1. From your profile settings page, click **Teams**.
2. Click the team to which you'd like to apply custom settings.
3. In the Teams panel, click **Apps & Integrations**.
4. Find **Azure Cards** and click on it.
5. In the App settings panel, choose **Apply custom settings** from the drop-down at right, then connect the Azure account you'd like to have custom settings.
6. Authorize Miro in Azure DevOps with your Microsoft account: click **Connect** next to "Microsoft account" and log in to your Microsoft account, allowing Miro to use it.
7. Enter your **Azure Organization URL** (which can be copied from Azure DevOps) and click **Connect.** Miro will accept either your instance's personalized URL or the general `https://dev.azure.com/` address ending with your instance's name.
   ![Animation showing how to apply custom Azure Cards settings for a specific team.](images/21017013136658_azure_cards_custom_team_settings.gif)
   *Adding custom Azure Cards settings to specific teams*

### Connect your personal Azure account to use Azure Cards

After a Miro Admin installs and approves the app, each team member who wishes to use Azure Cards must personally authorize the connection to their Azure account. This personalizes the card picker and allows importing of all Azure work items the user can access.

You can find the Azure Cards icon on the Creation toolbar. If the icon isn't there, you may need to search for it:

1. In the Creation bar, select **Tools, Media and Integrations** (**+**).
   The **Tools, Media and Integrations** panel opens.
2. In the **Tools** tab, search and select Azure Cards.

To connect your account:

1. Click the Azure Cards icon on the toolbar. A popup will ask you to **Authorize**.
2. Click the **Authorize** button and click **Continue**. You will be brought to Team settings > Apps & Integrations page.
3. Use the App Settings panel to connect your Microsoft account to Miro and specify the Azure instance you'd like to use. This URL can be copied from Azure DevOps; Miro accepts either your instance's personalized URL or the general `https://dev.azure.com/` address ending with your instance's name.
   ![Specifying Azure Organization URL in Miro app settings.](images/21017013107730_org%20URL.jpg)

:::note
Please note that only Team Admins can set up the initial team or company-level configuration. If you do not see the **Connect** button for the Azure Organization URL during the admin setup, ensure you have [Team Admin rights for the team](../../administration/user-management/06-how-to-manage-admin-roles.md).
:::

## Import Azure work items to a Miro board

Once the Azure Cards app is configured and you've connected your personal account, you can import Azure work items to any Miro board associated with the connected team. There are two primary ways to do this:

- Copy the Azure work item URL and paste it directly onto the Miro board. The item will automatically transform into an Azure Card.
- Use the Azure Card picker: Click the **Azure Cards** icon on the toolbar to open the picker.

  ![Azure Cards picker interface in Miro.](images/21017013109010_Azure%20cards%20picker.jpg)*Azure Cards picker*

  The picker supports search across all fields, allowing you to find a card by its title, type, state, etc. You can also use robust [keyword search](https://docs.microsoft.com/azure/devops/project/search/get-started-search?view=azure-devops#start-your-search-with-a-keyword) powered by Microsoft.

  ![Animation showing search functionality within the Azure Cards picker.](images/21017013114002_Azure%20Cards%20picker.gif)*Search Azure Cards in the picker*

  You can filter cards by project, assignee, type, area, and state, which unlocks advanced filtering of Azure work items directly within Miro.

  ![Filtering options within the Azure Cards picker.](images/21017013116306_filter.jpg)*Filter Azure Cards in the picker*

To navigate to the original Azure work item, select a card on the board and click the **Source** button on its context menu.

Azure Cards can be used as standalone board widgets or as components of interactive [Kanban](../../using-miro/advanced-tools/02-columns-(formerly-kanban).md) and [User Story Map](../../using-miro/advanced-tools/07-user-story-mapping.md) frameworks. You can add Azure Cards to these frameworks by dragging them in.

## Create and edit Azure Cards directly in Miro

The two-way integration between Miro and Azure DevOps allows teams to create new Azure work items and edit existing ones directly from a Miro board. You can also convert existing Miro cards and sticky notes into Azure Cards.

### Create a new Azure Card

To create a new Azure work item from Miro:

1. Select **Azure Cards** from the Creation toolbar and choose **Create work item** on the top-right of the picker.
2. Fill out the card fields, choose a project, item type, assignee, and click **Create**. The new item will be created in your Azure DevOps directory as well as on your Miro board.

### Convert Miro cards or sticky notes to Azure Cards

To convert an existing Miro card or sticky note into an Azure Card:

1. Select the sticky note or card on the board.
2. Click the convert option (usually an Azure DevOps icon or "Convert to Azure work item") on the object's context menu.
3. Set the card parameters (like project, item type) in the dialog and click **Convert**. The text on the sticky note/card will be converted into the card title.

> **💡** Save time by bulk converting stickies or Miro cards to Azure Cards. Click and drag to select all objects you wish to convert, and within the context menu, select **Convert to Azure work items**.

### Edit an Azure Card

The option to edit Azure Cards in Miro removes the hassle of switching between tools. To edit a card:

1. Click the Azure Card on your Miro board.
2. Click the **pen icon (edit)** on the card's context menu. A pop-up window will open, allowing you to edit the item's fields.
3. Click **Update** to save the changes. The changes will be reflected in Azure DevOps as well.

### Change Azure Card color

To customize the appearance of your Azure Cards on the board:

To change a card's fill color, click the card or cards and choose **fill color** from the context menu. If you duplicate the card or cards, all subsequent copies will have the same fill color.

## Uninstall the Azure Cards integration

If you no longer need the Azure Cards integration, you can uninstall it. Uninstalling at the team level requires Team Admin permissions.

1. Go to **Team settings** > **Apps & Integrations** > **Azure Cards**.
2. Select **Uninstall for team**.

## Supported Azure Card fields

The following fields are supported for Azure Cards in Miro:

- Title
- Project
- Type
- State
- Description (Edit is not supported)
- Parent WI
- Assignee
- Priority
- Story Points
- Area
- Iteration
- Acceptance Criteria

Custom fields are not supported.

## Azure Cards troubleshooting

If you encounter issues with the Azure Cards integration, consult the common problems and solutions below.

URL is not valid

The URL you used is not correct. Please check the spelling and formatting. For instance, the Azure Organization address must end with a slash.

Azure Organization URL cannot be reached

The URL entered does not exist. Please enter the existing URL or check the spelling. Also, check the following:

- Make sure your organization can accept 3rd party authorization: in **Organization Settings > Policies (Security)** **>** ensure "Third-party application access via OAuth" is enabled.
- Your Azure Organization is on a private network / your company firewall blocks external network connections. Please make the necessary changes to your firewall and VPN configuration, adding our domains to your allowlist: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com, realtimeboard.com*, *.realtimeboard.com, *static.miro-apps.com domains. If you use a proxy, please configure a reverse one allowing us access. Be sure to fill in the **Azure DevOps URL** field in the settings with the address that we can access (the address may differ from the actual address of your restricted Azure DevOps). You may also want to prolong the timeout value on your proxy server.
- All requests for the integration go through an Amazon load balancer, so providing specific network information isn't possible from Miro.

Failed to Create Service Hook Subscription

The currently logged in Azure user does not have the necessary permissions. The Azure user on whose behalf the Azure instance will be connected to Miro must have access to these REST API methods:

- [*Create service hook subscription*](https://docs.microsoft.com/rest/api/azure/devops/hooks/subscriptions/create?view=azure-devops-rest-6.0) ("*vso.serviceendpoint_manage"* [scope](https://docs.microsoft.com/azure/devops/integrate/get-started/authentication/oauth?view=azure-devops#scopes) required)
- [*Receive metadata about projects (this information is used to specify work items in subscription events correctly)*](https://docs.microsoft.com/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-6.0)
- *The following methods are also required to be accessible to all users using the integration:*
  - [*Get items*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/get%20work%20item?view=azure-devops-rest-6.0)
  - [*List items*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/list?view=azure-devops-rest-6.0)
  - [*Get item types*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/get?view=azure-devops-rest-6.0)
  - [*List item types*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/list?view=azure-devops-rest-6.0)

The user **username@microsoft.com** does not have access to any project in the specified Azure Organization URL.

You cannot access any projects in the Azure organization being used. To import cards you should have access to them on Azure Boards' side. Please reach out to the Azure organization owner and ask them to invite you to the Azure organization. [This article](https://docs.microsoft.com/azure/devops/organizations/security/look-up-organization-owner?view=azure-devops) can help you find out the name of the Organization Owner.

Failed to create service hook subscription: the user **username@microsoft.com** is not an Organization Owner. Please ask your Organization Owner to configure this step.

You should be both the Azure organization owner and the Miro Company Admin to set up Azure Cards within Miro.

Authorization has expired. Please reconnect the integration in your team's settings.

Azure authorization has expired. Please reconnect the integration on the Personal level as described in the "Connect your personal Azure account to use Azure Cards" section above.

The card you're working with is showing unexpected behavior.

- This can happen if the card was unsynced from the Azure organization. For instance if you copied the card from another board or are working on a board that was moved between teams. To solve the situation, please re-add the Azure item to the board.

The number of work items returned exceeds the size limit of 200. Change the query to return fewer items.

If you get this error message, it means that you've selected too many tasks to add to the board as cards. Please limit the number of tasks by using the search bar. At the moment, when you open the picker, no filters are applied, and all tasks from the last three months are displayed. Every time the picker tries to display more than 200 tasks, you will receive this error message.

I do not get the **Connect** button when trying to connect my Azure Organization with Miro in Miro settings.

Ensure you have Team Admin rights. Go to the **Active users** tab in your Team settings and [promote yourself to Team Admin](../../administration/user-management/06-how-to-manage-admin-roles.md) if necessary. This applies to the initial setup of the Azure Organization connection by an admin.

:::note
If you experience other issues, get in touch with [Miro Support](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).
:::

## Azure Cards frequently asked questions

Here are answers to some common questions about the Azure Cards integration.

What IPs should be allowlisted for Azure Cards?

For the Azure Cards integration to function correctly, especially in restricted network environments, you may need to allowlist the following IP addresses:

- 18.203.61.162
- 54.220.74.201
- 54.216.81.236
- 54.73.153.141
- 52.215.228.26
- 52.16.47.17
- 54.217.180.21

What happens to existing Azure Cards when you disconnect & uninstall the Azure Cards app?

Cards stay intact on the Miro boards with no data loss; however, they stop syncing with Azure, and the source button disappears.
