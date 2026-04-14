---
title: "Aper\xE7u du tableau de bord de classification"
article_id: 26886219054354
translation_id: 26886219054354
locale: fr
sidebar_position: 3
created_at: '2025-05-22T11:26:15Z'
updated_at: '2025-08-18T09:36:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Le tableau de bord Classification offre une vue centralisée permettant aux administrateurs de suivre et de gérer la classification des tableaux au sein de leur organisation. Le tableau de bord fournit une répartition claire des tableaux classifiés et non classifiés, ce qui aide à assurer une couverture complète et à identifier les zones nécessitant une attention.

Les administrateurs peuvent également surveiller la méthode de classification utilisée—qu'elle soit manuelle, automatique ou non classifiée—pour comprendre comment les tableaux sont catégorisés. De plus, l'historique de la méthode de classification visualise les changements au fil du temps, offrant un aperçu des tendances et de l'efficacité de la classification continue des tableaux.

:::note
Indicateurs sur les mesures :

- Tous les indicateurs dans Enterprise Guard excluent les tableaux des équipes mises à la corbeille et les tableaux sous mise en suspens juridique.
- Toutes les métriques de classification excluent les modèles et les tableaux dans la corbeille.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Titre** | **Description** | **Domaine** | **Apparaît dans le tableau de bord d’aperçu** | **Possède un indicateur d'historique** |
| Nombre total de tableaux classifiés | Nombre de tableaux auxquels un badge de classification est attribué | Classification | ✅ | ❌ |
| Nombre de tableaux par classification | Nombre de tableaux par badge de classification (nom du badge) | Classification | ✅ | ❌ |
| Nombre de tableaux non classifiés | Nombre de tableaux sans badge de classification attribué | Classification | ✅ | ✅ |
| Nombre de tableaux classifiés manuellement | Nombre de tableaux ayant un badge de classification attribué manuellement (lire non par classification automatique) | Classification | ❌ | ✅ |
| Nombre de tableaux classifiés automatiquement | Nombre de tableaux avec un badge de classification attribué automatiquement par la classification automatique | Classification | ❌ | ✅ |

## Comprendre les erreurs, les états vides et les changements historiques

Comprendre comment interpréter les états vides et les messages d’erreur est essentiel pour lire avec précision les métriques du tableau de bord Enterprise Guard.

### Comprendre le comportement des données historiques lorsque les paramètres changent

Si une fonctionnalité, telle que la classification, est désactivée après que les données ont été collectées, les métriques historiques continueront d'afficher les valeurs de la période où elle était active. Par exemple, si vous désactivez la fonctionnalité de classification en mai et que la fonctionnalité de classification était active en avril avec 20 tableaux classifiés :

- Les valeurs d’avril continueront d’apparaître sur le tableau de bord.
- Le graphique de mai affichera **aucune donnée disponible**, car la collecte de données a cessé.
