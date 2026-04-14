---
title: Set up Linear for your team
article_id: 30630697364626
sidebar_position: 2
created_at: '2025-10-29T14:09:41Z'
updated_at: '2026-02-23T11:23:44Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

The Linear integration is technically implemented through a REST API. For authentication and authorization purposes, it leverages the industry-standard OAuth 2.0 protocol. A core component of this architecture is a unified API platform used as a sub-processor for third-party data—managing authentication, normalization, and synchronization across different API providers.

## Data flows

Understanding data flow is crucial to manage security and compliance.

### High-level sequence diagram

Creating a Linear card widget

![Asana Cards (BETA) (1).jpg](images/30630873068946_Asana%20Cards%20(BETA) (1).jpg)

Updating a Linear card widget

![Asana Cards (BETA) (1).jpg](images/30630873068946_Asana%20Cards%20(BETA) (1).jpg)

### Linear data in Miro

When users import Linear issues onto a Miro board, the following data is integral to the Miro canvas:

- Title
- Description
- Assignee (name/email)
- Status
- Priority

This enumeration is vital for data governance, confirming what sensitive data enters the Miro environment. Note that custom fields are unsupported.

### Data retention

All imported Linear data adheres strictly to Miro's standard data retention policy, consistently applied across all customer data.

## Authentication and authorization

Upon first interaction, Linear integration initiates an authentication flow. For each user, Miro creates credentials with the integration service for subsequent interactions.

The integration typically requires approval from a Linear administrator.

### Required authorization scopes

| Scope | Description |
| --- | --- |
| Collections | Access collections of issues. |
| Users | Read user information for assignment/display. |
| Issues | Read, create, modify issues in Linear. |

## What is stored in Miro and how

- **Authorization-related data:** Tokens are stored in Miro's database for several days, encrypted with AES-256.
- **Unfurling-related data:** Issue titles are stored with encrypted references.

### Revoking a token

Revocation of tokens can occur via **Integration settings** or **Apps** tabs by selecting **Disconnect**. This action removes access to Linear and erases user credentials.

## How to set up Linear integration

Steps for both administrators and end-users ensure controlled deployment.

1. **Ensure Active Accounts:** Miro and Linear accounts must be active.
2. **Team-Level Installation (Admin Action):**
   - Administrators must authorize the Linear integration at the team level.
   - Installation via **Tools Media & Integrations**, searching for "Linear" and connecting.
3. **User Request and Admin Approval:**
   - In stringent consent organizations, pasting a Linear link can trigger a request for admin approval.
   - Admins can approve via Miro or Linear consoles.
4. **Individual User Connection:**
   - Users connect through the Linear widget and OAuth authorization.

## Security and compliance

### Access Restriction to Source File

Maintaining strict board sharing controls aligns Linear permissions with Miro.

### Error handling

The integration features a graceful UI fallback for third-party rejections.

### Miro data processing addendum (DPA)

Consult [Miro's Data Processing Addendum](https://miro.com/legal/customer-data-processing-addendum/) for detailed legal and compliance information.

## Troubleshooting & FAQs

### How to turn off integration (Team-level)

Administrators can uninstall from **Team settings Apps & Integrations** by selecting "Linear" and clicking **Uninstall for team**.

### How to turn off integration (Individual)

Users can navigate to **Apps & Integrations** and select "Uninstall for me" for Linear.

### Administrator permissions

Only Miro team administrators can directly install the app. Automatic setups occur when pasting a Linear URL on a board.

### Availability requirements

The Linear integration is available for Business and Enterprise plans.

### Administrator authorization requirement

Yes, team-level authorization by administrators is necessary for team access.
