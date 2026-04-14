---
title: 'Guide d''importation de Mural à Miro : Copier-coller'
article_id: 22957521683986
translation_id: 22957521683986
locale: fr
sidebar_position: 1
created_at: '2024-11-29T13:36:36Z'
updated_at: '2025-11-25T15:49:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personnes: Utilisateurs disposant d''un accès avec droits de modification
    Forfaits: Free, Starter, Business, Enterprise, Education Plateformes: Navigateur,
    Bureau, Mobile'
---

Vous pouvez transférer le contenu de vos tableaux Mural vers Miro en utilisant la méthode de copier-coller. Ce guide fournit les meilleures pratiques pour cette méthode d'importation, explique le processus étape par étape et détaille ce à quoi vous pouvez vous attendre en termes d'apparence et de comportement des différents objets une fois collés dans Miro.

## Lignes directrices pour l'importation depuis Mural

Le respect de ces directives vous aidera à obtenir les meilleurs résultats lors du transfert de contenu de Mural à Miro.

Pour les données structurées, comme les cartes mentales Mural, la méthode copier-coller est généralement la meilleure approche pour éviter de rompre les connexions entre les éléments.

:::note
Pour importer du contenu dans Miro en utilisant cette méthode, le contenu Mural doit être sous licence complète ou sous licence gratuite restreinte dans Mural.
:::

