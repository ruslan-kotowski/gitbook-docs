---
title: Define classification levels
article_id: 16494683650322
sidebar_position: 7
created_at: '2024-01-19T18:57:35Z'
updated_at: '2025-11-25T15:40:29Z'
draft: false
---

This is the first step of the auto-classification and guardrails configuration flow. In this step of the flow, you can define classification levels, which involves adding new classification levels or updating a classification level configuration, such as the classification name, sensitivity order, badge color, link to classification guidelines, and more. When defining classification levels you can:

- [Add or edit a classification level](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md#add-or-edit-a-classification-level)
- [Set up Data Classification by importing sensitivity labels from Microsoft Purview](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md#set-up-data-classification-by-importing-sensitivity-labels-from-microsoft-purview)
- [Update the default classification level for new boards](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md#update-the-default-classification-level-for-new-boards)
- [Update the sensitivity order of a classification level](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md#update-the-sensitivity-order-of-a-classification-level)
- [Remove a classification level](../../canvas-25-admin-features/data-classification/07-define-classification-levels.md#remove-a-classification-level)

## Prerequisites

- You must know the details of the board classification levels that you want to configure based on your security and governance requirements.
- You must have the [Sensitive Content Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Sensitive Content Admin role, contact your Company Admin.

## Add or edit a classification level

You can add or edit a classification level by performing the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Data classification**.
3. If you are defining classification levels for the first time, click **Set up classification** at the bottom of the screen.
   If you want to edit classification levels, click **Edit classification levels** at the top-right of the screen.
4. On the **Define classification levels** page:
   To add a classification level, click **Add level**.
   To edit a classification level, click **Edit classification levels**.
5. Add or edit the classification level per your requirements. The following table lists each field and its description.

   |  |  |
   | --- | --- |
   | **Field** | **Description** |
   | **Level** | Indicates the board sensitivity order for this classification level.  Currently, the sensitivity order **1** indicates the **least sensitive** classification level.  Click the up or down arrows to assign the board sensitivity order for this classification level. |
   | **Name** | Name of the classification level.  When users view a board that belongs to this classification level, this name appears on the board classification badge beside the board name.  Figure 1 illustrates an example where the name of the board classification is **INTERNAL**.  sample_board_internal.png Figure 1: Example where the name of the board classification is **INTERNAL** |
   | **Description** | Description of this classification level.  When users view a board that belongs to this classification level and they click the board classification badge, the description of the classification level appears.  We recommend that you add a meaningful description that guides your users about the sensitivity of this board and the recommended precautions or actions.  Figure 2 illustrates an example of the **description** added for the INTERNAL classification level.   sample_internal_description.png Figure 2: Example of the **description** added for the INTERNAL classification level |
   | **Badge color** | Background color for the board classification badge.  Figure 3 illustrates an example where the INTERNAL board classification level has a **Yellow** badge color.  sample_board_internal.png Figure 3: Example where the INTERNAL board classification level has a **Yellow** badge color |
   | **Link to guidelines** | URL that provides more information about policies or instructions applicable for this classification level. This could be a page that provides more information for users in your organization to learn more about your board classification levels and how to work with them. You must provide the URL in the following format: `http://www.example.com`  When the user clicks the **Learn more** icon (question mark icon) beside the board classification badge, this URL is loaded in a new browser tab. |
   | **Use as default level for new boards** | Select this checkbox to set this classification level as the default classification for all new boards. |
   | **Preview** | Displays a preview of the board classification badge with its description and learn more icon. The preview shows exactly how the classification badge appears for users on a board. |

   To save the classification level configuration, click **Done**.
6. Click **Next**. Your configuration is saved, but it will only take effect after you click **Publish** on the [**Review impact**](https://help.miro.com/hc/articles/16494764223378) page.

   You can then proceed with either of the following next steps:

   - [Define auto-classification](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md). This is optional. If you want to define auto-classification at a later point in time, click **Next**.
   - [Define guardrails](../../canvas-25-admin-features/data-classification/05-define-guardrails.md). This is optional. If you want to define guardrails a later point in time, click **Next**.
   - [Review impact](https://help.miro.com/hc/articles/16494764223378). This the last step of the workflow and it is mandatory.

## Set up Data Classification by importing sensitivity labels from Microsoft Purview

### Prerequisites

- Ensure that you have the necessary roles or privileges to work with sensitivity labels in Microsoft Purview.
- You must know the details of the board classification levels that you want to configure based on your security and governance requirements.
- You must have the [Sensitive Content Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Sensitive Content Admin role, contact your Company Admin.

:::note
Notes:
- Per Microsoft's documentation, updates to sensitivity labels in Microsoft Purview can take up to 24 hours to replicate to all apps and services. Please allow enough time for changes to take place and then import sensitivity labels. If the updates you made in MS Purview are not replicated after 24 hours, please contact the Microsoft Purview Support team.
- You can import up to 50 sensitivity labels from Microsoft Purview into Miro.
- If you already have an existing data classification configuration, you can import sensitivity labels from Microsoft Purview and transfer existing classification labels in Miro. For more information, see [Import sensitivity labels from Microsoft Purview into existing Data Classification configuration in Miro](../../canvas-25-admin-features/data-classification/08-import-microsoft-purview-sensitivity-labels.md#import-sensitivity-labels-from-microsoft-purview-into-existing-data-classification-configuration-in-miro).
:::

To import sensitivity labels from Microsoft purview and set up data classification in Miro, perform the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Data classification**.
3. On the **Classification** page, at the bottom of the screen, click **Get Started**.
4. On the **Import from Microsoft Purview** box, click **Sign In**.
5. On the **Microsoft Sign in** page that appears in a new tab, enter your Microsoft credentials and sign in. Once you are signed in to your Microsoft account, the tab is automatically closed,
6. On the **Classification** page, on the **Import from Microsoft Purview** box, click **Import**.
   The **Import classification from Microsoft Purview** page appears.
7. Select the check box for the Microsoft Purview sensitivity labels you want to use as classification levels in Miro, and then click **Next**.
   > ✏️ Per Microsoft's documentation, updates to sensitivity labels in Microsoft Purview can take up to 24 hours to replicate to all apps and services. Please allow enough time for changes to take place and then import sensitivity labels. If the updates you made in MS Purview are not replicated after 24 hours, please contact the Microsoft Purview Support team.
8. On the **Define classification levels** page, you can edit the classification levels to assign the default classification level or add a link to the guidelines. The following table lists each field and its description.

   |  |  |
   | --- | --- |
   | **Field** | **Description** |
   | **Link to guidelines** | URL that provides more information about policies or instructions applicable for this classification level. This could be a page that provides more information for users in your organization to learn more about your board classification levels and how to work with them. You must provide the URL in the following format: `http://www.example.com`  When the user clicks the **Learn more** icon (question mark icon) beside the board classification badge, this URL is loaded in a new browser tab. |
   | **Use as default level for new boards** | Select this checkbox to set this classification level as the default classification for all new boards. |
   | **Preview** | Displays a preview of the board classification badge with its description and learn more icon. The preview shows exactly how the classification badge appears for users on a board. |

   To save the classification level configuration, click **Done**.
9. Click **Next**. Your configuration is saved, but it will only take effect after you click **Publish** on the [**Review impact**](https://help.miro.com/hc/articles/16494764223378) page.

   You can then proceed with either of the following next steps:

   - [Define auto-classification](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md). This is optional. If you want to define auto-classification at a later point in time, click **Next**.
   - [Define guardrails](../../canvas-25-admin-features/data-classification/05-define-guardrails.md). This is optional. If you want to define guardrails a later point in time, click **Next**.
   - [Review impact](https://help.miro.com/hc/articles/16494764223378). This the last step of the workflow and it is mandatory.

## Update the default classification level for new boards

You can update the default classification level by performing the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Data classification**.
3. Click **Edit classification levels** at the top-right of the screen.
4. On the **Define classification levels** page, click **Edit classification levels**.
5. Click the **Edit** icon (![Screenshot 2024-01-22 at 23.20.18.png](images/21017417804818_Screenshot%202024-01-22%20at%2023.20.18.png)) for the level that you want to set as the default classification level.
6. Select the **Use as default level for new boards** checkbox.
7. Click **Done**.
   Your configuration is saved, but it will only take effect after you click **Publish** on the [**Review impact**](https://help.miro.com/hc/articles/16494764223378) page.
8. Click **Next**. Your configuration is saved, but it will only take effect after you click **Publish** on the [**Review impact**](https://help.miro.com/hc/articles/16494764223378) page.

   You can then proceed with either of the following next steps:

   - [Define auto-classification](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md). This is optional. If you want to define auto-classification at a later point in time, click **Next**.
   - [Define guardrails](../../canvas-25-admin-features/data-classification/05-define-guardrails.md). This is optional. If you want to define guardrails a later point in time, click **Next**.
   - [Review impact](https://help.miro.com/hc/articles/16494764223378). This the last step of the workflow and it is mandatory.

## Update the sensitivity order of a classification level

You can update the sensitivity order of a classification level by performing the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Data classification**.
3. Click **Edit classification levels** at the top-right of the screen.
4. On the **Define classification levels** page, click **Edit classification levels**.
5. The classification levels appear with their current sensitivity order. Click the up or down arrows for the classification levels for which you want to update the sensitivity order.

   > ✏️ Currently, the sensitivity order **1** indicates the **least sensitive** classification level.

   Your configuration is saved, but it will only take effect after you click **Publish** on the **[Review impact](https://help.miro.com/hc/articles/16494764223378)** page.
6. Click **Next**. Your configuration is saved, but it will only take effect after you click **Publish** on the [**Review impact**](https://help.miro.com/hc/articles/16494764223378) page.

   You can then proceed with either of the following next steps:

   - [Define auto-classification](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md). This is optional. If you want to define auto-classification at a later point in time, click **Next**.
   - [Define guardrails](../../canvas-25-admin-features/data-classification/05-define-guardrails.md). This is optional. If you want to define guardrails a later point in time, click **Next**.
   - [Review impact](https://help.miro.com/hc/articles/16494764223378). This the last step of the workflow and it is mandatory.

## Remove a classification level

:::note
You cannot remove a classification level if it is associated with a [retention policy](https://help.miro.com/hc/sections/19180529348754).
:::

You can remove a classification level by performing the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Data classification**.
3. Click **Edit classification levels** at the top-right of the screen.
4. On the **Define classification levels** page, click **Edit classification levels**.
5. Click the delete icon for the classification level that you want to remove.
6. If the classification level that you want to delete has already been applied to 1 or more boards, a notification window appears informing you about the number of boards that the classification level has been applied to.
   Select the new classification level that you want to apply for the affected boards.
7. Click **Done**.
   Your configuration is saved, but it will only take effect after you click **Publish** on the [**Review impact**](https://help.miro.com/hc/articles/16494764223378) page.
8. Click **Next**. Your configuration is saved, but it will only take effect after you click **Publish** on the [**Review impact**](https://help.miro.com/hc/articles/16494764223378) page.

   You can then proceed with either of the following next steps:

   - [Define auto-classification](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md). This is optional. If you want to define auto-classification at a later point in time, click **Next**.
   - [Define guardrails](../../canvas-25-admin-features/data-classification/05-define-guardrails.md). This is optional. If you want to define guardrails a later point in time, click **Next**.
   - [Review impact](https://help.miro.com/hc/articles/16494764223378). This the last step of the workflow and it is mandatory.
