---
title: "Fonctionnalit\xE9 d'exportation de tableau eDiscovery dans la Console d'administration"
article_id: 26529264912146
translation_id: 26529264912146
locale: fr
sidebar_position: 16
created_at: '2025-05-06T17:01:06Z'
updated_at: '2025-05-26T08:55:18Z'
draft: false
outdated: false
user_segment_id: 16307853619090
user_segment: Enterprise Company Admins
backstage_link:
  entity_kind: capability
  entity_id: content-explorer
---

Les administrateurs d'Enterprise Guard peuvent désormais utiliser la console d'administration pour mieux gérer les flux de travail eDiscovery. Ils peuvent :

- Exporter tous les tableaux sous mise en suspens juridique (l'exportation sélective n'est pas prise en charge).
- Afficher une liste des tâches d'exportation (terminées, en cours et prévues) au sein de chaque dossier eDiscovery.
- Voir le statut d'exportation des tableaux individuels dans un travail.
- Téléchargez les tableaux exportés individuellement, disponibles pendant 14 jours après l'export.

**Limites et comportement d'exportation :**

- Chaque tâche d'exportation peut inclure jusqu'à **1000 tableaux**. Les tâches ne démarreront pas si une mise en suspens juridique inclut plus de 1000 tableaux.
- Un maximum de **100 tâches d'exportation** peut être actif dans l’organisation.
- Jusqu'à **5 emplois** sont traités en parallèle (inchangé).

**Limites de l'API (API d'exportation de tableau) :**

- Jusqu'à **100 tâches d'exportation** pour les organisations Guard et **10 tâches** pour les organisations Enterprise.
- Limite de taille d'exportation de tâches : **1000 tableaux**.

Ces mises à jour facilitent les processus de conservation légale tout en assurant transparence et contrôle sur les activités d'exportation des tableaux.
