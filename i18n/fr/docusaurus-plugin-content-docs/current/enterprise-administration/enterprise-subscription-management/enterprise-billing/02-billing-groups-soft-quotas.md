---
title: Quotas conditionnels pour les groupes de facturation
article_id: 20150819688338
translation_id: 20150819688338
locale: fr
sidebar_position: 2
created_at: '2024-07-15T07:02:19Z'
updated_at: '2026-02-19T10:36:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: billing-groups
---

## Aperçu

Les quotas conditionnels sont une nouvelle mise à jour de l’interface utilisateur des groupes de facturation, qui permet aux administrateurs de définir une limite souple facultative sur le nombre de licences attribuées à un groupe de facturation. Cette fonctionnalité offre une plus grande transparence et des données exploitables pour la gestion des attributions de licences.

Les quotas conditionnels offrent un moyen flexible et informatif de gérer les attributions de licences au sein des groupes de facturation, garantissant que les administrateurs disposent des données dont ils ont besoin pour prendre des décisions éclairées.

## Fixation de quotas conditionnels

### Ajout d’un quota conditionnel

Les administrateurs peuvent ajouter un quota conditionnel lors de la création ou de la modification d’un groupe de facturation. Cette limite est basée sur le nombre total de licences attribuées par rapport au nombre total de licences disponibles.
La limite globale du quota conditionnel pour chaque groupe de facturation apparaît en haut de la vue d’ensemble du groupe de facturation, sous la forme d’une valeur numérique et d’une barre de progression.

Lorsqu’elles sont définies, les limites de quotas conditionnels apparaissent également dans le tableau des groupes de facturation.

### Indicateurs visuels

- **Barre verte :** Indique que le groupe de facturation est dans la limite de la licence attribuée.
- **Barre rouge et icône d’avertissement :** Indique que le groupe de facturation a dépassé la limite de licence attribuée.

## Gestion des quotas conditionnels

### Dépasser la limite

Le dépassement du quota conditionnel n’affecte pas la manière dont les licences sont attribuées. L’objectif est d’assurer la transparence et de fournir des données exploitables aux administrateurs.

### Filtres rapides

Les admins peuvent filtrer les groupes de facturation par :

- **Quota défini :** Pour consulter les groupes avec un quota conditionnel défini.
- **Quota dépassé :** Pour consulter les groupes qui ont dépassé leur limite de quota conditionnel.
