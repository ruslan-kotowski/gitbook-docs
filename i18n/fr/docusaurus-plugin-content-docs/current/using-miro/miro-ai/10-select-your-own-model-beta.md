---
title: Sélectionnez votre propre modèle (bêta)
article_id: 29484232754578
translation_id: 29484232754578
locale: fr
sidebar_position: 10
created_at: '2025-09-15T12:50:30Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-sidekicks
availability:
  notes: 'Qui peut le faire: Membres de l''équipe Quels forfaits: Free, Starter, Business,
    Enterprise Quelles plateformes: Navigateur, Desktop, Mobile'
---

Lorsque vous effectuez des actions d'IA avec Miro [flux](04-flows-overview.md) et partenaires d’IA, la fonction Sélectionner Votre Propre Modèle vous permet de spécifier le modèle de langue de grande taille (LLM) le plus approprié pour la tâche.

Par exemple, pour la génération d'images, vous pouvez décider d'utiliser Stable Diffusion 3.5 Large ou Gemini 2.5 Flash Image (Nano Banana).

Votre choix peut dépendre de la complexité ou de la spécificité de votre tâche.

:::tip
Les flux et partenaires d’IA de Miro incluent un LLM par défaut pré-sélectionné pour chaque tâche. Lorsque vous n'êtes pas sûr du modèle à choisir, utiliser le modèle par défaut est le meilleur choix. Le modèle par défaut est indiqué par un badge "Recommandé".
:::

Le sélecteur de modèle est disponible uniquement dans le cadre des flux et partenaires d’IA pour les éléments suivants :

- Documents et Formats d’image dans Partenaires d’IA et Flux
- Logique principale des partenaires d’IA
- Bloc d’instructions dans les flux

Cet article explique comment sélectionner votre propre modèle pour les flux et partenaires d’IA, et fournit des informations pour vous aider à choisir un LLM pour les tâches courantes.

## Sélectionner votre propre modèle

### Flux

Les documents, les images et les Blocs d'instruction dans un flux ont chacun une boîte de prompt où vous pouvez sélectionner votre propre modèle.

Suivez les étapes suivantes :

1. Ajoutez un document, une image ou un Bloc d'instruction sur le canevas.
2. Pour accéder à la liste des modèles disponibles, dans le coin supérieur droit de la boîte de prompt, cliquez sur le nom du modèle par défaut. Par exemple, `AWS | Claude 3.5`.
3. Sélectionnez un modèle.

Pour en savoir plus sur la création de Flux et l'expérience utilisateur des Flux, consultez [Flux](05-flows.md).

### Partenaires d’IA

Lors de la création ou de la modification de partenaires d’IA, vous voyez la section **Modèle (avancé)**, et vous pouvez sélectionner le modèle que vous souhaitez utiliser pour le traitement du partenaire d’IA, la génération d'images et la génération de documents.

Pour en savoir plus sur les partenaires d’IA, voir la [documentation sur les partenaires d’IA](08-ai-sidekicks.md).

## Comment les modèles diffèrent

Un modèle de langage large (LLM) est généralement un membre d'une famille de modèles qui inclut des modèles performants mais gourmands en ressources, des modèles optimaux et les modèles les plus rapides mais moins performants.

Par exemple, la famille GPT-5 comprend GPT-5, GPT-5-mini et GPT-5-nano.

Les modèles les plus rapides mais les moins performants sont idéaux pour une latence réduite.

### Raisonnement et non-raisonnement

Un différenciateur principal entre les LLM est les modèles de raisonnement par rapport aux modèles sans raisonnement.

*Raisonnement* signifie que le modèle prend plus de temps pour fournir une réponse de meilleure qualité.

:::note
Le *raisonnement* ne signifie pas toujours le résultat le plus précis. Si vous avez besoin de nombreuses itérations, un raisonnement élevé peut ne pas être le plus efficace.
:::

Pour les tâches complexes, comme la création de documents à destination des clients, la priorisation et les tâches nécessitant le traitement d'un grand volume d'informations, un modèle de raisonnement est le meilleur choix.

