---
title: AI Trust Capabilities and FAQ
article_id: 30943405198994
sidebar_position: 2
created_at: '2025-11-10T14:17:30Z'
updated_at: '2026-03-17T08:39:20Z'
draft: false
---

At Canvas 25, we announced the AI Innovation Workspace with visual AI workflows and collaborative AI agents on the canvas. In addition to the end-user features, we are introducing new admin capabilities to give you more visibility, smarter controls, and seamless ways to unlock Miro’s newest AI tools for your teams.

Use this page to explore AI Trust capabilities available with the Enterprise Guard add-on. Each section starts with a short overview, followed by expandable FAQ covering different aspects of each capability.

- [Miro AI granular admin controls](#miro-ai-granular-admin-controls-for-enterprise-guard-add-on): set feature-level access (Everyone/No one/Specific teams) within each capability category.
- [Block Miro AI usage with Intelligent Guardrails](#block-miro-ai-usage-with-intelligent-guardrails): use Intelligent Guardrails to block all AI-powered interactions in Miro when you need to protect sensitive or classified data.
- [Admin Analytics Overview dashboard](#admin-analytics-overview-dashboard): track boards, users, teams, licenses, and templates with historical trends and daily refresh.
- [AI Moderation (also available on Enterpise tier)](#miro-ai-moderation): set org-wide filtering levels (Strict, Default, Minimal) to screen prompts that could lead to harmful or inappropriate output.
- [Prompt blocking](#prompt-blocking): block prompts containing sensitive data or source code at the moment of submission; show a policy message instead of sending to an LLM.
- [Enterprise Guard and Microsoft Purview DSPM for AI integration](#enterprise-guard-and-microsoft-purview-dspm-for-ai-integration): forward prompts and responses to Purview for centralized monitoring, audit, and governance.

## Miro AI granular admin controls for Enterprise Guard add-on

Miro AI admin controls enable Enterprise Company Admins to decide which AI capabilities are available in their organization and manage who can use them. Admins can also view the models that power each AI feature. With the Enterprise Guard add-on, Miro AI controls extend to the feature level within each capability category, which helps prioritize features based on organizational needs and security requirements. In addition to the complete Miro AI capability category, Admins can also enable, restrict, or remove specific Miro AI features. For example, within the Images category, you can enable Create images with AI and disable Remove background. Use these controls to roll out AI safely and meet security requirements while driving adoption of AI capabilities.  For more information, see the [Miro AI granular admin controls documentation](../ai-trust/02-miro-ai-granular-admin-controls.md).

**Purpose and scope**

**What is granular control for Miro AI?**

With the Enterprise Guard add-on, Company Admins can enable, restrict, or remove access to individual AI features inside each capability category. This lets you choose exactly which features teams can use.

**Why use granular controls?**

To balance adoption with security. For example, within Images you can allow Create images while disabling Remove background.

**Access and prerequisites**

**Who can configure granular controls and on which plans?**

Company Admins on Enterprise plans with the Enterprise Guard add-on, in the browser.

**Where do I manage feature-level access?**

Admin Console → Miro AI → Capabilities. Expand a capability to see and set access for its individual features.

**Controls and behavior**

**Granular controls: what is the difference between capability-level and feature-level control, and what happens when I turn them on or off?**

- **Capability level:** Everyone, No one, or Specific teams applies to the entire category. If you deactivate a capability, users lose access to that capability and all of its features across boards. If you deactivate all capabilities, Create with AI appears disabled on the board.
- **Feature level:** With Enterprise Guard, you can set Everyone, No one, or Specific teams per individual feature. Deactivating a feature removes access to that feature only; other features in the same capability remain available if enabled.

**What access options exist at the feature level?**

For each feature, choose Everyone, No one, or Specific teams. Everyone enables the feature org-wide and overrides team-level restrictions. No one removes access for all users. Specific teams targets selected teams only.

**What happens when I deactivate an individual feature?**

Users cannot access that feature on any board, but other features in the same capability remain available if enabled.

**Reference and examples**

**Which features can I control individually?**

See the in-product reference for the current list. Examples under Create content include Create sticky notes, Cluster sticky notes, Create and edit docs, tables, diagrams, and text operations like rewrite, shorten, tone, and translate. Images includes Create images, Remove background, and Add captions. Summarize activity includes Catch up and Conversation summary. Flows, Sidekicks, and Prototyping appear if enabled for your org.

**Can I see which models power specific features?**

Yes. Admins can view the models associated with each AI feature in the reference area to support review and governance.

## Block Miro AI usage with Intelligent Guardrails

Use Intelligent Guardrails to block all AI-powered interactions in Miro when you need to protect sensitive or classified data. When this guardrail applies, all Miro AI tools are disabled across affected boards while collaboration without AI remains available. For background and setup, see the Intelligent Guardrails overview and Define guardrails.

**Purpose and scope**

**What does “Block Miro AI usage” do?**

It disables all Miro AI features (for example, text generation, image generation/recognition, smart suggestions) wherever this guardrail applies, preventing any AI-powered interaction with sensitive or classified content.

**What remains available to users?**

Users can continue regular, non-AI collaboration. Existing AI-generated content stays on boards and can be viewed, moved, or manually edited—but users cannot use Miro AI to modify or regenerate it.

**Access and prerequisites**

**Who can configure this guardrail and where?**

Sensitive Content Admins configure guardrails in *Enterprise Guard* under Data Classification → Guardrails. (Company Admins assign the Sensitive Content Admin role.)

**What do I need before assigning this guardrail?**

Define your classification levels and (optionally) auto-classification so the guardrail can be applied by classification (for example, INTERNAL, CONFIDENTIAL).

**Behavior and impact**

**Who is affected when the guardrail applies?**

Everyone—including board owners and co-owners—cannot access or invoke Miro AI on the affected boards.

**Does it remove existing AI content?**

No. It prevents further AI interactions; existing AI content remains available for viewing and manual edits.

**When do changes take effect?**

After you publish your guardrail updates, enforcement is immediate across affected boards.

**Setup and configuration**

**How do I turn on “Block Miro AI usage” for a classification?**

1. Go to *Enterprise Guard* → Data Classification → **Guardrails**.
2. Click the **Edit** icon for a classification level (for example, CONFIDENTIAL).
3. Select the **Block Miro AI usage** check box and **Done**.
4. Click **Next** and review the impact, then **Publish** to apply.

**Should I use Default or Strict mode?**

In Default mode, guardrails won’t override existing sharing settings. In Strict mode, guardrails override active sharing and apply the strictest controls. Choose based on your change-management needs.

**User experience**

**What will users see on boards where AI is blocked?**

Miro AI entry points appear disabled or unavailable, and users cannot invoke AI tools from the canvas or menus on those boards.

**Can users request exceptions on a single board?**

No. The guardrail is enforced by classification policy. Change the board’s classification (or the policy for that level) to alter enforcement.

**Interactions with other controls**

**How does this relate to granular Miro AI admin controls?**

Granular controls manage who can use specific AI features. The guardrail is a policy layer: when active, it blocks AI regardless of feature toggles.

**How does this differ from Prompt blocking or AI Moderation?**

- **Prompt blocking** stops sensitive prompts at submission; AI remains available for non-sensitive prompts.
- **AI Moderation** filters harmful or inappropriate content.
- **Block Miro AI usage** fully disables AI on affected boards.

**Troubleshooting**

**AI still appears on some boards. What should I check?**

- Confirm the board’s classification is one where the guardrail is enabled, and that you clicked **Publish** after editing guardrails.
- If using auto-classification, verify the board classification has updated based on current content.
- In Strict vs Default modes, ensure your expectation matches the rollout mode you selected.

**We need to re-enable AI for a subset of work.**

Adjust the guardrail for the relevant classification or reclassify the boards that should allow AI, then publish the update.

## Admin Analytics Overview dashboard

**Scope and metrics**

**What does the Overview dashboard cover?**

Boards, Users, Teams, Licenses, and Templates, with historical trends where applicable.

**How is “Active this period” defined for Boards, Users, and Teams?**

- **Boards:** Unique boards opened since the start of the selected period. Includes boards later moved to Trash.
- **Users:** Unique users who opened a board at least once since the start of the period. Includes users who are now deactivated.
- **Teams:** Unique teams with at least one member who opened a board since the start of the period. May include teams later moved to Trash.

**Do totals exclude items in Trash?**

Yes. Totals for Boards and Teams exclude items currently in Trash. Historical “active” counts may include items that were later trashed.

**What does the Licenses chart show?**

Allocation totals and history for Full, Free, and Free Restricted licenses, reflecting how many licenses are currently used.

**What does Templates show today?**

Most popular templates used from inside a board. Other sources may be added in future releases.

**Time and history behavior**

**How do historical values display on Overview charts?**

Historical widgets show values as of the last day of each period. Up to one year of history is available or as far back as data exists.

**Data freshness and controls**

**How often is Overview data refreshed and where do I see it?**

At least once every 24 hours. A “Last updated” timestamp is available in the dashboard.

**How do I change the time range?**

Use the time range selector at the top right of the Analytics page.

## Miro AI Moderation

With Miro AI moderation, Company Admins can adjust levels of filtering prompts that might contain potentially harmful or inappropriate text. You can set organization-wide Miro AI moderation sensitivity to filter content, including hate, sexual content, violence, and self-harm. This helps you align Miro AI usage with your organization's requirements, policies, and risk tolerance.  For more information, see the [Miro AI moderation documentation](../ai-trust/04-ai-moderation-overview.md).

**Purpose and scope**

**What is AI Moderation in Miro?**

AI Moderation lets Company Admins set an org-wide filtering level (Strict, Default, or Minimal) that screens prompts which could lead to harmful or inappropriate output (e.g., hate, sexual content, violence, self-harm).

**Who can configure it and on which plans?**

Company Admins on Enterprise with Enterprise Guard can configure the setting in org Settings.

**Does it work if my org connects its own LLM (e.g., a direct provider integration)?**

If a custom LLM is connected, the moderation selector may be disabled for that integration and any previously chosen level won’t apply to it.

**Access and prerequisites**

**Who can activate it and what do I need?**

Company Admins on Enterprise with the Enterprise Guard add-on can configure AI Moderation in org settings.

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

## Prompt blocking

Prompt blocking lets Sensitive Content Admins prevent users from submitting AI prompts that include sensitive information, helping you keep sensitive data out of Miro AI across your organization. Miro scans the text a user enters in the prompt field and any text-based content they add from the board. If that content matches the sensitivity labels or source code patterns selected in the Prompt blocking configuration, Miro blocks the prompt submission.  For more information, see the [Prompt blocking documentation](../ai-trust/06-prompt-blocking-overview.md).

**Purpose and scope**

**What is Prompt Blocking?**

Prompt Blocking prevents users from submitting AI prompts that include sensitive information. Miro scans the text a user types into the prompt field and any text-based content they add from the board; if it matches selected sensitivity labels or source-code patterns, the submission is blocked and a policy message is shown. At the moment, we support only text-based content.

**How is Prompt Blocking different from board scanning?**

Board scanning finds sensitive content on boards and can auto-classify boards; Prompt Blocking checks what users attempt to send to Miro AI at the time of submission.

**Which sensitivity labels are supported?**

Use the org-level categories listed in the Sensitivity labels and infotypes reference.

**What is Code Scanning?**

Code Scanning blocks prompts containing recognizable source code; by design, it requires a minimum block of code (e.g., 5+ lines) to trigger. Toggle it on/off in Prompt Blocking configuration.

**Is non-text content (e.g., images) scanned?**

No. At this moment, Prompt Blocking supports text-based content only.

**Access and prerequisites**

**Who can activate it and what do I need?**

Sensitive Content Admins on Enterprise with the Enterprise Guard add-on can activate it in Settings → Enterprise Guard → Data discovery → Configuration.

**How do I turn it on?**

Open Prompt blocking → Activate, choose Select all or specific label categories, optionally enable Code scanning, then Activate. Enforcement is immediate org-wide.

**Management and changes**

**How do I adjust labels or Code Scanning later?**

Go to Settings → Enterprise Guard → Data discovery → Configuration → Prompt blocking → Manage,

- **Labels:** Select the *Select all* check box to select all categories or select specific label category check boxes.
- **Code scanning:** Turn on Code scanning to block prompts that include source code (minimum 5 lines). For more information, see Code scanning.

Changes take effect immediately.

**What happens to prompts after I change settings?**

Newly unblocked items will go through. Items that still match blocked patterns remain stopped.

**User experience**

**What does a user see when a prompt is blocked?**

A policy message appears where they entered the prompt, and the request isn’t sent to any LLM.

**Is non-text content (e.g., images) scanned?**

No. At the moment, Prompt Blocking supports text-based content only.

**Interactions with other controls**

**How does Prompt Blocking work with guardrails and moderation?**

- **Intelligent Guardrails:** If “Block Miro AI usage” applies, AI is disabled; Prompt blocking won’t trigger because prompts can’t be submitted.
- **AI Moderation:** Both can apply when AI is available—Prompt blocking stops sensitive data; Moderation filters harmful categories.
- **Granular admin controls:** Feature access applies only when AI is available and the prompt isn’t blocked.

##

## Enterprise Guard and Microsoft Purview DSPM for AI integration

For organizations using Microsoft Entra ID (formerly Azure AD) as their identity provider, Enterprise Guard securely forwards AI prompts and responses to Microsoft Purview Data Security Posture Management (DSPM) for AI. Security and compliance teams can then monitor, audit, and control generative AI use from a single trusted platform, reducing operational overhead, mitigating risks such as data leakage and misuse, and strengthening Miro’s enterprise-grade AI governance. For more information, see the [Enterprise Guard and Microsoft Purview DSPM for AI integration documentation](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).

**Purpose and scope**

**What is the Microsoft Purview DSPM for AI integration in Miro?**

An integration that forwards Miro AI prompts and responses to Microsoft Purview’s DSPM for AI so security and compliance teams can monitor, audit, and govern AI activity in one place.

**Who can use this integration?**

Enterprise plans with Enterprise Guard, managed by Company Admins with access to Enterprise integrations. Your Miro org must use Microsoft Entra ID for SSO. A Microsoft Purview license is required.

**What are the benefits?**

Centralized visibility of Miro AI usage in Purview’s AI hub, auditability of prompts and responses, and alignment with your existing governance policies in Purview.

**Which Miro AI activity is included today?**

At the moment, text-based prompts and responses across Miro AI features are forwarded. Image content is not forwarded.

**Are all users’ activities logged?**

Only activity from users who sign in to Miro through the configured Microsoft Entra tenant is forwarded to Purview.

**How long until activity appears in Purview?**

Typically 10 to 30 minutes after the AI action in Miro. View it in Microsoft Purview → DSPM for AI → Activity explorer, or check Audit logs.

**Are there notable limitations?**

At the moment, one Entra tenant can be configured at a time. In multi-IdP or multi-tenant environments, only users authenticating via the configured tenant are logged. Images are not included.

**Setup and configuration**

**How do I enable the integration?**

In Miro: Enterprise settings → Enterprise integrations → toggle on Microsoft Purview DSPM for AI → enter your Entra tenant ID → Connect → sign in with an account that can grant tenant-wide admin consent → accept the Miro AI governance app → confirm Connected in Miro.

**What are the prerequisites?**

- **Miro:** Enterprise plan with Enterprise Guard, Company Admin role, Entra ID configured for SSO. To enable this feature, contact your Customer Success Manager.
- **Microsoft:** Microsoft Purview license, the Entra tenant ID used for Miro SSO, and an Entra role that can grant tenant-wide admin consent.

**How do I verify the setup works?**

Perform a simple Miro AI action, wait 10–30 minutes, then check Microsoft Purview → DSPM for AI → Activity explorer for new Miro entries.

**How do I disconnect or switch tenants?**

In Miro: Enterprise integrations → Microsoft Purview for AI → Disconnect. To change tenants, disconnect first, then reconnect using the new tenant ID.

**Usage and governance**

**Where can I see the forwarded data in Purview?**

Microsoft Purview → DSPM for AI → Activity explorer. You can also review details in Audit logs.

**Can I export or archive AI activity logs?**

Use Microsoft Purview export tooling. Miro forwards the activity to your Microsoft tenant where your policies apply.

**Can I apply Purview policies to Miro AI data?**

Yes. Once ingested, the data follows your organization’s Purview governance model.

**What about privacy and security responsibilities?**

Miro forwards prompts and responses to your Microsoft tenant. Governance and access controls are managed in Purview within your environment.

**Troubleshooting and support**

**The consent step fails or loops. What should I check?**

Ensure the account used for Connect can grant tenant-wide admin consent in Entra, or involve a Microsoft global admin.

**I see no activity in Purview. What now?**

Confirm Enterprise Guard is enabled and you have access to Enterprise integrations. Verify the tenant ID exactly matches your Miro SSO tenant. Make sure a test AI action was performed by a user authenticating via that tenant. Check Purview licensing and filters. Allow up to 30 minutes for ingestion.

**We use multiple IdPs or tenants. Will all users be logged?**

No. Only activity from users signing in via the single configured Entra tenant is forwarded.

**Who supports what?**

Contact Miro Support for setup or connectivity in Miro. For issues inside Microsoft Purview, contact Microsoft Support.
