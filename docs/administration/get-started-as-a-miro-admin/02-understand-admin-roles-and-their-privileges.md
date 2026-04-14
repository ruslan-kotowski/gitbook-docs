---
title: Understand admin roles and their privileges
article_id: 14766440626834
sidebar_position: 2
created_at: '2023-10-30T19:54:40Z'
updated_at: '2026-02-09T12:56:12Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Assigning predefined administrator roles is an easy way to give privileges to another user in your organization. Each admin role grants one or more privileges that together allow you to perform specific Miro functions.

Miro currently provides four predefined organization-level admin roles, namely the Company Admin, User Admin, Content Admin, and Security Admin.

The following table lists the privileges associated with each role.

:::note
This is an evolving list of roles and privileges. Check this page periodically for updates.
:::

|  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| **Account** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| View company profile | - View company profile page  - View primary contacts  - View company logo | ✅ | ❌ | ❌ | ❌ | ❌ |
| Edit company profile | - Edit company name  - Edit company logo  - Edit primary contacts | ✅ | ❌ | ❌ | ❌ | ❌ |
| View insights | - View Miro usage insights | ✅ | ❌ | ❌ | ❌ | ❌ |
| **User and Team Management** | | | | | | |
| **Users** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| View users | - View active users  - Apply user filters  - Look at user profiles  - View deactivated users | ✅ | ✅ | ✅ | ❌ | ❌ |
| Edit users | - Edit a user's teams  - Edit a user's roles, permissions  - Enable/disable users  - Change membership (guest, member) | ✅ | ✅ | ❌ | ❌ | ❌ |
| View invitations | - View active invitations | ✅ | ✅ | ❌ | ❌ | ❌ |
| Add users | - Add users to teams  - Add users to the organization | ✅ | ✅ | ❌ | ❌ | ❌ |
| Remove users | - Remove users from teams  - Delete users from the organisation | ✅ | ✅ | ❌ | ❌ | ❌ |
| View license requests | - View license requests | ✅ | ✅ | ❌ | ❌ | ❌ |
| Manage license requests | - Approve license requests  - Deny license requests | ✅ | ✅ | ❌ | ❌ | ❌ |
| **Teams** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| View teams | - View all teams in the organization  - View team members  - View team admins  - Perform team-related tasks, such as search for teams, filter, and so on  **Note:** Content, Security, & Team content admins can only view teams where they are member. Company admins can view all teams. | ✅ | ✅ | ❌ | ❌ | ❌ |
| Edit teams | - Update team name  - Update team logo  - Update team admins | ✅ | ✅ | ❌ | ❌ | ❌ |
| **User groups** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| View groups | - View all groups in the organization | ✅ | ❌ | ❌ | ❌ | ❌ |
| Edit groups | - Edit groups in the organization | ✅ | ❌ | ❌ | ❌ | ❌ |
| Assign group | - Assign a user to a group | ✅ | ❌ | ❌ | ❌ | ❌ |
| Remove group | - Remove a user from a group | ✅ | ❌ | ❌ | ❌ | ❌ |
| **Billing groups** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| View billing groups | - View all billing groups in the organization | ✅ | ❌ | ❌ | ❌ | ❌ |
| Edit billing groups | - Edit all billing groups in the organization | ✅ | ❌ | ❌ | ❌ | ❌ |
| Assign billing group | - Assign a user to a billing group | ✅ | ❌ | ❌ | ❌ | ❌ |
| Remove billing group | - Remove a user from a billing group | ✅ | ❌ | ❌ | ❌ | ❌ |
| **Content Management** | | | | | | |
| **Spaces** | | | | | | |
| **Privilege** | **Functions** | **Company Admin*** | **User** **Admin** | **Content Admin**** | **Security Admin** | **Team Content Admin**** |
| Create Spaces | - Create Spaces in the org | **✅** | **✅** | **✅** | **✅** | **✅** |
| Edit Spaces access | - Edit which users can access Spaces | **❌** | **❌** | **✅** | ❌ | **✅** |
| Edit Spaces | - Edit the organization’s space names and location | **❌** | **❌** | **✅** | ❌ | **✅** |
| Delete Spaces | - Delete Spaces in the org | **❌** | **❌** | **✅** | ❌ | **✅** |
| Create boards | - Create boards in private spaces | **❌** | **❌** | **✅** | ❌ | **✅** |
| **Boards** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| View boards | - View all boards (name, description, picture) within the organization | **❌** | **❌** | **✅** | ❌ | **✅** |
| Create boards | - Create boards | **✅** | **✅** | **✅** | **✅** | **✅** |
| Edit board access | - Edit which users can access boards | **❌** | **❌** | **✅** | ❌ | **✅** |
| Edit boards | - Edit all boards in the organization | **❌** | **❌** | **✅** | ❌ | **✅** |
| Edit sharing settings of board | - Update the board's sharing settings | **❌** | **❌** | **✅** | ❌ | **✅** |
| View boards in Trash | - View all boards in trash | **✅** | **❌** | **✅** | ❌ | ❌ |
| Delete boards | - Delete boards and send to Trash | **✅** | **❌** | **✅** | ❌ | **✅** |
| Delete boards from Trash | - Permanently delete boards in trash | **✅** | **❌** | **✅** | ç | ❌ |
| Restore boards from Trash | - Restore boards from trash | **✅** | **❌** | **✅** | ❌ | ❌ |
| Force delete boards under retention | - Delete boards under retention from Trash | **❌** | **❌** | **✅** | ❌ | ❌ |
| **Templates** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin***** |
| View templates | - View all organization templates | ❌ | ❌ | ✅ | ❌ | ✅ |
| Edit templates | - Delete and edit template details (to edit template content, they must share the board with themselves) | ❌ | ❌ | ✅ | ❌ | ✅ |
| Edit template sharing settings | - Edit the organization's sharing settings for templates | ❌ | ❌ | ✅ | ❌ | ✅ |
| **Apps** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| Manage allowed applications | - Manage the organization's application allowlist | ✅ | ❌ | ❌ | ❌ | ❌ |
| Manage application requests | - Approve or reject requests to allow applications in the organization | ✅ | ❌ | ❌ | ❌ | ❌ |
| Manage application settings | - View and update application settings at the organization and team levels. | ✅ | ❌ | ❌ | ❌ | ❌ |
| **Admin Roles** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| View admin roles | - View admin roles  - View *admin roles* privileges  - View a list of users who have admin roles assigned | ✅ | ❌ | ❌ | ❌ | ❌ |
| Assign admin roles | - Assign admin roles to users | ✅ | ❌ | ❌ | ❌ | ❌ |
| Remove admin roles | - Remove admin roles from users | ✅ | ❌ | ❌ | ❌ | ❌ |
| **Security Management** | | | | | | |
| **Audit logs** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| Configure audit logs | - Update the retention period for audit logs | ✅ | ❌ | ❌ | ✅ | ❌ |
| View/export audit logs | - View and export audit logs | ✅ | ❌ | ❌ | ✅ | ❌ |
| **Authentication settings** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| View authentication settings | - View authentication settings and configuration | ✅ | ❌ | ❌ | ✅ | ❌ |
| Edit authentication settings | - Edit authentication settings and configurations, such as adding a new SSO provider | ✅ | ❌ | ❌ | ✅ | ❌ |
| **Collaboration settings** | | | | | | |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| View collaboration settings | - View *invitation* settings (allowlist, who can invite, automatically deactivate guests settings) - View *sharing* settings (board sharing settings, embed) - View *team privacy* settings - View *Allow co-owner* settings - View *Restrict template sharing* settings | ✅ | ❌ | ❌ | ✅ | ❌ |
| Edit collaboration settings | - Edit *invitation* settings (allowlist, who can invite, automatically deactivate guests settings) - Edit *sharing* settings (board sharing settings, embed) - Edit *team privacy* settings - Edit *Allow co-owner* settings - Edit *Restrict template sharing* settings | ✅ | ❌ | ❌ | ✅ | ❌ |
| **Managed domains** | | | | | |  |
| **Privilege** | **Functions** | **Company Admin** | **User** **Admin** | **Content Admin** | **Security Admin** | **Team Content Admin** |
| View managed domains | - View all claimed domains, their status, and configurations - View *block deactivated users* settings | ✅ | ❌ | ❌ | ✅ | ❌ |
| Edit  managed domains | - Add domains - Edit domains - Delete domains - Verify domains - Edit *block deactivated users* settings | ✅ | ❌ | ❌ | ✅ | ❌ |

* Company admins have all Space permissions in Spaces where they are a member. Searching for Spaces only returns Spaces where the Company admin is a member.

** Content admins for the organization and team can create boards only in teams where they are a member. Content admins and Team Content admins can access private Spaces via API if they know the Space ID.

*** Applies only for teams where the user is Team content admin. For organization-level access to all templates, the user must be a Content admin.
