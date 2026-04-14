---
title: Import Microsoft Purview sensitivity labels
article_id: 22161930709010
sidebar_position: 8
created_at: '2024-10-23T15:05:49Z'
updated_at: '2025-12-01T16:32:38Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

For organizations utilizing Microsoft Purview, maintaining consistent data security and classification across multiple platforms is essential. Miro's integration with Microsoft Purview allows administrators to import sensitivity labels directly from Microsoft Purview into Miro, simplifying the management of classification schemas across both platforms.

By leveraging this integration, organizations can ensure that content within Miro is classified consistently with the established Microsoft Purview framework. This not only reduces the operational overhead of manually recreating or updating classification labels but also strengthens data security. By aligning Miro's data protection capabilities with Microsoft Purview, admins can confidently manage sensitive information across their entire digital ecosystem.

## Import Microsoft Purview sensitivity labels into Miro

If your organization does not have an existing data classification setup configured in Miro, you can easily set up Data Classification in Miro by importing existing sensitivity labels directly from Microsoft Purview.

If you already have an existing data classification configuration, you can import sensitivity labels from Microsoft Purview and transfer existing classification labels in Miro.

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
5. On the **Microsoft Sign in** page that appears in a new tab, enter your Microsoft credentials and sign in. Once you are signed in to your Microsoft account, the tab is automatically closed.
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
9. To save the classification level configuration, click **Done**.
10. Click **Next**. Your configuration is saved, but it will only take effect after you click **Publish** on the [**Review impact**](https://help.miro.com/hc/articles/16494764223378) page.

    You can then proceed with either of the following next steps:

    - [Define auto-classification](../../canvas-25-admin-features/data-classification/09-define-auto-classification.md). This is optional. If you want to define auto-classification at a later point in time, click **Next**.
    - [Define guardrails](../../canvas-25-admin-features/data-classification/05-define-guardrails.md). This is optional. If you want to define guardrails a later point in time, click **Next**.
    - [Review impact](https://help.miro.com/hc/articles/16494764223378). This the last step of the workflow and it is mandatory.

## Import sensitivity labels from Microsoft Purview into existing Data Classification configuration in Miro

### **Prerequisites**

- Ensure that you have the necessary roles or privileges to work with sensitivity labels in Microsoft Purview.
- You must know the details of the board classification levels that you want to configure based on your security and governance requirements.
- You must have the [Sensitive Content Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). To request for the Sensitive Content Admin role, contact your Company Admin.

:::note
Notes:
- Per Microsoft's documentation, updates to sensitivity labels in Microsoft Purview can take up to 24 hours to replicate to all apps and services. Please allow enough time for changes to take place and then import sensitivity labels. If the updates you made in MS Purview are not replicated after 24 hours, please contact the Microsoft Purview Support team.
- You can import up to 50 sensitivity labels from Microsoft Purview into Miro.
- You cannot transfer classification levels that are used in retention policies. You must ensure that the classification levels are not used in any retention policies before proceeding. For more information, see [Edit retention policy](../../canvas-25-admin-features/content-lifecycle-management/11-edit-retention-policy.md).
:::

To import sensitivity labels from Microsoft purview and transfer/map to existing classification labels in Miro, perform the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Data classification**.
3. On the **Classification** page, at the top of the screen, click **Import**.
4. If you are already signed in to Microsoft, skip this step and proceed to the next step.
   If you are not signed in to Microsoft, click **Sign In**. On the **Microsoft Sign in** page that appears in a new tab, enter your Microsoft credentials and sign in. Once you are signed in to your Microsoft account, the tab is automatically closed.
5. On the **Import from Microsoft Purview** box, click **Import** next to Import sensitivity labels to Miro. The **Import classification from Microsoft Purview** page appears.
6. On the **Import Levels** page, select the check box for the Microsoft Purview sensitivity labels you want to use as classification levels in Miro, and then click **Next**. The **Transfer existing levels** page appears.

   > ✏️ Per Microsoft's documentation, updates to sensitivity labels in Microsoft Purview can take up to 24 hours to replicate to all apps and services. Please allow enough time for changes to take place and then import sensitivity labels. If the updates you made in MS Purview are not replicated after 24 hours, please contact the Microsoft Purview Support team.
7. To ensure content is classified correctly, you must transfer existing Miro classification levels to the newly imported levels from Microsoft Purview. The levels listed on the left are the existing Miro classification levels and the ones listed in the drop-down list on the right are the imported Microsoft Purview sensitivity labels. Once you are done, click **Next**.
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

## Disconnect from Microsoft Purview

When you are connected to Purview, you cannot add or edit classification names, update classification levels, and so on. If you want to do these actions, you must disconnect from Microsoft Purview.  You cannot import updates from Microsoft Purview into Miro once you disconnect from Purview.

To disconnect from Microsoft Purview, perform the following steps:

1. Go to your [Miro settings](https://miro.com/app/settings).
2. On the left pane, under **Enterprise Guard,** click **Data classification**.
3. On the **Classification** page, at the top of the screen, click the **Last Import** button at the top of the screen, and then click **Disconnect from Purview**.
