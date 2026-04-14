---
title: Dépendances pour Azure DevOps
article_id: 15556757538450
translation_id: 15556757538450
locale: fr
sidebar_position: 6
created_at: '2023-12-05T11:50:18Z'
updated_at: '2025-11-25T15:39:53Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: dependencies
availability:
  notes: 'Disponible pour : les forfaits Business et Enterprise'
---

[Cartographiez les dépendances entre les cartes Azure sur votre planification, ou n’importe où sur votre tableau Miro. Avec l’application Dépendances, vous pouvez identifier, visualiser, discuter et enregistrer les dépendances entre les équipes en temps réel pendant les séances de planification.](../../integrations-apps/microsoft/09-planner-for-azure-devops.md)

:::note
Pour utiliser les dépendances pour Azure DevOps, commencez par [configurer votre intégration Azure](../../integrations-apps/microsoft/03-azure-cards.md).
:::

## Fonctionnement des dépendances

Les dépendances apparaissent sous la forme d’une couche de lignes de connexion et montrent les relations entre les cartes Azure.

Elles ne sont visibles que lorsque vous ouvrez des dépendances sur le tableau. Les participants peuvent filtrer différents types de dépendances pour discuter des obstacles et des relations.

![Mapping-dependencies-Azure.png](../../../../../../docs/using-miro/facilitation-tools/images/15603398527890_Mapping-dependencies-Azure.png)
*Dépendances mappées dans Azure*

## Comment afficher et filtrer les dépendances

:::note
Vous ne pouvez afficher et filtrer que les dépendances que vous avez déjà créées dans Azure. Bientôt, vous pourrez créer et modifier les dépendances entre les cartes Azure directement dans Miro.
:::

1. Allez dans la barre d'outils Création sur le côté gauche du tableau.
2. Cliquez sur l’icône **Dépendances**. Si l’icône Dépendances ne figure pas dans votre barre d’outils Création, vous devrez l’ajouter à partir de **Outils, médias et intégrations****(+).**
3. Le panneau Dépendances s'ouvre et toutes les dépendances existantes apparaissent sous forme de lignes sur le tableau.
4. Cliquez sur l’icône **Filtrer** en haut du panneau Dépendances
5. Utilisez les boutons à bascule pour filtrer par **Letype de dépendance, représenté par des lignes de couleurs différentes.**
6. **Utilisez la liste déroulante Afficher les lignes pour contrôler l’affichage des dépendances. Sélectionnez **Toujours** pour afficher toutes les dépendances actives. Choisissez Sur sélection pour voir les dépendances uniquement lorsque vous cliquez sur une carte Azure ou un type de dépendance spécifique.**

![Mapping-dependencies-Azure-and-Jira.png](../../../../../../docs/using-miro/facilitation-tools/images/15603699800338_Mapping-dependencies-Azure-and-Jira.png)
*Filtrer les dépendances mappées*

## Cartes Jira et Azure sur le même tableau

Si votre équipe utilise Azure DevOps et Jira, et que vous avez configuré les deux intégrations dans Miro, vous pouvez gérer les cartes et les dépendances des deux systèmes sur un seul tableau.

Les dépendances relient soit deux cartes Jira, soit deux cartes Azure. Lorsque vous ouvrez l’application Dépendances sur un tableau contenant à la fois des cartes Azure et Jira qui ont des dépendances, nous afficherons tous les liens existants entre ces cartes.

**Pour filtrer les dépendances d’un seul système, utilisez les toggles **Saved to Jira** et Saved to Azure.**

![Dependencies-mapped-between-Jira-and-Azure-cards.png](../../../../../../docs/using-miro/facilitation-tools/images/15603628660626_Dependencies-mapped-between-Jira-and-Azure-cards.png)
*Les dépendances Jira et Azure sur un seul tableau Miro.*
