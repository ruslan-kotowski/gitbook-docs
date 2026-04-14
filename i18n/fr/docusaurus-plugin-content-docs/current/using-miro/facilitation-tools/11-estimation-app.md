---
title: Application Estimation
article_id: 5651786248210
translation_id: 5651786248210
locale: fr
sidebar_position: 8
created_at: '2022-05-20T11:28:11Z'
updated_at: '2025-11-25T16:08:42Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: estimation
---

Les estimations sont un élément essentiel du développement et de la planification agiles. Elles aident à clarifier l’étendue du travail à réaliser par l’équipe, à identifier les lacunes dans l’analyse ou la compréhension, mais aussi à fixer des attentes claires pour la livraison.

Au cours de l’étape des estimations, les membres de l’équipe attribuent à chaque tâche un numéro qui reflète la quantité de travail requise. Afin d’obtenir des estimations réalistes, on utilise un système de numérotation qui additionne les chiffres précédents. Les membres de l’équipe peuvent ensuite discuter et s’aligner sur le nombre qu’ils ont choisi.

Utilisez notre application Estimation pour organiser des sessions d’estimation multijoueurs sur un tableau Miro avec des [cartes](../essential-tools/02-cards.md), des [pense-bêtes](../essential-tools/14-sticky-notes.md) et des [cartes Jira](../../integrations-apps/atlassian/03-jira-cards.md).

> **Disponible pour** : les forfaits Starter, Business, Enterprise
> **Installation par** : les membres de l’équipe ayant des droits d’édition sur le tableau.

Pour commencer l’estimation :

1. Accédez à l’application Estimation dans la barre d’outils Création et sélectionnez **Démarrer une nouvelle session.** Vous devrez peut-être ajouter l’application Estimation à partir de l’icône **Outils, médias et intégrations** **(+) :**
   ![estimation-entry-point.png](../../../../../../docs/using-miro/facilitation-tools/images/21537436002962_estimation-entry-point.png)*Application Estimation dans la barre d’outils*
2. Sélectionnez l’échelle d’estimation : dans le menu déroulant, choisissez la technique d’estimation **T-shirt** (disponible uniquement pour les [cartes](../essential-tools/02-cards.md) Miro) ou **Fibonacci** .
3. Faites glisser la zone d’estimation sur les objets que vous souhaitez estimer. Vous pouvez sélectionner des cartes, des pense-bêtes ou des [cartes Jira](../../integrations-apps/atlassian/03-jira-cards.md) pour l’estimation. Vous pouvez exclure des objets particuliers de l’estimation en cliquant sur les points bleus.
4. Si votre sélection comprend des cartes Jira, vous serez invité(e) à sélectionner le tableau Jira auquel ces cartes appartiennent. Vos estimations sont ainsi enregistrées de manière précise et prévisible dans Jira. Sans cette étape, Jira est imprévisible lors de l’enregistrement de ces estimations.
5. Cliquez sur **Estimer x cartes/pense-bêtes** une fois que vous êtes prêt à commencer l’estimation.![estimation_launch.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016786471186_estimation%20launch.gif)*Lancement de la session d’estimation*![estimation_app_jira_cards.png](../../../../../../docs/using-miro/facilitation-tools/images/21016786474514_estimation_app_jira_cards.png)*Utilisation de l’application Estimation avec les cartes Jira*

Toutes les personnes sur le tableau (et celles qui rejoignent le tableau quand la session d’estimation est en cours) pourront rejoindre la session d’estimation. Toutes les personnes qui participent doivent disposer des autorisations de modification du tableau et Jira. Les estimations peuvent être effectuées de manière synchrone ou asynchrone. Toutes les estimations sont anonymes.

![join_estimation.jpg](../../../../../../docs/using-miro/facilitation-tools/images/21016751234578_join%20estimation.jpg)
*La fenêtre contextuelle pour rejoindre la session d’estimation*

Les utilisateurs seront redirigés vers le premier élément pour ajouter leurs estimations après avoir cliqué sur **Rejoindre l’estimation**. Les utilisateurs peuvent voter sur tous les éléments ou en passer certains et voter uniquement sur des éléments particuliers. Pour modifier une estimation, cliquez sur l’icône de stylo.

![adding_estimates.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751237010_adding%20estimates.gif)
*Estimation en cours*

La personne en charge d’animer la session peut, en cours de session, voir un sondage des estimations fournies pour chaque élément et les avatars des personnes ayant fourni une estimation. Lorsque des estimations ont été fournies pour tous les éléments par tous les participants requis, la personne qui anime la session peut « Choisir l’estimation finale » pour chaque élément. Il ou elle peut également modifier les estimations approuvées.

![agreed_estimates.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751238162_agreed%20estimates.gif)
*Estimation terminée*

Une fois tout le monde d’accord sur les estimations pour tous les éléments, la personne qui anime la session verra apparaître la fenêtre contextuelle avec l’option de fin de session et de partage des résultats. Elle peut également cliquer sur **Terminer l’estimation pour tous** pour terminer la session à tout moment. Cela affiche le nombre total de points. Cliquez sur **Terminer et partager les résultats** dans la fenêtre contextuelle et les résultats de la session seront enregistrés.

![end_session.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751242386_end%20session.gif)
*Accord d’estimation*

Si vous estimez des cartes ou des pense-bêtes Miro, les estimations sont enregistrées en tant qu’étiquettes sur les cartes ou les pense-bêtes.

![estimate_tags.jpg](../../../../../../docs/using-miro/facilitation-tools/images/21016786489362_estimate%20tags.jpg)
*Les étiquettes indiquent les estimations des cartes*

Si vous estimez les cartes Jira à l’aide de la technique d’estimation **Fibonacci**, les estimations sont enregistrées sur Jira (la synchronisation ne fonctionne actuellement que pour les estimations Fibonacci). Notez que la personne qui organise la session doit se connecter avec ses identifiants Jira avant de donner les estimations finales. Les résultats de l’estimation seront automatiquement synchronisés avec les tickets Jira correspondants.

**Pour que les estimations Fibonacci s’affichent sur les cartes Jira et dans les tâches Jira :**

1. Vérifiez que le champ Story Points (Points du récit) est configuré dans Jira.
2. Vérifiez que vous disposez des autorisations nécessaires dans Jira pour mettre à jour la valeur du champ Story Points (Points du récit).
