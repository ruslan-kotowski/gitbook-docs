---
title: Select Your Own Model (Beta)
article_id: 29484232754578
sidebar_position: 9
created_at: '2025-09-15T12:50:30Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-sidekicks
availability:
  roles: team_member
  plans: free, starter, business, enterprise
  platforms: browser, desktop, mobile
---

When you perform AI actions with Miro [Flows](04-flows-overview.md) and Sidekicks, Select Your Own Model enables you to specify the most appropriate large-language model (LLM) for the task.

For example, for image generation you can decide whether to use Stable Diffusion 3.5 Large or Gemini 2.5 Flash Image (Nano Banana).

Your choice may depend on the complexity or specificity of your task.

:::tip
Miro Flows and Sidekicks include a default LLM pre-selected for each task. When are unsure which model to select, using the default model is the best start. The default model is shown with a Recommended label.
:::

The model selector is available only as part of Flows and Sidekicks for the following:

- Docs and Image Formats in Sidekicks and Flows
- Main logic of Sidekicks
- Instruction Block in Flows

This article explains how to select your own model for Flows and Sidekicks, and gives information to help you choose an LLM for common tasks.

## Selecting your own model

### Flows

Docs, images, and Instruction Blocks in a Flow each have a prompt box where you can select your own model.

Follow these steps:

1. Add a Doc, image, or Instruction Block, to the canvas.
2. To access the list of available models, in the upper-right of the prompt box, click the default model name. For example, `AWS | Claude 3.5`.
3. Select a model.

To learn more about creating Flows and Flows UX, see [Flows](05-flows.md).

### Sidekicks

When creating or editing Sidekicks, you see the **Model (advanced)** section, and you can select which model you want to use for Sidekick processing, Image generation, and Doc generation.

To learn more about Sidekicks, see the [Sidekicks documentation](08-ai-sidekicks.md).

## How models differ

A large language model (LLM) is usually a member of a family of models that includes capable but resource-intensive models, optimal models, and the fastest but less capable models.

For example, the GPT-5 family includes GPT-5, GPT-5-mini, and GPT-5-nano.

The fastest but least capable models are ideal for lower latency.

### Reasoning and non-reasoning

A main differentiator between LLMs is reasoning versus non-reasoning models.

*Reasoning* means that the model takes more time to provide a higher quality answer.

:::note
Reasoningdoes not always mean the most accurate result. If you require many iterations of output, high reasoning may not be the most efficient.
:::

For complex tasks, like creating customer-facing documents, prioritization, and tasks that require processing a large volume of information, then a reasoning model is the best choice.

For simple tasks, like checking grammar, translation, or reformatting text, a non-reasoning model is the most efficient choice.

The following table shows some reasoning and non-reasoning models.

| Reasoning capability | Models |
| --- | --- |
| Reasoning | GPT-5, GPT-5-mini, GPT-5-nano, Claude Sonnet 4, Claude Sonnet 4.5, Gemini 2.5, Gemini 2.5 Flash, o3, o4-mini |
| Non-reasoning | GPT 4o, GPT-4o-mini, GPT-4.1, GPT-4.1-mini, Claude Sonnet 3.7, Claude Sonnet 3.5, Gemini 2.5 Flash Lite |

### Style

Each LLM has a unique "style." As you experiment with different models, you may notice that a particular output style matches your requirements, whether for branding, vibe, or preference.

:::tip
Older models have a more distinct style, especially for creative, out-of-the box output.
:::

## Selecting your AI model by task

| Task | Models | Description |
| --- | --- | --- |
| Brainstorming | GPT-4o, o3, o4-mini, Sonnet 3.7 | Great for divergent thinking, idea bursts for features, playful tone, and "creative edge." Use to generate text, like alternative headlines and microcopy variants, for example. |
| Prioritization & scoring | GPT-5, Claude Sonnet 4.5, Gemini 2.5 | The best reasoning models for consistent scoring and clear rationales. For example, RICE/MoSCoW on backlog, tradeoff write-ups, and roadmap tiers. |
| Synthesis & research | GPT-5, GPT-5-mini, Claude Sonnet 4.5, GPT-4.1, Claude Sonnet 3.7, Gemini 2.5 Flash | Use for average to highly complex tasks. For example, generating personas from notes, and deriving insights from data and knowledge bases. |
| Schema & transformation | GPT-5-mini, GPT-5-nano, GPT-4.1, Sonnet 3.7, Gemini 2.5 Flash, Gemini 2.5 Flash Lite | Format change usually doesn't require complex reasoning so optimized versions will give results faster, but stick to later model families to ensure consistency when dealing with large contexts. notes → docs, doc → datable, spec → diagram) |
| Quick text edits | GPT-4o-mini, Gemini 2.5 Flash Lite, GPT-5-nano, Claude 3.7 | Fastest options. Best for simple text edits, like grammar, translation, and rewrites for clarity. |

## Selecting models for image generation

All large language models (LLM) that Miro supports can process text and images. However, most cannot generate images.

For image generation, Gemini 2.5 Flash Image (Nano Banana) is exceptionally adept at converting your general instructions into an image.

Most LLMs expect an image description, not specific instructions. For example, "a painting of a dog in a funny hat" as a description, versus "create a funny image of dog" as instruction. Nano Banana is able to generate images based on specific instruction.

:::note
Use Nano Banana for targeted edits to an existing image. Other models can use an existing image as a style reference.
:::

In terms of speed or output quality, there is little difference between LLMs. As with each use case, you can experiment with different models to find which best suits your preferences.
