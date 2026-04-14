---
title: Set up Microsoft and Power BI integrations
article_id: 25132703621394
sidebar_position: 3
created_at: '2025-03-06T10:27:14Z'
updated_at: '2025-11-25T15:49:57Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
---

:::note
For comprehensive admin docs specifically on the Miro integration with Microsoft or Power BI, including detailed diagrams and further FAQs, please refer to [Microsoft admin documentation](https://docs.google.com/document/d/1Gw94z5Pc-elS-pRXKGZVBWKKNEIFR9y9yzAAkbXKwMM/edit?usp=sharing) or [Power BI admin documentation](https://docs.google.com/document/d/1hMepF163jQF8LI-U8ES8DzHVMW4TltXDr14fJ2KU29k/edit?tab=t.0#heading=h.gu9ng058yy7y).
:::

This article explains how to set up a Microsoft or Power BI integration with Miro.

## Set up a Microsoft or Power BI integration

To set up a Microsoft or Power BI integration, you must enable users to authorize their own Microsoft or Power BI content in Miro.

### Prerequisites

- Ensure that you have admin access to Microsoft Entra.
- A Company admin has approved Microsoft or Power BI for your Miro organization (this refers to Miro-side app approval policies if your organization restricts app installations).

### Procedure

These steps focus on configuring Microsoft Entra to allow the Miro integration.

1. Log in to **Entra** as admin.
2. Go to **Enterprise applications** > **Consent and permissions**.
3. For **Users can request admin consent to apps they are unable to consent to**, select **Yes**.
4. Under **Who can review admin consent requests**, choose the necessary users, roles, or groups that you want to allow to review admin-consent requests for applications.

:::note
The Entra administrators designated in Step 4 above can then go to **Enterprise applications > Admin consent requests** in Microsoft Entra to review and approve the "Contenthub PowerBI Integratio" (or a similarly named) application for the organization.
:::

## Validate your Microsoft or PowerBI integration

Copy and paste a link to your Miro board.

If the app is pre-approved by your Company admin, then follow the modal instructions on-screen. Miro adds your app content to the board as an iFrame.

If the app is not pre-approved, then the **Add & allow** modal opens and enables you to send a request to your Company admin. Send your request.

When your Company admin responds, you will receive a notification.

**More information:** See [App management](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).
