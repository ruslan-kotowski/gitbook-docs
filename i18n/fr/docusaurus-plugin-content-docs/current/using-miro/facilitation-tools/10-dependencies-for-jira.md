---
title: "D\xE9pendances pour Jira"
article_id: 10649083010834
translation_id: 10649083010834
locale: fr
sidebar_position: 7
created_at: '2023-03-22T10:22:08Z'
updated_at: '2025-11-25T16:22:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

Mettez en correspondance les dépendances existantes ou créez-en de nouvelles entre les cartes Jira sur votre [planification](../../integrations-apps/atlassian/21-planner-for-jira.md) ou n’importe où sur votre tableau Miro, et elles seront instantanément synchronisées dans Jira. Avec l’application Dépendances, vous pouvez identifier, visualiser, discuter et enregistrer les dépendances entre les équipes en temps réel pendant les séances de planification.

> ****💡**** Cette fonctionnalité est désormais disponible pour [Azure DevOps](08-dependencies-for-azure-devops.md).

> **Disponible pour :** les forfaits Business et Enterprise
>
> **Disponible sur :** navigateur de bureau, application de bureau

## Fonctionnement des dépendances

Les dépendances apparaissent sous forme de calque de lignes de connexion, montrant les relations entre les cartes Jira.

Elles sont visibles uniquement lorsque vous ouvrez les dépendances sur le tableau. Les participants peuvent filtrer différents types de dépendances pour discuter des obstacles et des relations.

![Dependencies-app.png](../../../../../../docs/using-miro/facilitation-tools/images/13244544218258_Dependencies-app.png)
*Dépendances cartographiées entre les cartes Jira sur un widget de planification*

## Comment créer une nouvelle dépendance

1. Allez dans la barre d’outils Création sur le côté gauche du tableau.
2. Cliquez sur l’icône **Dépendances**. Si l’icône Dépendances ne se trouve pas déjà dans votre barre d’outils Création, vous devrez l’ajouter à partir de **Outils, médias et intégrations** (**+**).
3. Le panneau Dépendances s’ouvre.
4. Cliquez sur **Nouvelle dépendance**.
5. Cliquez sur **Première carte** et sélectionnez un ticket Jira dans le menu déroulant ou via la recherche.
6. Sélectionnez le **type de dépendance** en fonction de celles disponibles dans votre instance Jira (par exemple, blocages, clones, dupliquer, ou se rapporte à).
7. Cliquez sur la **Deuxième carte** et sélectionnez un ticket Jira dans le menu déroulant ou via la recherche.
8. Cliquez sur **Enregistrer le brouillon**, ou **Enregistrer dans Jira**directement.

:::tip
Les dépendances provisoires ne sont enregistrées que dans Miro. Vous pouvez créer des dépendances provisoires sous forme de suggestions pour les autres participants et équipes lors des séances de planification. Une fois qu’elles ont été examinées et discutées, vous pouvez soit les enregistrer dans Jira, soit les supprimer.
:::

![dependencies-entry-point.png](../../../../../../docs/using-miro/facilitation-tools/images/21537435953426_dependencies-entry-point.png)
*Création d'une nouvelle dépendance et enregistrement dans Jira*

## Comment afficher et filtrer les dépendances

1. Allez dans la barre d’outils Création sur le côté gauche du tableau.
2. Cliquez sur l’icône **Dépendances**. Si l’icône Dépendances ne se trouve pas déjà dans votre barre d’outils Création, vous devrez l’ajouter à partir de **Outils, médias et intégrations** (**+**).
3. Le panneau Dépendances s’ouvre et toutes les dépendances existantes apparaissent sous forme de lignes sur le tableau.
4. Cliquez sur l’icône **Filtrer** en haut du panneau Dépendances.
5. Utilisez les bascules pour filtrer par **Type de dépendance** et **État de synchronisation**.
6. Utilisez la liste déroulante **Afficher les lignes** pour contrôler l’affichage des dépendances. Sélectionnez **Toujours** pour afficher toutes les dépendances actives. Choisissez **Sur sélection** pour voir les dépendances uniquement lorsque vous cliquez sur une carte Azure spécifique ou un type de dépendance.

Les lignes pointillées montrent les dépendances provisoires, et les lignes pleines montrent les dépendances synchronisées avec Jira. La couleur de la ligne représente le type de dépendance.

![Filtering-dependencies.gif](../../../../../../docs/using-miro/facilitation-tools/images/13245295619730_Filtering-dependencies.gif)
*Filtrer l'affichage des dépendances* *dans le widget de Planification*

## Comment modifier, enregistrer, rétablir ou supprimer une dépendance

1. Allez dans la barre d’outils Création sur le côté gauche du tableau.
2. Cliquez sur l’icône **Dépendances**.
3. Le panneau Dépendances s’ouvre.
4. Cliquez sur l’icône **Modifier** à côté d’une dépendance.

![The_option_to_edit_a_Dependency.jpg](../../../../../../docs/using-miro/facilitation-tools/images/10866625733778_The%20option%20to%20edit%20a%20Dependency.jpg)
*Modification d'une dépendance*

Vous pouvez changer la **Première carte** et la **Seconde carte** d'une dépendance, ainsi que le **type de dépendance.**

*![Editing_a_dependency.gif](../../../../../../docs/using-miro/facilitation-tools/images/10866808392722_Editing%20a%20dependency.gif)**Modification de la Première carte et du Type de dépendance*

Cliquez sur **Enregistrer dans Jira** pour enregistrer et synchroniser une dépendance brouillon avec Jira.

![Save_to_Jira.png](../../../../../../docs/using-miro/facilitation-tools/images/10868740630034_Save%20to%20Jira.png)
*Enregistrement d'une dépendance brouillon dans Jira*

Cliquez sur **Rétablir le brouillon** pour repasser une dépendance synchronisée au statut de brouillon.

![Revert_to_draft.png](../../../../../../docs/using-miro/facilitation-tools/images/10868741500690_Revert%20to%20draft.png)
*Repasser une dépendance synchronisée dans Jira au statut de brouillon*

Cliquez sur l’icône **Corbeille** pour supprimer une dépendance.
![Delete_dependency.png](../../../../../../docs/using-miro/facilitation-tools/images/10868804195986_Delete%20dependency.png)*Suppression d'une dépendance*
