---
title: "Aper\xE7u du tableau de bord de d\xE9couverte de donn\xE9es"
article_id: 26806897106834
translation_id: 26806897106834
locale: fr
sidebar_position: 1
created_at: '2025-05-19T11:10:19Z'
updated_at: '2025-11-25T15:51:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Le tableau de bord Découverte de données fournit une vue centralisée des informations sensibles détectées sur les tableaux de votre organisation. Il permet aux admins de surveiller, classer et gérer les risques liés aux données en identifiant les contenus en lien avec la vie privée ou les informations sensibles de l’entreprise. Le tableau de bord Découverte de données comprend les indicateurs suivants :

:::note
Tous les indicateurs dans Enterprise Guard excluent les tableaux des équipes en corbeille et les tableaux sous mise en suspens juridique.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Titre** | **Description** | **Domaine** | **Apparaît dans le tableau de bord d’aperçu** | **Possède un indicateur d’historique** |
| Nombre de tableaux sensibles | Nombre de tableaux auxquels au moins un badge intégré, un badge de mot-clé ou un badge de confidentialité est attribué | Découverte de données | ✅ | ❌ |
| Nombre de tableaux comportant des éléments sensibles de l’entreprise | Nombre de tableaux qui ont au moins un badge intégré ou un badge de mot-clé assigné | Découverte de données | ✅ | ✅ |
| Nombre de tableaux contenant des éléments sensibles relatifs à la vie privée | Nombre de tableaux ayant au moins un badge de confidentialité assigné | Découverte de données | ✅ | ✅ |
| Nombre de tableaux avec un badge assigné par badge | Pour chaque badge individuel dans les trois catégories (intégré, mot-clé ou confidentialité), comptez le nombre de tableaux auxquels ce badge est attribué. | Découverte de données | ❌ | ❌ |
| Total des badges en lien avec la vie privée activés | Total des badges en lien avec la vie privée activés | Découverte de données | ❌ | ❌ |
| Total des badges de mots-clés activés | Total des badges de mots-clés activés | Découverte de données | ❌ | ❌ |
| Total des badges activés portant sur des informations sensibles de l’entreprise | Total des badges activés portant sur des informations sensibles de l’entreprise | Découverte de données | ❌ | ❌ |

## Comprendre les erreurs, les états vides et les changements historiques

Comprendre comment interpréter les états vides et les messages d’erreur est essentiel pour lire avec précision les métriques du tableau de bord Enterprise Guard.

### Comprendre le comportement des données historiques lorsque les paramètres changent

Si la découverte des données est désactivée après collecte des données, les métriques historiques continueront d’afficher les valeurs de la période active. Par exemple, si vous désactivez la découverte de données en mai et qu'elle était active en avril :

- Les valeurs d’avril continueront d’apparaître sur le tableau de bord.
- Le graphique de mai affichera **aucune donnée disponible**, car la collecte de données a cessé.

## Consulter les résultats de la découverte de données

Le cycle de découverte des données s’exécute au moins une fois par heure et analyse toutes les mises à jour des tableaux pour détecter les informations en lien avec la vie privée, les informations sensibles de l’entreprise ou personnalisées et sensibles de l’entreprise, selon votre configuration pour la découverte de données. Cela inclut les tableaux qui ont déjà été analysés lors du cycle précédent de découverte de données.

Les résultats de la découverte de données apparaissent sous les graphiques des métriques. Vous pouvez consulter des informations telles que le nom du badge, l’état, le type, la classification, le nombre de tableaux, etc.

Pour plus d’informations sur la documentation d’examen des tableaux contenant des informations en lien avec la vie privée, [consultez cet article](16-review-boards-with-privacy-related-information.md).

Pour plus d’informations sur l’examen des tableaux contenant des données sensibles de l’entreprise et des données personnalisées sensibles de l’entreprise, [consultez cet article](14-review-boards-with-business-sensitive-and-custom-business-sensitive-information-beta.md).

Pour plus d’informations sur l’examen des tableaux avec des badges personnalisés portant sur les informations sensibles de l’entreprise, [consultez cet article](15-review-custom-business-sensitive-labels-and-data-discovery-results.md).

:::note
- Pour consulter les résultats de la découverte de données, vous devez avoir le [rôle d’admin de contenu sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d’admin du contenu sensible, contactez l’admin de votre entreprise.

Bien que nous travaillions continuellement avec notre partenaire technologique et nos clients pour améliorer le système de détection de contenu sensible, nous ne pouvons garantir qu’il identifiera et signalera 100 % des données sensibles sur vos tableaux. Notre système de détection de contenu sensible utilise des modèles et d'autres critères pour déterminer la probabilité d'une correspondance. Il peut arriver que le système signale incorrectement des données sur vos tableaux comme étant probablement sensibles (un faux positif) ou ne parvienne pas à signaler des données comme sensibles (un faux négatif). Divers facteurs contribuent à ces occurrences, y compris la proximité de termes connexes ou le formatage de données sensibles.

Pour plus d’informations sur la façon dont vous pouvez supprimer les résultats qui sont des faux positifs, consultez [Supprimer une correspondance de contenu sensible](11-suppress-a-sensitive-content-match.md).
:::

##

##
