---
title: Miro pour Google Calendar
article_id: 360017150100
translation_id: 360017150100
locale: fr
sidebar_position: 9
created_at: '2020-10-23T12:49:04Z'
updated_at: '2025-02-26T11:39:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-calendar-addon
---

Organisez vos réunions et vos ateliers dans Miro plus rapidement, plus facilement et de manière plus fluide avec le module complémentaire de Miro pour Google Calendar ! Vous pouvez désormais facilement attacher des tableaux Miro à vos événements Google et partager les tableaux avec les personnes participant à votre réunion en quelques clics seulement.

Vous pouvez utiliser, soit le module complémentaire Google Workspace, soit l’extension Chrome pour joindre des tableaux Miro à vos événements Calendar. Pour profiter de la meilleure expérience possible, nous vous recommandons d’utiliser le **module complémentaire Miro for Google Calendar**, car il s’intègre à l’expérience Google Workspace et permet une collaboration plus fluide avec Miro et Google Workspace, le tout au même endroit.

:::note
Seules les personnes organisant la réunion doivent installer le module complémentaire ou l’extension.
:::

## Le module complémentaire de Miro pour Google Calendar

> **Disponible pour** : Plans Free, Starter, Education (options de partage limitées) ; Plans Business, Enterprise (fonctionnalité complète)

### Configurer l’intégration

