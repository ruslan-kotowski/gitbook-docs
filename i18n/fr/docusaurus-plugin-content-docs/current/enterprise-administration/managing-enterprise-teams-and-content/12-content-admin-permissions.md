---
title: Permissions d’administration du contenu
article_id: 360012777280
translation_id: 360012777280
locale: fr
sidebar_position: 13
created_at: '2020-03-26T12:31:39Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-admin-permissions
availability:
  notes: 'Disponible pour: le forfait Enterprise'
---

Les autorisations d’admin de contenu vous permettent de superviser tout le contenu de votre abonnement Enterprise. En tant qu’admin de contenu, vous pouvez gérer facilement l’accès aux tableaux, espaces, sections et modèles, et nettoyer le tableau de bord en supprimant les tableaux, espaces et sections inutilisés.

### Comment attribuer un rôle d’admin de contenu

1. Allez dans vos [paramètres](https://miro.com/app/settings/user-profile/).
2. Sous **Utilisateurs**, cliquez sur **Rôles d'admin**.
3. À côté du rôle de **Content Admin**, cliquez sur les trois points (**…**) et sélectionnez **Attribuer un rôle** dans le menu déroulant.
4. Sélectionnez l'utilisateur ou les utilisateurs auxquels vous souhaitez accorder des droits de Content Admin. Vous pouvez sélectionner jusqu'à 50 utilisateurs.
5. Cliquez sur le bouton **Attribuer** pour confirmer votre sélection.
6. Pour afficher tous les utilisateurs auxquels le rôle d'admin de contenu a été attribué, cliquez de nouveau sur les trois points (**…**), et sélectionnez **Afficher les utilisateurs**. Vous pouvez également cliquer n'importe où sur la **barre d'admin de contenu** pour voir la liste des utilisateurs.

Pour voir les autorisations attribuées aux admins de contenu, cliquez sur la **barre d'admin de contenu**, passez à l'onglet **Privilèges**, et faites défiler vers le bas pour voir toutes les autorisations **de contenu**.

## Gestion des tableaux et espaces

Pour des informations détaillées sur les autorisations que les admins de contenu ont sur les tableaux et espaces, consultez la [section sur la gestion du contenu dans la documentation des rôles d'admin](../../administration/get-started-as-a-miro-admin/02-understand-admin-roles-and-their-privileges.md).

De plus, les admins de contenu peuvent :

- ouvrir la boîte de dialogue Partager et gérer les paramètres de partage du tableau ([retirer et modifier l'accès des utilisateurs](../../using-miro/sharing-boards/01-board-access-rights.md), partager le tableau [avec une équipe](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)/un utilisateur/[une entreprise](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)/[publiquement](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#partage-de-tableaux-via-un-lien-public))
- modifier les détails du tableau (nom, description, couverture)
- déplacer le tableau vers un [espace](../../using-miro/spaces/01-spaces.md)
- déplacer le tableau vers une section
- [supprimer le tableau](../../using-miro/managing-boards/07-how-to-delete-a-board.md)
- [télécharger la sauvegarde du tableau](../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)
- configurer les [paramètres de contenu du tableau](../../using-miro/sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)
- configurer [les autorisations avancées de partage de tableau](../../using-miro/sharing-boards/02-who-can-share-a-miro-board.md)
- voir quel utilisateur a créé le [mot de passe pour un tableau public](../../using-miro/sharing-boards/13-password-protection-for-public-boards.md), et définir, changer ou supprimer des mots de passe pour les tableaux partagés publiquement
- restaurer n'importe quel tableau depuis la [corbeille](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md).

Les admins de contenu et les admins de contenu d'équipe peuvent déplacer un tableau vers une autre équipe dont le propriétaire du tableau est membre. Si le propriétaire du tableau n'est pas membre de l'équipe cible, vous pouvez [transférer la propriété du tableau](../../using-miro/managing-boards/05-how-to-transfer-board-ownership.md) à un membre.

Si le tableau n’est pas visible sur le tableau de bord, cela signifie qu’il n’a pas été partagé avec vous, mais vous pouvez quand même le trouver : [effectuez une recherche](../../getting-started/start-here/miro-dashboard/03-how-to-search-in-miro.md) dans le tableau de bord avec le nom du tableau, le propriétaire du tableau ou l’emplacement (équipe). Les tableaux qui n’ont pas été partagés avec vous apparaîtront avec une icône de cadenas à côté de leur nom. Pour gérer un tableau, cliquez sur les trois points en haut à droite.

Lorsque vous essayez d'ouvrir un tableau à partir d'un lien direct ou d'un résultat de recherche, le message **Accès au tableau refusé** s'affichera. En bas, vous trouverez les options pour **afficher les détails du tableau** et **gérer les autorisations d'accès**.

:::note
Vous ne pouvez pas modifier les paramètres des **espaces privés** dont vous **n’êtes pas** membre, et ils n'apparaîtront pas non plus dans la liste des espaces. Si vous devez modifier les paramètres d'un espace privé, demandez l'accès au propriétaire de l'espace ou utilisez [les API publiques de Miro](https://developers.miro.com/reference/enterprise-update-project-settings). Vous pouvez modifier les paramètres des espaces que vous *voyez* sur le tableau de bord*.*
:::

## Gestion des modèles

Vous pouvez modifier les paramètres de partage de votre modèle ([personnels, d’équipe ou d’entreprise](../../getting-started/start-here/your-first-board/02-custom-templates.md)), modifier les détails du modèle (nom, description et image de couverture) ou supprimer complètement un modèle.

**Comment gérer les modèles personnalisés**

1. Allez sur votre tableau de bord et cliquez sur **Explorer les modèles** en haut à droite.
2. Allez dans **Modèles personnalisés** dans la navigation à gauche et cliquez sur vos **modèles [Nom de l’entreprise]** ou **Personnels**.
3. Survolez le modèle que vous souhaitez modifier et cliquez sur les trois points (...).
4. Pour supprimer le modèle, cliquez sur **Supprimer**.
5. Pour gérer les autres détails du modèle, cliquez sur **Modifier**.
6. Le tableau s’ouvre. Cliquez sur le nom du modèle dans le menu du tableau.
7. Ajoutez ou modifiez le **nom du modèle** et la **description**, **sélectionnez la zone d’aperçu** pour l’image de couverture, et changez les paramètres de partage en **Personnel**, **Équipe** ou **Entreprise**.
8. Cliquez sur **Enregistrer les modifications**.
