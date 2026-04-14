---
title: How to integrate Miro and Tableau
article_id: 8948034187026
sidebar_position: 9
created_at: '2022-12-06T15:06:50Z'
updated_at: '2024-08-23T12:34:00Z'
draft: true
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: tableau
availability:
  roles: Tableau admin
  plans: '[Free](../../plans-billing/miro-plans/09-free-plan.md), [Starter](../../plans-billing/miro-plans/08-starter-plan.md),
    [Business](../../plans-billing/miro-plans/06-business-plan.md), and [Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
    plans'
---

Integrate Miro and Tableau so you and your users can add Tableau charts and dashboards to Miro boards as beautiful embeds.

![mceclip0.png](images/8946954685330_mceclip0.png)
*Example of a Tableau dashboard embed*

## How to add the Miro app in Tableau

1. In Tableau go to **Settings** > **Connected Apps** > click the **New Connected App** button:
   ![mceclip0.png](images/8970296327058_mceclip0.png)
*The option to create a new app in Tableau*
2. You will see a pop-up to define the name and the security levels (project access and domains' allowlist) of the new app. You may set the app however you like.
   ![mceclip1.png](images/8970375565330_mceclip1.png)
   *The new app pop-up*
3. Click to **Generate new secret** for this app:
   ![mceclip2.png](images/8970625365010_mceclip2.png)
   *The newly created app*
4. As a result, you will have the following values:
   - Secret ID,
   - Secret Value
   - Client ID

   Please provide the values to Miro. For security, we recommend using `https://onetimesecret.com/`
   When we have the values we will complete the integration on the backend and let you know when you can start using it.

> ✍️ The option to complete the integration autonomously without requiring our help is soon to be released.

## How to add embeds on the board

Simply paste any Tableau link onto the Miro board. The URL will automatically be converted into an embedded dashboard.
