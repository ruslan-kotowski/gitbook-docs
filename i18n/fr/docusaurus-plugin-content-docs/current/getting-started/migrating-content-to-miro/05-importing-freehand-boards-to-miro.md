---
title: Importation de tableaux Freehand dans Miro
article_id: 18580556555538
translation_id: 18580556555538
locale: fr
sidebar_position: 9
created_at: '2024-04-26T16:34:28Z'
updated_at: '2025-11-25T15:42:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personnes: Tous les utilisateurs avec des forfaits éligibles Forfaits: Starter,
    Business, Education et Enterprise Plateformes: Navigateur, bureau, mobile (pour
    accéder à Miro et initier l''importation)'
---

Cet article explique comment importer des tableaux Freehand dans Miro, y compris comment préparer vos tableaux Freehand, pour des importations simples et en masse.

:::note
Les modifications que vous apportez au contenu importé dans Miro ne se synchronisent pas avec leur contenu d'origine dans Freehand.
:::

:::note
Vous pouvez uniquement importer des tableaux Freehand sous licences gratuites ou restreintes.
:::

## Importer un seul tableau de Freehand vers Miro

Vous pouvez facilement importer des tableaux Freehand individuels dans Miro en les exportant au format de fichier `.RTB` de Miro. Voici comment procéder :

1. Accédez au tableau Freehand que vous souhaitez exporter vers Miro.
2. Téléchargez le fichier en .RTB, le format propriétaire de Miro, directement à partir de Freehand. Naviguez dans le menu **Outils** et sélectionnez **Exporter vers le tableau Miro**. Le fichier sera enregistré dans votre dossier de téléchargement par défaut. Freehand vous informera une fois le téléchargement terminé.
3. Ouvrez votre tableau de bord Miro.
4. Dans la partie supérieure droite du tableau de bord Miro, cliquez sur le bouton **+ Créer nouveau**, cliquez sur **Importer**, puis sur **Importer une sauvegarde**.
5. Choisissez le fichier `.RTB` précédemment téléchargé depuis votre système.
6. Tout le contenu est maintenant importé dans un nouveau tableau Miro dans un format modifiable.
7. Bien que la plupart des contenus fassent l’objet d’une transition transparente, des ajustements mineurs peuvent s’avérer nécessaires en raison des variations dans les options de style et de formatage entre Freehand et Miro. Reportez-vous à la section Comment se fait la cartographie des objets Freehand dans Miro pour comprendre les différences potentielles.

## Importation en masse de plusieurs fichiers de Freehand vers Miro

Pour migrer plusieurs tableaux Freehand à la fois, Miro propose un processus d'importation en masse. Tout d'abord, assurez-vous que vos tableaux Freehand sont correctement préparés.

**Prérequis : Préparez vos tableaux Freehand pour l'importation en masse**

Procédez comme suit dans Freehand pour préparer vos tableaux :

1. Dans Freehand, sur la barre de menu du panneau de gauche, sélectionnez **Documents**. Un menu déroulant s’ouvre.
2. Sélectionnez **Tous les documents** ou **Créé par moi**, et spécifiez la période pour les tableaux que vous souhaitez importer dans Miro.
3. Pour chaque tableau que vous souhaitez importer, sélectionnez les trois points (**...**) et choisissez **Sélectionner**.
4. Dans le dialogue en bas de votre écran, sélectionnez **Déplacer**.
5. Sélectionnez un espace pour déplacer vos tableaux. Cela les regroupe pour faciliter le traitement par l'outil d'importation en masse.

   Vous avez réussi à préparer plusieurs fichiers pour l'importation en masse dans Miro.

Pour effectuer l'importation en masse de vos tableaux Freehand préparés vers Miro, suivez les instructions fournies dans le guide intégré du tableau Miro suivant :

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1IT00=/?pres=1&amp;frameId=3458764590689727256&amp;embedId=507813406404&amp;&amp;autoplay=yep" width="100%"></iframe>

:::note
Remarques importantes pour l'importation en masse :
- Le jeton Freehand utilisé pour la migration groupée n'est valable que pendant deux semaines à compter de la date à laquelle vous l'avez reçu.
- À partir du 31 décembre 2024, à 23h59 EST, Freehand et tous les jetons de migration associés seront supprimés et invalidés. Les utilisateurs ne pourront plus générer de nouveaux jetons ni accéder à Freehand pour la migration.
:::

## Examiner les meilleures pratiques

Pour une expérience de migration fluide, il est important de comprendre les meilleures pratiques et les considérations clés lors du transfert de votre contenu de Freehand à Miro. Veuillez examiner les instructions détaillées dans le tableau Miro intégré ci-dessous :

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1FWSM=/?pres=1&amp;frameId=3458764590691451227&amp;embedId=480338444592&amp;autoplay=yep" width="100%"></iframe>

## Cartographie d'objets dans Miro

Ce tableau fournit une comparaison complète de la façon dont les objets de Freehand sont généralement importés et représentés dans Miro, avec des remarques sur les ajustements manuels qui pourraient être nécessaires :

