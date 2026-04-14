---
title: Set up Miro Connectors for Okta Workflows
article_id: 8166481458706
sidebar_position: 3
created_at: '2022-10-19T06:52:05Z'
updated_at: '2025-02-26T11:59:06Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: enterprise
---

Miro Connectors for Okta Workflows allow you to easily automate repetitive and multistep Admin tasks in Miro. Learn how to set up workflow automation and simplify team and user management.

## Miro User Management Connector

Miro User Management Connector allows Miro enterprise customers with SCIM enabled to add users to their organization and manage users’ licenses and statuses.

**Authorize your Miro User Management Connector:**

When you add a Miro User Management card to a flow for the first time, you’ll be prompted to set up a connection for your organization. See Authorization.

**Miro User Management Connector action cards:**

|  |  |
| --- | --- |
| **Action** | **Description** |
| Create User | Creates a new user. |
| Read User | Search an existing user in an organization by Email. |
| Upgrade User License Type to Full | Updates an existing user resource, changing its User License Type to **Full**. |
| Update User Status | Updates an existing user resource, changing its active status to a value of either true or false.The Miro User Management connector works using your SCIM token. Miro User Management is only available for enterprises with SSO and SCIM enabled. |

## Authorization

You can create and manage multiple connections from the **Connections** page.
This is useful if you plan to operate with multiple organizations. Each connection for the Miro User Management Connector can point to only one Miro Organization.

