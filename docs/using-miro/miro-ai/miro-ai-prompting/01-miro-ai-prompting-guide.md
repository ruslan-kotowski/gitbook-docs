---
title: Miro AI prompting guide
article_id: 30226743358226
sidebar_position: 1
created_at: '2025-10-14T17:24:22Z'
updated_at: '2025-11-25T15:54:58Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Better prompting produces better results when working with any AI model. More in-depth prompts generally create outputs that are more closely aligned with what you have in mind. Shorter, less-detailed prompts give the AI model more freedom to interpret what you want, which can produce surprising outputs.

This prompting guide will assist you in creating better prompts when working with Miro AI features.

## RISEN framework

The RISEN framework for prompting AI is a structured approach for generating better results from the start. It includes:

- **Role:** Is the AI a creator, advisor, or a problem-solver? Are they playing a particular role on your team? *Examples: “You are a senior product designer creating…” or “You are an expert technical writer advising...”*
- **Input:** This is where you provide information the AI will need to perform its task. In Miro, this can include written information or context from the board. For example, when creating a prototype, you could include the features of the product or which pages should be included.
- **Steps:** This is where you tell the AI what you want it to do. While you can give general instructions here, spelling out in more detail exactly what you want it to do will yield better results. *Example: “1. Summarize the material provided in the context from the board. 2. Create a sticky note for each important point from the material. 3. Organize the sticky notes in terms of which are likely to be most impactful.”*
- **Expectation:** If you don’t specify what you want the output to be, AI will make that decision for you, and won’t always get it right. Be specific here; instead of saying “create a slide deck,” tell it to “create a slide deck with twelve slides” and then tell it which topics each slide should cover.
- **Narrowing:** If there are things you *don’t* want the output to include, specify that at the end. For example, you might create an AI prototype for an online checkout process that *doesn’t* include a sign-in page in the flow.

By defining each of these parameters, the Miro AI will know exactly what you expect its output to be, creating better overall outputs.

## Adding context from your Miro board

One of the most powerful features of [Miro AI](../01-miro-ai-overview.md) is the ability to add context from the current board. This allows you to add a large volume of information in structured ways to improve your AI output.

Here are some tips for making the most of board context:

- **Don’t select everything on the board.** While it can feel easier to select everything on the board as context, narrowing it down to only the most relevant information will yield the best results.
- **Add industry-specific context to the board.** While Miro AI is powerful, it’s also built on a general Large Language Model (LLM) like most other AI models. Adding industry-specific documentation relevant to your prompt helps it produce better results the first time. This could include things like a glossary of industry terms, an example of a specific output you want it to make, or other industry knowledge that someone outside of your industry wouldn’t likely know.
- **Use Miro AI to create context.** If you need something like a product design brief based on notes from a meeting, you can use Miro AI to create that in a Doc on your board. Make necessary edits, then include that as context rather than including scattered meeting notes that may be confusing.

## Miro AI starter prompts

New to Miro AI? We’ve got you. We created ready-to-use starter prompts for popular workflows. Just replace the bracketed placeholders (for example, [role], [artifact], [tone]) with your context, then run the prompt. Explore our starter prompts by workflow:

- [Content generation and ideation starter prompts](02-content-generation-and-ideation-starter-prompts.md)
- [Content analysis and organization starter prompts](03-content-analysis-and-organization-starter-prompts.md)
- [Workflow optimization starter prompts](04-workflow-optimization-starter-prompts.md)

## Feature-specific prompting tips

Miro AI offers general and specialized Sidekicks, AI mode, Flows, and Format-specific AI tools to better focus on the output you want. If you’re trying to create a prototype, for example, open up Miro Prototypes instead of trying to create one from the general-purpose Sidekick.

### Miro Prototypes

[Miro Prototypes](../../miroverse/prototyping/07-miro-prototypes-add-on.md) allow you to create single- or multi-screen prototype flows with AI. Follow these tips for better prototyping results:

- Specify the screens you want the prototype to include, especially if any are outside of a typical UX pattern for the user journey you’re designing for.
- If you have any product or design requirements (i.e., hex codes for specific colors), include that as context on your board.
- Include screenshots of similar pages or designs you want to use as inspiration as context on your board.
- Include information about your target user in the prompt (i.e., “college students” or “design team leads”).

### Miro Slides

Use AI to create [Slides](../../formats/02-create-miro-slides-with-ai.md) to speed up your presentation preparation. Follow these tips for generating better slide decks:

- Define the color palette or other style considerations in your prompt. If you’ve specified a color palette in the Miro Brand Center, include that in you prompt.
- Include content for specific slides as a Doc or Sticky notes as context on the board.
- Specify who your audience is in the prompt (i.e., “C-suite executives” or “venture capitalists”).

### Images

Use Miro AI to create images on your boards. Here are some tips for creating better images:

- Specify the image style (i.e., “photorealistic,” “digital painting,” “impressionist”).
- Include relevant context from the board, such as a description of what the image should include (you can also include this in the prompt box, but if it already exists on the board, include it as context instead).
- Include any specific details the image should include (i.e., “the person is carrying a laptop” or “a stack of books is on the desk”).
- The more specific your prompt, the better your initial output will be.

## Editing and iterating with Miro AI

Miro AI is a tool for assisting with your work, not a replacement for human insights and knowledge. Editing and iterating is an important step in creating better outputs, both using AI and doing so manually.

When creating Formats with Miro AI, you’ll have the option to make edits before adding the content to your board. In Miro Prototypes and Miro Slides, you can edit one screen or slide at a time, but can do as many rounds of editing as you need. You can also revert to earlier versions at any time prior to adding the content to the board.

Here are some tips for editing with Miro AI:

- Specify one edit at a time when fine-tuning results. Entering too many instructions at once may provide unexpected results.
- Focus on the content, rather than the style, since you can only edit one screen or slide at a time.
- Try different phrasing or keywords if the output isn’t what you expected.

If you’ve created a Format that you want to iterate on but have already added it to the board, you can use that object as context for the next iteration. This is a good option if you decide you want to do something as simple as change the style of a slide deck or if you want to add additional screens in a prototype flow.

:::note
While using past AI-generated work as context for iterating new versions is a good starting point, the AI may change aspects of the work based on other prompting elements or additional context. Be sure to check all outputs.
:::
