---
title: Set up Microsoft Purview DSPM for Miro AI
article_id: 28698434922386
sidebar_position: 3
created_at: '2025-08-11T19:20:50Z'
updated_at: '2026-01-12T11:28:20Z'
draft: false
---

Use this procedure to set up Microsoft Purview Data Security Posture Management (DSPM) for Miro AI so AI prompts and responses from Miro appear in Microsoft Purview’s DSPM for AI. After setup, you’ll validate events and learn how to manage the integration.

## **Prerequisites**

### **Miro**

- Enterprise plan with **Enterprise Guard** enabled.
- You are a **Company Admin**.
- **Microsoft Entra ID** is configured as an **SSO provider** in Miro.
- To enable this feature, contact your Customer Success Manager.

### **Microsoft**

- Active Microsoft Purview license with support for DSPM for AI.
- Microsoft Entra ID tenant ID used for Miro SSO (the GUID that identifies your Microsoft organization/tenant).
- An Entra role that can grant tenant‑wide admin consent to an application.

## **Set up the integration in Miro**

1. In Miro, open **Enterprise settings → Enterprise integrations**.
2. Scroll down and then click to toggle on **Microsoft Purview DSPM for AI.**
3. In the Tenant ID box, enter your **Microsoft Entra tenant ID**.
4. Click **Connect**.
5. When prompted, sign in to Microsoft Entra with an account that can grant **tenant‑wide admin consent**.
6. Review the consent for the **Miro AI governance** application and click **Accept**.
7. Return to Miro and confirm the integration shows **Connected.**

## **Validate activity in Microsoft Purview**

1. In Miro, perform a simple AI action (for example, **summarize** sticky notes on a board).
2. Wait **up to 10–30 minutes** for ingestion.
3. In Microsoft Purview, go to **Microsoft Purview → DSPM for AI → Activity explorer** (the Purview view that lists AI activities). You can also view information in the Audit logs.
   Note: All text‑based prompts and responses across Miro AI features are forwarded to Purview. Currently, image content is not forwarded to Microsoft Purview.
4. Filter for **Recent** events and locate activity from Miro (for example, prompt and response).

## **Manage the integration**

- **Disconnect**: In Miro, go to **Enterprise integrations → Microsoft Purview for AI → Disconnect**.
- **Change tenant**: **Disconnect** first, then **Connect** again using a different **tenant ID**.

## **Troubleshooting**

- **Integration option missing**: Ensure your org has **Enterprise Guard** and your account can access **Enterprise integrations**. Ask a **Company Admin** to grant access.
- **Tenant ID mismatch or connect error**: The tenant ID must **exactly match** the Microsoft Entra tenant used for Miro **SSO**.
- **Consent failed or sign‑in loop**: Sign in with an account that can grant **tenant‑wide admin consent** (work with your Microsoft admin).
- **No activity visible**: Confirm a test AI action was performed by a user who signs in to Miro via the **configured tenant**; allow **10–30 minutes**; verify your **Purview license**; and check **DSPM for AI → Activity explorer**.
- **Multiple tenants/IdPs**: Only **one tenant** can be configured in Miro. Activity from users who sign in via SSO for other tenants/IdPs is **not** forwarded.

## **Known limitations**

For more information, see the [known limitations section in the overview documentation](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md#known-limitations).