To enable SCIM and obtain a new token, or to copy an existing token, follow the instructions in [How to enable SCIM](https://developers.miro.com/docs/how-to-enable-scim).
To create a new connection from an Action card:

1. Click **New Connection**.
2. Enter a **Connection Nickname**. We recommend a name that represents the organization.
3. Enable SCIM provisioning from Miro’s Enterprise integration page, following the [instructions](https://developers.miro.com/docs/how-to-enable-scim).
   1. Copy **Base URL** from Miro and paste it into **Base URL** field in the Connection
   2. Copy **Api Token** from Miro and paste it into **Access Token**field in Connection
4. Click **Create**. This saves your connection and takes you back to your flow.

### Create user

Creates a user within the organization.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **User Details** |  |  |  |
| Email | The email address of the user. | String | TRUE |
| Active | The status of the user.   - **True**: the user is active. - **False**: the user is inactive.    When not specified, it defaults to **false**. | Dropdown | FALSE |
| User License Type | The license type of the user.   - **Full** - **Free**    When not specified, the user license is set according to internal Miro logic, which depends on the organization's plan. | Dropdown | FALSE |
| Role | The role of the user within the organization.   - **Organization Member**: regular member without admin privileges. - **Organization Admin**: user with company-wide admin privileges.    When not specified, it defaults to **Organization   Member**. | Dropdown | FALSE |
| **Name** |  |  |  |
| Family Name | The family name or surname of the user. | String | FALSE |
| Given Name | The given name of the user. | String | FALSE |
| Display Name | The name to be displayed in Miro. | String | FALSE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **User** |  |  |
| User ID | The ID of the new user. | String |

### Read User

Search an existing user in an organization by Email

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Query** |  |  |  |
| Email | The email address of the user to search for | String | TRUE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **User** |  |  |
| User ID | The ID of the user. | Number |
| User License Type | The license type of the user. | Number |
| Active | The status of the user.  - **True**: the user is active. - **False**: the user is inactive. | Number |
| **Name** |  |  |
| Username | The email address of the user. | Number |
| Family Name | The family name or surname of the user. | Number |
| Given Name | The given name of the user. | Number |
| Display Name | The name displayed in Miro. | Number |

### Upgrade user license type to Full

Updates an existing user resource, changing its user type (license) to **Full**.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **User** |  |  |  |
| User ID | The ID of the user. | String | TRUE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Response** |  |  |
| Status Code | HTTP status of the request.  Codes indicating successful license update:   - **200**: OK    Codes indicating unsuccessful license update:   - **400**: Malformed request - **401**: Unauthorized - **403**: Forbidden - **404**: Not found - **409**: Conflict - **429**: Too many requests | Number |

### Update user status

Updates an existing user resource, changing its **active status** to a value of either true or false.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **User** |  |  |  |
| User ID | The ID of the user. | String | TRUE |
| Active | The new status of the user.  - **True**: the user is active. - **False**: the user is inactive. | Dropdown | TRUE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Response** |  |  |
| Status Code | HTTP status of the request.  Codes indicating successful active status update:   - **200:** OK    Codes indicating unsuccessful active status update:   - **400**: Malformed request - **401**: Unauthorized - **403**: Forbidden - **404**: Not found - **409**: Conflict - **429**: Too many requests | Number |

## Miro Administration Connector

Miro Administration Connector allows enterprise customers to create teams, and manage their team settings and members of the teams.

**Authorize your Miro Administration Connector**:

When you add a Miro card to a flow for the first time, you’ll be prompted to set up a connection for your organization. See [Authorization](#authorization).

**Miro Administration Connector** **action cards**:

|  |  |
| --- | --- |
| **Action** | **Description** |
| Create Team | Creates a new team in an existing organization. |
| Search Teams | Search existing teams in an organization. The first 10 matching records are selected from the Result Set.. |
| Add Member to Team | Adds a new member to an existing team. |
| Update Team Member Role | Updates a team member role in an existing team. |
| Get Team Settings | Retrieves the team settings of an existing team. |
| Update Team Sharing Policies   Settings | Updates the settings for the sharing policy of an existing   team. |
| Update Team Invitation Settings | Updates the settings for the invitation policy of an   existing team. |
| Update Team Collaboration Settings | Updates the settings for the collaboration policy of an   existing team. |
| Update Team Discovery Settings | Updates the settings for the discovery policy of an   existing team. |
| Update Team Copy Access Settings | Updates the settings for the copy access policy of an   existing team. |
| User Session Wipeout (BETA) | Wipes all user sessions for a given email address. |

## Authorization

The Miro Administration Connector works using OAuth API Token. Miro Administration Connector is only available for customers on the Enterprises plan. To create a new connection, users must have the necessary permissions to install apps with the supported scopes below.

You can create and manage multiple connections from the **Connections** page.
This is useful if you plan to operate with multiple organizations. Each connection for the Miro Administration Connector can point to only one Miro Organization.

To create a new connection from an Action card:

1. Click **New Connection**.
2. Enter a **Connection Nickname**. We recommend a name that represents the organization.
3. Get **Organization ID** and **Access Token** from the Miro’s Enterprise integration page, following the [instructions](../../enterprise-subscription-management/enterprise-workflow-automation/02-miro-connector-for-okta-workflows.md).
4. Click **Create**. This saves your connection and takes you back to your flow.

Supported scopes:

- organizations:teams:write
- organizations:teams:read

### Create team

Creates a team in an existing organization.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Team** |  |  |  |
| Team Name | The name of the team. | String | TRUE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Response** |  |  |
| Team ID | The ID of the new team. | String |

### Search Teams

Search existing teams in an organization. The first 10 matching records are selected from the Result Set.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Query** |  |  |  |
| Team Name | Words to be matched with team name. Any team whose name contains those exact words to be returned as a resultset. Teams with names that are a full match to the query will be on top of the result. | String | FALSE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Response** |  |  |
| **Teams** | List with 10 first teams found. Each team has the fields below. | List |
| Team ID | The ID of the team | String |
| Name | Name of the team | String |

### Add member to team

Adds a new member to an existing team.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Team** |  |  |  |
| Team ID | The ID of the team. | String | TRUE |
| **Member** |  |  |  |
| User Email | The email of the user that you want to add to the team. | String | TRUE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Response** |  |  |
| Member ID | The ID of the new team member. | String |

### Update team member role

Updates a team member's role in an existing team.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Team** |  |  |  |
| Team ID | The ID of the team. | String | TRUE |
| **Member** |  |  |  |
| Member ID | The ID of the team member. | String | TRUE |
| Role | The new role of the member within the team.  - **Member**: regular member. - **Admin**: member with admin privileges within the team. - **Team Guest**: guest with limited privileges. | Dropdown | TRUE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Response** |  |  |
| Member ID | The ID of the team member. | String |
| Role | The new role assigned to the team member.  - **member**: regular member. - **admin**: member with admin privileges within the team. - **team_guest**: guest with limited privileges. | String |

### Get Team settings

Retrieves the team settings of an existing team.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Team** |  |  |  |
| Team ID | The ID of the team. | String | TRUE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Team Invitation   Settings** |  |  |
| Who can Invite | - **only_org_admins**: only company admins can invite collaborators. - **admins**: company admins and team admins can invite collaborators. - **all_members**: all team members can invite collaborators. | String |
| Invite External Users | - **allowed**: allow collaborators who are not members of the team. - **Not_allowed**: don't allow collaborators who are not members of the team. | String |
| **Team Collaboration   Settings** |  |  |
| Co-Owner Role | - **enabled**: enable the Co-owner role on boards and projects. - **disabled**: disable the Co-owner role on boards and projects. | String |
| **Team Copy Access   Level Settings** |  |  |
| Copy Access Level | - **anyone**: anyone with access to the board can copy existing board content to newly created boards. WARNING: this option is available only if **Copy Access Level Limitation** is set to **anyone**. - **team_members**: team members can copy existing board content to newly created boards. - **team_editors**: team members with edit rights can copy existing board content to newly created boards. - **board_owner**: only board owners can copy existing board content to newly created boards. | String |
| Copy Access Level   Limitation | - **anyone**: team members and users outside the team can be granted permission to copy board content. - **team_members**: only team members can be granted permission to copy board content. | String |
| **Team Discovery   Settings** |  |  |
| Discovery | - **hidden**: only invited users can see and access the team. - **request**: members of the organization can find the team, and request to join the team with admin approval. - **join**: members of the organization can find and join the team. | String |
| **Team Sharing Policy Settings** |  |  |
| Default Board Access | - **private**: only board owners can access boards. - **view**: anyone in the team can view boards. - **comment**: anyone in the team can add comments to boards. - **edit**: anyone in the team can edit boards. | String |
| Default Organization   Access | - **private**: only board owners can access boards. - **view**: anyone in the organization can view boards. - **comment**: anyone in the organization can add comments to boards. - **edit**: anyone in the organization can edit boards. | String |
| Sharing on   Organization | - - **allowed**: allow sharing at organization level. - **allowed_with_editing**: allow sharing with edit rights at organization level. - **not_allowed**: don't allow sharing at organization level. | String |
| Sharing on Team | - - **allowed**: allow sharing at team level. - **allowed_with_editing**: allow sharing with edit rights at team level. - **not_allowed**: don't allow sharing at team level. | String |
| Sharing via Public   Link | - **allowed****:allow sharing via public link.** - **allowed_with_editing**:allow sharing with edit rights via public link. - **not_allowed**:don't allow sharing via public link. | String |
| Move Board to Team | - **allowed**: allow moving boards to a different team. - **not_allowed**: don't allow moving boards to a different team. | String |

### Update Team Sharing Policy settings

Updates the settings for the sharing policy of an existing team.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Team** |  |  |  |
| Team ID | The ID of the team. | String | TRUE |
| Default Board   Access | - **Private**: only board owners can access boards. - **View**: anyone in the team can view boards. - **Comment**: anyone in the team can add  comments to boards. - **Edit**: anyone in the team can edit boards. | Dropdown | FALSE |
| Default   Organization Access | - **Private**: anly board owners can access boards. - **View**: anyone in the team can view boards. - **Comment**: anyone in the team can add  comments to boards. - **Edit**: anyone in the team can edit boards. | Dropdown | FALSE |
| Sharing via Public   Link | - **Allowed**: allow sharing via public link. - **Allowed With Editing**: allow sharing with edit rights via public link. - **Not Allowed**: not allow sharing via public link. | Dropdown | FALSE |
| Sharing on Team | - **Allowed**: allow sharing at team level. - **Allowed With Editing**: allow sharing with edit rights at team level. - **Not Allowed**: don't allow sharing at team level. | Dropdown | FALSE |
| Sharing on   Organization | - **Allowed**: allow sharing at organization level. - **Allowed With Editing**: allow sharing with edit rights at organization level. - **Not Allowed**: don't allow sharing at organization level. | Dropdown | FALSE |
| Move Board to Team | - **Allowed** allow moving boards to a different team. - **Not Allowed** don't allow moving boards to a different team. | Dropdown | FALSE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Team Sharing Policy Settings** |  |  |
| Default Board Access | - **private**: only board owners can access boards. - **view**: anyone in the team can view boards. - **comment**: anyone in the team can add comments to boards. - **edit**: anyone in the team can edit boards. | String |
| Default Organization Access | - **private**: only board owners can access boards. - **view**: anyone in the organization can view boards. - **comment**: anyone in the organization can add comments to boards. - **edit**: anyone in the organization can edit boards. | String |
| Sharing on   Organization | - - **allowed**: allow sharing at organization level. - **allowed_with_editing**: allow sharing with edit rights at organization level. - **not_allowed**: don't allow sharing at organization level. | String |
| Sharing on Team | - - **allowed**: allow sharing at team level. - **allowed_with_editing**: allow sharing with edit right at team level. - **not_allowed**: don't allow sharing at team level. | String |
| Sharing via Public   Link | - - **allowed**:allow sharing via public link. - **allowed_with_editing**:allow sharing with edit rights via public link. - **not_allowed**:don't allow sharing via public link. | String |
| Move Board to Team | - **allowed**: allow moving boards to a different team. - **not_allowed**: don't allow moving boards to a different team. | String |

### Update Team Invitation settings

Updates the settings for the invitation policy of an existing team.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Team** |  |  |  |
| Team ID | The ID of the team. | String | TRUE |
| Invite External   Users | - **Allowed**: allow collaborators who are not members of the team. - **Not Allowed** don't allow collaborators who are not members of the team. | Dropdown | FALSE |
| Who can Invite | - **Only Organization Admins**: only company admins can invite collaborators. - **Admins**: company admins and team admins can invite collaborators. - **All Members**: all team members can invite collaborators. | Dropdown | FALSE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Team Invitation settings** |  |  |
| Invite External   Users | - **allowed**: allow collaborators who are not members of the team. - **Not_allowed**: don't allow collaborators who are not members of the  team. | String |
| Who can Invite | - **only_org_admins**: only company admins can invite collaborators. - **admins**: company admins and team admins can invite collaborators. - **all_members**: all team members can invite collaborators. | String |

### Update Team copy access settings

Updates the settings for the copy access policy of an existing team.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Team** |  |  |  |
| Team ID | The ID of the team. | String | TRUE |
| Copy Access   Level | - **anyone**: anyone with access to the board can copy existing board content to newly created boards. - **Team Members**: team members can copy existing board content to newly created boards. - **Team Editors**: team members with edit rights can copy existing board content to newly created boards. - **board_owner**: only board owners can copy existing board content to newly created boards. | Dropdown | FALSE |
| Copy Access   Level Limitation | - **Anyone**: team members and users outside the team can be granted permission to copy board content. - **Team Members**: only team members can be granted permission to copy board content. | Dropdown | FALSE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Team copy access settings** |  |  |
| Copy Access Level | - **anyone**: anyone with access to the board can copy existing board content to newly created boards. - **team_members**: team members can copy existing board content to newly created boards. - **team_editors**: team members with edit rights can copy existing board content to newly created boards. - **board_owner**: only board owners only can copy existing board content to newly created boards. | String |
| Copy Access Level Limitation | - **anyone**: team members and users outside the team can be granted permission to copy board content. - **team_members**: only team members can be granted permission to copy board content. | String |

### Update Team Collaboration settings

Updates the settings for the collaboration policy of an existing team.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Team** |  |  |  |
| Team ID | The ID of the team. | String | TRUE |
| Co-Owner   Role | - **Enabled**: enable the Co-owner role on boards and projects. - **Disabled**: disable the Co-owner role on boards and projects. | Dropdown | FALSE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Team Collaboration settings** |  |  |
| Co-Owner Role | - **enabled**: enable the Co-owner role on boards and projects. - **disabled**: disable the Co-owner role on boards and projects. | String |

### Update Team Discovery settings

Updates the settings for the discovery policy of an existing team.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **Team** |  |  |  |
| Team ID | The ID of the team. | String | TRUE |
| Discovery | - **Hidden**: only invited users can see and access the team. - **Request**: members of the organization can find and request to join the team with admin approval. - **Join**: members of the organization can find and join the team. | Dropdown | FALSE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Team Discovery settings** |  |  |
| Discovery | - **hidden**: only invited users can see and access the team. - **request**: members of the organization can find and request to join the team with admin approval. - **join**: members of the organization can find and join the team. | String |

### User Session Wipeout

Wipes all user sessions for a given email address.

Input

|  |  |  |  |
| --- | --- | --- | --- |
| **Field** | **Definition** | **Type** | **Required** |
| **User Details** |  |  |  |
| Email | The email address of the user whose sessions are to be wiped. | String | TRUE |

Output

|  |  |  |
| --- | --- | --- |
| **Field** | **Definition** | **Type** |
| **Response** |  |  |
| Status Code | HTTP status of the request.  Codes indicating successful user session wipeout update:   - **200:** User session deleted    Codes indicating unsuccessful user session wipeout update:   - **400**: Malformed request - **401**: Unauthorized - **403**: Forbidden - **404**: Not found - **409**: Conflict - **429**: Too many requests | Number |
