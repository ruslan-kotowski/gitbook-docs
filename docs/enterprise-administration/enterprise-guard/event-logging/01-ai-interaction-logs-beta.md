---
title: AI interaction logs (Beta)
article_id: 34049604547858
sidebar_position: 1
created_at: '2026-03-15T21:28:41Z'
updated_at: '2026-03-16T09:09:18Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

AI interaction logs allow admins with the Enterprise Guard add-on to collect and review records of Miro AI usage across their organization. By enabling AI interaction logs, admins can provide security, compliance, and governance teams with greater visibility into how AI features are used and what information is processed by AI systems.

AI interaction logs help organizations:

- Monitor how AI features are used across the organization
- Support governance, compliance, and security reviews
- Provide visibility into information shared with AI systems
- Strengthen trust and responsible adoption of AI tools

AI interaction logs capture records of interactions between users and AI-powered features in Miro. These records help organizations review how AI is used across the organization and support internal auditing, governance, and compliance processes.

When enabled, AI interaction logs capture:

- User prompts submitted to AI features
- AI-generated responses returned by the system
- System context associated with the interaction

## Before you begin

- You must be an admin to enable or configure AI interaction logs.
- The Enterprise Guard add-on is required to use this feature.
- AI interaction logs must be enabled before data collection begins.
- Only interactions that occur after logging is enabled are recorded.

## Enable AI interaction logs

1. Go to **Admin console**.
2. Select **Security**.
3. Click **Audit logs**.
4. Open the **Settings** tab.
5. In the **AI interaction logs** section, enable **Collect AI interaction logs**.
6. Select the **log retention period**.
7. Save your changes.

After enabling this setting, Miro begins collecting AI interaction logs for new AI interactions.

## Configure log retention

Admins can configure how long AI interaction logs are stored.

1. Go to **Admin console > Security > Audit logs**.
2. In the **AI interaction logs** section, select the desired **retention period**.
3. Save your changes.

Logs are automatically deleted when the configured retention period expires.

## Access AI interaction logs via APIs

AI interaction logs can be retrieved using the AI interaction logs API.

This allows organizations to export and analyze AI interaction data using their existing governance, compliance, or security monitoring systems.

Common use cases include:

- AI governance and oversight
- Security monitoring
- Compliance auditing
- Internal investigations

For more information, see the [developer documentation](https://developers.miro.com/reference/enterprise-get-ai-interaction-logs).

## Limitations

The current release includes the initial version of AI interaction logging. The following limitations apply:

- Tool invocations from AI features are not currently logged.
- Interactions related to Miro MCP integrations are not currently logged.
- Moderation events and sensitive prompt blocks are not currently logged.
- Images are not included in AI interaction logs.
