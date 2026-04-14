---
title: Bring your own AI (BETA)
article_id: 21885197978642
sidebar_position: 20
created_at: '2024-10-09T18:45:40Z'
updated_at: '2026-03-16T12:37:03Z'
draft: true
availability:
  plans: Desktop
---

Bring Your Own AI (BYOAI) enables you to use your own AI provider instead of Miro AI, for some Miro AI features.

You can connect your AI provider to Miro with BYOAI, and leverage [AI features that rely on GPT](18-miro-ai-reference.md). Miro AI features not supported by BYOAI, like image generation, can be optionally disabled. For more information, see [Disabling AI features not powered by Bring Your Own AI](#disabling-ai-features-not-powered-by-bring-your-own-ai).

Currently, BYOAI supports OpenAI and Azure OpenAI.

:::note
BYOAI only supports Miro AI features powered by GPT. To learn which Miro AI features are GPT-powered, see [Miro AI overview](18-miro-ai-reference.md).
:::

## How to set up Bring Your Own AI

> **Available for:** Company admins

The following procedures explain how to set up Bring Your Own AI (BYOAI) for Open AI, and Azure OpenAI.

### OpenAI

Follow these steps:

1. In admin settings, select **Apps and integrations**.
2. Under **Enterprise integration**, for **Bring your own AI** select **OpenAI**.
3. For **API key**, enter your OpenAI key.
   > ⚠️ For highest security, copy and paste the API key.
4. Select **Connect**.
5. Ensure that you have Miro AI enabled for your organization.
   **More information:** See [Enable Miro AI for Bring Your Own AI](#enable-miro-ai-for-bring-your-own-ai).

   You have successfully set up BYOAI with OpenAI.

:::note
Miro uses a one-way storage system to securely store and encrypt your API key, which is never visible during key input. Miro nor admins can retrieve the API key after the key is updated and stored securely.
:::

### Azure OpenAI

Follow these steps:

1. In admin settings, select **Apps and integrations**.
2. Under **Enterprise integration**, for **Bring your own AI** select **Azure OpenAI**.
3. Input your Azure API key, deployment name, and deployment URL.
   > ⚠️ For highest security, copy and paste the API key. Ensure the deployment is using GPT-4o.
4. Select **Connect**.
5. Ensure that you have Miro AI enabled for your organization.
   **More information:** See [Enable Miro AI for Bring Your Own AI](#enable-miro-ai-for-bring-your-own-ai).

   You have successfully set up BYOAI with Azure OpenAI.

:::note
Miro uses a one-way storage system to securely store and encrypt your API key, which is never visible during key input. Miro nor admins can retrieve the API key after the key is updated and stored securely.
:::

### Enable Miro AI for Bring Your Own AI

After you have connected Open AI or Azure Open AI, ensure that you have Miro AI enabled for your organization.

Follow these steps:

1. In admin settings, select **Feature access**.
2. Under **Feature activation**, for **Miro AI** select one of the following options:
   - **Everyone can use**
   - **Specific teams can use**
3. (Optional) Toggle **Enable Miro AI Beta Features** to the on position.

   You have successfully enabled Miro AI for your organization.

:::note
By default, all Miro AI features are available when you enable Miro AI. To disable Miro AI features not supported by your AI provider, contact Miro Support. To learn more, see [Disabling AI features not powered by Bring Your Own AI](#disabling-ai-features-not-powered-by-bring-your-own-ai).
:::

## Disabling AI features not powered by Bring Your Own AI

By default, all Miro AI features are available when you enable Miro AI. Bring Your Own AI (BYOAI) supports only LLM features, which leverage GPT. To ensure that BYOAI uses only LLM features that your AI provider supports, you can optionally disable non-LLM Miro AI features.

To disable non-LLM Miro AI features, contact your Miro customer success manager, or [Miro Support](../tools/troubleshooting/06-contacting-miro-support.md).

**More information:** See [Miro AI overview](18-miro-ai-reference.md).

## FAQ

**Who is responsible for creating AI output when I use BYOAI?**

With BYOAI, you take control of generating output with AI, with the quality that you have set with your AI provider.

**How does leveraging my own AI provider impact input moderation?**

With BYOAI, Miro does not filter content before your AI provider generates output. If you prefer to have moderation enabled, please validate if you have input moderation enabled by your provider and then, contact your customer success manager or [Miro Support](../tools/troubleshooting/06-contacting-miro-support.md).

**How does BYOAI impact AI credit consumption?**

With BYOAI, you consume tokens from your own AI provider to run Miro AI features. You also continue to consume Miro AI credits. To learn more, see [Miro AI Credits for Enterprise Plans](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/03-miro-ai-credits-for-enterprise-plans.md).

**What happens if my API key expires, or I run out of tokens?**

As an admin you will see an error message, and end users will no longer be able to use AI features powered by BYOAI.

**How do I get support if I experience issues with my AI-provider integration?**

Contact your customer success manager or customer support. We recommend that you also reach out to your AI provider.

**Will Miro use any input or output if I use BYOAI?**

No, the data input and output is subject to the agreement you have with your provider.
