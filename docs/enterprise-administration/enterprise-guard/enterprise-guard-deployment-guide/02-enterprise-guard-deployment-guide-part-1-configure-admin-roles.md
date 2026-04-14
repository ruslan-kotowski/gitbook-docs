---
title: 'Enterprise Guard Deployment Guide Part 1: Configure Admin Roles'
article_id: 17120595534994
sidebar_position: 2
created_at: '2024-02-19T09:19:59Z'
updated_at: '2025-11-25T15:41:04Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Company Admins can grant themselves and others additional admin roles once Enterprise Guard is enabled. As a result, the number of Company Admins in your organization should be kept to a minimum. Carefully consider your existing admin configuration and move Company Admins to other roles (such as team or user admin) when appropriate to balance security, compliance, and operational efficiency.

Although recommended, a holistic reevaluation of your admin configuration is not required to deploy Enterprise Guard. Move on to [Part 2: Deploy Data Security](../../enterprise-subscription-management/enterprise-guard-deployment-guide/03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md) at your discretion.

## Miro admin roles overview

Here’s a list of available admin roles in Miro including a description of responsibilities and who they are suitable for in a typical organization.

:::note
Notes:
- This is an evolving list of roles and privileges. Check this page periodically for updates.
- To assign the Data Governance Admin or Sensitive Content Admin role to a user, you must be a Company Admin.
:::

|  |  |  |
| --- | --- | --- |
| **Admin role** | **Responsibilities** | **Recommended for** |
| **Company Admins** | Responsible for overarching management and delegating specific responsibilities to other admin roles. Should have a broad understanding of the organization's operational needs and compliance obligations. | - Senior IT administrators - Department Managers - Project Managers - Team Leaders - Operations Managers - Business Technology Managers - Miro Product Owner |
| **Team Admins** | Manage team-specific settings and user access within their respective teams. Ensures team autonomy while aligning with broader organizational policies. | - Department Managers - Project Managers - Team Leaders - Operations Managers |
| **User Admins** | Handle user management and licensing. Ideal for managing employee access and accounts. Efficiently manage users without overburdening Company or Team Admins. | - IT Manager - IT Administrators - IT Service Desk |
| **Data Governance Admins (Enterprise Guard)** | Responsible for compliance and data governance. Should understand the legal and regulatory landscape relevant to the organization's data, including the organization's retention and disposition policies. | - Chief Compliance Officer (CCO) - Data Governance Manager - Compliance Manager - Regulatory Affairs Manager - Risk Manager - Records Manager - eDiscovery Analyst - Forensics Analyst |
| **eDiscovery Admins (Enterprise Guard)** | Manage legal hold settings to preserve boards relevant to ongoing investigations or legal cases. This includes creating, modifying, and releasing legal holds or cases to prevent the permanent deletion of content, ensuring compliance with legal and regulatory obligations. This role is crucial for organizations requiring stringent data preservation to support legal proceedings and compliance mandates. | - Legal Counsel - eDiscovery Specialists - Compliance Officers - Risk Managers - Forensics Analysts - Chief Information Security Officer (CISO) - Data Protection Officer (DPO) - Privacy Officer/Privacy Manager |
| **Sensitive Content Admins (Enterprise Guard)** | Responsible for data protection and privacy. Crucial in classifying, managing, and safeguarding sensitive information across the organization. Important for handling PII, PHI, PCI, or intellectual property. | - Chief Information Security Officer (CISO) - Data Protection Officer (DPO) - Privacy Officer/Privacy Manager - Cybersecurity Analyst - IT Security Consultant |

:::tip
Learn more about [admin roles and their privileges](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) in the Enterprise Plan.
:::

## Detailed Enterprise Guard privilege and admin role matrix

The following table lists the detailed privileges and admin role matrix for each feature.

