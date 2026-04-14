---
title: "D\xE9finir ou mettre \xE0 jour le niveau de mod\xE9ration de Miro IA (b\xEA\
  ta)"
article_id: 30613174297618
translation_id: 30613174297618
locale: fr
sidebar_position: 3
created_at: '2025-10-29T01:15:35Z'
updated_at: '2026-01-12T11:22:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Avec la modération de Miro IA, les admins d’entreprise peuvent ajuster les niveaux de filtrage des prompts qui pourraient mener à des sorties potentiellement nuisibles ou inappropriées. Vous pouvez contrôler la sensibilité de la modération Miro IA à travers votre organisation et filtrer par catégories telles que la haine, le contenu sexuel, la violence et l'automutilation. Cela vous aide à aligner l'utilisation de Miro IA avec les exigences, les politiques et la tolérance au risque de votre organisation.

**Remarque** : Si votre organisation connecte son propre fournisseur de LLM (par exemple, une intégration directe avec OpenAI), le sélecteur de modération est désactivé et tout niveau précédemment choisi est ignoré pour cette intégration.

## Prérequis

- Assurez-vous de disposer du module complémentaire Enterprise Guard.
- Assurez-vous d'être un **Admin de l'entreprise** pour l'organisation que vous souhaitez configurer.
- Examinez vos exigences de gouvernance et de politique pour choisir un niveau de départ approprié. Le mode par défaut est recommandé pour la plupart des organisations.

## Définir ou mettre à jour le niveau de modération de Miro IA

1. Ouvrez les **Paramètres** de votre organisation dans Miro.
2. Allez dans **Miro AI** › **Modération**.
3. Choisissez un niveau :
   - **Strict :** Bloque tout ce qui est filtré par Défaut, ainsi que les contenus à risque faible à modéré (par exemple, haine subtile ou codée, contenu sexuellement suggestif, violence non graphique, mentions de l'automutilation non explicites).
   - **Défaut (recommandé) :**  Bloque les contenus modérément à gravement nuisibles (par exemple, haine explicite, contenu sexuel explicite, violence graphique, incitation à l'automutilation).
   - **Minimal :** Bloque uniquement les contenus gravement nuisibles.
4. Cliquez sur **Confirmer**.
   Le changement est appliqué immédiatement à toute l'organisation et est enregistré dans le journal d'audit.

## Valider le niveau de modération (facultatif)

- Demandez à un groupe pilote de tester des prompts typiques et de signaler tout excès ou défaut de filtrage.
- Surveillez les canaux de service d’assistance ou d'escalade pour détecter les faux positifs ou les préjudices manqués pendant la première semaine suivant un changement.

## Conseils et meilleures pratiques

- Commencez avec **Par défaut**, puis ajustez en fonction des retours du groupe pilote et des examens des escalades.
- Si les utilisateurs signalent trop de prompts bloqués, essayez **Par défaut** (à partir de Strict) ou **Minimal** (à partir de Par défaut) et publiez des exemples de prompts acceptables.
- Si du contenu limite passe à travers, passez à **Strict** et ajoutez des directives internes pour réduire les frictions.
- Réexaminez le niveau après des changements de politiques, réglementations ou cas d'utilisation.

## Résolution des problèmes

**Le contrôle de modération est désactivé**
Une intégration LLM personnalisée est connectée. Déconnectez-la pour réactiver le sélecteur. Tant qu'elle est connectée, tout niveau précédemment choisi est ignoré pour cette intégration.

**Trop de faux positifs**
Envisagez de passer de **Strict → Default** et partagez des exemples d'utilisation acceptable. Consultez les modifications récentes dans le journal d'audit pour confirmer le calendrier.

**Exposition à des contenus nuisibles**
Assurez-vous que le niveau n'est pas **Minimal**. Envisagez **Default** ou **Strict** en fonction de votre tolérance au risque.

**Les utilisateurs ne savent pas pourquoi les prompts sont bloqués**
Publiez des directives internes indiquant le niveau choisi, des exemples de prompts et les voies d'escalade.
