---
title: Miro AI Admin security
article_id: 11277533556626
sidebar_position: 4
created_at: '2023-05-02T11:08:21Z'
updated_at: '2026-03-27T16:19:31Z'
draft: false
availability:
  plans: free, starter, business, enterprise, education
---

This article explains for admins how Miro ensures Enterprise-grade security, how to enable and disable Miro AI, and frequently asked questions.

**More information:** See [Miro AI Whitepaper](../../canvas-25-admin-features/data-security/05-miro-ai-whitepaper.md)

## What is Miro AI?

Unlock the power of your ideas with Miro AI–your new launchpad for creativity, collaboration, and productivity.

Miro uses machine learning models along with your input to generate or modify content on your board. Miro AI can do things like generate mind maps, summarize content, generate sticky notes, and more.

**More information:** [Overview of Create and Edit with AI](../../../using-miro/miro-ai/03-create-with-ai.md)

## Enterprise-grade security

Miro is the enterprise-ready online workspace for innovation that empowers distributed teams of any size to dream, design, and build the future together.

However, great collaboration requires great security, which is why we offer industry best practices and standards to ensure your information is as secure as possible. Read on to learn how we secure your boards and content.

|  |  |  |
| --- | --- | --- |
| **Checkmark.png**  **Approved and certified** | **Security_lock.png**  **Trusted protection** | **Fingerprint.png**  **Secure access management** |
| Industry best practices and regulatory requirements | Protect and manage your intellectual property | Who can access Miro AI |
| - Generally, your Miro data is stored at rest on servers in the EU, US, and AU depending on your data residency. However, your interactions with Miro AI may be processed outside your selected region, depending on model availability in-region. For more information, see [Data Residency at Miro](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md). - Data is not retained and is not used to train AI models. - To learn about participation and usage provisions, see [AI Features Addendum](https://miro.com/legal/ai-features-addendum/). - To learn more about how Miro AI processes data, see [Miro AI Privacy Policy](https://miro.com/legal/privacy-policy/#miro-ai). | - Miro AI conforms to ISO 27001 and SOC2 certifications and privacy commitments. - To learn how we approach security, our governance model, and how we stay compliant with GDPR & CCPA, visit our [Trust Center](https://miro.com/trust/). - Miro asserts no rights to the content that is created by Miro AI. To learn more, see the FAQ at the end of this article. | - Miro AI is available for Members only. Guests and visitors cannot use Miro AI. |

## How to enable and disable Miro AI

> **Available for:** Enterprise, Education Plans

Follow these steps:

1. Go to **Admin Console**.
   From the **Home** dashboard, in the top-right select your avatar. Then click **Admin Console.** Or from any board, click your avatar and select **Profile settings**.
2. Go to **Miro AI** > **Capabilities**.
3. Under **Miro AI**, select one of the following options:
   - **No one can use**
     Disables Miro AI for your entire company
   - **Everyone can use**
     Enables Miro AI for your entire company
   - **Specific teams can use**
     Enables Miro AI only for teams that you specify.
4. (Optional) Enable Miro AI beta features.
   You have successfully enabled or disabled Miro AI.

## FAQ

### Miro AI models & model training

**How will my data be used?**

The data submitted through Miro AI are used solely to generate a response from the AI model and provide that response back to the user. Depending on the AI feature used, the AI model might be hosted in Miro or in Microsoft Azure AI. In both cases, the input data submitted are not used for model training, and content and usage data will be used according to Miro’s [Privacy Policy](https://miro.com/legal/privacy-policy/).

**Where is my data processed?**

Generally, your Miro data is stored at rest on servers in the EU, US, and AU depending on your data residency. However, your interactions with Miro AI may be processed outside your selected region, depending on model availability in-region. For more information, see [Data Residency at Miro](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md).

**Which AI models does Miro AI use?**

To learn which AI models Miro AI uses, see [Miro AI overview](../../../using-miro/miro-ai/18-miro-ai-reference.md).

**Does Miro train models with customer data?**

Miro does not use customer data for training or refining models. In the future, if Miro introduces the ability to use customer data to improve models and performance of Miro AI functionality, Miro will offer self-serve customers the ability to opt-out. Enterprise customers will be opt-out by default and need to explicitly opt in.

**How often is the Miro AI model updated?**

Miro uses different Azure OpenAI models for different use cases. The updates largely depend on the model updates pushed by Azure. In-house models are updated on a need basis to ensure quality results.

### Reliable & safe AI

**Who owns the intellectual property rights to the content that is created by Miro AI?**

As between Miro and you, Miro asserts no rights to the content that is created by Miro AI. Rights to the output generated by Miro AI are determined by the underlying AI providers themselves. For example, in the Microsoft Azure AI (OpenAI terms of use), OpenAI assigns to you all right, title, and interest to the output generated and returned by its services. For more information, see [AI Features Addendum](https://miro.com/legal/ai-features-addendum/) and [Miro AI Privacy Policy](https://miro.com/legal/privacy-policy/#miro-ai).

**Are AI results validated and correct?**

Due to the nature of LLMs, not all generated content may be accurate. The output should always be checked before using it.

**How does Miro ensure that no malicious or illegal prompts are used?**

Miro partners with Azure and leverages their content moderation services to filter out malicious or inappropriate outputs. Miro do not offer prompt tracking.
