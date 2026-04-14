---
title: Importer des diagrammes Visio dans Miro
article_id: 11842818558738
translation_id: 11842818558738
locale: fr
sidebar_position: 8
created_at: '2023-06-06T10:11:36Z'
updated_at: '2026-02-16T14:27:52Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personnes: Tous les utilisateurs avec des forfaits éligibles Forfaits: Business,
    Enterprise Plateformes: Navigateur, Bureau, Mobile'
---

Transférez facilement vos diagrammes depuis MS Visio vers Miro et commencez à collaborer dans un outil unifié.

Les diagrammes importés sont entièrement fonctionnels, vous pouvez donc les modifier, les colorier, les déplacer et les redessiner selon vos besoins.

:::warning
La modification des diagrammes importés ne fonctionne que dans un sens. Les modifications apportées dans Miro ne seront pas répercutées dans Visio.
:::

## Importer un seul diagramme Visio vers un nouveau tableau Miro

Procédez comme suit pour importer un diagramme Visio individuel. Le diagramme importé créera un nouveau tableau Miro :

1. Dans Visio, ouvrez le diagramme que vous souhaitez exporter.
2. Sélectionnez le menu **Fichier** et choisissez **Enregistrer sous**. Sélectionnez un emplacement et enregistrez votre fichier au format `.vsdx`.
3. Naviguez jusqu’au tableau Miro à partir duquel vous souhaitez initier l'importation. Cela peut être n'importe quel tableau, car l'importation en créera un nouveau.
4. Dans la barre d'outils de création à gauche, sélectionnez **Formes** > **Plus de formes**, puis sélectionnez l'icône **Importer un diagramme** située en haut à droite du panneau de la bibliothèque de formes de diagrammes.
5. Dans la boîte de dialogue qui apparaît, faites glisser et déposez le fichier `.vsdx` Visio, ou cliquez sur le bouton **Choisir un fichier** et naviguez pour sélectionner le fichier depuis votre système.
6. Sélectionner **Importer**.
   Lorsque le processus d'importation est terminé, vous verrez une boîte de dialogue **Fichier importé**.
7. Cliquez sur **Aller au tableau** pour ouvrir le nouveau tableau Miro contenant votre diagramme importé.

## Importation en masse de plusieurs diagrammes Visio

Vous pouvez également importer plusieurs diagrammes Visio dans Miro simultanément depuis votre tableau de bord. Chaque diagramme sera importé dans son propre nouveau tableau Miro, nommé d'après le nom de fichier d'origine :

1. Accédez à votre [tableau de bord Miro](https://miro.com/app/dashboard/).
2. Sélectionnez **+ Créer un nouveau** > **Importer** > **Importer un diagramme**.
3. Glissez vos fichiers `.vsdx` dans la zone désignée ou utilisez le lien **choisir des fichiers** pour sélectionner plusieurs diagrammes Visio. Notez que vous pouvez toujours supprimer des fichiers avant l'importation.
4. Sélectionnez **Importer des fichiers**.
   Lorsque le processus d'importation est terminé, vous verrez une boîte de dialogue **Fichiers importés**.
5. Sélectionnez **Terminé**.

Cela crée un nouveau tableau pour chaque diagramme, nommé d'après le nom de fichier d'origine.

## Comprendre la cartographie des objets Visio dans Miro

Le tableau suivant compare comment les objets et formes de Visio sont généralement représentés une fois importés dans Miro. Notez que bien que Miro s'efforce de garantir une grande fidélité, certains ajustements manuels ou recréations peuvent être nécessaires pour les éléments complexes.

| **Visio** | **Miro** |
| --- | --- |
| Bloc | Texte, formes |
| Conteneurs | Formes |
| Documents | 🟠 Peut être recréé manuellement |
| Clé de répartition | Texte, formes |
| cadres | Cadres et formes |
| GIF | Images |
| Point d’accès | Lier vers |
| Images | Images |
| Ligne | Connecteurs |
| Organigrammes | Formes, images |
| formes | Formes |
| Conteneurs intelligents | Formes |
| Table intelligente | Formes |
| Pense-bête | Pense-bêtes |
| Tableaux | Formes |
| Texte | Texte |
| Calendrier | Formes |
| Activités visuelles | Formes |
| **Autres propriétés** | |
| Auteurs | 🟠 Peut être recréé manuellement |
| Collaborateurs et partage | 🟠 Peut être recréé manuellement |
| Commentaires | 🟠 Peut être recréé manuellement |
| Regrouper | Importé |
| Jeux d’icônes | Attaché aux formes |
| Calques | 🟠 Peut être recréé manuellement |
| Lier vers | Importé |
| Verrouiller | 🟠 Peut être recréé manuellement |
| Notes/Annotations | 🟠 Peut être recréé manuellement |
| **Formes** | |
| **Formes Visio** | **Formes Miro** |
| Architecture AWS | Formes > AWS |
| Azure | Formes > Azure |
| BPMN 2.0 | Formes > BPMN |
| Diagrammes de circuits | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Flux de données | Formes > Flux de données |
| Formes dynamiques | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Architecture d’entreprise | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Intégration d’entreprise | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Entité-association | Formes > ERD |
| Équations | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Plans d’étage | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Formes de diagramme de flux | Formes > Diagramme de flux |
| Formes géométriques | Formes |
| Google Cloud Platform | Formes > GCP |
| Kubernetes | Formes > Kubernetes |
| Cartes mentales | Cartes mentales |
| Infrastructure de réseau | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Ingénierie des procédés | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Architecture Salesforce | Formes > Salesforce |
| Diagrammes de racks de serveurs | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Plans du site | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Formes standard | Formes |
| Tech Clipart | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| Maquettes d’interface utilisateur | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
| UML | Formes > UML |
| Chaîne de valeur | Formes > Cartographie de la chaîne de valeur |
| Diagrammes de Venn | Importé et modifiable, mais non disponible dans la bibliothèque de formes de Miro |
