---
title: Vue d'ensemble des journaux d'audit d'Enterprise Guard
article_id: 17331872857746
translation_id: 17331872857746
locale: fr
sidebar_position: 0
created_at: '2024-02-27T21:08:55Z'
updated_at: '2025-11-25T15:41:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Les journaux d’audit fournissent aux admins une entrée exhaustive de tous les événements associés à Enterprise Guard. Ces journaux sont une ressource précieuse pour un dépannage efficace et offrent des insights détaillés sur des événements critiques, tels que les mises à jour de la politique de durée de vie de la corbeille et de la politique de permissions des tableaux supprimés, la création, la mise à jour ou la suppression de politiques de conservation pour l'organisation, ou la suppression permanente d'un tableau de la corbeille. Le suivi systématique de ces activités renforce la surveillance, l'analyse et la maintenance, garantissant un système sécurisé et bien géré.

## Événements d'Enterprise Guard dans les journaux d’audit

En plus des [événements existants enregistrés](../../security-integrations/security-management/01-audit-logs.md), les journaux d’audit incluent des enregistrements concernant les catégories d’événements suivantes et les événements associés à Enterprise Guard.

### Politique de gestion de la corbeille

Le tableau suivant présente les catégories d'événements et les actions d'événements enregistrées pour le composant de la Politique de gestion de la corbeille de l'organisation.

|  |  |
| --- | --- |
| **Catégorie d'événement** | **Action d'événement** |
| Administration | La politique de durée de conservation de la corbeille a été modifiée pour l’organisation. |
| Administration | La politique de permission des tableaux supprimés a été modifiée pour l'organisation. |

*Tableau 1: Catégories d'événements et actions d'événement enregistrées pour le composant de la politique de corbeille de l'organisation*Pour plus d’informations sur les politiques de corbeille, consultez [notre documentation](https://help.miro.com/hc/articles/13860817985426-Trash-Policy).

### Politique de conservation

Le tableau suivant répertorie les catégories d'événements et les actions d'événements enregistrées pour le composant de politiques de conservation du contenu.

|  |  |
| --- | --- |
| **Catégorie d'événement** | **Action d'événement** |
| Administration | Politique de conservation créée pour l'organisation |
| Administration | Politique de conservation mise à jour pour l'organisation |
| Administration | Politique de conservation supprimée pour l'organisation |

*Tableau 2: Catégories d'événements et actions d'événements enregistrées pour le composant des politiques de conservation du contenu*Pour plus d’informations sur les politiques de conservation, consultez [notre documentation](https://help.miro.com/hc/articles/16855776325778-Retention-Beta).

### Découverte de données

Le tableau suivant répertorie les catégories d'événements et les actions d'événements enregistrées pour le composant de Découverte de contenu.

|  |  |
| --- | --- |
| **Catégorie d'événement** | **Action d'événement** |
| Administration | Détection de l'information privée modifiée pour l'organisation  (activé/désactivé) |
| Administration | Suppression d'une correspondance de découverte de données dans l'organisation |

*Tableau 3 : Catégories d'événements et actions d'événements enregistrées pour le composant de découverte de contenu*

Pour plus d'informations sur la découverte de données, consultez [notre documentation](../../canvas-25-admin-features/data-discovery/01-data-discovery-overview.md).

### Garde-fous intelligents

Le tableau suivant présente les catégories d'événements et les actions d'événements enregistrées pour le composant des garde-fous intelligents.

|  |  |
| --- | --- |
| **Catégorie d'événement** | **Action d'événement** |
| Garde-fous intelligents | Garde-fous intelligents modifiés pour un tableau |

*Tableau 4 : Catégories d'événements et actions d'événements enregistrées pour le composant des garde-fous intelligents*

Pour plus d'informations sur les garde-fous intelligents, consultez [notre documentation](../../canvas-25-admin-features/data-classification/01-intelligent-guardrails-overview.md).

### eDiscovery (découverte électronique)

Le tableau suivant présente les catégories d'événements et les actions d'événements enregistrées pour le composant eDiscovery.

|  |  |
| --- | --- |
| **Catégorie d'événement** | **Action d'événement** |
| Administration | Enquête créée pour l'organisation |
| Administration | Enquête clôturée pour l'organisation |
| Administration | Mise en suspens juridique créée pour l'organisation |
| Administration | Mise en suspens juridique clôturée pour l'organisation |
| Administration | Mise en suspens juridique appliquée au tableau Tableau libéré de la mise en suspens juridique |

*Tableau 3 : Les catégories d'événements et les actions d'événements journalisées pour le composant eDiscovery*

Pour plus d'informations sur eDiscovery, consultez [notre documentation](https://help.miro.com/hc/sections/22049853357842-eDiscovery-Legal-Hold-Beta).
