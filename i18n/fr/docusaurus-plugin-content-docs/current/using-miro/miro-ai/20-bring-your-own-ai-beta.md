---
title: "Apportez votre propre IA (b\xEAta)"
article_id: 21885197978642
translation_id: 21885197978642
locale: fr
sidebar_position: 20
created_at: '2024-10-09T18:45:40Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: ai-generate-image
---

Bring Your Own AI (BYOAI) vous permet d'utiliser votre propre fournisseur d'IA au lieu de Miro IA, pour certaines fonctionnalités de Miro IA.

> **Disponible pour :** Enterprise
> **Disponible sur :** Bureau

Vous pouvez connecter votre fournisseur d'IA à Miro avec BYOAI, et tirer parti des [fonctionnalités d'IA qui s'appuient sur le GPT](18-miro-ai-reference.md). Les fonctions de Miro IA qui ne sont pas prises en charge par BYOAI, comme la génération d'images, peuvent être désactivées en option. Pour plus d'informations, consultez la section Désactivation des fonctionnalités d'IA non optimisées par Bring Your Own AI.

Actuellement, BYOAI prend en charge OpenAI et Azure OpenAI.

:::note
BYOAI ne prend en charge que les fonctions de Miro IA alimentées par GPT. Pour savoir quelles fonctions de Miro IA sont alimentées par GPT, consultez l'[aperçu de Miro IA.](18-miro-ai-reference.md)
:::

## Comment mettre en place le système Bring Your Own AI

> **Disponible pour :** les admins d’entreprise

Les procédures suivantes expliquent comment configurer le BYOAI (Bring Your Own AI) pour Open AI, et Azure OpenAI.

### OpenAI

Suivez les étapes suivantes :

1. Dans les paramètres d'administration, sélectionnez **Applications et intégrations**.
2. Sous **Intégration Enterprise**, pour **Bring your own AI (Apportez votre propre intelligence artificielle** ), sélectionnez **OpenAI**.
3. Pour la **clé API**, entrez votre clé OpenAI.
   > ⚠️ Pour une sécurité maximale, copiez et collez la clé API.
4. Sélectionnez **Connecter**.
5. Assurez-vous que l'option Miro IA est activée pour votre organisation.
   **En savoir plus :** Voir Activer Miro IA pour Bring Your Own AI (Apportez votre propre IA).

   Vous avez configuré avec succès BYOAI avec OpenAI.

:::note
Miro utilise un système de stockage à sens unique pour stocker et chiffrer en toute sécurité votre clé API, qui n'est jamais visible lors de la saisie de la clé. Miro ni les admins ne peuvent récupérer la clé API après sa mise à jour et son stockage sécurisé.
:::

### Azure OpenAI

Suivez les étapes suivantes :

1. Dans les paramètres d'administration, sélectionnez **Applications et intégrations**.
2. Sous la rubrique **Intégration Enterprise**, pour **Bring your own AI (Apportez votre propre IA** ), sélectionnez **Azure OpenAI**.
3. Saisissez votre clé d'API Azure, le nom du déploiement et l'URL du déploiement.
   > ⚠️ Pour une sécurité maximale, copiez et collez la clé API. Assurez-vous que le déploiement utilise GPT-4o.
4. Sélectionnez **Connecter**.
5. Assurez-vous que l'option Miro IA est activée pour votre organisation.
   **En savoir plus :** Voir Activer Miro IA pour Bring Your Own AI (Apportez votre propre IA).

   Vous avez configuré avec succès le BYOAI avec Azure OpenAI.

:::note
Miro utilise un système de stockage à sens unique pour stocker et chiffrer en toute sécurité votre clé API, qui n'est jamais visible lors de la saisie de la clé. Miro ni les admins ne peuvent récupérer la clé API après sa mise à jour et son stockage sécurisé.
:::

### Activez Miro IA pour Bring Your Own AI (Apportez votre propre IA)

Après avoir connecté Open AI ou Azure Open AI, assurez-vous que vous avez activé Miro IA pour votre organisation.

Suivez les étapes suivantes :

1. Dans les paramètres admin, sélectionnez **Accès aux fonctionnalités.**
2. Sous **Activation des fonctionnalités**, pour **Miro IA**, sélectionnez l'une des options suivantes :
   - **Tout le monde peut l’utiliser**
   - **Des équipes spécifiques peuvent l’utiliser**
3. (Facultatif) Activez les **fonctions bêta de Miro IA**.

   Vous avez activé avec succès Miro IA pour votre organisation.

:::note
Par défaut, toutes les fonctionnalités de Miro IA sont disponibles lorsque vous activez Miro IA. Pour désactiver les fonctions de Miro IA qui ne sont pas prises en charge par votre fournisseur d'IA, contactez l'assistance Miro. Pour en savoir plus, consultez la section Désactiver les fonctionnalités d'IA non optimisées par Bring Your Own AI.
:::

## Désactiver les fonctions d'IA qui ne sont pas alimentées par Bring Your Own AI

Par défaut, toutes les fonctionnalités de Miro IA sont disponibles lorsque vous activez Miro IA. Bring Your Own AI (BYOAI) ne prend en charge que les fonctions LLM, qui s'appuient sur GPT. Pour garantir que le BYOAI n'utilise que les fonctions LLM prises en charge par votre fournisseur d'IA, vous pouvez éventuellement désactiver les fonctions Miro IA qui ne sont pas des fonctions LLM.

Pour désactiver les fonctions Miro IA non LLM, contactez votre responsable Customer Success de Miro ou le [service d'assistance de Miro](../tools/troubleshooting/06-contacting-miro-support.md).

**En savoir plus :** Voir l'[aperçu de Miro IA.](18-miro-ai-reference.md)

## FAQ

**Qui est responsable de la création de la sortie AI lorsque j'utilise le BYOAI ?**

Avec BYOAI, vous prenez le contrôle de la production d'informations par l'IA, avec la qualité que vous avez définie avec votre fournisseur d'IA.

**Quel est l'impact de l'utilisation de mon propre fournisseur d'IA sur la modération des entrées ?**

Avec BYOAI, Miro ne filtre pas le contenu avant que votre fournisseur d'IA ne génère la sortie. Si vous préférez que la modération soit activée, veuillez vérifier si votre fournisseur a activé la modération des entrées, puis contactez votre responsable Customer Success ou le [service d'assistance de Miro](../tools/troubleshooting/06-contacting-miro-support.md).

**Quel est l'impact du BYOAI sur la consommation de crédits d'IA ?**

Avec BYOAI, vous consommez des jetons de votre propre fournisseur d'IA pour exécuter les fonctions d'IA de Miro. Vous continuez également à consommer des crédits d'IA Miro. Pour en savoir plus, consultez les [crédits d'IA de Miro pour les plans d'entreprise](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/03-miro-ai-credits-for-enterprise-plans.md).

**Que se passe-t-il si ma clé API expire ou si je n'ai plus de jetons ?**

En tant qu'admin, vous verrez un message d'erreur, et les utilisateurs finaux ne pourront plus utiliser les fonctionnalités d'IA alimentées par BYOAI.

**Comment puis-je obtenir de l'aide si je rencontre des problèmes avec l'intégration de mon fournisseur d'IA ?**

Contactez votre responsable Customer Success ou le service clientèle. Nous vous recommandons également de prendre contact avec votre fournisseur d'IA.

**Miro utilisera-t-il une entrée ou une sortie si j'utilise BYOAI ?**

Non, l'entrée et la sortie des données sont soumises à l'accord que vous avez conclu avec votre fournisseur.
