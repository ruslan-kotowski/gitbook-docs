---
title: AI Moderation overview
article_id: 29491049430674
sidebar_position: 4
created_at: '2025-09-15T16:27:59Z'
updated_at: '2026-01-12T11:21:56Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-granular-admin-settings
---

With Miro AI moderation, Company Admins can adjust levels of filtering prompts that might contain potentially harmful or inappropriate text. You can set organization-wide Miro AI moderation sensitivity to filter content, including hate, sexual content, violence, and self-harm. This helps you align Miro AI usage with your organization's requirements, policies, and risk tolerance.

:::note
*If your organization connects its own LLM provider (for example, a direct OpenAI integration), the moderation selector is disabled and any previously chosen level is ignored for that integration.*
:::

## Moderation levels

Control Miro AI content across your organization with Miro AI moderation. Set the filtering level to Strict, Default, or Minimal to determine what prompts are blocked. Review the table below to compare levels quickly, then dive into the detailed sections for more guidance.

| Level | What it does | Best for | Trade-offs |
| --- | --- | --- | --- |
| Strict | Blocks Default + low-to-moderate risk content. | Highly regulated orgs, education. | More false positives; potential over-filtering. |
| Default (recommended) | Blocks moderately to severely harmful content. | Most business use cases. | Some borderline content may pass. |
| Minimal | Blocks only severely harmful content. | Creative/gaming/media contexts. | More exposure to low-to-moderate harm. |

:::note
*Default is recommended for most organizations. It filters content that most people consider inappropriate or harmful while maintaining broad usability.*
:::

## Strict level

### What it filters

Everything in Default plus low-to-moderate risk content (for example, subtle or coded hate speech, sexually suggestive content, non-graphic violence, or non-explicit mentions of self-harm).

### When to use

- Regulated industries or risk-averse org policies
- Education or youth-focused programs
- Pilots with low risk tolerance

### Trade-offs

- More false positives and blocked borderline prompts
- Requires guidance to reduce user friction

## Default level (recommended)

### What it filters

Moderately to severely harmful content (explicit hate speech, explicit sexual content, graphic violence, encouragement of self-harm).

### When to use

- Most organizations seeking balanced safety/usability

### Trade-offs

- Contextual/borderline prompts may pass

## Minimal level

### What it filters

Only severely harmful content.

### When to use

- Creative teams that need broader expression (gaming, media)
- Internal ideation with clear escalation paths

### Trade-offs

- Higher exposure to low-to-moderate harmful content in outputs

## Auditing and compliance

Changes to the moderation level are captured in the organization audit log, including the previous value, the new value, who changed it, and when it changed. For more information, see our documentation on [Audit Logs](../../security-integrations/security-management/01-audit-logs.md).

## Best practices

- Start with Default, then adjust based on pilot feedback and escalation reviews.
- Pair Strict with clear internal guidance on acceptable prompts to reduce false positives.
- If you need Minimal, define when teams should escalate or report problematic outputs.
- Revisit your setting after major policy or regulatory updates.

- AI Moderation overview
- Moderation levels
- Strict level
- Default level (recommended)
- Minimal level
- Auditing and compliance
- Best practices
