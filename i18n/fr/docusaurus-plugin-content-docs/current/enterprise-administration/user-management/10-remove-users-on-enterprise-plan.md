---
title: Supprimer des utilisateurs du plan Enterprise
article_id: 360017730193
translation_id: 360017730193
locale: fr
sidebar_position: 10
created_at: '2019-02-11T10:09:21Z'
updated_at: '2025-11-04T11:30:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-management
---

La gestion avancée des utilisateurs dans Miro permet aux admins de filtrer et de gérer facilement tous les utilisateurs en un seul endroit. En tant qu’admin, vous pouvez supprimer des utilisateurs à tout moment.

> **Disponible pour** : Forfait Enterprise

### Supprimer un utilisateur d’une équipe

Pour supprimer un utilisateur d'une équipe particulière dans votre abonnement Enterprise, ouvrez les paramètres de l'équipe en survolant le nom de l'équipe sur le tableau de bord, puis en cliquant sur l'icône **Membres de l'équipe**.

L'onglet **Utilisateurs** s'ouvre. Recherchez le membre de l'équipe que vous souhaitez supprimer et sélectionnez **Supprimer de l'équipe** dans le menu à **trois points** (**.**..).

![delete-users-from-team.png](../../../../../../docs/enterprise-administration/user-management/images/23921781390482_delete-users-from-team.png)

Supprimer un utilisateur d’une équipe

Notez que la suppression d’un utilisateur d’une équipe ne le supprime pas complètement de l’organisation Enterprise et ne libère pas une licence. Pour supprimer un utilisateur de l’organisation (Company), suivez les étapes ci-dessous.

Vous pouvez également sélectionner plusieurs utilisateurs ou jusqu’à 50 utilisateurs d’équipe en une fois et les supprimer en bloc.

### Supprimer un utilisateur de l’entreprise

:::warning
Avant de supprimer des utilisateurs, vérifiez si vous avez activé le paramètre [Bloquer les utilisateurs désactivés](02-block-deactivated-users.md). Les utilisateurs supprimés sont traités différemment des utilisateurs désactivés.
:::

Pour supprimer complètement un utilisateur du plan Enterprise[,](01-deactivated-users.md) vous devez d’abord le **désactiver** dans la section **Active users** (Utilisateurs actifs) des paramètres Company (Entreprise). Ensuite, ouvrez l' onglet  **Utilisateurs désactivés** et choisissez **Supprimer** dans le menu à **trois points** (**.**..) dans la ligne de l'utilisateur.

Vous pouvez également sélectionner en lot jusqu’à 50 utilisateurs et les supprimer tous en même temps.

Si l’utilisateur est propriétaire de certains tableaux/[modèles](../../getting-started/start-here/your-first-board/04-templates.md)/[projets](../../using-miro/sharing-boards/16-projects.md) créés dans le plan Enterprise, vous pourrez choisir à qui le contenu sera réaffecté (vous pouvez sélectionner des utilisateurs admins et non admins). Si vous choisissez de l’option **Delete user and content** (Supprimer l’utilisateur et le contenu), le contenu de l’utilisateur sera supprimé. Les admins pourront [restaurer les tableaux supprimés](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md) dans les 90 jours après la suppression.

L’utilisateur supprimé perdra immédiatement l’accès aux ressources du plan (sans être notifié). Veuillez noter que l’utilisateur conservera l’accès aux tableaux qui ont été partagés [avec un lien public](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#partage-de-tableaux-via-un-lien-public) s’il a enregistré les liens vers ces tableaux spécifiques.

Si vous supprimez un utilisateur géré de votre abonnement Enterprise, il sera compté comme [non capturé](../canvas-25-admin-features/domain-control/01-domain-control.md) dans vos paramètres de contrôle de domaine.