|  |  |  |  |
| --- | --- | --- | --- |
| **Content lifecycle management** | | |  |
| **Privilege** | **Data Governance Admin** | **Sensitive Content Admin** | **eDiscovery Admin** |
| View trash settings | ✅ | ❌ | ❌ |
| Edit trash settings | ✅ | ❌ | ❌ |
| Add retention policy | ✅ | ❌ | ❌ |
| Edit retention policy | ✅ | ❌ | ❌ |
| Delete retention policy | ✅ | ❌ | ❌ |
| Add disposition policy | ✅ | ❌ | ❌ |
| Edit disposition policy | ✅ | ❌ | ❌ |
| Delete disposition policy | ✅ | ❌ | ❌ |
| **Data classification** | | |  |
| **Privilege** | **Data Governance Admin** | **Sensitive Content Admin** | **eDiscovery Admin** |
| View data classification settings | ❌ | ✅ | ❌ |
| Edit classification levels | ❌ | ✅ | ❌ |
| Edit auto-classification settings | ❌ | ✅ | ❌ |
| Edit classification guardrails settings | ❌ | ✅ | ❌ |
| Edit default classification level | ❌ | ✅ | ❌ |
| **Data discovery** | | |  |
| **Privilege** | **Data Governance Admin** | **Sensitive Content Admin** | **eDiscovery Admin** |
| View privacy labels | ❌ | ✅ | ❌ |
| Turn privacy data detection on/off | ❌ | ✅ | ❌ |
| View count of matches - privacy labels | ❌ | ✅ | ❌ |
| View redacted matches - privacy labels | ❌ | ✅ | ❌ |
| View full matches - privacy labels | ❌ | ✅ | ❌ |
| **eDiscovery** | | |  |
| **Privilege** | **Data Governance Admin** | **Sensitive Content Admin** | **eDiscovery Admin** |
| Manage legal hold settings | ❌ | ❌ | ✅ |
| View legal hold settings | ❌ | ❌ | ✅ |

*Table 2: Detailed privileges and admin role matrix for each feature*

## Transitioning your admin configuration

### Audit your current admin configuration

Review the list of users who have admin rights in Miro and their responsibilities. Use the [Admin Configuration Assessment Tool](#resources) to generate a summary of the current state.

- Filter the list of users from the **Active users** section of Company settings to view Company Admins.
- View the list of User Admins, Data Governance Admins, and Sensitive Content Admins using the **Admin role** section of the Company settings.

### Map a new admin configuration

Compare your current admin configuration against the [table above](#miro-admin-roles-overview) and your company policies. Use the Admin Configuration Assessment Tool to generate a new configuration.

Consider questions such as:

- Who needs the Data Governance role?
- Who needs the Sensitive Content role?
- Which Company Admins can be transitioned to User Admins?
- Which Company Admins can be transitioned to Team Admins?

### Reassign roles and inform users

The Help Center articles below show how to assign the various roles. For your convenience, customize the provided email templates to inform users of transitions.

- [How to assign Company Admins and Team Admins](../../../administration/user-management/06-how-to-manage-admin-roles.md)
- [How to assign User Admins, Data Governance Admins, and Sensitive Content Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)

### Assign the Data Governance Admin role

:::note
To assign the Data Governance Admin role to a user, you must be a Company Admin.
:::

1. Go to your profile settings.
   - From a board: **Main menu > Preferences > Profile settings**.- From the dashboard: click your avatar in the top-right corner and click **Settings**.
   - From the URL `https://miro.com/app/settings`: Choose your Company from the list in the top-left corner.
2. Under **User management**, click **Admin roles**.
3. On the right pane, click the **Data Governance Admin** **ellipsis (****…)**, and then select **Assign role**.
4. Choose the user to whom you want to assign the Data Governance Admin role to, scroll to the bottom of the window, and then click **Assign**.

### Assign the Sensitive Content Admin role

:::note
To assign the Sensitive Content Admin role to a user, you must be a Company Admin.
:::

1. Go to your profile settings.
   - From a board: **Main menu > Preferences > Profile settings**.- From the dashboard: click your avatar in the top-right corner and click **Settings**.
   - From the URL `https://miro.com/app/settings`: Choose your Company from the list in the top-left corner.
2. Under **User management**, click **Admin roles**.
3. On the right pane, click the **Sensitive Content Admin** **ellipsis (****…)**, and then select **Assign role**.
4. Choose the user to whom you want to assign the Sensitive Content Admin role to, scroll to the bottom of the window, and then click **Assign**.

### Assign the eDiscovery Admin role

:::note
To assign the eDiscovery Admin role to a user, you must be a Company Admin.
:::

1. Go to your profile settings.
   - From a board: **Main menu > Preferences > Profile settings**.- From the dashboard: click your avatar in the top-right corner and click **Settings**.
   - From the URL `https://miro.com/app/settings`: Choose your Company from the list in the top-left corner.
2. Under **User management**, click **Admin roles**.
3. On the right pane, click the **eDiscovery Admin** **ellipsis (****…)**, and then select **Assign role**.
4. Choose the user to whom you want to assign the eDiscovery Admin role to, scroll to the bottom of the window, and then click **Assign**.

### Resources

- [Admin Configuration Assessment Tool](https://docs.google.com/spreadsheets/d/1a0WQc-fBpuVwfnoY8VCx66PjOXS76q7DJ__xDYcp8rk/edit?usp=sharing) (make a copy)
- [Email Templates | Admin Configuration Communications](https://docs.google.com/document/d/18Kw4GNPq7GnAx8R8co5PaZ04peVogfVDgsdKK2MuARM/edit?usp=sharing) (make a copy)
