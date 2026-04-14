---
title: Miro AI granular admin controls
article_id: 27016283682578
sidebar_position: 2
created_at: '2025-05-28T12:30:26Z'
updated_at: '2026-03-10T15:25:49Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-granular-admin-settings
availability:
  roles: company_admin
  plans: Enterprise with Miro AI Workflows Add-on or Enterprise Guard Add-on
  platforms: browser
---

Miro AI admin controls enable Enterprise Company Admins to decide which AI capabilities are available in their organization and manage who can use them. Admins can also view the models that power each AI feature.

With the Enterprise Guard add-on, Miro AI controls extend to the feature level within each capability category, which helps prioritize features based on organizational needs and security requirements. In addition to the complete Miro AI capability category, Admins can also enable, restrict, or remove specific Miro AI features. For example, within the Images category, you can enable *Create images with AI* and disable *Remove background*.

Use these controls to roll out AI safely and meet security requirements while driving adoption of AI capabilities. For more information on the Miro AI features you can toggle, see Miro AI admin controls reference.

## Enable, restrict, or remove Miro AI capabilities and features

1. **Go to the Admin Console.**
   From your Miro dashboard, click your avatar in the top-right. Then select **Admin Console**.
2. On the left sidebar, click **Miro AI > Capabilities**.
3. **To enable, restrict, or remove a Miro AI capability and apply to entire category:**
   1. Click the drop-down list to the right of a Miro AI capability, and then turn on the **Apply to entire category** toggle.
   2. Click the drop-down list to the right of the same Miro AI capability once again, and then select one of the following options:

      - **Everyone.** If you select **Everyone**, the Miro AI capability is enabled for all users and teams across your organization (including any teams created later). Any team-level restrictions are overridden.
      - **No one.** If you select **No one**, a dialog box appears to confirm if you want to remove access to the specific Miro AI capability for everyone. Click **Remove access** to confirm.

      When a Miro AI capability category is deactivated, users can no longer access that capability and all its associated features on any Miro board.
      If you deactivate all Miro AI capabilities, then **Create with AI** appears disabled on the board.

      - **Specific teams.** If you select **Specific teams**, click to select the check box beside the team for which you want to enable the Miro AI capability, and then click **Save**.
4. **To enable, restrict, or remove access to a specific feature within a Miro AI capability:**
   1. Ensure that the **Applied per feature** option is active. To activate per feature controls, click the drop-down list to the right of a Miro AI capability, and then turn on the **Apply to entire category** toggle.
   2. Click the arrow to the left of a Miro AI capability category to expand and view all the features that are available for the capability.
      The list of features belonging to the Miro AI capability appears along with the access settings for each feature.
   3. Click the drop-down list to the right of a feature, and then select one of the following options:
      - **Everyone.** If you select **Everyone**, the feature is enabled for all users and teams across your organization (including any teams created later). Any team-level restrictions are overridden.
      - **No one.** If you select **No one**, a dialog box appears to confirm if you want to remove access to the specific feature for everyone. Click **Remove access** to confirm.
        When a Miro AI feature is deactivated, users can no longer access that feature on any Miro board.
      - **Specific teams.** If you select **Specific teams**, click to select the check box beside the team for which you want to enable the Miro AI feature, and then click **Save**.

## Miro AI admin controls reference

Use this reference to review all of the Miro AI capability categories you can enable or restrict in the Admin Console. You can also view the list of specific features under each category section. It explains what each toggle controls and helps you plan Miro AI capability rollouts by team or across your organization.

### Create content

Use AI to create and edit canvas content like sticky notes, Docs, Tables, Timelines, and more. [Learn more about AI content creation.](../../../using-miro/miro-ai/03-create-with-ai.md)

- **Create sticky notes:** Create sticky notes with AI.
- **Cluster sticky notes:** Automatically group sticky notes by keywords or sentiment.
- **Create and edit docs:** Create and edit documents with AI.
- **Create and edit tables:** Create and edit tables with AI.
- **Create and edit diagrams:** Create diagrams with AI assistance
- **Edit, refine, or translate text:** Corrects, rewrites, and translates text to improve clarity, tone, and readability.
- **Shorten text:** Rephrases selected text into a shorter version without losing clarity and readability.
- **Rewrite for clarity:** Rewrites selected text for clarity.
- **Change tone:** Modifies the tone for selected text to convey friendly, professional, business, or fun.
- **Translate:** Translates selected text between 18 languages.

:::note
Managing access to these features individually is available with the Enterprise Guard add-on.
:::

### Images

Create and edit images with AI on the canvas.

- **Create images:** Create images with AI.
- **Remove background:** Remove image backgrounds with AI.
- **Add captions to images:** Create alt text for images

:::note
Managing access to these features individually is available with the Enterprise Guard add-on.
:::

### Summarize activity

Create a summary of board activity and comment threads. [Learn more about AI activity summary](../../../using-miro/miro-ai/11-conversation-summaries.md).

- **Catch up:** Get an overview of changes to the board since your last visit
- **Conversation summary:** Get a summary of long comment threads on your Miro board

:::note
Managing access to these features individually is available with the Enterprise Guard add-on.
:::

### Beta features

Give users access to new features as soon as they're available.

For more information on Miro AI features, description, and models, see **Miro AI reference**.

### Flows

Connect AI prompts to canvas content to create automated workflows.

:::note
You can view and manage these settings only if the feature is enabled for your organization.
:::

### Sidekicks

AI partners that collaborate on exploring ideas, building solutions, and moving work forward. Learn more about [Sidekicks.](../../../using-miro/miro-ai/08-ai-sidekicks.md)

:::note
You can view and manage these settings only if the feature is enabled for your organization.
:::

### Prototyping

Create interactive prototypes from prompts or image recognition.

:::note
You can view and manage these settings only if the feature is enabled for your organization.
:::
