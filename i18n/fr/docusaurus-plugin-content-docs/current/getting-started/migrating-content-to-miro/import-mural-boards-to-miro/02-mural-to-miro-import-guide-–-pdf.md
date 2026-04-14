---
title: Guide d'importation de Mural vers Miro – PDF
article_id: 22856050009362
translation_id: 22856050009362
locale: fr
sidebar_position: 2
created_at: '2024-11-25T14:36:20Z'
updated_at: '2026-01-19T14:43:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personnes: Utilisateurs avec accès de modification Formules: Business, Education,
    Enterprise, Starter Plateformes: Navigateur, Bureau'
---

Vous pouvez importer vos tableaux Mural existants dans Miro en les exportant de Mural sous forme de fichiers PDF, puis en important ces PDF dans Miro. Cet article fournit des conseils pour obtenir les meilleurs résultats avec les importations PDF, explique la procédure d'importation et décrit ce à quoi vous pouvez vous attendre lorsque différents éléments de Mural sont importés dans Miro en utilisant cette méthode.

La méthode d'importation PDF est particulièrement efficace pour le contenu qui peut ne pas se transférer facilement via le copier-coller ou les importations basées sur l'API. L'importateur PDF de Miro analyse les formes et leurs coordonnées au sein du PDF de Mural et tente de reconstruire la disposition originale. Par exemple, il peut interpréter des lignes qui se croisent comme une structure de table.

Veuillez noter que certains objets peuvent apparaître différemment dans Miro après l'importation, et que le style ou la mise en page précis peuvent nécessiter des ajustements manuels ou une recréation dans Miro. En général, le contenu plus simple avec un style moins complexe tend à donner des résultats d'importation plus précis.

## Lignes directrices pour l'importation depuis Mural

Pour obtenir les meilleurs résultats lors de l'importation de contenu Mural sous forme de PDF, il est utile de comprendre comment fonctionne l'importateur et quel contenu se transfère le plus efficacement. L'importateur PDF correspond principalement aux formes élémentaires et aux lignes.

:::note
**Remarque :** Pour importer du contenu dans Miro, votre contenu Mural doit être sous licence totale ou licence gratuite restreinte dans Mural.
:::

Un espacement clair entre les éléments dans votre Mural permet à l'importateur Miro de mieux interpréter le contenu. Un tableau Mural avec de nombreux éléments rapprochés peut produire des résultats d'importation mitigés ou moins précis.

Pour un import avec la meilleure fidélité, assurez-vous que votre contenu Mural **ne contient pas** les attributs suivants, car ils peuvent ne pas bien se transférer via PDF :

- Polices personnalisées
- Stylisation complexe transformant les formes de base (par exemple, coins très arrondis sur les rectangles, flèches courbées de manière unique)
- Nombreuses formes et lignes qui se chevauchent
- Éléments pivotés

:::tip
**Conseil :** Si vous devez préserver le style exact, les mises en page complexes ou les coordonnées précises de votre contenu Mural, la méthode la plus fiable est d'exporter le contenu de Mural en tant qu'image statique (par exemple, PNG, JPG) et d'importer ensuite cette image dans votre tableau Miro.
:::

## Importer des tableaux Mural dans Miro sous forme de PDF

Cette section explique comment importer votre contenu Mural dans Miro en utilisant la fonctionnalité d'importation de PDF.

### Prérequis pour l'importation de PDF

Avant de commencer le processus d'importation, veuillez vous assurer que vous remplissez les prérequis suivants :

