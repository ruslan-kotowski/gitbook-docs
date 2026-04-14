---
title: Glean
article_id: 27381947979922
sidebar_position: 7
created_at: '2025-06-13T12:16:09Z'
updated_at: '2025-06-13T12:16:09Z'
draft: true
availability:
  roles: all_users
  plans: starter, business, enterprise, education
  platforms: desktop, browser
---

The Glean integration for Miro brings the power of Glean's AI-powered search directly into your Miro boards. You can access and use knowledge from across your company's apps right within the Miro canvas, boosting your team's productivity and collaboration.

By connecting Miro with Glean, you can centralize knowledge from over 100 source systems. This reduces the time your team spends switching between tools and helps accelerate projects from idea to outcome.

## Key features

- **Unified Search:** Connect all your workplace apps for a seamless, AI-driven search experience. This breaks down information silos and gives you instant access to the information you need.
- **Personalized Results:** Get relevant insights based on your past interactions and workflows, thanks to AI that understands intent and context.
- **Enhanced Collaboration:** Generate sticky notes, documents, and diagrams from your search results to improve collaboration and visualize information.
- **Insight Summaries:** With a single click, you can create insight summaries relevant to your work, improving productivity and decision-making.
- **Action Shortcuts:** Open the Glean AI app in the side panel for quick access to its features.
- **Source Navigation:** Easily review the sources used to generate information and navigate directly to the original data from Miro.

## Set up the Glean integration

You can install the Glean app from the Miro Marketplace. Admins will need to configure the app before it can be used.

1. On your Miro board, click the plus icon (+) on the creation toolbar and then click **Get more apps**.
2. Search for "Glean AI" in the Miro Marketplace and select it.
3. Click **Add** to install the app.
4. You will be prompted to authenticate with your Single Sign-On (SSO) provider. Glean supports Okta.
   > **Note:** While Azure is also available as an SSO option, it has not been fully tested by Miro and may not work as expected.
5. For the initial setup, a Company Admin must configure the app with your organization's Glean and Okta details.
6. The admin also needs to install the app for the teams in your organization that will use the integration.

## Use the Glean integration

Once the integration is set up, you can start using Glean within your Miro boards:

1. Open a Miro board and click the Glean icon in the toolbar to open the side panel.
2. Use the search bar in the Glean panel to find information from your connected workplace apps.
3. You can refine Glean's responses before generating content to ensure the outputs are tailored to your needs.
4. Generate sticky notes, documents, or diagrams based on the search results directly onto your board.
5. Use the action buttons to add the generated content to a custom template or your Miro board.

## Limitations

- **SSO Provider Dependency:** The availability of the integration depends on your SSO provider. Okta is fully supported. While Azure may work, it has not been fully tested and may have limitations.
- **Beta Features:** Some features of this integration are in beta. We welcome your feedback to help us improve them.

## Feedback and custom setups

- **Provide Feedback:** You are encouraged to provide feedback to help improve the integration through the app's feedback mechanisms.
- **Custom API Setups:** If you use custom apps, you can use the Miro developer platform to link Miro to your own Large Language Model (LLM).
