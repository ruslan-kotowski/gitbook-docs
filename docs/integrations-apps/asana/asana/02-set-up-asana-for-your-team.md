---
title: Set up Asana for your team
article_id: 28252196453778
sidebar_position: 2
created_at: '2025-07-22T13:30:20Z'
updated_at: '2026-02-20T09:00:03Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

This section provides comprehensive technical and administrative details, essential for IT and security professionals responsible for the deployment, security, and ongoing management of the Asana integration within their organization.

## Technical overview

The Asana integration is technically implemented through a REST API. For authentication and authorization purposes, the integration leverages the industry-standard OAuth 2.0 protocol. A key component of this architecture is the utilization of a unified API platform as a sub-processor for third-party data. This platform provides unified APIs that are responsible for authenticating, normalizing, and synchronizing data across various API providers.

## Data flows

A thorough understanding of data flow is paramount to manage security and compliance within your organization.

### High-level sequence diagram

Creating an Asana card widget

![image (7).png](images/30596487942930_image%20(7).png)

Updating an Asana card widget

![image (8).png](images/30596482753682_image%20(8).png)

### Asana data in Miro

When users import Asana tasks onto a Miro board, the relevant task data becomes an integral part of the Miro canvas data. Miro stores the following specific data points for imported tasks, provided they are available within Asana:

- Title
- Description
- Assignee (including the user's name and/or email address)
- Status
- Priority

The explicit enumeration of stored data types is crucial for organizational data governance and compliance. It enables administrators to accurately assess precisely what information, particularly any potentially sensitive data, is being replicated into the Miro environment. This transparency ensures alignment with their organization's internal data handling policies. It is also noteworthy that, as per the "Limitations" section, custom fields are not supported and therefore not stored, which is a key detail for data mapping and compliance assessments. Miro employs a hybrid approach to data storage, minimizing data stored directly on the card widget and fetching additional details when the user opens the edit view.

### Data retention of stored information at Miro

All imported Asana data that is stored within Miro adheres strictly to Miro’s standard data retention policy. This policy is applied consistently across all customer data, ensuring a uniform approach to data lifecycle management.

## Authentication and authorization

The Asana integration initiates an authentication flow when a user first interacts with the integration. Authorization within Asana is handled by the integration service. For each individual user, Miro establishes an account with the integration service, and these credentials are subsequently used for all user interactions with the integration.

The integration typically requires approval from an Asana administrator (or a Microsoft Entra administrator, if Asana is managed via Azure AD) to authorize the integration application within their organization's ecosystem. Additionally, individual users must also authorize the Miro Asana integration through Asana's OAuth authorization page when they first attempt to embed an Asana link.

### Required authorization scopes

The authorization scope may vary depending on the specific third-party system. However, for ticketing integrations like Asana, Miro generally requires access to the following data:

| Scope | Description |
| --- | --- |
| Tickets (read and write) | Grants the integration permission to read existing tasks and create or modify tasks within Asana. |
| Users (read) | Grants the integration permission to read user information within Asana, typically for assigning tasks or displaying assignee names. |
| Tags (read) | Grants the integration permission to read tags associated with tasks in Asana. |
| Collections (read) | Grants the integration permission to read collections of tasks or projects within Asana. |

### What is stored in Miro and how

Miro securely stores both authorization-related and unfurling-related data for the Asana integration:

- **Authorization-related data:** This encompasses access tokens and refresh token values, which are stored in Miro's database for a limited duration of several days. These tokens are automatically refreshed upon expiration using the refresh token to ensure continuous access. All such data stored within the database for this integration is encrypted using 256-bit Advanced Encryption Standard, providing a robust layer of data security.
- **Unfurling-related data:** This includes titles of tasks, which are stored as part of the Miro boards themselves. Additionally, titles and encrypted references to these elements are stored in an internal service, further secured through encryption (EKM).

### Revoking a token

If it becomes necessary, administrators or individual users can revoke the tokens granted to the Asana integration. Users can navigate to the integration settings either by opening an integrations task picker, clicking the three dots menu at the top right corner, and selecting **Integration settings**, or by accessing the team’s **Apps** tab in the Miro team settings, finding the specific integration, and clicking on it. On the settings page, authorization can be revoked by clicking the **Disconnect** button. Upon this action, Miro will revoke access to Asana and delete the user’s associated account. For team-level uninstallation, administrators can follow specific steps outlined in the "Troubleshooting & FAQs (Admin)" section.

## How to set up Asana integration

The setup process for the Miro + Asana integration involves distinct steps for both administrators and end-users, ensuring controlled deployment within an organization.

1. **Ensure active accounts:** Before initiating the installation, ensure that both active Miro and Asana accounts are available.
2. **Team-level installation (Admin Action):**
   - Administrators may need to explicitly authorize the Asana integration for their Miro team. Team members can only utilize the integration if it has been installed at the team level.
   - A Miro team administrator can directly install the app by opening a Miro board, selecting **Tools Media & Integrations (+)**, searching for "Asana," and clicking **Connect** to authorize the integration. If a Miro team administrator performs this action, the app will be automatically authorized and installed without requiring further administrative approval.
3. **User request and admin approval flow (if applicable):**
   - In organizations where strict administrative consent is required, a non-admin user on a Miro team configured for Asana integration may paste an Asana link onto a Miro board. This action could trigger an "app install request" dialogue for the user, prompting them to seek administrative approval.
   - The designated administrators can then review and approve this pending request through their Miro or Asana administrative consoles, depending on the specific consent flow configured.
4. **Individual user connection:**
   - After the integration has been successfully installed and authorized at the team level by an administrator, individual users will proceed to click **Connect** on the Asana widget that appears on the Miro board.
   - Users will then be redirected to an Asana authorization page where they grant Miro access to their individual Asana account, thereby confirming their personal authorization to embed and interact with content.

## Security and compliance considerations

### Access restriction to source file

To ensure that access to embedded Asana data remains restricted to the same individuals as in the source Asana file, Miro organization administrators must maintain strict controls over board sharing and content export. While the core Asana integration respects individual permissions for live interaction, any export or static snapshot of board content could potentially expose data to unauthorized individuals if the Miro board itself is not securely managed.

### Error handling

The integration is designed with a graceful UI fallback and error handling in cases where card data updates fail due to third-party rejection.

### Miro data processing addendum (DPA)

For comprehensive legal and compliance details regarding Miro's data processing practices, administrators are directed to consult the [Miro Data Processing Addendum](https://miro.com/legal/customer-data-processing-addendum/).

## Troubleshooting & FAQs

### How can you turn the integration off (team-level uninstallation)?

A Miro team administrator can uninstall the Asana integration at the team level. This action disables the integration for all team members. To do so, navigate to **Team settings Apps & Integrations**. Find "Asana Ticketing" in the list of installed apps, scroll down, and click **Uninstall for team**.

### How can you turn the integration off (individual uninstallation)?

Individual users can uninstall the integration for themselves. Navigate to **Apps & Integrations** in your Miro settings. Locate "Asana Ticketing" and click **Uninstall for me**.

### Which administrators can install the Asana integration for their team?

Only Miro team administrators can directly install the app. If a Miro team administrator pastes an Asana URL onto a Miro board, the app will be automatically authorized and installed without requiring further action.

### What are the availability requirements for the Asana integration?

The Asana integration is available for Miro's Business and Enterprise plans.

### Do administrators need to authorize the Asana integration for their team?

Yes, administrators may need to authorize the Asana integration for their Miro team. Team members can only use the Asana integration if it has been installed at the team level.
