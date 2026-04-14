---
title: Whiteboards.io Importer pour Miro
article_id: 20624350720402
translation_id: 20624350720402
locale: fr
sidebar_position: 3
created_at: '2024-08-07T16:30:40Z'
updated_at: '2026-01-19T14:08:30Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
---

ServiceRocket's Whiteboards.io Importer for Miro est une solution conviviale conçue pour rationaliser l'importation de données à partir de l'application [Tableau blanc.io](https://whiteboards.io/) vers l'application [Miro](https://miro.com/app/dashboard/). Chargez rapidement et facilement vos sauvegardes générées par le tableau blanc.

Obtenez votre accès à l'importateur dès aujourd'hui. Visitez le site `https://www.servicerocket.com/miro/whiteboards-io-miro-migration` pour plus de détails.

## **Exporter des tableaux depuis Whiteboards.io**

1. Connectez-vous à [Tableaux blancs.io](https://whiteboards.io/).
2. Sur la page principale, cliquez sur Exporter les tableaux dans le message d'état d'avertissement.

*Cliquez sur Exporter les tableaux dans le message d'état de l'avertissement pour démarrer*

3. Ensuite, procédez aux étapes suivantes pour exporter le tableau.

*Vérifiez que les tableaux sont corrects lors de l'exportation de votre tableau*

1. 1. Sélectionnez le format .json uniquement.
   2. Décochez la case Inclure les médias (images, vidéos et autres fichiers).
   3. Cliquez sur Exporter pour confirmer les tableaux et exporter le tableau.

4. Un fichier .zip sera généré avec succès.

## **Importation des tableaux de Whiteboards.io dans Miro**

1. Ouvrez votre tableau Miro.
2. Dans la barre d'outils, cliquez sur Plus d'applications > sélectionnez ou recherchez Whiteboards.io Miro Importer.
3. Cliquez sur Choisir un fichier pour charger le fichier (.zip) généré à partir de l'application [Tableaux blancs.io](http://whiteboards.io/) application.
4. Ensuite, sélectionnez le tableau que vous souhaitez importer et cliquez sur Importer.
5. Une fois l'importation terminée, le système affichera le statut du tableau comme étant TERMINÉ.
6. Fermez l'application et revenez à la page principale de Miro. L'application importera les tableaux sélectionnés dans votre compte d'équipe.

## **Cartographie des données de tableaux blancs.io dans Miro**

Le mappage des données est essentiel pour maintenir l'intégrité et la cohérence des données, ainsi que les différences de schéma pendant la transition d'une application à l'autre. Les tableaux ci-dessous répertorient toute la terminologie équivalente, les structures de données, les noms de champs, les formats, etc.

|  |  |  |
| --- | --- | --- |
| **Tableaux blancs.io** | **Miro** | notes |
| Texte | [Texte](https://developers.miro.com/docs/text-1) | N/A |
| forme | [forme](https://developers.miro.com/docs/shape-1) | - La forme du cœur sera importée sous la forme d'un nuage. - La forme paperTape sera importée sous la forme d'un diagramme de flux entrée-sortie. - Une icône sera importée sous forme d'image. |
| Carte | [Pense-bête](https://developers.miro.com/docs/stickynote-1) | - Le formatage des polices sera perdu lors de la conversion vers une carte. - La couleur de la carte sera perdue et l'alignement ne sera pas correct. - La taille de la pense-bête peut varier. |
| Ligne | [Connecteur](https://developers.miro.com/docs/connector_intro) | N/A |
| cadre | [cadre](https://developers.miro.com/docs/frame-1) | Les objets enfants du cadre ne peuvent pas être liés au cadre parent. |
| Free Draw | [Image](https://developers.miro.com/docs/image-1) (.svg) | N/A |
| Commentaires | N/A | Aucune méthode n'est prévue dans Miro pour cartographier cela. |
| Fichier | [Fichier](../../troubleshooting-technical-questions/technical-guidelines/03-supported-file-formats.md) | Type et format de fichier :   - Images - Tableaux et feuilles de calcul - Documents de texte - Présentations |
| Image | [Image](https://developers.miro.com/docs/image-1) | N/A |
| Intégrer une iFrame | [Intégration](https://developers.miro.com/docs/embed-2) | N/A |
| Table à cartes | [Carte](https://developers.miro.com/docs/card-1) et [cadre](https://developers.miro.com/docs/frame-1) | Sans le nom de la colonne et du couloir. |
| Carte mentale | [Carte mentale](https://developers.miro.com/docs/mind-maps) (expérimentale) | La couleur de la bordure n'est pas prise en charge. |
| Carte GitHub | [Carte](https://developers.miro.com/docs/card-1) | N/A |
| Carte Jira | Texte avec l'URL du ticket Jira | N/A |
