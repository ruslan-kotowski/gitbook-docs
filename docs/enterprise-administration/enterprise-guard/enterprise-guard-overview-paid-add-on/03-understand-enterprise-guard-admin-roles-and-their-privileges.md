---
title: Understand Enterprise Guard admin roles and their privileges
article_id: 15695755655954
sidebar_position: 3
created_at: '2023-12-11T18:33:53Z'
updated_at: '2026-03-17T08:39:20Z'
draft: false
---

Enterprise Guard capabilities are controlled through admin privileges. These privileges can be granted through predefined admin roles or through custom admin roles configured with the required privileges.

The following table lists the available privileges for each feature and shows which predefined admin roles include them by default. When creating custom admin roles, Company Admins can assign these privileges to grant access to specific Enterprise Guard capabilities.

The following table lists the detailed privileges and admin role matrix for each feature.

|  |  |  |  |
| --- | --- | --- | --- |
| **Content lifecycle management** | | | |
| **Privilege** | **Data Governance Admin** | **Sensitive Content Admin** | **eDiscovery Admin** |
| View trash settings | ✅ | ❌ | ❌ |
| Edit trash settings | ✅ | ❌ | ❌ |
| Add retention policy | ✅ | ❌ | ❌ |
| Edit retention policy | ✅ | ❌ | ❌ |
| Delete retention policy | ✅ | ❌ | ❌ |
| Add disposition policy | ✅ | ❌ | ❌ |
| Edit disposition policy | ✅ | ❌ | ❌ |
| Delete disposition policy | ✅ | ❌ | ❌ |
| **Data classification** | | | |
| **Privilege** | **Data Governance Admin** | **Sensitive Content Admin** | **eDiscovery Admin** |
| View data classification settings | ❌ | ✅ | ❌ |
| Edit classification levels | ❌ | ✅ | ❌ |
| Edit auto-classification settings | ❌ | ✅ | ❌ |
| Edit classification guardrails settings | ❌ | ✅ | ❌ |
| Edit default classification level | ❌ | ✅ | ❌ |
| **Data discovery** | | | |
| **Privilege** | **Data Governance Admin** | **Sensitive Content Admin** | **eDiscovery Admin** |
| View privacy labels | ❌ | ✅ | ❌ |
| Turn privacy data detection on/off | ❌ | ✅ | ❌ |
| View count of matches - privacy labels | ❌ | ✅ | ❌ |
| View redacted matches - privacy labels | ❌ | ✅ | ❌ |
| View full matches - privacy labels | ❌ | ✅ | ❌ |
| **eDiscovery** | | | |
| **Privilege** | **Data Governance Admin** | **Sensitive Content Admin** | **eDiscovery Admin** |
| Manage legal hold settings | ❌ | ❌ | ✅ |
| View legal hold settings | ❌ | ❌ | ✅ |

*Detailed privileges and predefined admin role matrix for each feature*

:::note
Enterprise Guard capabilities can be granted through predefined admin roles or through custom admin roles configured with the required privileges.
:::

## Assign an Enterprise Guard admin role

:::note
To assign an Enterprise Guard admin role to a user, you must be a **Company Admin**.
:::

1. Go to your **profile settings**:

   - From a board: **Main menu > Preferences > Profile settings**.
   - From the dashboard: Click your **avatar** in the top-right corner and click **Settings**.
   - From the URL: Go to `https://miro.com/app/settings`, and choose your **Company** from the list in the top-left corner.
2. Under **User management**, click **Admin roles**.
3. In the right pane, find the admin role you want to assign (for example **Data Governance Admin**, **Sensitive Content Admin**, or **eDiscovery Admin**).
4. Click the **ellipsis (… )** next to the role and select **Assign role**.
5. Choose the user to whom you want to assign the role.
6. Scroll to the bottom of the window and click **Assign**.

## Custom admin roles for Enterprise Guard

Custom admin roles allow Company Admins to grant access to individual Enterprise Guard capabilities without assigning broader administrative roles. This enables organizations to tailor access based on internal governance, security, or compliance responsibilities.

When creating or editing a custom admin role, Company Admins can select the privileges that determine which Enterprise Guard capabilities the role can access and manage. These privileges span multiple Enterprise Guard domains, such as Data classification, Data discovery, Content lifecycle management, eDiscovery.

By assigning only the required privileges, organizations can delegate administrative tasks, such as reviewing sensitive content findings, managing classification settings, configuring lifecycle policies, or accessing eDiscovery tools, to the appropriate teams. The table below lists privileges that can be assigned when configuring custom admin roles.

|  |  |  |
| --- | --- | --- |
| **Capability** | **Privilege** | **Description** |
| **Data classification** | View data classification settings | Admin can view the organization's classification settings. |
| Edit auto-classification settings | Admin can edit the organization's auto-classification settings. |
| **Data discovery** | View data discovery settings | Admin can view the organization's data discovery settings. |
| Manage data discovery settings | Admin can manage the organization's data discovery settings. |
| View data discovery results | Admin can view data discovery related results. |
| Manage data discovery results | Admin can manage data discovery related results. |
| **eDiscovery** | View legal hold settings | Admin can view legal holds within the eDiscovery cases settings page. |
| Manage legal hold settings | Admin can manage legal holds within the eDiscovery cases settings page. |
| View board exports | Admin can view eDiscovery board exports. |
| Manage board exports | Admin can manage eDiscovery board exports. |
| **Content lifecycle management** | View trash settings | Admin can view the organization's board trash settings. |
| Manage trash settings | Admin can manage the organization's board trash time to live and permissions. |
| View content lifecycle retention settings | Admin can view the content lifecycle retention settings page. |
| Manage content lifecycle retention settings | Admin can manage the content lifecycle retention settings page. |
| View content lifecycle disposition settings | Admin can view the content lifecycle disposition settings page. |
| Manage content lifecycle disposition settings | Admin can manage the content lifecycle disposition settings page. |
| View content under retention or disposition | Allows the user to view content impacted by retention or disposition policies. |
