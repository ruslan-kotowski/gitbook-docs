---
title: "Examiner l\u2019impact"
article_id: 16594793714066
translation_id: 16594793714066
locale: fr
sidebar_position: 5
created_at: '2024-01-24T19:34:48Z'
updated_at: '2025-08-18T09:36:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
id: 06-review-impact
---

Il s'agit de la dernière étape du flux de configuration de l'auto-classification et des garde-fous. Dans cette étape du flux, vous devez examiner l'impact des mises à jour de la classification ou de la configuration des garde-fous. Dans cette étape du flux, vous devez examiner l'impact des modifications que vous apportez à la configuration de la classification ou des garde-fous. Les sections suivantes décrivent les informations disponibles dans la page d'impact de la révision et les différentes actions que vous pouvez entreprendre.

## Distribution des niveaux de classification

Cette section vous permet d'examiner l'impact de votre configuration mise à jour en termes de changements pour chaque niveau de classification des tableaux.

La section **Distribution des niveaux de classification** est repliable, ce qui vous permet de faire défiler plus efficacement la liste des mises à jour (voir figure 1).

![Repliable Répartition de la section des niveaux de classification](images/24937307965842_Collapsible_Distribution_of_classification.png)

*Figure 1 : Repliable Répartition de la section des niveaux de classification*
L'interface utilisateur basée sur des colonnes simplifie le processus de comparaison et d'examen des mises à jour de la classification des tableaux. Nous avons prévu des colonnes distinctes qui affichent le nombre de tableaux ajoutés, le nombre de tableaux supprimés et le total actualisé pour chaque niveau de classification (figure 2).

![Interface utilisateur à colonnes affichant le nombre de tableaux ajoutés, le nombre de tableaux retirés et le total actualisé pour chaque niveau de classification.](images/24937307971602_columnview.png)

*Figure 2 : Interface utilisateur à colonnes affichant le nombre de tableaux ajoutés, le nombre de tableaux retirés et le total actualisé pour chaque niveau de classification.*

La fonction d'analyse descendante offre une vue d'ensemble (figure 3) des détails suivants :
- Ajout ou suppression d'étiquettes de classification automatique.
- Ajout ou suppression de garde-fous.
- Nombre de tableaux qui sont passés à un niveau de classification spécifique.
- Nombre de tableaux non affectés par les changements de configuration que vous avez effectués.

![Fonction d'exploration avec vue d'ensemble des mises à jour](images/24937307973522_drilldown_feature_classification.png)

*Figure 3 : Fonction d'exploration avec vue d'ensemble des mises à jour*

## Impact des garde-fous

Cette section affiche les garde-fous qui seront appliqués en fonction du niveau de classification d'un tableau, le nombre total de tableaux qui auront chaque garde-fou spécifique. Le chiffre entre parenthèses indique le nombre de tableaux pour lesquels le garde-fou est ajouté ou retiré après la publication de la nouvelle configuration. En outre, cette section indique également le nombre de tableaux non classés (figure 4).

Pour mettre à jour la configuration des garde-fous, cliquez sur **Précédent.**
*![Configurer la classification Examiner l'impact](images/24937307976850_guardrails.png)
Figure 4 : Configurer la classification > Examiner l'impact*

## Mettre à jour la configuration des garde-fous

Pour effectuer des mises à jour après avoir examiné l'impact des mises à jour que vous avez apportées à la configuration de l'auto-classification et des garde-fous, cliquez sur le bouton **Précédent**, effectuez les mises à jour de la configuration, puis examinez à nouveau l'impact.

## Publier la configuration

Après avoir examiné l'impact de la classification ou de la configuration des garde-fous que vous avez effectuée, cliquez sur **Publier**.

:::note
**Notes** :
- La configuration du niveau de classification est appliquée immédiatement.
- La configuration des garde-fous est appliquée immédiatement.
- Lorsque de nouveaux tableaux contenant des données sensibles sont ajoutés, ces tableaux sont classés automatiquement à l'issue du prochain cycle de découverte des données.
- Lorsque le contenu des tableaux est mis à jour (suppression ou ajout de contenu sensible), ces tableaux sont classés automatiquement à l'issue du prochain cycle de découverte des données.
:::
