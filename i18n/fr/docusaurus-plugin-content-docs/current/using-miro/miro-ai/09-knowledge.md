---
title: Connaissances
article_id: 29737566936850
translation_id: 29737566936850
locale: fr
sidebar_position: 9
created_at: '2025-09-25T08:24:51Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: sticky-notes
availability:
  notes: 'Qui peut le faire: Membres de l''équipe Quels forfaits: Business, Enterprise
    Quelles plateformes: Navigateur, Bureau, Mobile'
---

Le savoir dans Miro s'intègre avec des fournisseurs comme Glean, Microsoft Copilot (bêta) et Miro Insights, pour rendre les connaissances de votre entreprise accessibles et exploitables directement sur le canevas.

Le savoir permet aux équipes de récupérer des informations internes et des résultats de recherche web de manière transparente, et d'utiliser le canevas de Miro comme prompt pour un développement plus rapide.

Connectez les systèmes de connaissances que vous utilisez déjà, puis convertissez facilement ce que votre entreprise sait en formats comme documents, tables, pense-bêtes et diapositives.

Le savoir supporte les intégrations suivantes, y compris la recherche web.

- [Amazon Q](../../integrations-apps/amazon-web-services-aws/03-amazon-q-beta.md) (bêta)
- [Gemini Enterprise](../../integrations-apps/google/01-gemini-enterprise-integration.md) (bêta)
- [Glean](../../integrations-apps/glean/01-glean-for-miro.md)
- [Microsoft Copilot](../../integrations-apps/microsoft/01-microsoft-copilot-integration.md) (bêta)
- [Miro Insights](../tools/use-miro-insights/02-use-miro-insights-on-the-canvas.md)

Les admins de l’entreprise doivent activer et approuver chaque intégration pour leurs équipes.

:::note
Certaines intégrations, comme Microsoft Copilot et Gemini Enterprise, nécessitent des licences payantes auprès du fournisseur concerné.
:::

Pour en savoir plus sur les intégrations spécifiques de connaissances, consultez [Intégrations & Applications](../../integrations-apps).

## Fonctionnalités clés

- **Intégrations de connaissance**
  Les connaissances connectent Miro à des fournisseurs de premier plan comme [Glean](../../integrations-apps/glean/01-glean-for-miro.md), [Microsoft Copilot](../../integrations-apps/microsoft/01-microsoft-copilot-integration.md) (bêta), [Amazon Q](../../integrations-apps/amazon-web-services-aws/03-amazon-q-beta.md) (bêta) et Miro Insights, ce qui vous permet de récupérer et d'appliquer les connaissances de votre entreprise directement sur le canevas.
- **Connaissances d'entreprise comme prompt**
  Utilisez les connaissances récupérées comme contexte pour solliciter [Miro IA](01-miro-ai-overview.md) et passer plus rapidement de l'idéation à la création.
- **Points d'entrée multiples**
  La connaissance est accessible à plusieurs points d'entrée dans Miro, tels que [partenaires d’IA](07-sidekicks.md) et [flux](04-flows-overview.md), vous assurant de spécifier le contenu le plus pertinent pour une étape donnée de votre workflow.

:::note
Les admins peuvent gérer les permissions de Connaissance et de Miro IA, les capacités de recherche web, et la création de modules pour garantir la conformité avec les politiques de leur organisation.
:::

## Utiliser la Connaissance pour récupérer les informations de l'entreprise

Accédez à Connaissance à l'un des points d'entrée suivants.

:::note
Lorsque vous connectez un fournisseur de connaissances pour la première fois, une authentification est requise.
:::

- [**Partenaires d’IA**](06-sidekicks-overview.md)
  Au-dessus de la barre de création, cliquez sur **Partenaires d’IA**. Le panneau **Partenaire d’IA** s'ouvre. Dans la boîte de prompt, cliquez sur **Knowledge**. Connectez ou basculez un fournisseur de connaissances en position "activé".
  ![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)*Dans le panneau Partenaire d’IA, sélectionnez un fournisseur de connaissances pour récupérer les connaissances de l'entreprise dans Miro.*
  Rédigez votre prompt de partenaire d’IA. Vous pouvez éventuellement sélectionner des objets sur le canevas pour ajouter du contexte. Lorsque vous exécutez votre prompt, Knowledge exploite le ou les fournisseurs que vous avez sélectionnés.

  > 💡 Utilisez le module Connaissance pour créer des partenaires d’IA spécialisés qui vous aident avec des tâches sur le canevas en tant qu'agents IA personnalisés.
- [**Documents**](04-flows-overview.md) **dans les flux**
  Dans le menu contextuel du Document, cliquez sur **Modifier avec IA**. Le panneau **Partenaire d’IA** s'ouvre. Dans la boîte de prompt, cliquez sur **Connaissance**. Connectez ou sélectionnez un fournisseur de connaissance. Lorsque vous exécutez votre prompt, le module Connaissance utilise le fournisseur que vous avez sélectionné.
- [**Bloc d'instruction IA**](05-flows.md) **dans les flux**
  Dans un bloc d'instruction IA, cliquez sur **Sélectionner la base de connaissances.** Connectez ou sélectionnez un fournisseur de connaissances. Lorsque vous exécutez votre instruction IA, Knowledge exploite le fournisseur que vous avez sélectionné.
- **Chat indépendant**
  Vous pouvez accéder aux ressources de Connaissances dans l'application de chat indépendante de Miro.
  - Au-dessus de la barre de création, cliquez sur **partenaires d’IA**. Le panneau **partenaire d’IA** s'ouvre. Au-dessus de **Salut \{Votre nom\}**, cliquez sur la flèche vers le bas, puis sur **Explorer plus de partenaires d’IA**. Cliquez sur l'onglet **Connaissances**.
  - Dans la barre de création, sélectionnez **Outils, médias et intégrations**. Recherchez et sélectionnez votre fournisseur de Connaissances. Par exemple, **Gemini**.Le panneau de chat s'ouvre.
