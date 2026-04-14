---
title: Managing custom terms of service
article_id: 27621616452882
sidebar_position: 5
created_at: '2025-06-24T23:29:13Z'
updated_at: '2026-03-17T08:39:20Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

## Creating custom terms of service

:::note
Notes:

- Admins must have the following Enterprise Guard privileges to view and manage Custom terms of service:
  - Sensitive content admin has built-in permissions.
  - Custom admin roles must include:
    - View custom terms of service
    - Manage custom terms of service
- Guests and external users are excluded.
- Miro does not store the terms, only the link and metadata.
:::

1. Go to **Settings** > **Enterprise Guard** > **Custom terms of service**.
2. If you’re creating custom terms of service for the first time, click **Add terms of service**.
   If you already have an existing configuration and want to add another, click **Create new** from the list view.
3. In **Set up** → **Conditions**:
   - **Trigger**: Choose between **Successful login** or **AI usage**.
     **Successful login**

     - The dialog appears immediately after sign-in.
     - Users can click **Continue** to accept and proceed, or **Sign out**.

     **AI usage**

     - The dialog appears when the user interacts with Miro AI, such as toggling the AI layout, opening the AI side panel, or starting an AI tool or action (for example, Sidekick).
     - Users can click **Continue** to accept and use AI features. If users click **Cancel**, they remain signed in and can continue using all non-AI features.
   - **Scope**: **All users and admins in the organization**.
   - **Recurrence period**: enter a number and select **Days**, **Weeks**, or **Months**.Default: two weeks.
     Users are not prompted again until the recurrence window ends or terms are updated.
4. In **Set up** → **Content**:
   - **Title** (max 32 characters)
   - **Description** (max 200 characters)
   - **Link:** Policy links (externally hosted). To include additional links, click +Add link. Up to three links are supported. Each link URL must be unique.
   - **Link text** (max 60 characters). Each link text must be unique.
5. Click **Show preview** (top right) to review the custom terms of service dialog box content. Make adjustments to the custom terms of service content, if needed.
6. Once you've ready with the custom terms of service content, click **Next**.
7. Review the custom terms of service, confirm your settings and content, then click **Publish**.
   Enforcement is immediate for the selected trigger.

## Editing custom terms of service

1. Open **Settings** > **Enterprise Guard** > **Custom terms of service**.
2. In the list, select the custom terms of service configuration you want to update, then click **Edit**.
3. Update fields as needed in **Conditions** and **Content**.
4. If you want to update the custom terms of service and reset  all user acceptances immediately, click **Publish immediately.**
   If you want to update the custom terms of service and prompt users again after the configured recurrence period ends, click the down arrow, select **Publish in next cycle**, and then click **Publish in next cycle**.

## Deleting custom terms of service

Deletion disables custom terms of service immediately and cannot be undone.

1. Open **Settings** > **Enterprise Guard** > **Custom terms of service**.
2. In the list, select the custom terms of service configuration you want to remove, then click **Delete**.
3. To permanently delete the custom terms of service you selected, click **Delete terms**.
