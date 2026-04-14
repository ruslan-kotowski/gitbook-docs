---
title: "R\xE9f\xE9rence des indicateurs du tableau de bord Enterprise Guard"
article_id: 26718144750610
translation_id: 26718144750610
locale: fr
sidebar_position: 5
created_at: '2025-05-15T00:17:54Z'
updated_at: '2025-07-22T20:38:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: admin-analytics
---

:::note
Notes sur les indicateurs :

- Toutes les métriques dans Enterprise Guard excluent les tableaux des équipes mises à la corbeille.
- Tous les indicateurs de classification excluent les modèles et les tableaux à la corbeille.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Titre** | **Description** | **Domaine** | **Apparaît dans le tableau de bord d’aperçu** | **Possède un indicateur d’historique** |
| Nombre total de tableaux classifiés | Nombre de tableaux auxquels un badge de classification est attribué | Classification | ✅ | ❌ |
| Nombre de tableaux par classification | Nombre de tableaux par badge de classification (nom du badge) | classification | ✅ | ❌ |
| Nombre de tableaux non classifiés | Nombre de tableaux sans badge de classification attribué | classification | ✅ | ✅ |
| Nombre de tableaux classifiés manuellement | Nombre de tableaux ayant un badge de classification attribué manuellement (pas par classification automatique) | Classification | ❌ | ✅ |
| Nombre de tableaux classifiés automatiquement | Nombre de tableaux avec un badge de classification attribué automatiquement par la classification automatique | Classification | ❌ | ✅ |
| Nombre de tableaux sensibles | Nombre de tableaux auxquels au moins un badge intégré, un badge de mot-clé ou un badge de confidentialité est attribué | Découverte de données | ✅ | ❌ |
| Nombre de tableaux comportant des éléments sensibles de l’entreprise | Nombre de tableaux qui ont au moins un badge intégré ou un badge de mot-clé assigné | Découverte de données | ✅ | ✅ |
| Nombre de tableaux contenant des éléments sensibles relatifs à la vie privée | Nombre de tableaux ayant au moins un badge de confidentialité assigné | Découverte de données | ✅ | ✅ |
| Nombre de tableaux avec un badge assigné par badge | Nombre de tableaux par badge (intégré, mot-clé ou confidentialité) | Découverte de données | ❌ | ❌ |
| Total des badges en lien avec la vie privée activés | Nombre de badges en lien avec la vie privée activés | Découverte de données | ❌ | ❌ |
| Total des badges de mots-clés activés | Nombre de badges de mots-clés activés | Découverte de données | ❌ | ❌ |
| Total des badges activés portant sur des informations sensibles de l’entreprise | Nombre de badges activés concernant les informations sensibles de l’entreprise | Découverte de données | ❌ | ❌ |
| Nombre total de tableaux | Nombre total de tableaux dans tous les états du cycle de vie (actif, corbeille, conservé) | Gestion du cycle de vie du contenu | ✅ | ❌ |
| Nombre de tableaux actifs Notez que ceci n’est PAS l’activité des tableaux mais des tableaux qui sont dans l’état de cycle de vie actif | Nombre total de tableaux dans l’état de cycle de vie actif | Gestion du cycle de vie du contenu | ✅ | ✅ |
| Nombre de tableaux dans la corbeille | Nombre total de tableaux dans l’état de cycle de vie supprimé | Gestion du cycle de vie du contenu | ✅ | ✅ |
| Nombre de tableaux conservés | Nombre total de tableaux dans l’état de cycle de vie conservé | Gestion du cycle de vie du contenu | ✅ | ✅ |
| Nombre de tableaux en cours de conservation | Nombre total de tableaux qui ont au moins une politique de conservation non expirée assignée | Gestion du cycle de vie du contenu | ❌ | ✅ |
| Nombre de tableaux en cours de suppression | Nombre total de tableaux auxquels au moins une politique de suppression non expirée est assignée | Gestion du cycle de vie du contenu | ❌ | ❌ |
| Nombre de tableaux suivant une politique de conservation, regroupés par politique | Nombre de tableaux dans n’importe quel état du cycle de vie qui ont au moins une politique de conservation assignée | Gestion du cycle de vie du contenu | ✅ | ❌ |
| Nombre de tableaux suivant une politique de suppression, regroupé par politiques | Nombre de tableaux dans tout état du cycle de vie ayant au moins une politique de suppression assignée | Gestion du cycle de vie du contenu | ✅ | ❌ |
| Nombre de tableaux créés ce jour/semaine/mois | Nombre de tableaux créés cette semaine | Gestion du cycle de vie du contenu | ❌ | ✅ |
| Nombre de tableaux supprimés (mis à la corbeille) ce jour/semaine/mois | Nombre de tableaux supprimés (mis à la corbeille) cette semaine | Gestion du cycle de vie du contenu | ❌ | ✅ |
| Nombre de tableaux concernés par des politiques de suppression, regroupés par date de la politique de suppression effective par mois |  | Gestion du cycle de vie du contenu | ❌ | ❌ |
| Nombre d’enquêtes | Nombre total d’enquêtes | Découverte électronique | ✅ | ❌ |
| Nombre de mises en suspens juridiques | Nombre total de mises en suspens juridiques | Investigations informatiques (eDiscovery) | ✅ | ❌ |
| Nombre de mises en suspens juridiques pour une enquête spécifique | Nombre total de mises en suspens juridiques pour une enquête spécifique | Investigations informatiques (eDiscovery) | ❌ | ❌ |
| Nombre de tableaux sous mise en suspens juridique | Nombre total de tableaux sous mise en suspens, parmi toutes les mises en suspens juridiques | Investigations informatiques (eDiscovery) | ❌ | ❌ |
| Utilisateurs sous mise en suspens juridique et nombre total de leurs tableaux | Répertorie les utilisateurs sous mise en suspens juridique et le nombre total de leurs tableaux | Investigations informatiques (eDiscovery) | ❌ | ❌ |
