---
title: "D\xE9finir la classification automatique"
article_id: 16494707596050
translation_id: 16494707596050
locale: fr
sidebar_position: 9
created_at: '2024-01-19T19:01:08Z'
updated_at: '2025-11-25T15:40:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Pour vous aider à protéger votre contenu sensible, Enterprise Guard comprend une fonction de classification automatique des données, qui permet de classer les tableaux Miro en fonction de leur degré de sensibilité. La classification automatique représente une avancée significative dans la manière dont vous gérez et protégez vos données sensibles. L'automatisation du processus de classification permet à votre organisation de maintenir un niveau plus élevé de sécurité des données, de se conformer aux exigences réglementaires et d'offrir une meilleure expérience aux administrateurs de la sécurité. Le passage de la classification manuelle à la classification automatique est une évolution stratégique vers un cadre de sécurité des données plus précis, plus sûr et plus efficace.

Pour plus d'informations sur la classification automatique et des exemples de scénarios, voir [Vue d'ensemble de la classification automatique.](03-auto-classification-overview-and-scenarios.md)

## Définir la classification automatique

Il s'agit de la deuxième étape du flux de configuration de l'auto-classification et des garde-fous. Dans cette étape du flux, vous configurerez l'étiquette de sensibilité de l'auto-classification applicable à chaque niveau de classification. La classification des tableaux est automatiquement appliquée à tous les nouveaux tableaux et aux tableaux existants correspondant aux critères définis. Cette opération est effectuée après que vous avez examiné l'impact et décidé de publier des mises à jour.

## Prérequis

- [Vous devez activer la recherche de données](../data-discovery/13-activate-privacy-related-data-discovery.md).
- Vous devez effectuer la première étape du flux d'auto-classification et de garde-fous, [1 : Définir les niveaux de classification](07-define-classification-levels.md)
- Vous devez connaître les étiquettes de sensibilité que vous souhaitez attribuer à chaque niveau de classification en fonction de vos exigences en matière de sécurité et de gouvernance.
- Vous devez avoir le [rôle d'administrateur de contenu sensible.](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) Pour demander le rôle d’admin du contenu sensible, contactez l’admin de votre entreprise.

## Attribuez des des étiquettes de sensibilité pour l'auto-classification

Pour attribuer des étiquettes de sensibilité à un niveau de classification, procédez comme suit :

1. Sur la page **Définir l'auto-classification**, cliquez sur l'icône **Modifier** du niveau de classification pour lequel vous souhaitez attribuer les étiquettes de sensibilité. Par exemple, si vous souhaitez attribuer les étiquettes de sensibilité de classification automatique pour le niveau de classification **CONFIDENTIEL**, cliquez sur l'icône Modifier sur la ligne du niveau de classification **CONFIDENTIEL**.
2. Cochez la case de chaque étiquette de sensibilité que vous souhaitez attribuer à ce niveau de classification. Par exemple, si vous souhaitez classer automatiquement tous les tableaux qui contiennent les données sensibles liées au GDPR, cochez la case **GDPR Règlement général sur la protection des données.** Vous pouvez attribuer une ou plusieurs étiquettes de sensibilité par étiquette de classification.
3. Cliquez sur Done (Terminé).
   La classification des tableaux est automatiquement appliquée à tous les nouveaux tableaux et aux tableaux existants correspondant aux critères définis. Cette opération est effectuée après que vous avez examiné l'impact et décidé de publier des mises à jour.
4. Lorsque vous avez terminé d'attribuer des étiquettes de sensibilité pour les différents niveaux de classification, passez à l'étape [Terminer la configuration de l'auto-classification](09-define-auto-classification.md).

## Configuration complète de l'auto-classification

Une fois que vous avez terminé d'attribuer des étiquettes de sensibilité pour la classification automatique, cliquez sur **Suivant.** Votre configuration est sauvegardée, mais elle ne prendra effet que lorsque vous aurez cliqué sur **Publier** dans la fenêtre d'impact de l'examen. [**Examiner l'impact**](https://help.miro.com/hc/articles/16494764223378) sur la page Examiner l'impact.

Vous pouvez ensuite passer à l'une des étapes suivantes :

- Définir les garde-fous Cette option est facultative. Si vous souhaitez définir les garde-fous ultérieurement, cliquez sur **Suivant.**
- Examiner l’impact Il s'agit de la dernière étape du workflow et elle est obligatoire.