La méthode de copier-coller est également recommandée pour importer des widgets individuels qui ne sont pas pris en charge par le [guide d'importation de Mural vers Miro (PDF)](02-mural-to-miro-import-guide-–-pdf.md), ou pour les widgets qui ne sont pas importés avec une grande fidélité en utilisant la méthode PDF.

Soyez conscient de certaines limitations avec la méthode copier-coller : certains attributs de style et toutes les images qui ont été initialement chargées sur Mural (plutôt que liées via URL) ne seront pas copiés dans votre presse-papiers et ne seront donc pas transférés vers Miro.

## Copier et coller le contenu de Mural vers Miro

La procédure suivante explique comment copier le contenu d'un tableau Mural et le coller sur un tableau Miro.

**Prérequis**

Assurez-vous d'avoir accès en modification au tableau source dans Mural et au tableau de destination dans Miro.

Pour copier le contenu d'un tableau Mural et le coller sur un tableau Miro :

1. Dans Mural, sélectionnez les objets que vous souhaitez copier.
   > 💡 Pour sélectionner tous les objets sur le tableau Mural, utilisez le raccourci clavier **Ctrl+A** (Windows) ou **Cmd+A** (Mac).
2. Pour copier les objets sélectionnés, utilisez le raccourci clavier **Ctrl+C** (Windows) ou **Cmd+C** (Mac).
   Vos objets Mural sont maintenant copiés dans votre presse-papiers.
3. Dans Miro, ouvrez le tableau où vous souhaitez coller le contenu. Utilisez le raccourci clavier **Ctrl+V** (Windows) ou **Cmd+V** (Mac) pour coller.

   Vous avez réussi à copier et coller du contenu de Mural vers Miro.
   > 📌 Le contenu collé depuis Mural peut nécessiter un ajustement manuel dans Miro. Certains aspects de style et de formatage peuvent apparaître différemment après collage.

## Apparence de l'objet après collage

Les objets de Mural peuvent généralement être copiés et collés dans Miro avec quelques variations par rapport à leur état d'origine. Cette section décrit les résultats attendus pour certains objets courants et fournit les meilleures pratiques, le cas échéant.

### Zones

Les zones de Mural copié-collé en tant que cadres et formes dans Miro.

Une zone Mural avec une transparence de 100 % affichera une bordure transparente mais visible lorsque collée dans Miro. Si la zone Mural a un titre, ce titre apparaît et se comporte dans Miro comme un titre de cadre.

![Zone murale avec titre, et arrière-plan et bordure transparents à 100 %.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Un espace libre Mural avec un titre, et un fond et une bordure à 100 % transparents*

![Une zone collée de Mural à Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Une zone collée de Mural à Miro*

### Connecteurs

Les connecteurs de Mural copié-collés en tant que connecteurs Miro.

Pour les badges de connecteurs, les positions verticales et horizontales seront collées comme centrées dans Miro. Miro ne prend en charge qu'une position centrée pour les libellés de connecteur.

En ce qui concerne les types de connecteurs, Miro prend en charge les lignes *pleines*, *pointillées* et *en tirets*. Mural inclut également un type de connecteur *pointillé large*. Miro mappe les types de connecteurs collés depuis Mural comme suit : *solid* se mappe à *solid*, et le type *loosely dashed* de Mural se mappe au type *dashed* de Miro. D'autres correspondances directes (comme pointillé à pointillé) sont également préservées.

Miro prend en charge chaque type de courbe de connecteur Mural, bien que leur apparence dans Miro puisse légèrement différer.

![Une courbe de connecteur Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Courbe de connecteur Mural*

![Une courbe de connecteur Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Courbe de connecteur Miro*

### GIFs et images

Les GIF et les images qui ont été initialement ajoutés à Mural à partir d'une URL peuvent être copiés-collés dans Miro.

:::note
Un GIF ou une image dans Mural qui a été téléchargé(e) directement depuis un appareil ou ajouté(e) depuis la barre d'outils de Mural ne peut pas être copié-collé dans Miro en utilisant cette méthode.
:::

### Cartes mentales

Les cartes mentales de Mural sont copiées-collées en tant que cartes mentales Miro, y compris le nœud racine, chaque nœud enfant et leur texte.

Le style du nœud racine est en grande partie préservé. Cependant, le rayon de la forme peut différer, et la taille de police du texte n'est pas conservée lors du passage de Mural à Miro.

Les nœuds enfants à partir de Mural se collent comme des nœuds de texte Miro, et leur style n'est pas préservé.

La couleur et l'épaisseur des connecteurs dans la carte mentale peuvent également varier.

![Une carte mentale copiée dans Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)
*Carte mentale copiée dans Mural*

![Une carte mentale copiée-collée de Mural vers Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Carte mentale copiée-collée dans Miro*

Pour les cartes mentales de Mural qui ont plusieurs niveaux de nœuds, l'ordre des nœuds peut changer lorsqu'ils sont collés dans Miro.

![Une carte mentale dans Mural avec plusieurs niveaux de nœuds.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Carte mentale dans Mural avec plusieurs niveaux de nœuds*

![Une carte mentale avec plusieurs niveaux de nœuds copiés-collés de Mural à Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Carte mentale avec plusieurs niveaux de nœuds copiés-collés de Mural vers Miro*

:::tip
Les cartes mentales copiées-collées de Mural vers Miro peuvent perdre leur échelle originale. Pour redimensionner la carte mentale après l'avoir collée, vous pouvez l'étirer manuellement sur le tableau Miro.
:::

### Formes

Les formes de Mural se collent généralement sous forme de formes Miro. Miro prend en charge la plupart des formes de Mural directement.

Cependant, Mural inclut 16 formes spécifiques qui n'ont pas d'équivalent direct dans Miro. Ces formes seront collées dans Miro sous forme de rectangles.

![Les 16 formes qui se copient-collent de Mural à Miro en tant que rectangles.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Les 16 formes qui se copient-collent de Mural à Miro sous forme de rectangles*

### Pense-bêtes

Les pense-bêtes de Mural se collent comme des pense-bêtes de Miro.

Miro mettra en correspondance la couleur et le niveau d'opacité des pense-bêtes avec les options les plus proches disponibles dans Miro.

Les différences suivantes peuvent également apparaître lorsque vous copiez-collez des pense-bêtes de Mural vers Miro :

- Les pense-bêtes circulaires de Mural sont collés dans Miro en pense-bêtes carrés.
- Les listes à l'intérieur des pense-bêtes ne sont pas conservées en tant que listes interactives, bien que les éléments de ligne individuels apparaissent sur des lignes distinctes à l'intérieur du pense-bête Miro.
- La taille de la police du texte n'est pas conservée, car les pense-bêtes Miro définissent automatiquement la taille de la police en fonction du contenu et de la taille du pense-bête.
- La rotation appliquée aux pense-bêtes dans Mural n'est pas conservée lors du collage.

![Pense-bêtes copiés dans Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Pense-bêtes copiés dans Mural*

![Pense-bêtes copiés-collés depuis Mural vers Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Pense-bêtes copiés-collés dans Miro*

### Tables

Les tables de Mural collent comme des tables Miro.

Les différences suivantes peuvent apparaître lorsque vous copiez-collez des tableaux de Mural à Miro. Pour chacun de ces éléments, vous pouvez généralement restaurer vos préférences manuellement dans Miro après avoir collé :

- Les tables positionnées au-dessus d'autres objets dans Mural (comme des zones, des formes ou des images) peuvent être partiellement cachées derrière ces objets lorsqu'elles sont collées dans Miro. Vous devrez peut-être ajuster leur superposition (mettre au premier plan).
- La couleur de la bordure est ignorée ; les bordures seront collées en gris.
- L'opacité de l'arrière-plan est ignorée. Les cellules transparentes dans Mural seront collées en tant que cellules blanches dans Miro. Cependant, la couleur de fond elle-même (si elle n'est pas transparente) est généralement préservée.
- La famille de polices de texte est ignorée ; le texte sera collé en utilisant la police de tableau par défaut de Miro (RobertPro).
- La mise en forme du texte en ligne, comme le gras et l'italique, est ignorée dans les cellules du tableau.

![Une table avec un formatage mixte copiée dans Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Tableau avec formatage mixte copié dans Mural*

![Table with mixed formatting copy-pasted from Mural to Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Tableau avec mise en forme mixte copié-collé dans Miro*

### Texte

Les objets texte de Mural se collent comme des objets texte dans Miro. Les familles de polices originales de Mural ne sont pas conservées. Miro associe la famille de polices Mural à la police la plus proche disponible dans Miro et adapte le texte collé pour des résultats optimaux sur le tableau Miro.
