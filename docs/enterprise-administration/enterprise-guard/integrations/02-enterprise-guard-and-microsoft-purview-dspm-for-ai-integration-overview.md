---
title: Enterprise Guard and Microsoft Purview DSPM for AI Integration Overview
article_id: 28617278171154
sidebar_position: 2
created_at: '2025-08-07T15:17:38Z'
updated_at: '2026-01-12T11:27:56Z'
draft: false
---

For organizations using Microsoft Entra ID (formerly Azure AD) as their identity provider, Enterprise Guard securely forwards AI prompts and responses to Microsoft Purview Data Security Posture Management (DSPM) for AI Security and compliance teams can then monitor, audit, and control generative AI use from a single trusted platform, reducing operational overhead, mitigating risks such as data leakage and misuse, and strengthening Miro’s enterprise‑grade AI governance.

:::note
This release supports Miro AI formats, including diagrams, mindmaps, docs, prototypes, sticky notes, and tables, but not images. We’re working to add support for images and more AI features in upcoming releases.
:::

## **Who this is for**

This feature is available for Enterprise Guard customers who manage Miro and Microsoft Entra ID (formerly Azure AD)/Microsoft Purview.

## **What you get**

- **Centralized visibility:** View Miro AI usage in Microsoft Purview’s AI hub.
- **Auditability:** Prompts (user inputs) and responses (AI outputs) are logged for review.
- **Governance alignment:** Use your existing Purview workflows for monitoring, alerting, and retention.

## **Requirements**

### **Miro**

- Enterprise plan with **Enterprise Guard** enabled.
- You are a **Company Admin**.
- Microsoft **Entra ID** configured as an SSO provider in Miro.
- Access to the **Enterprise Integrations** page (if you can’t see it, ask a **Company Admin** to grant access).
- To enable this feature, contact your Customer Success Manager.

### **Microsoft**

- Active **Microsoft Purview** license.
- Your **Microsoft Entra ID tenant ID** (the same tenant used for Miro SSO; the GUID that identifies your Microsoft organization/tenant).
- An Entra role that can **grant tenant‑wide admin consent** to an application.

## **How it works**

1. A Miro admin connects your Microsoft Entra tenant from the **Enterprise Integrations** page in Miro.
2. This installs the **Miro AI governance** application in your Microsoft tenant (via tenant‑wide admin consent).
3. When users sign in to Miro via that tenant and use Miro AI, Miro forwards the prompt/response to Microsoft Purview.
4. Activities appear in the **DSPM for AI → Activity explorer** (Purview view that lists AI activities) in Microsoft Purview (allow ingestion time).

## **Data visibility & latency**

- Logged data: **AI prompts and responses** generated in Miro by users who sign in via SSO for the configured tenant.
- Where to see it: **Microsoft Purview → DSPM for AI → Activity explorer** (the Purview view that lists AI activities). You can also view information in the Audit logs.
:::note
All text‑based prompts and responses across Miro AI features are forwarded to Purview. Currently, image content is not forwarded to Microsoft Purview.
:::
- Latency: Records typically appear **within 10–30 minutes** after the AI action in Miro.

## **Known limitations**

- This release supports Miro AI formats, including diagrams, mindmaps, docs, prototypes, sticky notes, and tables, but not images. We’re working to add support for images and more AI features in upcoming releases.
- You can configure **one Microsoft Entra tenant ID** in Miro at a time.
- In multi‑IdP or multi‑tenant environments, **only** activity from users who sign in to Miro via the **configured tenant** is logged to Microsoft Purview.

## **Security and privacy**

Miro forwards AI prompts and responses to **your Microsoft tenant** so they can be monitored in Purview. **Governance, retention, and access controls** are managed in your Microsoft environment.

##

## **FAQs**

- **Q: Which Miro AI features are logged?**
  **A:** All text‑based prompts and responses across Miro AI features are forwarded to Purview. Currently, image content is not forwarded to Microsoft Purview.
- **Q: Does this cover all users?**
  **A:** Only users who authenticate into Miro using the configured Microsoft Entra tenant are covered.
- **Q: Can I export logs from Miro?**
  **A:** Use Microsoft Purview for export and retention. Miro forwards activity to your Microsoft tenant where it’s governed by your policies.
- **Q: What about security and privacy?**
  **A:** Miro forwards AI prompts and responses to **your Microsoft tenant** so they can be monitored in Purview. **Governance, retention, and access controls** are managed in your Microsoft environment.

## **Support and resources**

- For Entra consent prerequisites, see Microsoft documentation on **granting tenant‑wide admin consent** to an application.
- For Enterprise Guard setup instructions, see [this documentation](../../enterprise-subscription-management/integrations/03-set-up-microsoft-purview-dspm-for-miro-ai.md).
