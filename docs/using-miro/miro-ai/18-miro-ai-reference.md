---
title: Miro AI reference
article_id: 20970362792210
sidebar_position: 18
created_at: '2024-08-26T09:34:26Z'
updated_at: '2026-03-18T18:21:50Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  roles: all_users
  plans: free, starter, business, enterprise, education
  platforms: browser, desktop, mobile
---

This reference article describes Miro AI functionality.

## Miro AI models

Models are generally hosted on provider infrastructure, or Microsoft’s Azure AI service or AWS Bedrock. For customers who procure Miro through [AWS Marketplace](#aws-marketplace-customers), all models are hosted on AWS Bedrock.

### AI powered creation & iteration

| **Miro AI feature** | **Description** | **Model** |
| --- | --- | --- |
| Conversation summaries | Generates a summary of lengthy comment threads on your Miro board. | GPT 4o-mini |
| Create diagram - Flow chart | Creates a flow chart from a user prompt and selected board content. | GPT-4o |
| Edit diagram - Flow chart | Edits a flow chart from a user prompt and selected board content. | GPT-4o |
| Create diagram - Mind map | Creates a mind map from a user prompt and selected board content. | GPT 4o-mini |
| Edit diagram - Mind map | Edits a mind map from a user prompt and selected board content. | GPT-4o |
| Create diagram - ERD | Creates an entity relationship diagram (ERD) from a user prompt. A **Create with AI** option. | GPT 4o-mini |
| Edit diagram - ERD | Edits an ERD from a user prompt and selected board content. | GPT-4o |
| Digitize diagram | Transforms images of hand-drawn diagrams to fully editable diagrams in Miro. | Claude 3.7 Sonnet (AWS Bedrock) |
| Create Doc | Creates a Miro Doc from a user prompt and selected board content. A **Create with AI** option. | GPT-4o |
| Edit Doc | Edits a Miro Doc from a user prompt and selected board content. | GPT-4o |
| Create image | Creates an image from a user prompt, including board objects for context. A **Create with AI** option. | Segmind Stable Diffusion 1B (SSD-1B) + StabilityAI Diffusion XL Refiner 1.0 |
| Edit image | Edits an image from a user prompt, including board objects for context. A **Create with AI** option. | GPT-4o |
| Convert image to Prototype | Converts a sketch or prototype image to an editable Miro Prototype. | Claude Opus 4.6 and Gemini 2.5 Pro |
| Image alt text | Generates alt text for an image. Does not consume AI credit. | Miro proprietary model |
| Create sticky notes | Creates Miro sticky notes from a user prompt and selected board content. | GPT-4o |
| Edit sticky notes | Edits Miro sticky notes from a user board and selected board content. | GPT-4o |
| Sticky capture | Converts an image of physical stickies into Miro sticky notes. | Miro proprietary model |
| Create Prototype | Creates a Miro Prototype from a user prompt and selected board content. | GPT-4o + Claude Opus 4.6 and Gemini 2.5 Pro + GPT 4o-mini + Gemini 2.5 Flash Image (nano-banana) |
| Edit Prototype screen | Edits a Miro Prototype screen from a user prompt and selected board content. | Claude 4.5 Sonnet + Gemini 2.5 Flash Image (nano-banana) |
| Remove background | Removes the background from an image. | Miro proprietary model |
| Smart drawings | Converts a pencil drawing into a line, shape, or sticky note. | Miro proprietary model |
| Create Table | Creates a Miro Table from a user prompt and selected board content. | Claude 3.7 Sonnet |
| Edit Table | Edits a Miro Table from a user prompt and selected board content. | Claude 3.7 Sonnet |

### AI powered Sidekicks

|  |  |  |
| --- | --- | --- |
| **Miro AI feature** | **Description** | **Model** |
| AI Sidekicks - Agile Coach | Identifies key themes in a retrospective, and suggests next steps. | GPT-4o |
| AI Sidekicks - Product Leader | Gives feedback and suggestions as comments on frames, sticky notes, or text. Also provides solution ideas as sticky notes. | GPT-4o |
| AI Sidekicks - Product Marketing Alliance | Gives feedback and suggestions as comments on frames, sticky notes, or text. | GPT-4o |

### AI powered clustering

| **Miro AI feature** | **Description** | **Model** |
| --- | --- | --- |
| Sticky notes clustering by keywords | Collates sticky notes into groupings by keyword, with a title for each grouping. | Claude 3.5 Haiku + Amazon Nova Micro |
| Sticky notes clustering by sentiment | Collates sticky notes by sentiment, like opinions and points of view, into positive, neutral, and negative groupings. | Claude 3.5 Haiku |

### AI powered text editing

The following table shows text editing powered by Miro AI:

|  |  |  |
| --- | --- | --- |
| **Miro AI feature** | **Description** | **Model** |
| Change tone | Modifies the tone for selected text to convey friendly, professional, business, or fun. | GPT-5 nano |
| Fix grammar and spelling | Corrects spelling and grammar for selected text. | GPT-5 |
| Rewrite for clarity | Rewrites selected text for clarity. | GPT-5 Chat |
| Shorten text | Rephrases selected text into a shorter version without losing clarity and readability. | GPT-5 mini |
| Translate | Translates selected text into English, Spanish, German, French, Japanese, Portuguese, Korean, Polish, Italian, Turkish, Arabic, Russian, Danish, Finnish, Norwegian, Dutch, Swedish, or Thai. You can translate single or multiple objects simultaneously. | GPT-5 mini |

### AI powered Mind Maps

| **Miro AI feature** | **Description** | **Model** |
| --- | --- | --- |
| Generate mind map | Generates a mind map from a selected root node. | GPT 4o-mini |
| Mind map - Expand with ideas | Generates ideas from a selected root node or child node. | GPT 4o-mini |
| Mind map - Expand with topics | Generates topics from a selected root node or child node. | GPT 4o-mini |
| Mind map - Expand with questions | Generates a question from a selected root node or child node. | GPT 4o-mini |

### AI powered Slides

Miro Slides uses the following models:

- Amazon Titan
- Claude 4 Sonnet
- Claude 3.7 Sonnet
- Claude 3.5 Sonnet
- GPT-5
- GPT-4o
- Stable Diffusion 3.5 Large
- Stability Image Core

### Miro Insights

To synthesize customer feedback, [Miro Insights](https://help.miro.com/hc/articles/25438311770770) uses GPT-4o.

### AWS Marketplace customers

**AWS Marketplace models**

| **Miro AI feature** | **Model** |
| --- | --- |
| Conversation summaries | Claude Haiku 3.7 (AWS Bedrock) |
| Create diagram – Flow chart | Claude Sonnet 3.7 (AWS Bedrock) |
| Edit diagram – Flow chart | Claude Sonnet 3.7 (AWS Bedrock) |
| Create diagram – Mind map | Claude Sonnet 3.7 (AWS Bedrock) |
| Edit diagram – Mind map | Claude Sonnet 3.7 (AWS Bedrock) |
| Create diagram – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| Edit diagram – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| Create doc | Claude Sonnet 3.7 (AWS Bedrock) |
| Edit doc | Claude Sonnet 3.7 (AWS Bedrock) |
| Create Stick notes | Claude Sonnet 3.7 (AWS Bedrock) |
| Edit Sticky notes | Claude Sonnet 3.7 (AWS Bedrock) |
| Sticky capture | Claude Sonnet 3.7 (AWS Bedrock) + Miro proprietary model |
| Create image | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Edit image | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Image alt text | Claude Sonnet 3.7 (AWS Bedrock) |
| Create Prototype | Amazon Nova Pro + Claude Opus 4.6 (AWS Bedrock) + Bedrock Stability Image Core |
| Edit Prototype screen | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| Convert image to Prototype | Claude Opus 4.6 (AWS Bedrock) and Amazon Nova Pro |
| Create table | Claude Sonnet 3.7 (AWS Bedrock) |
| Edit table | Claude Sonnet 3.7 (AWS Bedrock) |
| Digitize Diagram | Claude Sonnet 3.7 (AWS Bedrock) |
| Sticky notes clustering by keywords | Claude Sonnet 3.7 (AWS Bedrock) + Miro proprietary model |
| Sticky notes clustering by sentiment | Miro proprietary model |
| AI-powered Sidekicks | Claude Sonnet 3.7 (AWS Bedrock) |
| AI-powered text editing | Claude Sonnet 3.7 (AWS Bedrock) |
| AI-powered mind maps | Claude Sonnet 3.7 (AWS Bedrock) |

## Select Your Own Model

The following lists show which models are available with [Select Your Own Model](https://help.miro.com/hc/articles/29484232754578), available for [Flows](https://help.miro.com/hc/articles/29681832191378) and Sidekicks.

### Large language models

**Claude**

- Claude 3.7 Sonnet
- Claude Sonnet 4

**OpenAI**

- GPT-4o
- GPT-4o mini
- OpenAI o4-mini
- GPT-5
- GPT-5 mini
- GPT-4.1
- GPT-4.1 mini

### Image models

**Stability AI**

- Stable Image Core
- Stable Image Ultra
- Stable Diffusion 3.5 Large

**Amazon**

- Amazon Titan Image Generator
- Amazon Nova Canvas

**Google**

- Gemini 2.5 Flash Image (Nano Banana)
- Vertex AI Imagegen 3
- Vertex AI Imagegen 3 Fast
- Vertex AI Imagegen 4

## Miro AI credits and add-on

Miro allocates a set number of AI credits to your account each month. The amount of credits allocated depends on your plan. Your allocation resets on the first day of each calendar month.

For each AI action you perform, you consume AI credits. Most AI actions consume one (1) credit per action, however some features may consume more.

To increase your allocation of AI credits, you can optionally purchase a Miro AI credit add-on subscription. To learn more, see [Miro AI credits and AI add-on](https://help.miro.com/hc/articles/19756209116178).

## Miro AI privacy and security

Starting February 3, 2025, Miro collects AI interaction data from Free plan users to improve Miro AI features like AI summaries, diagrams, and AI Sidekicks.

To learn more about how Miro uses AI interactions to improve Miro AI, and how you can control your data preferences, see [Miro AI quality improvements](https://help.miro.com/hc/articles/22874000865554).