Suivez [ce lien](https://workspace.google.com/marketplace/app/miro/1062019541050) pour installer l’application dans votre Google Calendar.

:::note
L’admin de votre Google Workspace peut avoir besoin d’installer l’application pour votre organisation ou votre équipe. Veuillez vérifier la disponibilité de l’application auprès de votre admin. [En savoir plus](https://www.google.com/url?q=https://support.google.com/a/topic/1056395?hl%3Den%26ref_topic%3D27380&sa=D&source=docs&ust=1648103128093296&usg=AOvVaw0gTVCloXueNePrGm3wLxLL).
:::

Ouvrez votre Google Calendar et cliquez sur l’icône de Miro à droite.

Miro_in_Google_Calendar.jpg
Miro dans Google Calendar

Cliquez sur **Authorize access** (Autoriser l’accès). Vous devez octroyer à Miro un droit d’accès à votre compte Google pour commencer à utiliser l’intégration.

authorize_access.jpg
Autorisation à Miro d’accéder à votre compte Google

Les admins Google Workspace peuvent [pré-installer certains modules complémentaires](https://support.google.com/a/answer/172482?hl=en) pour les utilisateurs de leur domaine et [autoriser/bloquer certains modules complémentaires](https://support.google.com/a/answer/6089179?hl=en) au sein de leur domaine. Si l’admin n’a pas bloqué le module complémentaire de Miro, tous les utilisateurs devraient pouvoir l’installer/le désinstaller par défaut. Si l’admin pré-installe le module complémentaire pour l’ensemble du domaine, personne n’a besoin de l’installer, car il sera pré-installé.

### Joindre des tableaux Miro aux événements Google Calendar

Une fois que le module complémentaire est configuré pour votre Google Calendar, vous pouvez ajouter des tableaux Miro sous forme de pièces jointes aux réunions Google. Lorsque vous créez un nouvel événement ou que vous modifiez un événement existant, cliquez sur **Attachments** (Pièces jointes) et choisissez **Miro** dans le menu déroulant, cliquez sur **Choose or create a board** (Choisir ou créer un tableau) dans la fenêtre contextuelle suivante.

attach_a_Miro_board.gif
Ajout de tableaux Miro en tant que pièces jointes aux événements Google

Dans le sélecteur de Miro, choisissez un tableau ou créez-en un nouveau. Vous pouvez sélectionner n’importe lequel des tableaux auxquels vous avez accès sur votre tableau de bord Miro. Pour créer un nouveau tableau, cliquez sur le bouton plus bleu.

picking_a_board.gif
Choix d’un tableau dans le sélecteur

Après avoir sélectionné/créé le tableau, vous pouvez le partager avec les personnes participant à votre réunion si vous avez les autorisations appropriées du côté de Miro et si votre plan le permet. Définissez les droits d’accès des personnes participant à votre réunion en choisissant une option sous la ligne **Anyone the organizer invites to the event** (Toute personne invitée à l’événement par l’organisateur). Vous pouvez autoriser les personnes participant à votre réunion à lire/commenter/modifier le tableau. Si vous ne disposez [pas des autorisations nécessaires pour partager un tableau](../../using-miro/sharing-boards/02-who-can-share-a-miro-board.md), un message contextuel vous l’indiquera.

sharing_a_board_from_Calendar.jpg
Partage du tableau avec les personnes participant aux réunions

Si vous partagez un tableau depuis un plan Free, le tableau ne sera **pas** partagé si, parmi les personnes invitées, certaines ne font **pas** partie de l’équipe dans laquelle se trouve le tableau.

En ce qui concerne les plans Starter et Education, le tableau ne sera **pas** partagé si vous le partagez avec des **droits de modification** alors que, parmi les personnes invitées, certaines ne font **pas** partie de l’équipe à laquelle appartient le tableau.

Sur les plans Business et Enterprise, le tableau ne sera pas partagé si certains des invités à la réunion **ne font pas** partie de l'équipe à laquelle appartient le tableau et si les invités **ne** sont **pas** autorisés dans les [paramètres d'invitation de l'équipe.](../../administration/user-management/02-invitation-settings.md) Si le rôle d’invité est autorisé, les personnes invitées ne faisant pas partie de l’équipe seront invitées dans le tableau en tant qu’[invités](../../using-miro/sharing-boards/07-collaboration-with-guests.md).

### Ajouter plusieurs tableaux et supprimer les tableaux joints

Pour ajouter plusieurs tableaux à une réunion, ajoutez une pièce jointe supplémentaire à la réunion, choisissez Miro dans le menu déroulant et sélectionnez/créez un tableau comme expliqué ci-dessus.

Pour supprimer un tableau de l’événement, cliquez simplement sur l’icône en forme de croix et supprimez la pièce jointe. Veuillez noter que les personnes participant à la réunion qui ont été invitées dans le tableau lorsque vous l’avez ajouté en pièce jointe et partagé ne seront pas supprimées du tableau automatiquement.

removing_a_board.jpg
Suppression d’un tableau des pièces jointes

### Foire aux questions

1. *Dois-je être propriétaire d'une réunion pour joindre le tableau Miro à l'événement Google Calendar ?*- Cela dépend des paramètres sélectionnés par le créateur de la réunion. Toute personne pouvant modifier l’événement peut joindre un tableau Miro. Vous trouverez davantage d’informations à ce sujet dans le Centre d’assistance de Google.

## Miro pour Google Calendar (extension Chrome)

:::warning
L’extension Miro pour Google Chrome sera dépréciée le 30 juin 2023 afin de rationaliser l’expérience des utilisateurs de Google Agenda. Comme alternative, nous vous recommandons d’utiliser notre [module complémentaire pour Google Workspace](https://workspace.google.com/marketplace/app/miro/1062019541050). Si vous avez des questions, veuillez contacter notre [équipe d’assistance](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) ou poser une question à la [communauté Miro](https://community.miro.com/).
:::

Vous pouvez trouver l’extension de Miro pour Google Calendar dans le [Chrome Web Store](https://chrome.google.com/webstore/category/extensions) ou tout simplement en suivant [ce lien](https://chrome.google.com/webstore/detail/miro-for-google-calendar/ihojbjcmeipmljclncfnfibdbkbmepck). Cliquez sur **Add to Chrome** (Ajouter dans Chrome) pour installer l’extension.

Une fois l'extension ajoutée, vous verrez deux boutons dans le mode d'édition de vos événements Google : **Créer un nouveau tableau**, **Choisir un tableau existant**. Pour commencer à utiliser l’extension, configurez-la en connectant votre compte Google et Miro. Appuyez sur l’un des boutons et cliquez sur **Connecter** à côté de Google Agenda.

connect_Google_calendar_to_Miro.gif
Connexion de Google Calendar et de Miro

Autorisez Miro à accéder à votre compte Google en cliquant sur **Continue** (Continuer). Dans l’étape suivante, vous devez connecter l’extension à Miro. Cliquez sur **Conne****ct** (Connecter) et connectez-vous sur Miro.

connect_to_extension.jpg
L’option permettant de connecter Miro à l’extension

Ensuite, choisissez une équipe et cliquez sur **Authorize** (Autoriser). Le tableau de bord de l’équipe choisie apparaîtra sur votre sélecteur lorsque vous ajoutez des tableaux existants en pièces jointes à vos événements Google. Si vous souhaitez connecter *plusieurs équipes*, cliquez sur l’icône plus dans la fenêtre de configuration.

connect_one_more_team.jpg
Option permettant de connecter une équipe Miro supplémentaire

Pour déconnecter une équipe, cliquez sur l’icône fléchée à côté de celle-ci.

disconnect_a_team.jpg
/em>Déconnexion d’une équipe Miro de l’extension Chrome Google Calendar

### Joindre un tableau Miro via l’extension Chrome

Si vous prévoyez d’inviter les personnes participant à votre réunion dans un nouveau tableau Miro, cliquez sur le bouton **Create new board** (Créer un nouveau tableau) à côté de l’icône Miro lorsque vous configurez un événement dans Google Calendar. Si vous avez connecté plusieurs équipes, vous devrez choisir l’équipe dans laquelle le tableau sera créé. Le tableau aura le titre de la réunion. Si la réunion n’a pas encore été nommée, le nom du tableau sera **Untitled** (Sans titre). Toutes les personnes participant à la réunion et qui sont membres de l’équipe Miro dans laquelle le tableau a été créé seront automatiquement invitées dans le tableau en tant qu’éditeurs.

Vous trouverez le lien du tableau dans la description de l’événement.

attach_a_board_to_Google_Calendar_event.gif
Ajout d’un nouveau tableau Miro en tant que pièce jointe à un événement Google

:::warning
Vous ne pouvez pas modifier le nom du tableau dans la description de l’événement : si vous modifiez le lien, cela n’entraînera que la modification du texte du lien. Le nom du tableau ne peut être modifié que du côté de Miro.
:::

:::warning
Veuillez noter que l’ajout de tableaux Miro en tant que pièces jointes aux réunions Google Calendar ou la création de nouveaux tableaux ne fonctionnent **pas** pour les événements passés.
:::

Pour ajouter un tableau Miro existant à un événement, cliquez sur **Choose existing board** (Choisir un tableau existant) et sélectionnez un tableau dans le sélecteur :

attach_an_existing_board_to_Google_Calendar_event.gif
Ajout d’un tableau Miro en tant que pièce jointe à un événement Google Calendar

:::note
Vous pouvez joindre plusieurs tableaux à une réunion en cliquant sur le bouton.
:::

L’extension vous permet d’inviter toutes les personnes participant à la réunion avec des droits de lecture/de commentaire/de modification ou de laisser les paramètres du tableau tels quels. Une fois que vous avez cliqué sur **Save** (Enregistrer), toutes les personnes participantes seront automatiquement invitées dans le tableau et recevront des invitations par e-mail (si leurs [paramètres de notification](../../using-miro/managing-your-profile/02-miro-notifications.md) le permettent). Veuillez noter que si une personne invitée n’est pas membre de votre équipe, cette dernière ne sera pas ajoutée au tableau. Assurez-vous que toutes les personnes participant à la réunion détiennent déjà chacune une licence dans votre équipe.

Si vous ne souhaitez pas modifier les paramètres de partage existants du tableau, choisissez l’option **As in sharing settings** (Conforme aux paramètres de partage).

sharing_settings.jpg
/em>Choix des paramètres d’accès au tableau pour les personnes participant à la réunion

:::note
Veuillez noter que l’accès des utilisateurs ayant déjà été invités dans le tableau *ne sera pas dégradé.*
:::

Les utilisateurs qui seront ajoutés à la réunion plus tard recevront également des invitations au tableau joint (s’ils font partie de l’équipe). *Toutes les personnes invitées à la réunion ont accès au tableau si les paramètres d’accès au tableau dans Google Calendar le permettent.*

Les utilisateurs supprimés de la réunion ne seront pas supprimés du tableau joint. Veuillez [modifier leur niveau d’accès du côté de Miro](../../using-miro/sharing-boards/01-board-access-rights.md).
