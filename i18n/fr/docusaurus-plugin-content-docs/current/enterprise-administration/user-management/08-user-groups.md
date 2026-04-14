---
title: Groupes d’utilisateurs
article_id: 30658859384594
translation_id: 30658859384594
locale: fr
sidebar_position: 8
created_at: '2025-10-30T13:00:25Z'
updated_at: '2026-01-20T13:17:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: groups
availability:
  notes: 'Qui peut le faire: (Configuration) Admins d''entreprise, Membres de l''équipe
    Quels forfaits: Enterprise Quelles plateformes: Navigateur, Bureau, Mobile'
---

En tant qu'admin d'entreprise, les Groupes d'Utilisateurs vous permettent de gérer l'accès au contenu pour des groupes d'utilisateurs, au lieu de partager avec chaque membre individuellement. Tous les membres de votre organisation peuvent voir et partager leur contenu avec les Groupes d'Utilisateurs que vous créez.

Cet article explique comment créer, gérer et partager du contenu avec les Groupes d'Utilisateurs. Pour des informations plus générales sur cette fonctionnalité, voir [Vue d'ensemble des Groupes d'Utilisateurs](07-user-groups-overview.md).

:::note
Pour en savoir plus sur la gestion des Groupes d'Utilisateurs via SCIM, contactez votre responsable Customer Success ou le service d’assistance de Miro.
:::

## Guide de l'admin d’entreprise

### Créer un groupe d’utilisateurs

1. En tant qu’admin d’entreprise, accédez à la console d’admin.
2. Rendez-vous sur **Utilisateurs** > **Groupes**.
3. En haut à droite, cliquez sur **+ Créer un groupe**.
   La fenêtre modale **Créer un nouveau groupe** s'ouvre.
4. Nommez votre groupe.
5. (Facultatif) Ajoutez une description pour votre nouveau groupe. Vous pouvez toujours ajouter ou modifier votre description ultérieurement.
6. Cliquez sur **Créer un groupe**.
   Votre nouveau groupe est ajouté à la vue **Groupes**.

### Ajouter des utilisateurs à un Groupe d'utilisateurs

1. Dans la console d’admin, allez à **Utilisateurs** > **Groupes**.
2. Pour le Groupe d'utilisateurs que vous souhaitez gérer, sélectionnez les trois points (**...**) à la fin de la ligne.
3. Cliquez sur **Ajouter des utilisateurs**.
   La **fenêtre modale Ajouter des utilisateurs** s'ouvre.
4. Pour repérer votre ou vos utilisateurs, recherchez par nom ou par adresse e-mail.
5. Cochez chaque utilisateur que vous souhaitez ajouter.
6. Cliquez sur **Ajouter les utilisateurs sélectionnés**.
   Chaque utilisateur sélectionné est ajouté à votre Groupe d'utilisateurs.

### Ajouter un Groupe d'utilisateurs aux équipes

1. Dans la console d’admin, allez sur **Utilisateurs** > **Groupes**.
2. Pour le groupe d'utilisateurs que vous souhaitez gérer, sélectionnez les trois points (**...**) à la fin de la ligne.
3. Cliquez sur **Ajouter aux équipes**.
   La fenêtre modale **Ajouter le groupe aux équipes** s’ouvre.
4. Pour localiser votre ou vos équipes, recherchez par nom.
5. Cochez chaque équipe que vous voulez que votre groupe d'utilisateurs rejoigne.
6. Cliquez sur **Ajouter**.
   Votre groupe d'utilisateurs a rejoint chaque équipe que vous avez sélectionnée.

   > ✏️ Les membres du groupe d'utilisateurs ont des droits de modification sur tout le contenu de chaque équipe sélectionnée.

### Modifier un groupe d’utilisateurs

1. Dans la console d’admin, allez à **Utilisateurs** > **Groupes**.
2. Pour le groupe d’utilisateurs que vous souhaitez gérer, sélectionnez les trois points (**...**) à la fin de la ligne.
3. Cliquez sur **Modifier le groupe**.
   La fenêtre modale **Modifier le groupe** s'ouvre.
4. (Facultatif) Renommez votre groupe.
5. (Facultatif) Ajoutez une description pour votre nouveau groupe.
6. Cliquez sur **Enregistrer**.

### Supprimer un groupe d’utilisateurs

:::warning
La suppression d’un groupe d’utilisateurs ne peut pas être annulée. En supprimant un groupe d’utilisateurs, certains utilisateurs peuvent être retirés de certaines équipes.
:::

1. Dans la console d’admin, allez à **Utilisateurs** > **Groupes**.
2. Pour le groupe d’utilisateurs que vous souhaitez gérer, sélectionnez les trois points (**...**) à la fin de la ligne.
3. Cliquez sur **Supprimer le groupe**.
   La fenêtre modale **Supprimer \{Nom du groupe d’utilisateurs\}** s’ouvre.
4. Cliquez sur **Supprimer**.
   Le groupe d’utilisateurs est supprimé définitivement.

## Guide utilisateur

### Partager un tableau avec un groupe d’utilisateurs

Les membres de l'équipe peuvent partager un tableau avec n'importe quel groupe d'utilisateurs de leur organisation. Le tableau est partagé avec tous les membres de ce groupe d'utilisateurs.

Suivez ces étapes :

1. Sur un tableau Miro, cliquez en haut à droite sur **Partager**.
   Une fenêtre modale s'ouvre.
2. Saisissez le nom de votre groupe d'utilisateurs cible.
3. Dans les options qui s'affichent automatiquement, sélectionnez le groupe d'utilisateurs.
4. (Facultatif) Mettez à jour les autorisations. Par défaut : **Peut modifier**.
5. (Facultatif) Ajoutez un message personnalisé.
6. Cliquez sur **Envoyer les invitations**.
   Chaque utilisateur du groupe d'utilisateurs reçoit une invitation par e-mail pour accéder à votre tableau.

### Partager un Espace avec un Groupe d'utilisateurs

Les membres de l'équipe peuvent partager un Espace avec n'importe quel Groupe d'utilisateurs au sein de leur organisation, et spécifier les autorisations. L'Espace est partagé avec tous les membres de ce Groupe d'utilisateurs.

Suivez ces étapes :

1. Depuis le tableau de bord Miro, pour l'Espace que vous souhaitez partager, cliquez sur les trois points verticaux pour ouvrir le menu **Options**.

   > 💡 Alternativement, dans la barre latérale des Espaces, en haut, cliquez sur les trois points verticaux pour ouvrir le menu **Options**.
2. Cliquez sur **Partager**.
   La fenêtre modale **Partager Espace '\{Space Name\}'** s'ouvre.
3. Saisissez le nom du Groupe d'utilisateurs.
4. (Facultatif) Mettez à jour les autorisations. Par défaut : **Peut modifier**.
5. (Facultatif) Ajoutez un message personnalisé.
6. Cliquez sur **Envoyer les invitations**.
   Chaque membre du groupe d'utilisateurs reçoit une invitation par e-mail pour accéder à votre espace.

:::note
Les membres ajoutés au groupe d'utilisateurs ont automatiquement accès aux espaces partagés. Pour les membres supprimés du groupe d'utilisateurs, leur accès est automatiquement révoqué.
:::
