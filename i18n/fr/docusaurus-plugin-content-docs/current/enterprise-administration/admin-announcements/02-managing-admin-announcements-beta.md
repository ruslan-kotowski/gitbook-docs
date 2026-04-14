---
title: "G\xE9rer les annonces admin"
article_id: 31013703080722
translation_id: 31013787617426
locale: fr
sidebar_position: 6
created_at: '2025-11-12T21:54:14Z'
updated_at: '2026-03-19T07:59:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: in-app-notifications
---

Utilisez la page Annonces pour consulter toutes les annonces, suivre leur état et les gérer tout au long de leur cycle de vie.

## Consulter et comprendre les annonces

Accédez à **Console d’administration > Organisation > Annonces**. Le tableau des annonces offre un aperçu de toutes les annonces, y compris leur nom, état, dates, public et créateur.

## États des annonces

| Statut | Description |
| --- | --- |
| **Brouillon** | Enregistré mais pas encore publié. |
| **Planifié** | Publié et prévu pour apparaître à une date ultérieure. |
| **En ligne** | Actuellement visible par les utilisateurs. |
| **Terminé** | Ne plus actif après la date de fin. |
| **Annulé** | Arrêté avant la date de début. |

## Mettre à jour les annonces

### Modifier une annonce

1. Allez à **Annonces**.
2. Sélectionnez l'annonce.
3. Cliquez sur **Modifier**.
4. Mettez à jour les détails de l'annonce.
   Vous pouvez mettre à jour le message, le texte du lien, l'URL du lien, le public, le calendrier ou la priorité.
5. Cliquez sur **Publier**.
   Les modifications sont appliquées immédiatement, y compris pour les annonces en direct.

### Publier une annonce

1. Ouvrez l'annonce.
2. Examinez les détails.
3. Cliquez sur **Publier**.
   L'annonce devient **Planifiée** si la date de début est dans le futur, ou **En direct** si la date de début est actuelle ou passée.

## Réutiliser les annonces

### Dupliquer une annonce

1. Dans la liste des annonces, ouvrez le menu **Actions**.
2. Cliquez sur **Dupliquer**.
3. Mettez à jour les détails de l'annonce.
   Modifiez le nom, les dates, le public ou d'autres champs selon vos besoins.
4. Cliquez sur **Enregistrer un brouillon** ou **Publier**.
   **Enregistrer un brouillon** conserve l'annonce sans la publier.
   **Publier** met l'annonce en ligne ou la programme en fonction des dates sélectionnées.

## Contrôler le cycle de vie de l'annonce

### Annuler une annonce

1. Dans la liste des annonces, ouvrez le menu **Actions**.
2. Cliquez sur **Annuler**.

Vous pouvez annuler une annonce dans n'importe quel état. L'annonce n'est plus affichée aux utilisateurs.

### Supprimer une annonce

1. Dans la liste des annonces, ouvrez le menu **Actions**.
2. Cliquez sur **Supprimer**.

L'annonce est supprimée de façon permanente et ne peut être récupérée.

## Suivre les modifications

Chaque annonce comprend une section historique qui montre les événements du cycle de vie et de mise à jour.

L'historique inclut des actions telles que :

- Créé
- Publié ou mis en ligne
- Modifié
- Annulé

Ces actions sont également enregistrées dans les journaux d'audit.
