---
title: Importer des tableaux Lucidspark dans Miro
article_id: 9549014537490
translation_id: 9549014537490
locale: fr
sidebar_position: 7
created_at: '2023-01-12T09:05:07Z'
updated_at: '2026-01-19T14:30:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  plans: free, starter, business, Education et Enterprise
  notes: 'Utilisateurs: Tout utilisateur disposant des droits de modification sur
    les tableaux Lucidspark et Miro Plateformes: Navigateur, Desktop'
---

Migrez votre contenu Lucidspark de manière transparente dans Miro pour une expérience de collaboration plus robuste. Ce guide décrit comment importer vos tableaux et ce à quoi s'attendre pendant le processus.

> **⚠️ Avertissement :** L’édition de contenu importé est à sens unique. Les changements effectués dans Miro ne seront pas synchronisés avec Lucidspark.

> **💡 Note :** Les tableaux Lucidspark sous licence Free ou restreinte peuvent être migrés.

## Comment importer des tableaux Lucidspark via l'export PDF

Suivez ces étapes pour importer vos tableaux Lucidspark dans Miro en utilisant la méthode d'exportation PDF :

1. Assurez-vous d'exporter le contenu **Lucidspark** que vous souhaitez importer dans Miro en tant que PDF.
2. Sur le tableau de bord **Home** de Miro, cliquez sur **+ Créer nouveau**.
3. Sélectionnez **Importer**, puis **Importer de Lucidspark**.
   La fenêtre modale **Importer de Lucidspark** s'ouvre. Vous pouvez importer en masse plusieurs PDF de Lucidspark.
4. Suivez les instructions à l'écran fournies dans la fenêtre modale.
5. Sélectionnez **Importer les tableaux**.
6. Examinez le contenu importé et procédez aux ajustements nécessaires. Bien que Lucidspark et Miro aient des fonctionnalités similaires, il peut y avoir des différences dans les options de style et de formatage. Consultez [Comment les objets Lucidspark apparaissent dans Miro (méthode d'importation en masse de fichiers PDF)](#lucidspark-object-mapping-bulk-import) pour obtenir des conseils sur la manière dont les objets sont traduits.

## Méthode alternative : Copier et coller le contenu

Pour une alternative plus rapide pour de petites quantités de contenu, vous pouvez directement copier des éléments depuis un tableau Lucidspark ouvert et les coller sur un tableau Miro.

> **Remarque :** Tout utilisateur disposant d’un accès d’édition aux tableaux Lucidspark et Miro devrait pouvoir copier le contenu de Lucidspark et le coller dans Miro. Pour plus de détails sur la façon dont les objets sont traduits avec cette méthode, voir [Comment les objets Lucidspark apparaissent dans Miro (Méthode Copier/Coller)](#lucidspark-object-mapping-copy-paste).

## Comment les objets Lucidspark apparaissent dans Miro (Méthode Copier/Coller)

Ce tableau fournit une comparaison complète de la façon dont les objets sont traduits lorsque vous copiez du contenu directement de Lucidspark et le collez dans Miro.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Cartes Azure | Les cartes Azure sont migrées en tant que cartes Miro : 1. Configurez l’intégration Azure dans Miro. 2. Convertissez les cartes Miro en [cartes Azure](../../integrations-apps/microsoft/03-azure-cards.md). |
| Collaborateurs et partage | 🟠 Peut être recréé manuellement |
| Commentaires | 🟠 Peut être recréé manuellement |
| Connecteurs et Séparateurs | Connecteurs |
| Conteneurs | Formes |
| Documents à partir de fichiers et d'URL | 🟠 Peut être recréé manuellement |
| URL des documents (PDF) | Documents intégrés |
| Dessiner | Images |
| Tableaux dynamiques | Tables |
| Émojis | Images |
| Cadres | Cadres |
| GIF de la barre d’outils | Images |
| GIF à partir de fichiers | Images |
| GIF depuis des URL | GIF |
| Images | Images |
| Cartes Jira | Les cartes Jira sont migrées en tant que cartes Miro :  1. Configurer l’intégration de Jira dans Miro 2. Convertir les cartes Miro en [cartes Jira](../../integrations-apps/atlassian/03-jira-cards.md). |
| Cartes Lucid | Cartes |
| Carte mentale | Carte mentale |
| Formes | Formes |
| Pense-bête | Pense-bêtes |
| Tables | Tables |
| Texte | Texte |
| Planning | 🟠 Peut être recréé manuellement |
| Vidéos et autres URL | Aperçus |

## Comment les objets Lucidspark apparaissent dans Miro (Méthode d'importation massive par PDF)

Ce tableau fournit une comparaison complète des objets entre Lucidspark et Miro après l’importation en masse de votre contenu via PDF.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Cartes Azure | Images |
| Collaborateurs et partage | 🟠 Peut être recréé manuellement |
| Commentaires | 🟠 Peut être recréé manuellement |
| Connecteurs et séparateurs | Connecteurs |
| Conteneurs | Formes |
| Documents | 🟠 Peut être recréé manuellement |
| Dessiner | Lignes |
| Tableaux dynamiques | Formes et connecteurs |
| Émojis | Images |
| Cadres | Cadres et formes |
| GIFs | Images |
| Images | Images |
| Cartes Jira | Formes |
| Cartes Lucid | Formes |
| Carte heuristique | Formes et connecteurs |
| Formes | Formes |
| Pense-bête | Pense-bêtes |
| Tables | Tables/formes et connecteurs |
| Texte | Texte |
| Planning | Formes et connecteurs |
| Vidéos et autres URL | 🟠 Peut être recréé manuellement |

## Limitations de l'import

Bien que Lucidspark et Miro offrent des fonctionnalités similaires, veuillez noter les différences et limitations suivantes lors de l'importation de contenu :

- Les zones de texte Miro peuvent contenir jusqu’à 6 000 caractères, espaces compris. Tout texte supplémentaire sera recadré.
- Les couleurs et les styles sont rétablis au plus proche de la version d’origine dans Miro.
- Les valeurs d’opacité de Lucidspark ne sont pas extraites avec précision lors de l’importation.
- Les pense-bêtes Miro ne prennent pas en charge la rotation, l’ajustement de la palette de couleurs ou le formatage du texte en liste à puces, qui peuvent avoir été appliqués dans Lucidspark.

## Obtenir de l’aide

> **Remarque :** Pour toute autre question ou assistance concernant la migration de Lucidspark, veuillez contacter l’[assistance Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) ou votre Customer Success Manager Miro directement.
