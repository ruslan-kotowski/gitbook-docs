---
title: Connect tools with Zapier
article_id: 30124629305106
sidebar_position: 3
created_at: '2025-10-10T11:48:03Z'
updated_at: '2025-10-14T12:37:35Z'
draft: false
---

Connect Miro Insights with hundreds of tools through [Zapier](http://zapier.com/) to automatically capture feedback and data from sources that don't have direct integrations. This allows you to centralize customer insights from across your entire tech stack.

The Zapier integration allows you to:

- Automatically create feedback items from customer support tickets, surveys, or chat conversations.
- Capture data from any tool that Zapier supports, even if Miro Insights doesn't have a direct integration.
- Reduce manual data entry by setting up automated workflows.

## Create feedback

Zapier offers two main actions for creating feedback items in Miro Insights.

### Create feedback

The standard action for creating general feedback items in Miro Insights with the following fields:

- **Feedback title**: Brief summary of the feedback.
- **Content**: Detailed feedback content or description.
- **Reporter name**: Name of the person providing feedback.
- **Reporter email**: Email address of the feedback provider.
- **Owner email**: Internal owner or assignee for the feedback.
- **Provided date and time**: When the feedback was originally given.
- **Origin URL**: Link to the original source (ticket, survey response, etc.).
- **Company name**: Organization the feedback is associated with.
- **Company domain**: Company's website domain.

### Create feedback (Call)

A specialized action designed specifically for capturing feedback from calls and conversations with these fields:

- **Call title**: Title or subject of the call.
- **Call transcript**: Full transcript or notes from the call.
- **Origin URL**: Link to the call recording or meeting details.
- **Participants**: Information about call participants.
  - **Email**: Participant's email address.
  - **Name**: Participant's name.
- **Owner email**: Internal owner or assignee for the call feedback.
- **Start date and time**: When the call took place.
- **Company name**: Organization associated with the call.
- **Company domain**: Company's website domain.

## Setting up Zapier integration

To get started with Zapier and Miro Insights, follow these steps.

### Prerequisites

- Active Miro Insights account
- Zapier account (free or paid)
- Access to the source tool you want to connect

### Quick start with templates

Miro Insights offers pre-built Zapier templates for popular conversation intelligence tools, such as Grain, Fathom, and Fireflies.

To set up a Zap using a template:

1. Go to Miro Insights settings > **Integrations & Automations** section.
2. Select your conversation tool. For example, Grain.
3. Log in to Zapier, if needed.
4. Connect your Grainaccount.
5. Map fields from Grain to Miro Insights fields.
6. Test and activate the pre-configured integration.

Templates provide a faster setup experience with optimized field mappings for each specific tool, making it easier to start capturing customer feedback from your recorded conversations.

### Basic setup

1. **Create a new Zap** in your Zapier dashboard.
2. Choose your **trigger app**. The tool where feedback originates from.
3. Select **Miro Insights** as your action app.
4. Choose your **action event**:
   - **"Create Feedback"** for general feedback items.
   - **"Create Feedback (Call)"** for call-specific feedback.
5. Connect your **Miro Insights account** when prompted.
6. **Map fields** from your trigger app to Miro Insights fields.
7. Test the integration to ensure data flows correctly.
8. **Activate the Zap** to start automated data collection.

### Field mapping best practices

When mapping fields from your source tool to Miro Insights, consider the following best practices to ensure high-quality data capture.

**Required fields:**

- **Feedback title**: Use clear, descriptive titles from your source data.
- **Content**: Map the main feedback content or combine multiple fields.

**Recommended fields:**

- **Reporter information**: Capture customer contact details when available.
- **Company data**: Essential for account-based product management.
- **Origin URL**: Maintain traceability back to original sources.
- **Provided date**: Use actual feedback date, not processing date.

**Field mapping tips:**

- Use Zapier's formatter tools to combine multiple source fields.
- Include source tool name in title or content for clarity.
- Use consistent formats for dates, company names, and categories.
- Set default values for optional fields.
