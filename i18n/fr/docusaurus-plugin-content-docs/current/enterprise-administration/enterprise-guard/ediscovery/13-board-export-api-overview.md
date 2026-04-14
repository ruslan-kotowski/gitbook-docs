---
title: Vue d'ensemble de l'API d'exportation de tableaux
article_id: 17774560667794
translation_id: 17774560667794
locale: fr
sidebar_position: 12
created_at: '2024-03-19T12:52:09Z'
updated_at: '2025-07-09T17:32:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: discovery-board-export
---

Les [API eDiscovery](https://developers.miro.com/reference/enterprise-create-board-export) permettent aux clients du plan Enterprise d'exporter les tableaux de Miro pour les examiner manuellement ou les intégrer dans des outils spécialisés à des fins juridiques, de conformité et de sécurité.

L'API d'exportation du tableau fournit un fichier ZIP avec un instantané des données du tableau au moment où le travail s'exécute, y compris l'exportation du contenu du tableau dans un format spécifié SVG, PDF ou HTML, un fichier JSON avec un enregistrement de tous les commentaires, un fichier JSON avec une liste de tous les utilisateurs qui ont consulté ou modifié le tableau, des enregistrements vidéo des séquences de la webcam d'Enregistrement associées au tableau, le cas échéant, et un JSON avec les matadonnées du tableau. Pour les tableaux de grande taille, l'exportation au format PDF produit plusieurs fichiers PDF représentant le tableau complet.

L'API asynchrone comprend des points de terminaison permettant de récupérer des informations sur une tâche d'exportation de tableaux, comme son statut.

:::note
Si vous bénéficiez du plan Enterprise, vous ne pouvez exécuter qu'une seule tâche d'exportation de tableaux à la fois. En tant que client Enterprise Guard, vous pouvez exécuter simultanément jusqu'à cinq tâches d'exportation de tableaux avec une vitesse d'exportation nettement supérieure.
:::

## Cas d’utilisation

Parmi les cas d'utilisation courants de l'eDiscovery, on peut citer

- **eDiscovery (découverte électronique) :** processus d'identification, de collecte, de préservation et d'examen des informations stockées électroniquement en vue de leur utilisation dans le cadre d'une affaire juridique.
- **Archivage de l'information :** pratique par laquelle les organisations conservent des données en dehors du système d'origine à des fins de stockage et d'archivage à long terme. Le contenu et les métadonnées aident les clients à indexer et à rechercher les archives et à surveiller de manière proactive les problèmes de conformité.
