---
title: Set or update the Miro AI moderation level
article_id: 30613174297618
sidebar_position: 5
created_at: '2025-10-29T01:15:35Z'
updated_at: '2026-01-12T11:22:05Z'
draft: false
---

With Miro AI moderation, Company Admins can adjust levels of filtering prompts that could lead to potentially harmful or inappropriate output. You can control Miro AIl moderation sensitivity across your organization and filter across categories such as hate, sexual content, violence, and self‑harm. This helps you align Miro AI usage with your organization's requirements, policies, and risk tolerance.

:::note
: If your organization connects its own LLM provider (for example, a direct OpenAI integration), the moderation selector is disabled and any previously chosen level is ignored for that integration.
:::

## Prerequisites

- Ensure you have the Enterprise Guard add-on.
- Ensure you are a **Company Admin** for the organization you want to configure.
- Review your governance and policy requirements to choose an appropriate starting level. Default is recommended for most organizations.

## Set or update the Miro AI moderation level

1. Open your organization **Settings** in Miro.
2. Go to **Miro AI** › **Moderation**.
3. Choose a level:
   - **Strict:** Blocks everything in Default plus low to moderate risk content (for example, subtle or coded hate, sexually suggestive content, non-graphic violence, non-explicit self-harm mentions).
   - **Default (recommended):** Blocks moderately to severely harmful content (for example, explicit hate, explicit sexual content, graphic violence, encouragement of self-harm).
   - **Minimal:** Blocks only severely harmful content.
4. Click **Confirm**.
   The change applies to everyone in the organization immediately and is recorded in the audit log.

## Validate the moderation level (optional)

- Ask a pilot group to test typical prompts and report any over- or under-filtering.
- Monitor support or escalation channels for false positives or missed harms during the first week after a change.

## Tips and best practices

- Start with **Default**, then adjust based on pilot feedback and escalation reviews.
- If users report too many blocked prompts, try **Default** (from Strict) or **Minimal** (from Default) and publish examples of acceptable prompts.
- If borderline content slips through, move to **Strict** and add internal guidance to reduce friction.
- Revisit the level after policy, regulatory, or use-case changes.

## Troubleshooting

**Moderation control is disabled**
A custom LLM integration is connected. Disconnect it to re-enable the selector. While connected, any previously chosen level is ignored for that integration.

**Too many false positives**
Consider changing **Strict → Default** and share acceptable-use examples. Review recent changes in the audit log to confirm timing.

**Harmful content exposure**
Ensure the level is not **Minimal**. Consider **Default** or **Strict** depending on risk tolerance.

**Users are unsure why prompts are blocked**
Publish internal guidance pointing to your chosen level, example prompts, and escalation paths.
