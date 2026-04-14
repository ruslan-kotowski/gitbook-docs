---
title: Planification pour Azure DevOps
article_id: 15280547945618
translation_id: 15280547945618
locale: fr
sidebar_position: 10
created_at: '2023-11-23T14:12:19Z'
updated_at: '2025-11-25T15:39:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: program-board-widget
availability:
  notes: 'Disponible pour : Plan d''éducation, Plan d''entreprise, Plan d''affaires'
---

Lors des évènements de planification de l’équipe et de l’entreprise, tels que le PI Planning, Big Room planning, roadmapping et les sprints, les équipes de développement discutent et s’alignent les unes sur les autres.

Avec planner for Azure, les facilitateurs et les équipes peuvent exécuter et participer à des événements de planification sur un tableau Miro, tout en synchronisant les mises à jour avec leur tableau Azure en temps réel - ce qui permet d'économiser des heures de travail manuel.

## Comment créer un planificateur pour Azure DevOps ?

:::note
Pour utiliser la planification pour Azure DevOps, commencez par [configurer votre intégration Azure](03-azure-cards.md).
:::

1. Accédez à la barre d’outils [barre d’outils de création](../../getting-started/start-here/your-first-board/05-toolbars.md) sur le côté gauche de votre tableau.
2. Cliquez ****Plus d’applications****(+) et recherchez "Planification".
3. Cliquez sur **Planification**.
4. Un curseur apparaît sur le tableau. Cliquez n’importe où pour placer une planification vierge.
5. La source de données de votre Planification sera par défaut l'intégration que vous avez autorisée. Si vous n'avez pas encore autorisé une intégration, elle se fera par défaut sur Jira. Vous pouvez facilement changer cela en Azure DevOps en cliquant sur le menu déroulant intitulé **Jira** et en sélectionnant **Azure DevOps**.
6. Si vous n'avez pas encore autorisé votre compte Azure DevOps dans Miro, vous serez prompt à de vous connecter.
7. Une fois que vous êtes connecté, cliquez sur le menu déroulant du **projet Azure** et sélectionnez un projet à connecter au planificateur.
8. Cliquez ensuite sur le menu déroulant **Équipes** et sélectionnez une équipe.
9. La première ***Colonnes*** est votre type de colonne. L'**itération** est automatiquement sélectionnée. D'autres champs Azure seront bientôt disponibles.
10. Utilisez le deuxième menu déroulant **Colonnes** pour affiner les itérations que vous souhaitez afficher.

## Comment travailler avec le widget de planification ?

Faites glisser les cartes Azure d'une colonne à l'autre pour les mettre à jour. Par exemple, si vous faites glisser une carte Azure de l'itération 1 à l'itération 2 dans le planificateur, elle sera mise à jour à la fois dans Miro et dans Azure.

Les participants peuvent commenter les cartes Azure pour suivre les discussions et les notes en cours.

![Commentez un planificateur Azure.png](../../../../../../docs/integrations-apps/microsoft/images/21016020674450_Comment-on-an-Azure-Planner.png)*Commentaire sur la Planification*

## Synchronisation de la planification

### De Miro à Azure

Lorsque vous faites glisser une carte entre des champs personnalisés dans Miro, Azure est mis à jour automatiquement. Cela peut prendre quelques secondes.

### D'Azure à Miro

Pour vous assurer que votre planification reste à jour par rapport aux modifications que vous apportez dans Azure, sélectionnez le planificateur et cliquez sur le bouton **Sync** dans le menu contextuel.

![Synchronisation du planificateur avec Azure.png](../../../../../../docs/integrations-apps/microsoft/images/21016020674962_Syncying-the-planner-with-Azure.png)*Synchronisation du planificateur avec Azure*

Les champs pris en charge pour Azure sont actuellement les suivants :

- Itération (ou sprint).
- Affecté à
- Tous les autres domaines qui répondent aux critères suivants :
  - Modifiable (c'est-à-dire pas en lecture seule).
  - Valeurs de type chaîne (texte).
  - Une liste de valeurs prédéfinies qui peuvent être définies (c'est-à-dire pas de texte libre).
  - Valable pour les éléments de travail Azure (certains champs Azure ont d'autres utilisations).

# Vous ne voyez pas les sprints de votre équipe ?

Assurez-vous que vos itérations dans Azure sont mappées à votre équipe afin que vous puissiez les visualiser dans le planificateur.

1. Accédez à votre **projet** dans Azure.
2. En bas du menu latéral droit, cliquez sur l'icône **Paramètres du projet.**
3. Allez dans la section **Tableaux** et cliquez sur **Configuration de l'équipe**.
4. Cliquez sur l'onglet **Itérations** en haut de l'écran.
5. Cliquez sur **+ Sélectionnez l'itération**. Assurez-vous d'avoir ajouté toutes les itérations liées à votre équipe.

![Ajout d'itérations à Azure-Devops.png](../../../../../../docs/integrations-apps/microsoft/images/21016020675858_Adding-iterations-Azure-Devops.png)*Ajouter des itérations à Azure*

## Mappage des dépendances

Les participants peuvent visualiser les dépendances entre les tâches sur la planification. En savoir plus sur les [dépendances pour Azure](../../using-miro/facilitation-tools/08-dependencies-for-azure-devops.md).
