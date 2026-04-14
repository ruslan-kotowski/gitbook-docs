---
title: "Aper\xE7u du tableau de bord Enterprise Guard"
article_id: 26707467343890
translation_id: 26707467343890
locale: fr
sidebar_position: 4
created_at: '2025-05-14T13:14:06Z'
updated_at: '2025-11-25T15:51:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: admin-analytics
---

## Vue centralisée de la sécurité et de la gouvernance

Le tableau de bord Enterprise Guard offre une vue centralisée et de haut niveau des insights sur la sécurité et la gouvernance de l'information de votre organisation dans une vue unifiée. Conçu pour les administrateurs d'Enterprise Guard, ce tableau de bord regroupe des indicateurs clés à travers des domaines centraux, y compris la Découverte de données, la Classification, le Cycle de vie du contenu et l'eDiscovery, dans une interface unique et consolidée. Il offre une visibilité rapide sur l'exposition actuelle, la couverture des politiques et l'état de préparation juridique, permettant aux administrateurs de détecter rapidement les risques potentiels, de prendre des mesures proactives en temps opportun et de traiter les points nécessitant une attention particulière.

## Indicateurs exploitables en temps réel

Chaque indicateur du tableau de bord Enterprise Guard reflète des données en temps réel, mises à jour quotidiennement. Tous les indicateurs sont exploitables et renvoient directement à leurs tableaux de bord de domaine respectifs, permettant aux administrateurs d'explorer des insights détaillés et de configurer les paramètres selon les besoins. Que vous surveilliez la sensibilité des tableaux, l'état de la classification, les politiques de conservation ou les mises en suspens juridiques, ce tableau de bord fournit un point de départ centralisé. Cette approche par calques assure la cohérence dans l'ensemble du produit Enterprise Guard et simplifie la navigation pour les admins occupés.

## Prise en charge de la gouvernance à grande échelle

Le tableau de bord Enterprise Guard est particulièrement utile pour les admins d'Enterprise Guard qui gèrent des déploiements à grande échelle avec le forfait Enterprise. Il apporte de la clarté aux configurations complexes de gouvernance de l’information et soutient la prise de décisions éclairées en regroupant les signaux les plus importants en un seul endroit. Dans le cadre de notre engagement pour une expérience Enterprise Guard plus intuitive, le tableau de bord Enterprise Guard aide les admins non seulement à comprendre ce qui se passe, mais aussi à savoir quoi faire ensuite, avec des liens pour agir directement à partir des données. Que vous fassiez un rapport à la direction ou que vous gériez la gouvernance des données au quotidien, ce tableau de bord vous garantit un accès rapide aux informations pertinentes, vous permet de hiérarchiser les actions et de démontrer la valeur de la stratégie de sécurité et de conformité de votre organisation.

## Tableaux de bord spécifiques au domaine

En plus du tableau de bord Enterprise Guard, les administrateurs peuvent explorer une suite de tableaux de bord spécifiques au domaine conçus pour fournir des insights plus profonds et un contrôle accru sur les domaines clés de la gouvernance. Chacun de ces tableaux de bord permet de prendre des décisions ciblées dans son domaine spécifique tout en maintenant l'alignement avec le cadre plus large d'Enterprise Guard. Ceux-ci incluent :

- **Tableau de bord Découverte de données :** identifiez et analysez où se trouvent les informations sensibles sur vos tableaux.
- **Tableau de bord de classification :** suivez et gérez la couverture de classification au niveau du tableau et les badges de sensibilité.
- **Tableau de bord du cycle de vie du contenu :** surveillez les politiques de conservation des données et automatisez les actions de gestion du cycle de vie.
- **Tableau de bord eDiscovery :** obtenez une visibilité sur les mises en suspens juridiques et rationalisez les workflows de préparation eDiscovery.

## Comprendre les indicateurs du tableau de bord

Les tableaux de bord Enterprise Guard incluent deux types de métriques : les métriques actuelles et les métriques historiques. Pour garantir la clarté et la cohérence, chaque métrique présentée dans les tableaux de bord Enterprise Guard est définie dans la [documentation des métriques des tableaux de bord Enterprise Guard](07-enterprise-guard-dashboard-metrics-reference.md).

:::note
Notes sur les indicateurs :

- Tous les indicateurs dans Enterprise Guard excluent les tableaux des équipes mises à la corbeille et les tableaux sous mise en suspens juridique.
- Tous les indicateurs de classification excluent les modèles et les tableaux dans la corbeille.
:::

## Comprendre les erreurs, les états vides et les changements historiques

Comprendre comment interpréter les états vides et les messages d’erreur est essentiel pour lire avec précision les métriques du tableau de bord Enterprise Guard.

### Comprendre le comportement des données historiques lorsque les paramètres changent

Si une fonctionnalité, telle que la classification, est désactivée après que les données ont été collectées, les métriques historiques continueront d’afficher les valeurs de la période active. Par exemple, si vous désactivez la classification en mai et qu'elle était active en avril avec 20 tableaux classifiés :

- Les valeurs d’avril continueront d’apparaître sur le tableau de bord.
- Le graphique de mai affichera **aucune donnée disponible**, car la collecte de données a cessé.