|  |  |  |
| --- | --- | --- |
| **Freehand** | **Miro** | **Des retouches sont nécessaires** |
| Tableaux | Kanban | Aucun |
| Cartes | Cartes | Les cartes Jira dans Freehand seront importées en tant que cartes Jira dans Miro. Cependant, ils ne seront pas connectés à l’instance existante car les utilisateurs devront réauthentifier leurs comptes Jira dans Miro.    Les cartes ADO, Trello et Asana ne sont pas prises en charge. |
| Collaborateurs et partage | Peut être recréé manuellement | Aucun |
| Commentaires | Peut être recréé manuellement | Aucun |
| Connecteurs / Lignes | Connecteurs / Lignes |  |
| Dessins / Diagrammes / Formes | Formes, textes et connecteurs | Aucun |
| Tableaux de données dynamiques | CSV | Le contenu peut être téléchargé et modifié sous forme de fichier .CSV à partir du tableau Miro. |
| Enchâssements :    Google et Microsoft Docs, YouTube, Spotify, Loom | Nom de la source (par exemple, Google, YouTube) et l’URL pour l’intégration | Si les utilisateurs souhaitent réintégrer un document, ils peuvent utiliser l’option [Charger via l’URL](../../using-miro/import-and-export/import/05-uploading-files-to-boards.md). |
| Réactions émojis | Peut être recréé manuellement |  |
| cadres | Cadres | Aucun |
| Grilles (tableaux) | Tableaux | Aucun |
| Objets groupés | Objets non groupés | Pour regrouper des objets, sélectionnez tous les objets concernés et appuyez sur **Cmd/Ctrl + G**, ou cliquez sur **Grouper les objets** dans le menu contextuel. |
| Images | Images | Aucun |
| Pages | Document intégré | Le contenu peut être téléchargé et modifié sous forme de fichier .docx à partir du tableau Miro. |
| Prototypes | Nom de la source (InVision) et l’URL pour l’intégration | Si les utilisateurs souhaitent réintégrer un document, ils peuvent utiliser l’option Charger via l’URL. |
| Widgets intelligents :    Carte double face, Sondage, Ceci ou Cela, Graphiques, Compteur, Classement, Roue, Buzzer, Personnes, Story points, Taille de T-Shirt, Minuteur, Boutons d’action | Création d’un PNG du widget intelligent au moment de l’importation | Le contenu n’est pas modifiable. |
| Pense-bêtes | Pense-bêtes | Il peut être nécessaire d’ajuster la taille des polices de texte dans les pense-bêtes. |
| Planning (Gantt) | CSV | Le contenu peut être téléchargé et modifié sous forme de fichier .CSV à partir du tableau Miro. |
| Wireframes | Wireframes | Il se peut que certains objets doivent être redessinés. |

## Principales restrictions

Prenez en compte les limitations et différences structurelles suivantes lors de la migration de votre contenu de Freehand vers Miro pour garantir une transition plus fluide :

- Les zones de texte Miro peuvent contenir jusqu’à 6 000 caractères, espaces compris. Tout texte supplémentaire sera recadré.
- Les pense-bêtes Miro ne prennent pas en charge les ajustements de la palette de couleurs ni le formatage du texte en liste à puces de la même manière que Freehand ; certains formats peuvent différer.
- Les widgets Smart Freehand sont importés sous forme d'images statiques (PNG) et ne sont pas modifiables dans Miro.
- Les commentaires, les réactions émoji et les prototypes de Freehand ne sont pas migrés vers Miro.
- Le jeton Freehand requis pour l'importation en masse n'est valable que pendant deux semaines à compter de la date à laquelle vous l'avez reçu.
- À partir du 31 décembre 2024, à 23h59 EST, Freehand et tous les jetons de migration associés seront supprimés et invalidés. Les utilisateurs ne pourront plus générer de nouveaux jetons ni accéder à Freehand.

### Comparez la structure organisationnelle entre Freehand et Miro

Pour planifier efficacement votre migration, il est important de comprendre comment les structures organisationnelles dans Freehand correspondent à celles de Miro :

**Calques d'organisation Freehand**

- Équipes Chaque sous-domaine auquel vous avez accès dans InVision est considéré comme une équipe. Si vous n’avez accès qu’à un seul sous-domaine, vous n’avez qu’une seule équipe.
- Groupes : Des dossiers de documents qui permettent de regrouper et de partager des documents au sein de votre équipe.
- Espaces : Un niveau d’organisation supplémentaire au sein des groupes pour vos documents.

:::note
Si votre équipe a utilisé la fonction d'aperçu de l'espace dans Freehand, vous devrez migrer manuellement ce contenu vers Miro. Nous vous recommandons de copier le contenu de la vue d’ensemble de l’espace sur un tableau Miro.
:::

**Les niveaux d’organisation de Miro**

- Organisations Vous n’avez généralement accès qu’à une seule organisation dans Miro.
- Équipes Espaces de travail partagés où les utilisateurs collaborent sur des tableaux et des projets (anciennement appelés Espaces dans certains contextes, soyez attentifs à l'évolution de la terminologie de Miro ; en général, les équipes sont le principal espace de travail collaboratif).
- Projets : Collections de tableaux au sein d’une équipe, facilitant l’organisation, la recherche et le partage des tableaux.

Considérez vos groupes InVision comme étant à peu près équivalents aux projets Miro (ou à ce qui aurait pu être conceptuellement similaire à des dossiers/espaces pour organiser les tableaux au sein d’une équipe). Pour chaque InVision Group que vous prévoyez de migrer, nous vous recommandons de créer un projet Miro portant le même nom. Par exemple, si vous aviez un groupe InVision nommé "Acme Corp Relaunch Project", nous vous suggérons de créer un projet Miro avec le même nom, "Acme Corp Relaunch Project", au sein de l'équipe Miro appropriée.

:::tip
Pour toute autre question concernant la migration de Freehand, veuillez contacter le [service d’assistance de Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) ou adressez-vous directement à votre Responsable Customer Success Miro.
:::