- Vous devez avoir accès pour modifier le tableau source dans Mural (pour l'exporter sous forme de PDF).
- Vous devez avoir accès pour modifier le tableau de destination dans Miro où vous envisagez d'importer le contenu.
- Vous devez avoir déjà téléchargé votre ou vos tableaux Mural sous forme de fichiers PDF.

**Plus d'informations :** Pour obtenir des instructions sur l'export depuis Mural, consultez la documentation de Mural sur [l'exportation et le téléchargement du contenu de votre Mural](https://support.mural.co/s/article/export-and-download-your-mural-s-content) (lien externe).

### Importer le PDF

Suivez ces étapes pour importer vos fichiers PDF de Mural dans Miro :

1. Depuis votre tableau de bord Miro, cliquez sur le bouton **+ Créer nouveau**.
2. Dans le menu déroulant, sélectionnez **Importer**, puis choisissez **Importer depuis Mural**.
   La **fenêtre modale Importer des tableaux depuis Mural** s'ouvrira.
3. Suivez les instructions à l’écran dans la fenêtre modale. Vous serez invité à charger vos fichiers PDF Mural.
   Vous pouvez éventuellement choisir d’ajouter votre contenu importé à un espace Miro spécifique. Si vous ne spécifiez pas d’espace, le contenu importé sera ajouté à votre espace principal d’équipe.
4. Une fois que vous avez chargé vos fichiers et configuré les options, sélectionnez **Importer des tableaux**.
   Le processus d’importation débutera. Vous recevrez une notification par e-mail de Miro lorsque l’importation sera terminée.

Vous avez maintenant importé avec succès votre contenu Mural dans Miro via PDF.

## Résultats attendus

Lorsque les objets Mural sont importés dans Miro via PDF, quelques variations dans le style et le formatage peuvent survenir, en raison des différences entre les plateformes et de la nature de la conversion en PDF. Cette section décrit les résultats typiques de l'importation pour les objets Mural courants et propose quelques bonnes pratiques.

### Zones

La zone la plus externe de votre export Mural sera généralement importée comme un Cadre Miro. Les autres zones internes sont habituellement importées comme des formes classiques dans Miro.

:::note
**Remarque :** Les zones imbriquées (zones au sein d'autres zones) peuvent parfois être incorrectement identifiées ou structurées lors de l'importation. Le convertisseur PDF se base sur les coordonnées visuelles pour déterminer les relations parent-enfant des widgets, ce qui peut être ambigu avec des imbrications complexes.
:::

### Connecteurs

Le module d'importation PDF reconnaît principalement et recrée les connecteurs à ligne continue. Les connecteurs pointillés ou en tirets peuvent ne pas s'importer comme prévu.

Si un connecteur dans Mural comprend du texte intégré directement sur la ligne, le module d'importation PDF peut interpréter cela comme deux lignes séparées avec l'objet texte à proximité, plutôt qu'un seul connecteur avec texte.

![A connector with text that the PDF importer breaks into two lines.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Un connecteur avec texte que le module d'importation PDF "divise" en deux lignes.*

### Dessins

Les éléments dessinés à la main à partir de Mural s'importent généralement comme une collection de lignes ou de courbes dans Miro.

Pour les dessins complexes, l'importateur PDF peut parfois lier incorrectement des parties du dessin à des objets chevauchants ou voisins, les interprétant comme des connecteurs là où il n'y en avait pas l'intention.

![A drawing may import as linked to a nearby or overlapping object.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Un dessin peut être importé comme lié à un objet voisin ou chevauchant.*

### GIFs

L'importateur PDF reconnaîtra les GIFs de Mural mais les importera comme des images statiques (typiquement le premier cadre du GIF).

:::note
**Note :** Le format de fichier PDF ne prend pas en charge les GIFs animés. C'est une limitation du PDF, non de l'importateur Miro.
:::

### Images

Les images de votre tableau Mural seront importées en tant qu'images dans Miro. Cependant, leur position exacte sur le tableau peut changer légèrement en raison des différences entre les systèmes de coordonnées de Mural et de Miro, ainsi que du processus de conversion en PDF.

### Listes

Les listes (numérotées et à puces) de Mural sont généralement importées comme des listes dans Miro. Pour obtenir les meilleurs résultats, assurez-vous que vos listes dans Mural utilisent des marqueurs par défaut (chiffres standards pour les listes ordonnées, et puces basiques pour les listes non ordonnées).

![A numbered list, and a bulleted list, with default markers, numerals and bullets respectively.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Une liste numérotée et une liste à puces avec des marqueurs par défaut, des chiffres et des puces respectivement.*

### Cartes mentales

La méthode d'importation en PDF fonctionne mieux pour les cartes mentales de Mural ayant un seul nœud racine et des bordures visibles sur tous les nœuds. Les cartes mentales complexes avec plusieurs racines ou des bordures cachées peuvent ne pas être importées avec précision.

![A basic Mind map is easier to import as PDF.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Une carte mentale basique est plus facile à importer en PDF*

L'importateur de PDF peut rencontrer des difficultés pour analyser avec précision les cartes mentales car elles contiennent souvent de nombreuses lignes et objets en proximité. Si l'importation de votre carte mentale en PDF est mal effectuée, envisagez de copier et coller directement le contenu de la carte mentale de Mural à Miro. Bien que la méthode de copie-collage puisse nécessiter des ajustements manuels de style et d'échelle dans Miro, la fidélité structurelle globale pourrait être meilleure pour certaines cartes mentales.

### Formes

L'importateur de PDF est conçu pour importer les formes de base de Mural (par exemple, rectangles, ovales, triangles) en tant que formes modifiables dans Miro.

![Only basic shapes import as editable content.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Seules les formes de base sont importées comme contenu modifiable*

Les formes avancées, personnalisées ou fortement stylisées de Mural, ainsi que les formes pivotées, peuvent être importées sous forme d'images statiques plutôt que de formes éditables de Miro.

### Pense-bêtes

Les pense-bêtes standard de Mural sont généralement importés en tant que pense-bêtes de Miro. Pour une fidélité maximale, utilisez des pense-bêtes de Mural avec des formats d'image par défaut (par exemple, tailles courantes 3x3 ou 5x3).

![Sticky notes with the default size can be easily imported.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Les pense-bêtes avec des tailles par défaut peuvent être facilement importés*

:::note
**Note :** Les pense-bêtes ronds de Mural seront importés sous forme de formes régulières dans Miro, car Miro ne dispose pas d'un objet pense-bête rond natif.
:::

Les pense-bêtes qui se chevauchent ou qui sont tournés peuvent ne pas être importés avec une grande fidélité et pourraient nécessiter un repositionnement ou des ajustements manuels dans Miro.

![Import results vary for rotated sticky notes, and sticky notes that overlap.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Les résultats d’importation varient pour les pense-bêtes tournés et ceux qui se chevauchent.*

### Tables

Les tables simples de Mural avec des lignes de grille claires s'importent généralement avec une grande fidélité sous forme de tables Miro ou comme un ensemble de formes et de lignes formant une structure de table.

Les tables avec une géométrie complexe peuvent être importées sous la forme d'une série de lignes déconnectées et de zones de texte. Pour obtenir les meilleurs résultats lors de l'importation de tables, assurez-vous que les tables de votre export Mural **ne possèdent pas** les attributs suivants :

- Cellules fusionnées
- Bordures invisibles ou cachées
- Coins arrondis sur les cellules ou la bordure de la table

![Complex tables do not import with high fidelity.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Les tables complexes ne s'importent pas avec une haute fidélité.*

### Texte

Les objets texte de Mural sont généralement importés en tant que texte modifiable dans Miro, souvent dans un seul bloc de texte ou une forme correspondant à la zone de texte originale de Mural.

Pour un import de texte de la plus haute fidélité, utilisez les polices par défaut et les marges standards dans Mural.

:::note
**Note :** La taille de la police peut varier après l'importation et vous devrez peut-être l'ajuster manuellement dans Miro.
:::

L'importateur PDF peut diviser le texte qui utilise des polices personnalisées ou s'il a un style complexe (par exemple, plusieurs styles dans une seule zone de texte) en plusieurs blocs de texte plus petits.
