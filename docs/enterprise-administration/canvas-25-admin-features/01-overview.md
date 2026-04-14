---
title: Overview
article_id: 30969987585938
sidebar_position: 1
created_at: '2025-11-11T12:42:45Z'
updated_at: '2026-01-12T16:04:30Z'
draft: false
---

At Canvas 25, we announced the AI Innovation Workspace with visual AI workflows and collaborative AI agents on the canvas. In addition to the end-user features, we are introducing new admin capabilities to give you more visibility, smarter controls, and seamless ways to unlock Miro’s newest AI tools for your teams.

Use this page to explore AI admin capabilities available to admins on the Enterprise tier. Each section starts with a short overview, followed by expandable FAQs covering different aspects of each capability.

- [Miro AI admin controls:](01-overview.md#miro-ai-admin-controls) decide which AI capabilities are available in your organization and manage who can use them.
- [AI Moderation](#miro-ai-moderation): set org-wide filtering levels (Strict, Default, Minimal) to screen prompts that could lead to harmful or inappropriate output.
- [Admin Analytics](#admin-analytics): use in-product dashboards (Overview and Miro AI) to track adoption and understand organization activity, license allocation, template usage, and Miro AI usage across your organization.

:::note
During the AI Workflows beta, AI Custom Terms of Service and Miro AI granular admin controls were available to AI Workflows customers. With AI Workflows now in General Availability, these capabilities are now available only as part of Enterprise Guard. For more information, see [Advanced AI governance with Enterprise Guard](01-overview.md#advanced-ai-governance-with-enterprise-guard).
:::

## Miro AI admin controls

Miro AI admin controls help you decide which AI capabilities are available in your organization and manage who can use them. For more information, see the [Miro AI admin controls documentation](../managing-enterprise-teams-and-content/01-miro-ai-admin-controls.md).

**Purpose and scope**

**What are Miro AI admin controls?**

Miro AI admin controls let admins manage access to Miro AI capabilities across the organization. Depending on your setup, you can enable access for everyone, restrict access to specific teams, or disable access.

**What’s the difference between an AI capability and an AI feature?**

A **capability** is a category of AI functionality (for example, creating content, working with images, or summarizing activity). A **feature** is a specific action within a capability (for example, c*reate sticky notes* or r*emove background*).

Feature-level controls (managing individual features inside a capability) are available with [Enterprise Guard](01-overview.md#advanced-ai-governance-with-enterprise-guard).

**Access and prerequisites**

**Where do I manage Miro AI admin controls?**

In the Admin Console, go to **Miro AI** > **Capabilities**. From there, you can enable, restrict, or remove access to each AI capability (and, if available, individual AI features).

**Who can configure these settings?**

Company Admins can manage Miro AI access in the Admin Console (AI feature availability depends on your plan and enabled add-ons).

**Access options and behavior**

**What do the access options mean (Everyone, No one, Specific teams)?**

Use the drop-down next to a capability (or feature, if available) to choose how access is granted.

| Option | What it does | When to use it |
| --- | --- | --- |
| **Everyone** | Enables access for all users and teams across your organization (including teams created later). Any team-level restrictions are overridden. | Standard rollout across the org. |
| **No one** | Removes access for everyone. You’ll be asked to confirm removal. | Lock down usage org-wide. |
| **Specific teams** | Enables access only for the teams you select. | Pilot with a subset of teams or phased rollout. |

**What happens if I deactivate a capability?**

When a capability is deactivated, users can no longer access that capability and its associated features on boards. If all Miro AI capabilities are deactivated, **Create with AI** appears disabled on the board.

**Do these settings apply to teams created later?**

If you set a capability (or feature) to **Everyone**, it applies to your organization, including teams created later. If you choose **Specific teams**, you’ll need to update the selection as new teams are created (if you want them included).

**Enterprise Guard and feature-level control**

**How does Enterprise Guard change what I can control?**

With [Enterprise Guard](01-overview.md#advanced-ai-governance-with-enterprise-guard), you can manage access at the **feature level** inside each capability (not just at the category level). This lets you allow some features while restricting others within the same capability.

Example: You can allow c*reate images* and restrict r*emove background* (within the Images capability).

**Visibility and availability**

**Why can’t I see settings for Flows, Sidekicks, or Prototyping?**

Some capabilities (like **Flows**, **Sidekicks**, and **Prototyping**) are visible and manageable only if they’re enabled for your organization.

**Can I see which AI model powers a feature?**

Yes. In Admin Console > **Miro AI** > **Capabilities**, admins can view the models that power each AI feature.

**Can guests or visitors use Miro AI if I enable it?**

Miro AI is available for **Members**. Guests and visitors can’t use Miro AI.

**Troubleshooting and best practices**

**I changed access settings, but users still see Miro AI. What should I check?**

- **Confirm scope:** Make sure you updated the correct capability (or the specific feature, if feature-level controls apply).
- **Check team targeting:** If set to *Specific teams*, confirm the user’s team is selected.
- **Allow time to propagate:** In some cases, changes may take a short time to apply across sessions.
- **Refresh session:** Ask the user to refresh the browser tab, sign out/in, or restart the desktop app (if applicable).

## Miro AI Moderation

With Miro AI moderation, Company Admins can adjust levels of filtering prompts that might contain potentially harmful or inappropriate text. You can set organization-wide Miro AI moderation sensitivity to filter content, including hate, sexual content, violence, and self-harm. This helps you align Miro AI usage with your organization's requirements, policies, and risk tolerance. For more information, see the [Miro AI moderation documentation](../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Purpose and scope**

**What is AI Moderation in Miro?**

AI Moderation lets Company Admins set an org-wide filtering level (Strict, Default, or Minimal) that screens prompts which could lead to harmful or inappropriate output (e.g., hate, sexual content, violence, self-harm).

**Who can configure it and on which plans?**

Company Admins on Enterprise plan with the Miro AI Workflows add-on can configure the setting in org Settings.

**Does it work if my org connects its own LLM (e.g., a direct provider integration)?**

If a custom LLM is connected, the moderation selector may be disabled for that integration and any previously chosen level won’t apply to it.

**Access and prerequisites**

**Who can activate it and what do I need?**

Company Admins on Enterprise plan with the Miro AI Workflows add-on can configure AI Moderation in org settings.

**How do I turn it on?**

Go to Settings → Miro AI → Moderation, choose Strict/Default/Minimal, and then click **Save Changes**. Enforcement is immediate org-wide.

**Levels and behavior**

**What do the levels mean?**

- **Strict:** Blocks Default + low-to-moderate-risk content (e.g., subtle/coded hate, suggestive sexual content, non-graphic violence, non-explicit self-harm mentions).
- **Default (recommended):** Blocks moderately to severely harmful content.
- **Minimal:** Blocks only severely harmful content.

**When do changes take effect?**

Immediately for the entire organization.

**Are changes tracked?**

Yes. Updates are recorded in your organization’s audit trail.

**Setup and configuration**

**Where do I set or update the moderation level?**

Go to Settings → Miro AI → Moderation, choose Strict/Default/Minimal, and then click **Save Changes**.

**What starting level do you recommend?**

Default suits most orgs; adjust based on pilot feedback and risk tolerance.

**Interactions with other controls**

**How does AI Moderation relate to guardrails and prompt controls?**

- **Intelligent Guardrails:** If a board is covered by the “Block Miro AI usage” guardrail, AI is disabled regardless of moderation level.
- **Prompt blocking:** Works alongside Moderation. Prompt blocking stops sensitive prompts at submission; Moderation filters harmful categories.
- **Granular admin controls:** Feature toggles govern who can access AI features when AI is available.

**Troubleshooting and best practices**

**We’re seeing too many false positives.**

Consider moving Strict → Default (or Default → Minimal) and publish acceptable-use examples. If issues persist after you adjust the settings, contact your Miro Customer Success Manager to report this so our product team can review.

**We’re seeing harmful content slip through.**

Move to Default or Strict and provide internal guidance. Revisit after policy/regulatory updates. If issues continue after these changes, contact your Miro Customer Success Manager to report this so our product team can review.

## Admin Analytics

Admin Analytics gives Company Admins data-driven, actionable insights into adoption, usage, and management of Miro at scale. It includes two dashboards: **Overview** and **Miro AI**. For more information, see [Analytics overview](../getting-started/admin-analytics/01-analytics-overview.md), [Overview dashboard](../getting-started/admin-analytics/02-overview-dashboard.md), and [Miro AI dashboard](../getting-started/admin-analytics/03-miro-ai-dashboard.md).

**Purpose and scope**

**What is Admin Analytics?**

Admin Analytics provides trusted, in-product metrics to help you understand how Miro is being used, manage your organization, drive adoption, and support security and compliance needs.

**What dashboards are included?**

Admin Analytics includes two dashboards: **Overview** (organization activity and adoption across boards, users, teams, licenses, and templates) and **Miro AI** (adoption and usage of Miro AI across the organization).

**Dashboards and navigation**

**How do I switch between dashboards?**

Use the tabs at the top of the Analytics page to switch between **Overview** and **Miro AI**.

**How do I change the time range?**

Use the **Time range selector** at the top right of the Analytics page to adjust the time range displayed (**daily**, **weekly**, **monthly**, or **quarterly**).

**When is data refreshed?**

Metrics are refreshed **daily**. Each dashboard shows a **Last updated** timestamp.

**Overview dashboard**

**What can I track in the Overview dashboard?**

The Overview dashboard helps you track adoption and understand organization activity using these metric groups:

- **Boards:** board totals, active boards, and historical trends.
- **Users:** active user trends. You can also track by role, such as members, company admins, guests, or team guests.
- **Teams:** team counts and activity levels.
- **Licenses:** allocated license types and how allocation changes over time.
- **Templates:** which templates are used most across your organization.

**How should I interpret historical charts?**

- In widgets that show historical data, values represent data as of the **last day of each period**.
- The **current ongoing period** is not displayed in historical charts.
- Historical data is available for up to **one year** or as far back as the data exists.

**Miro AI dashboard**

**What can I track in the Miro AI dashboard?**

The Miro AI dashboard helps you track adoption and understand how Miro AI is used across your organization using these metrics:

- **Teams using AI:** teams actively using AI features, including totals of teams using versus not using AI. You can filter usage by use case.
- **People using AI:** adoption totals for people using versus not using AI, with monthly usage history.
- **AI by use case:** usage over time split by **AI creation** and **AI automation**.
- **Sidekick collaborations:** how frequently teams engage with Sidekicks through chat sessions (prompts, follow-up questions, and responses). Analytics displays the number of sessions started.
- **Executed AI flows:** how many times users ran an AI flow with at least two consecutive steps or nodes. Execution is counted at the timestamp of the first event associated with the flow.

**How are AI use cases defined?**

- **AI creation:** actions such as creating from prompts and creating from visual context.
- **AI automation:** actions such as iterating through chat or context menu, text editing, clustering, and removing image backgrounds.

**Is AI Credits usage the same as AI usage metrics?**

No. **AI Credits are not directly correlated** with the AI usage metrics displayed in this dashboard.

**Data considerations**

**Why do I see partial data?**

If a feature was disabled for part of a selected period, you may see partial data in metric history (for example, if a feature was enabled mid-month).

**Why do charts show no data for a time period?**

If no activity was recorded during a given period (day, week, or month), the chart will show no data for that timeframe.

**Older data looks missing. What should I do?**

Historical data is available for up to one year or as far back as the data exists. If older data appears missing, contact Miro Support to request backfill verification.

**Troubleshooting and best practices**

**Our numbers look lower than expected. What should I check?**

- Confirm the **time range** and period type (daily, weekly, monthly, quarterly).
- Remember that **historical charts show completed periods**, not the current ongoing period.
- If a capability was turned on mid-period, expect **partial data** for that timeframe.

**How do I use these insights effectively?**

Use Overview metrics to spot underused teams, templates, or license trends, then run targeted enablement. Use Miro AI metrics to identify where AI adoption is growing, support champions, and guide responsible rollout.

## Advanced AI governance with Enterprise Guard

Enterprise Guard provides additional advanced AI governance capabilities for Enterprise admins. Use these controls to fine-tune access, protect sensitive information, and strengthen monitoring and compliance for AI usage in Miro. For more information, see [Enterprise Guard AI Trust capabilities and FAQs](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md).

- [Miro AI granular admin controls](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md#miro-ai-granular-admin-controls-for-enterprise-guard-add-on): set feature-level access (Everyone/No one/Specific teams) within each capability category.
- [Block Miro AI usage with Intelligent Guardrails](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md#block-miro-ai-usage-with-intelligent-guardrails): use Intelligent Guardrails to block all AI-powered interactions in Miro when you need to protect sensitive or classified data.
- [Prompt blocking](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md#prompt-blocking): block prompts containing sensitive data or source code at the moment of submission; show a policy message instead of sending to an LLM.
- [Enterprise Guard and Microsoft Purview DSPM for AI integration](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md#enterprise-guard-and-microsoft-purview-dspm-for-ai-integration): forward prompts and responses to Purview for centralized monitoring, audit, and governance.
