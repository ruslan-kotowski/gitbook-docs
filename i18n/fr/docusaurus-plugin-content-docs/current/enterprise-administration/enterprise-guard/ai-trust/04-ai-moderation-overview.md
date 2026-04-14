---
title: "Vue d'ensemble de la mod\xE9ration de l'IA (b\xEAta)"
article_id: 29491049430674
translation_id: 29491049430674
locale: fr
sidebar_position: 2
created_at: '2025-09-15T16:27:59Z'
updated_at: '2026-01-12T11:21:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Avec la modération de Miro IA, les admins d’entreprise peuvent ajuster les niveaux de filtre des prompts pouvant contenir du texte potentiellement nuisible ou inapproprié. Vous pouvez définir la sensibilité de la modération de Miro IA à l'échelle de l'organisation pour filtrer les contenus, y compris la haine, le contenu sexuel, la violence et l'automutilation. Cela vous aide à aligner l'utilisation de Miro IA avec les exigences, politiques et tolérance au risque de votre organisation.

:::note
*Si votre organisation relie son propre fournisseur de LLM (par exemple, une intégration directe avec OpenAI), le sélecteur de modération est désactivé et tout niveau précédemment choisi est ignoré pour cette intégration.*
:::

## Niveaux de modération

Contrôlez le contenu Miro IA dans toute votre organisation avec la modération Miro IA. Définissez le niveau de filtrage à Strict, Par Défaut, ou Minimal pour déterminer quels prompts sont bloqués. Consultez le tableau ci-dessous pour comparer rapidement les niveaux, puis explorez les sections détaillées pour obtenir plus de conseils.

| Niveau | Fonctionnement | Idéal pour | Compromis |
| --- | --- | --- | --- |
| Strict | Bloque Défault + contenu à risque faible à modéré. | Organisations fortement réglementées, enseignement. | Plus de faux positifs ; éventuel sur-filtrage. |
| Par défaut (recommandé) | Bloque le contenu modérément à hautement nuisible . | La plupart des cas d'utilisation professionnelle. | Certains contenus limites peuvent passer. |
| Minimal | Bloque uniquement le contenu extrêmement dangereux. | Contextes créatifs/jeux/médias. | Plus d'exposition à un danger faible à modéré. |

:::note
*Le niveau par défaut est recommandé pour la plupart des organisations. Il filtre le contenu que la majorité des gens considèrent comme inapproprié ou nuisible tout en maintenant une large accessibilité.*
:::

## Niveau strict

### Ce qu'il filtre

Tout ce qui est inclus dans le niveau par défaut, plus le contenu à faible risque à risque modéré (par exemple, discours de haine subtils ou codés, contenu sexuellement suggestif, violence non graphique, ou mentions non explicites d'automutilation).

### Quand l'utiliser

- Industries réglementées ou politiques organisationnelles averses au risque
- Programmes éducatifs ou axés sur les jeunes
- Programmes pilotes avec faible tolérance au risque

### Compromis

- Plus de faux positifs et de prompts en limite bloqués
- Nécessite des instructions pour réduire les frictions utilisateurs

## Niveau par défaut (recommandé)

### Ce qu'il filtre

Contenu modérément à gravement nuisible (discours haineux explicite, contenu sexuel explicite, violence graphique, incitations à l'automutilation).

### Quand l'utiliser

- La plupart des organisations recherchant un équilibre entre sécurité et convivialité

### Compromis

- Les prompts contextuels ou limites peuvent passer

## Niveau minimal

### Ce qu'il filtre

Uniquement le contenu gravement nuisible.

### Quand l'utiliser

- Équipes créatives qui ont besoin de plus de liberté d'expression (jeux, médias)
- Idéation interne avec des voies d'escalade claires

### Compromis

- Exposition accrue à du contenu de faible à moyenne nuisance dans les résultats

## Audit et conformité

Les changements du niveau de modération sont consignés dans le journal d'audit de l'organisation, y compris la valeur précédente, la nouvelle valeur, la personne qui l'a modifié et quand cela a été fait. Pour plus d'informations, consultez notre documentation sur les [journaux d'audit](../security-management/01-audit-logs.md).

## Bonnes pratiques

- Commencez avec le niveau par défaut, puis ajustez en fonction des avis et des retours des pilotes et des revues d’escalade.
- Associez le niveau Strict à des directives internes claires sur les prompts acceptables pour réduire les faux positifs.
- Si vous avez besoin du niveau Minimal, définissez quand les équipes doivent signaler ou escalader les sorties problématiques.
- Revisitez vos paramètres après des mises à jour majeures de politique ou de réglementation.

- Aperçu de la modération par l'IA
- Niveaux de modération
- Niveau strict
- Niveau par défaut (recommandé)
- Niveau minimal
- Audit et conformité
- Bonnes pratiques
