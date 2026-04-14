---
title: Working with custom admin roles
article_id: 22182074695698
sidebar_position: 3
created_at: '2024-10-24T13:17:04Z'
updated_at: '2025-04-25T13:57:02Z'
draft: false
---

Company admins and admins with the necessary privileges can now create and manage custom roles tailored to specific organizational needs. This functionality enhances control over user management, security, and content lifecycle by offering customizable privileges. Admins can efficiently assign, update, or remove custom admin roles as required, ensuring alignment with organizational workflows. Key benefits of custom admin roles include:

- **Flexibility:** Tailor custom admin roles to fit diverse administrative needs.
- **Scalability:** Adapt as your organization grows and requirements evolve.
- **Enhanced security:** Assign precise privileges to maintain data integrity and compliance.
- **Ease of use:** Intuitive interface for creating and managing roles.

## Create custom admin role

:::note
To create a custom admin role, you must be a company admin or a custom admin that has view, edit, and assign admin role privileges.
:::

1. Go to your [Admin console](https://miro.com/app/settings).
2. On the left pane, under **Users**, click **Admin roles**.
3. On the top-right of the **Admin roles** page, click **Create role**.
4. On the **Enter Details** page:
   a. In the **Role name** box, enter a unique, descriptive name for the new custom admin role that you are creating. The role name can have a maximum of 60 characters. The role name must be unique across all custom role names in an organization.
   b. In the **Role description** box, enter a description that helps other admins understand this custom admin role. The role description can have a maximum of 120 characters.
   c. Click **Next**.
5. On the **Set privileges** page:
   a. Select the checkbox for each privilege you want to enable for this custom role. If you want to select all privileges under a specific privilege category, click **Select all**.
   b. Click **Next**.
6. On the **Assign users** page:
   a. Select the checkbox beside each user for whom you want to enable this custom role. You can also use the search bar to search the list by name, email, or domain.
   b. Click **Next**.
7. On the **Review** page:
   a. Review all the information for this custom role to ensure correctness of the custom role details, privileges, and users.
   b. If the custom role details are correct, click **Create role**.
   If you need to make updates after reviewing the custom role details, click the **Previous** button, make the updates needed, and then review the custom role details once again.

   After the custom role is created, the custom role appears in the list of Admin roles and is marked with a CUSTOM tag.

:::note
If a user loses the ORGANIZATION_INTERNAL_USER or ORGANIZATION_INTERNAL_ADMIN membership role in the organization, the user also loses all associated custom or predefined roles.
:::
