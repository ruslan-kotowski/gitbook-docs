---
title: Vue d'ensemble de l'exportation de tableau depuis la console d'admin
article_id: 26259747401362
translation_id: 26259747401362
locale: fr
sidebar_position: 0
created_at: '2025-04-24T14:18:00Z'
updated_at: '2025-11-25T15:50:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: discovery-board-export
---

Les admins eDiscovery peuvent désormais exporter directement les tableaux sous mise en suspens juridique depuis la console d’admin.
Cette capacité permet aux admins eDiscovery de :

- Initier les exports de tableaux depuis la console d’admin.
- Surveillez la progression des exports en temps réel via l'onglet **Exports** dans chaque enquête.
- Filtrez les tâches d’export par statut et par créateur et voyez quels tableaux sont inclus.
- Obtenez un journal complet du contenu pour chaque tableau exporté.
- Consulter une liste des tableaux exportés et leurs métadonnées (classification, propriétaire, état).
- Téléchargez les tableaux exportés individuellement, directement depuis la console d’admin.
- Complétez le workflow d’export sans dépendre des API ou des intégrations.
- Annulez les tâches d'export en file d'attente ou en cours.

:::note
Pour exporter des tableaux et gérer les opérations d'export, vous devez avoir le rôle d’[admin eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d’admin de contenu sensible, contactez l’admin de votre entreprise.
:::

## **Capacités d’exportation de tableau**

- Chaque **tâche d'export** peut contenir jusqu'à **1 000 tableaux**.
- **Limites d'exportation** par forfait :

  - **Enterprise Guard :** Jusqu'à **100** tâches d’exportation actives.
  - **Enterprise :** Jusqu'à **10** tâches d’exportation actives.
- **Limites de traitement parallèle** :

  - **Enterprise Guard** : Jusqu'à **5** tâches d’exportation traitées en parallèle.
  - **Enterprise** : **1** tâche d’exportation traitée à la fois.
- **Journaux de contenu avec les tâches d’exportation :** Les exports peuvent facultativement inclure un journal de contenu complet pour chaque tableau exporté.
- **Filtres pour les tâches d’exportation** : Filtrer les tâches d’exportation et voir quels tableaux sont inclus.
- **Annuler les tâches d’export en cours et en attente** : Gérer efficacement la bande passante pour l'export.
  > ✏️ Lorsque vous annulez un export, tous les tableaux en cours seront terminés et disponibles au téléchargement. Les tableaux non démarrés ne seront pas exportés.

- **Accès au téléchargement** : Les résultats peuvent être téléchargés pendant **14 jours.**
- **Portée de la console d’admin** : Seuls les exports initiés via la console d’admin apparaissent dans l’onglet **Exports**. Les tâches d’export basées sur l’API ne sont pas incluses dans la liste de la console d’admin.
