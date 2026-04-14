---
title: Journaux de contenu
article_id: 17774729839378
translation_id: 17774729839378
locale: fr
sidebar_position: 5
created_at: '2024-03-19T13:00:06Z'
updated_at: '2026-03-15T21:32:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
availability:
  notes: 'Mise en place par: admins d’entreprise, admins de sécurité'
---

Les journaux de contenu permettent aux clients entreprise de collecter des enregistrements détaillés de l'activité des utilisateurs sur les tableaux et de les exploiter pour des enquêtes ou des archivages réglementaires.

Les journaux de contenu peuvent être intégrés à divers outils conçus à des fins légales, de conformité et de sécurité. En fournissant une solution pour exporter des données d'activité utilisateur à grande échelle, Miro réduit le risque pour ses clients et ouvre des opportunités pour que davantage de travailleurs du savoir au sein de l'entreprise expérimentent le pouvoir collaboratif de Miro tout en respectant des exigences strictes en matière de sécurité et de conformité.

## Données des journaux de contenu

Lorsque un utilisateur met à jour un widget sur le tableau, une entrée de journal est créée avec des informations, telles que l'heure de l'action de l'utilisateur, les détails de l'utilisateur, le type d'action (créer, mettre à jour, supprimer), les IDs du tableau et du widget, et d'autres informations pertinentes sur l'état du widget résultant des actions des utilisateurs. Les journaux de contenu *ne consignent pas* les mises à jour de la position, de la taille ou de la rotation du widget.

## Collecter les journaux de contenu

Les événements sont enregistrés dès qu'un admin active la collecte des journaux de contenu. Les événements collectés sont stockés pendant 30 jours, par défaut.

Pour activer la collecte des journaux de contenu, effectuez les étapes suivantes :

1. Rendez-vous dans les paramètres de l'entreprise.
2. Dans le panneau de gauche, cliquez sur **Sécurité** > **Journaux d'audit**.
3. Sous **Journaux d'audit**, cliquez sur l'onglet **Paramètres**.
4. Sous la section **Journaux de contenu**, cliquez pour activer le bouton bascule **Collecter les journaux de contenu**.
   ![content_logs.png](images/24937029892370_content_logs.png)
   *Activation de la collecte des journaux de contenu*

## Accéder aux journaux de contenu via l’API

Les admins peuvent utiliser l’[API des journaux de contenu](https://developers.miro.com/reference/board-content-logs) pour accéder de manière programmée aux données des journaux de contenu au sein de leur organisation. Les admins peuvent également collecter les données des journaux de contenu en utilisant des intégrations prises en charge, comme Smarsh ou Theta Lake.

Pour authentifier l’accès à l’API, les admins peuvent choisir parmi les options suivantes :

- Activer le bouton de basculement eDiscovery dans les intégrations Enterprise.
- Créer une application Platform et lui donner accès à la portée Content log:read.
- Installer et autoriser l'une des intégrations eDiscovery à partir du Marketplace.

## Suppression des journaux de contenu

Les admins peuvent définir une politique de conservation pour les journaux de contenu, en choisissant entre 30, 90, 180 ou 365 jours. Par défaut, la période de conservation est fixée à 30 jours.

:::note
Une fois que les journaux de contenu sont supprimés, ils ne peuvent pas être récupérés.
:::

Pour définir une période de suppression, procédez comme suit :

1. Rendez-vous dans les paramètres de l’entreprise.
2. Dans le panneau de gauche, cliquez sur **Sécurité** > **Journaux d'audit**.
3. Sous **Journaux d'audit**, cliquez sur l'onglet **Paramètres**.
4. Sous **Journaux de contenu**, choisissez une option dans la liste déroulante. Il vous sera demandé de confirmer votre choix.
   ![content_logs_duration.png](images/24937022291602_content_logs_duration.png)
   *Définition de la politique de conservation des journaux de contenu*