Pour des tâches simples comme la vérification de la grammaire, la traduction ou la reformulation du texte, un modèle sans raisonnement est le choix le plus efficace.

Le tableau suivant montre quelques modèles de raisonnement et sans raisonnement.

| Capacité de raisonnement | Modèles |
| --- | --- |
| Raisonnement | GPT-5, GPT-5-mini, GPT-5-nano, Claude Sonnet 4, Claude Sonnet 4.5, Gemini 2.5, Gemini 2.5 Flash, o3, o4-mini |
| Non-raisonnement | GPT 4o, GPT-4o-mini, GPT-4.1, GPT-4.1-mini, Claude Sonnet 3.7, Claude Sonnet 3.5, Gemini 2.5 Flash Lite |

### Style

Chaque LLM possède un "style" unique. En expérimentant différents modèles, vous pourriez remarquer qu'un style de résultat particulier correspond à vos exigences, que ce soit pour le branding, l'ambiance ou votre préférence.

:::tip
Les anciens modèles ont un style plus distinct, surtout pour des résultats créatifs et originaux.
:::

## Sélectionner votre modèle d’IA par tâche

| Tâche | Modèles | Description |
| --- | --- | --- |
| Brainstorming | GPT-4o, o3, o4-mini, Sonnet 3.7 | Idéal pour la pensée divergente, les jaillissements d'idées pour les fonctionnalités, un ton ludique et une « touche créative ». Utilisez-le pour générer du texte, comme des titres alternatifs et des variantes de microtextes, par exemple. |
| Priorisation & notation | GPT-5, Claude Sonnet 4.5, Gemini 2.5 | Les meilleurs modèles de raisonnement pour des notations cohérentes et des justifications claires. Par exemple, RICE/MoSCoW sur le backlog, les compromis écrits et les niveaux de roadmap. |
| Synthèse & recherche | GPT-5, GPT-5-mini, Claude Sonnet 4.5, GPT-4.1, Claude Sonnet 3.7, Gemini 2.5 Flash | Utilisez pour des tâches de complexité moyenne à élevée. Par exemple, pour générer des personas à partir de notes et pour dériver des insights à partir de bases de données et de connaissances. |
| Schéma & transformation | GPT-5-mini, GPT-5-nano, GPT-4.1, Sonnet 3.7, Gemini 2.5 Flash, Gemini 2.5 Flash Lite | Les changements de format ne nécessitent généralement pas de raisonnement complexe, donc les versions optimisées donneront des résultats plus rapides, mais restez sur les dernières familles de modèles pour assurer la cohérence lors du traitement de contextes volumineux. notes → documents, document → table, spécifications → diagramme) |
| Corrections textuelles rapides | GPT-4o-mini, Gemini 2.5 Flash Lite, GPT-5-nano, Claude 3.7 | Options les plus rapides. Idéal pour les corrections simples de texte, comme la grammaire, la traduction et la réécriture pour plus de clarté. |

## Sélection des modèles pour la génération d'images

Tous les modèles de langage étendu (LLM) pris en charge par Miro peuvent traiter du texte et des images. Cependant, la plupart ne peuvent pas générer d'images.

Pour la génération d'images, Gemini 2.5 Flash Image (Nano Banana) excelle à convertir vos instructions générales en image.

La plupart des LLM s'attendent à une description d'image, pas à des instructions spécifiques. Par exemple, "une peinture d'un chien avec un chapeau drôle" comme description, contre "créer une image drôle de chien" comme instruction. Nano Banana est capable de générer des images à partir d'instructions spécifiques.

:::note
Utilisez Nano Banana pour des modifications ciblées sur une image existante. D'autres modèles peuvent utiliser une image existante comme référence de style.
:::

En termes de vitesse ou de qualité de sortie, il y a peu de différence entre les LLM. Comme pour chaque cas d’utilisation, vous pouvez expérimenter différents modèles pour trouver celui qui convient le mieux à vos préférences.
