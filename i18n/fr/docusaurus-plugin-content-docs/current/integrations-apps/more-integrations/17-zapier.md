---
title: Zapier
article_id: 360025942994
translation_id: 360025942994
locale: fr
sidebar_position: 18
created_at: '2019-07-04T17:26:16Z'
updated_at: '2025-02-26T12:10:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Connectez vos applications préférées à Miro à l’aide de Zapier et élargissez la liste des possibilités d’automatisation de vos tâches quotidiennes. Déplacez automatiquement des informations entre vos applications et vos tableaux afin de vous concentrer sur les tâches essentielles.

> **Disponible sur :** les forfaits Free, Starter, Business et Enterprise

## Créer un Zap avec Miro

Vous devez avoir un compte Zapier pour connecter Miro à d’autres applications via Zapier.

Pour créer un Zap, cliquez sur le bouton correspondant sur le [tableau de bord dans Zapier](https://zapier.com/app/dashboard).

Create_Zap.jpg
Création d’un bouton Zap

Zapier crée un workflow automatisé entre les applications avec des **Triggers (Déclencheurs)** et des **Actions**.

:::warning
Pour l’instant, Miro ne peut fonctionner que comme **Action** dans Zapier.
:::

**Déclencheur**

Un Déclencheur est un événement dans une application qui déclenche le Zap. Une fois un Zap configuré, Zapier surveillera l’application pour détecter cet événement. Dans l’exemple suivant présentant l’enregistrement de nouveaux événements Google Agenda en tant que widgets carte Miro, le Zap est déclenché uniquement lorsqu’un nouvel événement est créé dans Google Agenda.

new_event_trigger.jpg
Configuration d’un événement Déclencheur dans Zap

**Action**

Une Action est un événement qui complète le Zap. Dans l’exemple précédent sur l’enregistrement de nouveaux événements Google Agenda en tant que widgets carte Miro, les nouvelles cartes Miro font office d’Action.

:::warning
Pour l’instant, Miro ne peut fonctionner que comme une Action dans Zapier.
:::

Trouvez Miro et choisissez l'une des trois actions qui s'y trouvent : Copier le tableau, Créer le tableau, Créer le widget carte.

creating_a_Zap_with_Miro_as_an_action.gif
Création de votre propre Zap avec Miro comme Action

### Action Copy board (Copier le tableau)

Il s’agit d’une action conçue pour créer une copie d’un tableau donné. Vous devrez sélectionner l’équipe où la copie du tableau sera créée.

install_Zapier.jpg
Sélection d’une équipe Miro

Dans l’étape suivante, choisissez les paramètres suivants :

- Original board (Tableau original) : choisissez un tableau de l’équipe pour en faire une copie. Vous pouvez rechercher le tableau par son nom ou son ID *(*par exemple *o9J_rxLXasqA)*.  Si vous ne trouvez pas le tableau dans la liste, essayez d’actualiser les données et vérifiez à nouveau.
- Title (Titre) : saisissez un nom pour le tableau copié. Si vous laissez ce champ vide, le tableau sera créé avec le nom **Untitled (Sans Titre)**.
- Description : saisissez un texte de description pour le tableau.
- Team access (Accès d’équipe) : vous pouvez choisir un accès **Private (Privé)**, **View (Consulter)**, **Comment (Commenter)** et **Edit (Modifier)** pour le tableau.
- Access via link (Accès via un lien) : créez des règles pour le partage de ce tableau avec un lien. Vous pouvez définir des groupes avec un accès **Private (Privé)**, **View (Consulter)** et **Comment (Commentaire)**.

set_up_action.jpg
/em> Configuration de l’événement d’action Copy board (Copier le tableau) /font>

### Action Create board (Créer un tableau)

Cette action créera un tableau avec un titre, une description et des paramètres d’accès spécifiques.

- Title (Titre) : saisissez un nom pour le nouveau tableau. Si vous laissez ce champ vide, le tableau sera créé avec le nom **Untitled (Sans Titre)**.
- Description : saisissez un texte de description pour le tableau.
- Team access (Accès de l’équipe) : vous pouvez choisir entre les types d’accès **Private (Privé)**, **View (Consulter)**, **Comment (Commenter)** et **Edit (Modifier)** pour votre équipe.
- Access via link (Accès via un lien) : créez des règles pour le partage de ce tableau avec un lien. Vous pouvez définir un accès **Private (Privé)**, **View (Consulter)** ou **Comment (Commenter)** via un lien public.

create_board_action.jpg
Configuration de l’événement d’action Create board (Créer un tableau)

### Action Create card widget (Créer un widget carte)

Cette action vous permet de transférer des informations (par exemple des messages Slack) sous forme de widget [carte](../../using-miro/essential-tools/02-cards.md) directement dans un [cadre](../../using-miro/essential-tools/07-frames.md) spécifique sur un tableau Miro avec des règles personnalisées.

- Board (Tableau) : choisissez un tableau de l’équipe que vous souhaitez utiliser. Vous pouvez rechercher le tableau par son nom ou son ID *(*par exemple *o9J_rxLXasqA)**.*  Si vous ne trouvez pas le tableau dans la liste, essayez d’actualiser les données et vérifiez à nouveau.
- Frame (Cadre) : sélectionnez un cadre du tableau que vous avez choisi. Vous pouvez rechercher le cadre par son nom. Si vous ne le trouvez pas, essayez d’actualiser les données et vérifiez à nouveau.
- Card title (Titre de la carte) : saisissez un titre pour votre carte.
- Cart title link (Lien du titre de la carte) : vous pouvez insérer un lien d’une application connectée (par exemple, vous pouvez créer une carte avec un lien vers une nouvelle tâche dans Asana).
- Card description (Description de la carte) : rédigez une description pour votre carte.
- Card due date (Date d’échéance de la carte) : définissez une date d’échéance pour la carte.
- Card border-color (Couleur de bordure de la carte) : choisissez une couleur personnalisée pour les contours de la carte (par exemple, si vous saisissez **#ff0000** dans ce champ, la couleur de la carte sera rouge).

create_card_action.jpg
Configuration de l’événement d’action Create card (Créer une carte)

## Désactiver l’intégration Zapier

Pour supprimer l’intégration Zapier de votre équipe Miro, ouvrez les [Paramètres de l’équipe](../../administration/get-started-as-a-miro-admin/06-manage-starter-and-education-plan.md) **> Applications et intégrations > Zapier** et cliquez sur **Désinstaller***.*

uninstall_Zapier.jpg
Options de désinstallation de Zapier

## Foire aux questions

1. *Dois-je disposer d'un compte Zapier d'entreprise pour l'utiliser avec Miro ?*
   - Non, ce n'est pas obligatoire. L’intégration Miro peut être établie avec n’importe quel forfait Zapier.
2. *Où sont stockées mes données Zapier ?*
   - Il s'agit d'une intégration officielle gérée par Miro et toutes les pratiques de stockage des données de Miro s'appliquent également ici.
3. *Dois-je être l'admin d'équipe dans Miro pour paramétrer l'intégration Zapier ?*
   - Cela dépend des paramètres de l'administrateur dans Miro et dans Zapier. Par défaut, même les membres qui ne sont pas admins d’équipe peuvent configurer l’intégration.
4. *Les cartes (Trello, Asana, etc.) se synchronisent-elles avec les cartes importées dans les tableaux Miro ?*
   - Non, Zapier n'offre actuellement pas de synchronisation. Par exemple, si vous déplacez votre carte Trello de « en cours » à « fait », cela n’est pas répercuté du côté de Miro.
5. *Je n’arrive pas à lier Gmail à Miro via Zapier.*  Pourquoi ?
   - Veuillez vérifier votre e-mail. Pour le moment, les utilisateurs ayant un compte Gmail finissant par *@gmail.com* ou *@googlemail.com* ne peuvent pas lier Gmail à Miro, car Zapier ne peut envoyer des informations Gmail qu’à un nombre limité d’applications.
