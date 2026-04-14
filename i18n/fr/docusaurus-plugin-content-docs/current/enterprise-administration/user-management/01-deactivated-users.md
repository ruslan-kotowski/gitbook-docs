---
title: "Utilisateurs d\xE9sactiv\xE9s"
article_id: 360025025894
translation_id: 360025025894
locale: fr
sidebar_position: 1
created_at: '2019-06-19T22:16:18Z'
updated_at: '2026-02-19T10:44:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-deactivation
---

La gestion avancée des utilisateurs dans Miro permet aux admins d’entreprise de désactiver les utilisateurs au lieu de les supprimer. Les utilisateurs désactivés restent dans le répertoire du forfait et peuvent être réactivés à tout moment.

> **Disponible pour** : [forfait Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Paramétré par :** admins d’entreprise

## Règles

- Les utilisateurs désactivés ne pourront pas accéder à votre compte Enterprise et à ses fonctionnalités.
- Si vous avez activé le paramètre de [blocage des utilisateurs désactivés](02-block-deactivated-users.md), la désactivation d’un utilisateur géré l’empêchera de se connecter à Miro.
- Les utilisateurs désactivés ne pourront plus utiliser l’option de SSO de votre entreprise pour se connecter et devront à nouveau utiliser les méthodes d’authentification standard.
- Les tableaux et les espaces partagés créés par des utilisateurs désactivés ne sont *pas* réassignés à quelqu'un d'autre et restent disponibles pour les collaborateurs (sauf si, lors de la désactivation, vous retirez également l'utilisateur de son équipe. Dans ce cas, les tableaux sont réassignés à un admin d’équipe. C'est généralement pertinent pour les opérations [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)).
- Toutes les [notifications](../../using-miro/managing-your-profile/02-miro-notifications.md) aux utilisateurs désactivés sont bloquées.
- Les autres utilisateurs ne peuvent pas partager des tableaux et des espaces avec les utilisateurs désactivés.
- Les utilisateurs désactivés ne peuvent pas être ajoutés aux équipes dans votre abonnement Enterprise. Les admins d’entreprise peuvent réactiver les utilisateurs désactivés en les invitant comme membres, [en savoir plus](05-manage-user-invitations-on-enterprise-plan.md).
- Les utilisateurs désactivés ne sont pas facturés. Leurs licences sont libérées et peuvent être assignées à un autre utilisateur actif.
- Les attributs suivants ne peuvent pas être mis à jour pour les utilisateurs désactivés :

|  |
| --- |
| `nomUtilisateur` |
| `typeUtilisateur` |
| `rôles.valeur` |

## Désactiver un utilisateur

Vous pouvez désactiver un utilisateur à tout moment. Lorsque vous désactivez un utilisateur, il passe d’un état **Actif** à un état **Désactivé** et cesse d’utiliser une licence. Ce changement est également reflété dans les listes des utilisateurs actifs et désactivés dans les paramètres **Utilisateurs**.

Pour désactiver un utilisateur :

1. Ouvrez les paramètres de votre **Entreprise**.
2. Sélectionnez **Tous les utilisateurs** dans le menu **Utilisateurs****.**
3. Cliquez sur l'icône **trois points** (**...**) à droite d'un utilisateur que vous souhaitez désactiver.
4. Cliquez sur **Désactiver**.
   ![deactivate-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921781594002_deactivate-users.png)
   *L'option de désactivation d'un utilisateur sur le forfait Enterprise*

   Vous pouvez également désactiver les utilisateurs en bloc. Sélectionnez plusieurs utilisateurs en cochant les cases à gauche ou appliquez des filtres et sélectionnez jusqu'à 50 utilisateurs filtrés à la fois, puis choisissez **Désactiver** sous **actions en bloc**.
5. Cochez la case **Réattribuer le contenu de l'utilisateur** si vous souhaitez transférer les tableaux, [modèles](../../getting-started/start-here/your-first-board/02-custom-templates.md) et [espaces](../../using-miro/spaces/01-spaces.md) de l'utilisateur. Un nouveau propriétaire doit être choisi pour chaque équipe dans laquelle le(s) utilisateur(s) sélectionné(s) avait du contenu. La réattribution du contenu des utilisateurs ne peut pas être annulée.
   ![deactivate-reassign-content.png](../../../../../../docs/enterprise-administration/user-management/images/23921804187154_deactivate-reassign-content.png)
   *L'option de réattribution du contenu de l'utilisateur lors de sa désactivation*
6. Sélectionnez **Désactiver.**

La désactivation des utilisateurs n’entraînera pas la suppression de leurs données dans Miro. Leurs autorisations seront sauvegardées et elles seront restaurées à leur réactivation.

:::note
Note : pour désactiver un admin d’entreprise, vous devez tout d’abord révoquer son rôle d’admin d’entreprise.
:::

:::note
Si la notification **L’équipe doit au moins compter un admin** s’affiche lorsque vous tentez de désactiver un utilisateur, cela signifie que cet utilisateur est l’*unique* admin d’une ou de plusieurs équipes Enterprise. Pour résoudre ce problème, [invitez-vous dans ces équipes](05-manage-user-invitations-on-enterprise-plan.md) et [attribuez-vous les droits d’admin d’équipe](../../administration/user-management/06-how-to-manage-admin-roles.md). Cliquez sur le nombre d’équipes de l’utilisateur respectif pour découvrir les équipes dont il fait partie.
:::

:::note
Si votre entreprise utilise une solution [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md), vous pouvez également désactiver des utilisateurs via votre fournisseur d’identité. Lorsqu’un utilisateur est désactivé par le SCIM, son contenu n’est pas réattribué : l’option de réattribution n’est prise en charge que dans l’interface utilisateur pour ce scénario.
:::

### Désactivation automatique des invités

Pour les invités (utilisateurs initialement invités sur vos tableaux par e-mail), vous pouvez activer la [désactivation automatique](03-invitation-settings-on-enterprise-plan.md).

## Réactiver un utilisateur

Pour réactiver un utilisateur :

1. Ouvrez vos paramètres de **Entreprise**.
2. Sélectionnez **Tous les utilisateurs** dans le menu Utilisateurs, puis l’onglet **Utilisateurs désactivés****.**
3. Cliquez sur l'icône **trois points** (...) à droite d'un utilisateur que vous souhaitez réactiver.
4. Sélectionnez **Réactiver**.
5. Ajoutez l'utilisateur aux équipes si nécessaire.
6. Confirmez **Réactiver**.

![reactivate-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921804191762_reactivate-users.png)
*Réactivation d’un utilisateur*

Lorsque vous réactivez des utilisateurs :

- Ces utilisateurs peuvent se connecter immédiatement.
- Ils auront accès aux tableaux partagés, aux tableaux d’équipe et aux tableaux qu’ils ont créés avant leur désactivation (sauf si les tableaux ont été réaffectés).

:::note
Note : les admins d’entreprise sont les seuls à pouvoir réactiver les utilisateurs désactivés.
:::

### Supprimer définitivement des utilisateurs

Pour supprimer définitivement des utilisateurs désactivés :

1. Ouvrez vos paramètres de **l'entreprise**.
2. Cliquez sur **Utilisateurs** > **Tous les utilisateurs** dans le menu.
3. Sélectionnez l'onglet **Utilisateurs désactivés**.
4. Cliquez sur l'icône **trois points** (**...**) à droite d'un utilisateur que vous souhaitez supprimer.
5. Sélectionnez **Supprimer**.
   ![delete-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921781612562_delete-users.png)
   *Suppression d'un utilisateur désactivé*
6. Choisissez soit de réassigner le contenu de l'utilisateur en sélectionnant le nouveau propriétaire et en cliquant sur **Supprimer l’utilisateur**, soit de supprimer l'utilisateur et son contenu en cliquant sur **Supprimer l'utilisateur et son contenu**.

Vous pouvez également supprimer des utilisateurs en utilisant les actions en masse :

1. Dans l'onglet Utilisateurs désactivés, cochez la case à côté des utilisateurs que vous souhaitez supprimer.
2. Cliquez sur le bouton **Supprimer de l'entreprise** en haut.

:::note
Remarque : après leur suppression, les utilisateurs peuvent être à nouveau invités à votre forfait en tant que membres ou sur un tableau en tant qu'invités par toute personne ayant la permission d’[ajouter de nouveaux utilisateurs](05-manage-user-invitations-on-enterprise-plan.md).
:::
