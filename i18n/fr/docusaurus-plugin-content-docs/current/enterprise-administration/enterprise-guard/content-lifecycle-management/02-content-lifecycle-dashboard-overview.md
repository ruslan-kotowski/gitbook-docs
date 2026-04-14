---
title: "Aper\xE7u du tableau de bord du cycle de vie du contenu"
article_id: 26894063726482
translation_id: 26894063726482
locale: fr
sidebar_position: 2
created_at: '2025-05-22T16:02:58Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

Le tableau de bord du cycle de vie du contenu offre une vue centralisée permettant aux administrateurs de surveiller et de gérer le cycle de vie complet des tableaux, depuis leur création jusqu'à leur suppression, tout en étant en conformité avec les politiques de conservation des données de l'organisation. Il offre une visibilité sur la phase actuelle du cycle de vie de chaque tableau, aidant à garantir une gestion appropriée du contenu.

Les administrateurs peuvent également suivre les tableaux régis par des politiques de conservation et de suppression, et consulter les tendances historiques de l'application des politiques. Le tableau de bord inclut une prévision de suppression, permettant une planification proactive des actions automatisées du cycle de vie à venir. Cela active une gouvernance de contenu cohérente et basée sur des politiques dans l'ensemble de l'organisation.

:::note
Tous les indicateurs d'Enterprise Guard excluent les tableaux des équipes en corbeille et les tableaux sous mise en suspens juridique.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Titre** | **Description** | **Domaine** | **Apparaît dans le tableau de bord d’aperçu** | **Possède un indicateur d’historique** |
| Nombre total de tableaux | Nombre total de tableaux dans tous les états du cycle de vie (actif, corbeille, conservé) | Gestion du cycle de vie du contenu | ✅ | ❌ |
| Nombre de tableaux actifs Notez que ceci n’est PAS l’activité des tableaux mais des tableaux qui sont dans l’état de cycle de vie actif | Nombre total de tableaux dans l'état de cycle de vie actif | Gestion du cycle de vie du contenu | ✅ | ✅ |
| Nombre de tableaux dans la corbeille | Nombre total de tableaux dans l’état de cycle de vie supprimé | Gestion du cycle de vie du contenu | ✅ | ✅ |
| Nombre de tableaux conservés | Nombre total de tableaux dans l’état de cycle de vie conservé | Gestion du cycle de vie du contenu | ✅ | ✅ |
| Nombre de tableaux en cours de conservation | Nombre total de tableaux qui ont au moins une politique de conservation non expirée assignée. | Gestion du cycle de vie du contenu | ❌ | ✅ |
| Nombre de tableaux en cours de suppression | Nombre total de tableaux auxquels au moins une politique de suppression non expirée est assignée | Gestion du cycle de vie du contenu | ❌ | ❌ |
| Nombre de tableaux suivant une politique de conservation, regroupés par politique | Nombre de tableaux dans n’importe quel état du cycle de vie qui ont au moins une politique de conservation assignée par politique | Gestion du cycle de vie du contenu | ✅ | ❌ |
| Nombre de tableaux suivant une politique de suppression, regroupée par politiques | Nombre de tableaux dans tout état du cycle de vie ayant au moins une politique de suppression assignée par politique | Gestion du cycle de vie du contenu | ✅ | ❌ |
| Nombre de tableaux créés ce jour/semaine/mois | Nombre de tableaux créés cette semaine | Gestion du cycle de vie du contenu | ❌ | ✅ |
| Nombre de tableaux supprimés (mis à la corbeille) ce jour/semaine/mois | Nombre de tableaux supprimés (mis à la corbeille) cette semaine | Gestion du cycle de vie du contenu | ❌ | ✅ |
| Nombre de tableaux concernés par des politiques de suppression, regroupés par date de la politique de suppression effective par mois |  | Gestion du cycle de vie du contenu | ❌ | ❌ |

## Comprendre les erreurs, les états vides et les changements historiques

Comprendre comment interpréter les états vides et les messages d’erreur est essentiel pour lire avec précision les métriques du tableau de bord Enterprise Guard.

### Comprendre le comportement des données historiques lorsque les paramètres changent

Si la découverte des données est désactivée après collecte des données, les métriques historiques continueront d’afficher les valeurs de la période active. Par exemple, si vous désactivez la découverte de données en mai et qu’elle était active en avril :

- Les valeurs d’avril continueront d’apparaître sur le tableau de bord.
- Le graphique de mai affichera **Aucune donnée disponible**, car la collecte de données a cessé.

###
