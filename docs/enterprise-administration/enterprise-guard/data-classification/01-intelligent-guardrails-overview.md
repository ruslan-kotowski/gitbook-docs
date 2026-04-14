---
title: Intelligent Guardrails overview
article_id: 14375998880018
sidebar_position: 1
created_at: '2023-10-12T12:35:03Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Miro board items can contain privacy and regulatory data (such as PII, PHI, PCI) or confidential business-critical content (such as financial information, HR information, IP, trade secrets). After data discovery and auto-classification, organizations must implement proactive controls that are crucial for maintaining sustained privacy, security, and compliance with relevant regulations.

- With guardrails, you can now automatically enforce proactive controls, such as:
  Automatically restricting sharing capabilities at various levels (public, team, organization) based on the board's content and classification level.
- Restricting content replication.
- Blocking Miro AI usage to prevent AI-powered interactions with sensitive or classified data.

These proactive controls ensure sustained privacy and compliance without hindering business operations.

Admins have two options for rolling out Intelligent Guardrails in their organization:
- **Default mode:** By default, guardrails do not affect active sharing options on boards to avoid disrupting ongoing collaboration, including when the boards are reclassified during auto-classification.

- **Strict mode:** When the **Apply guardrails in strict mode** toggle is turned on, guardrails override all active sharing options. This provides Admins with the strictest levels of control, but can also result in some users losing board access immediately.

Consider a scenario where you configured guardrails to ensure that users of boards classified as CONFIDENTIAL are not allowed to share the board with public, share with teams, share with organization, or replicate content. Someone in your organization created a new board named Financial Plan, added some revenue numbers, and assigned the *CONFIDENTIAL* classification level for this board. Guardrail settings are automatically applied and all users are not able to share the board and all users except the board owner cannot replicate content (Figure 2).

For more information on each guardrails, their descriptions, and users affected, see the [Guardrails reference documentation](../../canvas-25-admin-features/data-classification/02-guardrails-reference.md).
