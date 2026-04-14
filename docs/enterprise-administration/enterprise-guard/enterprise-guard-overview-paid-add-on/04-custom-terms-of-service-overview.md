---
title: Custom terms of service overview
article_id: 27375760557330
sidebar_position: 4
created_at: '2025-06-13T08:24:28Z'
updated_at: '2026-03-17T08:39:20Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

The custom terms of service feature allows admins to display a custom Terms of Service dialog for all internal members of their Miro organization. This ensures users review and acknowledge your organization’s terms and policies before using Miro. Use this feature to inform users about acceptable-use policies for Miro features, including Miro AI. Admins can add multiple links to externally hosted policies and configure recurrence so users are prompted on a schedule that matches internal requirements. All actions related to custom terms of service are logged in the audit logs for traceability.

:::note
Custom Terms of Service is currently available only on the web app and browsers.
:::

## Key benefits

- Display terms of service across your organization.
- Present the custom terms of service dialog at relevant points of use: after successful login or upon interaction with Miro AI.
- Enforce user acceptance on a schedule you configure (days, weeks, or months) or upon updates.
- Link up to three internally or externally hosted policies in your preferred language or format.
- Maintain auditability in the audit logs.

## Scope

- Applies to: internal users only, all organization members and admins.
- Excluded: guests and external collaborators.
- Triggers:
  - Successful login: shown immediately after sign-in.
  - AI usage: shown when a user interacts with Miro AI (for example, toggling the AI layout, opening the AI side panel, or starting an AI action such as Sidekick).
- Recurrence: admin-configurable in days, weeks, or months. Each custom terms of service has its own status and recurrence. Default: two weeks.
- Terms format: content must be externally hosted. Miro references the links and does not store full policy text.
- Links: up to three policy links, each with a clear label.
- Configuration: you can configure one custom terms of service for each trigger (successful login and Miro AI usage). Each custom terms of service has its own status and recurrence.

## Who can use this feature?

Admins must have the following Enterprise Guard privileges to view and manage Custom terms of service:

- **Sensitive content admin:** has built-in permissions.
- **Custom admin roles**, must include:
  - View custom terms of service
  - Manage custom terms of service

## How it works

1. **Configure conditions:** choose the trigger (successful login or AI usage), scope (internal members), and recurrence.
2. **Add content:** provide a concise title, short description, and up to three labeled links to externally hosted policies.
3. **Review and enable:** preview the end-user dialog and enable the configuration.
4. **Enforcement:**

- **Successful login:** the dialog is not dismissible. Users must accept to proceed or sign out.
- **AI usage:** the dialog allows **Continue** or **Cancel**. Cancel keeps the user signed in with AI features disabled.

5. **Logging:** configuration changes and user acceptances are recorded in audit logs.

### User experience

- **Successful login**

  - The dialog appears immediately after sign-in.
  - Users can click **Continue** to accept and proceed, or **Sign out**.
- **AI usage**

  - The dialog appears when the user interacts with Miro AI, such as toggling the AI layout, opening the AI side panel, or starting an AI tool or action (for example, Sidekick).
  - Users can click **Continue** to accept and use AI features. If users click **Cancel**, they remain signed in and can continue using all non-AI features.
- Users are not prompted again until the recurrence window ends or terms are updated.

## Acceptance behavior

- **Login trigger:** users must accept on the configured schedule or sign out. The dialog cannot be bypassed.
- **AI usage trigger:** users can accept to enable AI features or cancel to keep AI features disabled. Cancel keeps the user signed in and able to use non-AI features.
- **Recurrence and versions:** users are not prompted again until the recurrence period ends or a new version is published, according to the configured trigger.

##

###
