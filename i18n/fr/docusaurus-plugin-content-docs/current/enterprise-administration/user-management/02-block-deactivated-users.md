---
title: "Bloquer les utilisateurs d\xE9sactiv\xE9s"
article_id: 11846063620882
translation_id: 11846063620882
locale: fr
sidebar_position: 2
created_at: '2023-06-06T12:47:53Z'
updated_at: '2025-11-04T11:30:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-deactivation
---

Lorsqu’un admin d’entreprise [désactive un utilisateur](01-deactivated-users.md), celui-ci perd l’accès à l’abonnement Enterprise et ne peut plus se connecter avec l’authentification unique (SSO). Les utilisateurs désactivés peuvent continuer d’utiliser d’autres abonnements Miro avec la même adresse e-mail.

Vous pouvez bloquer les [utilisateurs gérés](06-managed-users-on-enterprise-plan.md) désactivés pour les empêcher d’accéder à tout autre abonnement Miro.

> **Disponible pour :** le forfait Enterprise
> **Qui peut le faire :** les admins d’entreprise

## Bloquer les utilisateurs désactivés

**Lorsque le paramètre est activé :** les utilisateurs gérés désactivés verront leur accès aux abonnements Miro bloqué. Ce paramètre s’applique à tous les utilisateurs qui sont actuellement désactivés dans votre abonnement et à tous les utilisateurs que vous pourrez désactiver à l’avenir.

**Lorsque le paramètre est désactivé :** les utilisateurs gérés désactivés peuvent accéder aux autres abonnements Miro avec leur adresse e-mail d’entreprise et leur mot de passe.

> L’activation du paramètre **Bloquer les utilisateurs désactivés** aura un impact sur tous les utilisateurs précédemment désactivés de votre abonnement. Avant d’activer le paramètre ou de vérifier les nouveaux domaines alors que le paramètre est activé, nous vous recommandons d’abord de passer en revue votre liste d’utilisateurs désactivés pour comprendre qui sera bloqué.

### Comment bloquer les utilisateurs désactivés

1. Allez dans **Paramètres** > **Sécurité** > **Domaines gérés**
2. Activez l’option **Bloquer les utilisateurs désactivés**.
   *![Bloquer les utilisateurs désactivés dans la console d'administration Enterprise](../../../../../../docs/enterprise-administration/user-management/images/23921780232082_image.png)*
   *Bloquer les utilisateurs désactivés dans la console d'administration Enterprise.*

## Que voient les utilisateurs bloqués ?

Les utilisateurs gérés désactivés et bloqués seront immédiatement déconnectés. Lorsqu’ils essaieront de se connecter la fois suivante, ils verront l’un des messages suivants :

![Compte](../../../../../../docs/enterprise-administration/user-management/images/21017430794898_Account%20deactivated.png)*L'utilisateur a tenté de se connecter avec son e-mail et son mot de passe.*

![E-mail](../../../../../../docs/enterprise-administration/user-management/images/21017417753746_Email%20not%20associated%20with%20an%20SSO%20account.png)*L'utilisateur a tenté de se connecter avec SSO*

## Débloquer les utilisateurs désactivés

Les admins d’entreprise peuvent débloquer des utilisateurs de trois façons :

**Réactiver ou réinviter l’utilisateur**

Réactivez ou réinvitez l’utilisateur dans votre abonnement Enterprise où le domaine est vérifié. Cet utilisateur aura accès à tous les abonnements dont il fait partie. Si cet utilisateur n’utilise pas activement votre abonnement Enterprise, vous pouvez lui attribuer une licence [gratuite restreinte](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md). Pour en savoir plus sur l’invitation de membres, consultez Gérer les invitations sur le forfait Enterprise.

**Désactiver le paramètre Bloquer les utilisateurs désactivés**

Ceci débloquera tous les utilisateurs gérés désactivés. Ils pourront ainsi se connecter dans Miro avec leur adresse e-mail d’entreprise. Cela ne leur donnera pas accès à votre abonnement Enterprise. Cette option ne fonctionne que si l’utilisateur n’a pas été supprimé de l’abonnement. Rendez-vous dans les paramètres des **Domaines gérés** et désactivez l’option **Bloquer les utilisateurs désactivés.**

**Supprimer le domaine**

Vous pouvez supprimer le domaine de votre liste de domaines vérifiés. Cela débloquera tous les utilisateurs gérés de ce domaine, sauf s’ils ont été supprimés de l’abonnement. Pour supprimer un domaine, dans les paramètres de votre entreprise, rendez-vous dans **Sécurité et conformité** > **Collaboration** > cliquez sur **Supprimer** à côté du nom de domaine.

> **✏️** Bloquer l’accès à Miro d’un utilisateur signifie qu’il ne peut pas se connecter aux autres abonnements Miro avec son adresse e-mail d’entreprise et son mot de passe ou via l’authentification unique. Le déblocage ne donne pas à l’utilisateur accès à l’abonnement Enterprise, sauf si cet accès lui est explicitement accordé.

## Scénarios d’utilisateurs bloqués

Utilisez ce tableau pour mieux comprendre ce qui se passe dans différents scénarios avec des utilisateurs bloqués.

|  |  |
| --- | --- |
| Action | Résultat |
| **L’utilisateur est bloqué.** | |
| L’admin d’entreprise désactive l’utilisateur géré. | L’utilisateur est bloqué. |
| **Un membre de votre abonnement Enterprise tente d’inviter un utilisateur géré** désactivé dans son équipe. | L’utilisateur reste bloqué.  La personne à l’origine de l’invitation verra un message indiquant que l’utilisateur est désactivé. L’utilisateur ne peut pas être invité. Les admins peuvent réactiver les utilisateurs. |
| L’admin d’entreprise désactive et supprime un utilisateur géré. | L’utilisateur est bloqué. |
| L’utilisateur géré est désactivé dans le fournisseur d’identité. | L’utilisateur est bloqué. |
| L’utilisateur géré est supprimé de l’application/groupe Miro dans le fournisseur d’identité. | L’utilisateur est bloqué. |
| L’admin d’entreprise ajoute et vérifie un domaine alors que le paramètre est activé. | Tous les utilisateurs des domaines nouvellement vérifiés dans la liste de désactivation sont bloqués. |
| Quelqu’un d’un autre abonnement (tout abonnement autre que celui où le domaine est vérifié) tente d’inviter votre utilisateur géré désactivé dans son abonnement.   Cela s’applique également même si l’utilisateur géré est supprimé de votre abonnement. | L’utilisateur reste bloqué.  Il peut être invité dans d’autres abonnements et recevra des notifications d’invitation, mais ne peut pas se connecter à Miro. |
| **L’utilisateur est débloqué**. | |
| L’admin d’entreprise réactive un utilisateur géré désactivé. | L’utilisateur est débloqué. |
| L’admin d’entreprise invite à nouveau un utilisateur géré désactivé ou supprimé dans l’abonnement. | L’utilisateur est invité et débloqué. |
| L’utilisateur géré est réactivé via le SCIM. | L’utilisateur est débloqué. |
| L’utilisateur géré est à nouveau ajouté à l’application/au groupe Miro dans le fournisseur d’identité et synchronisé via le SCIM. | L’utilisateur est débloqué. |
| **Un membre de votre abonnement Enterprise invite un utilisateur géré** supprimé dans son équipe. | Si les [paramètres d’invitation](03-invitation-settings-on-enterprise-plan.md) permettent aux membres d’inviter de nouveaux utilisateurs dans leurs équipes, l’utilisateur est invité et débloqué. |
| **Scénarios mixtes** | |
| Le domaine vérifié est supprimé du contrôle de domaine. | Les utilisateurs désactivés à partir du domaine supprimé sont débloqués.  Les utilisateurs supprimés restent bloqués et doivent être réinvités dans l’abonnement pour être débloqués. |
| Le paramètre est désactivé après avoir été activé. | Tous les utilisateurs désactivés gérés sont débloqués.  Les utilisateurs supprimés restent bloqués et doivent être réinvités dans l’abonnement pour être débloqués. |

## Foire aux questions

**Quelles informations peuvent voir les autres abonnements à propos des utilisateurs désactivés bloqués ?**

Désactiver l’utilisateur dans votre abonnement ne le désactivera que dans votre abonnement Enterprise. Le blocage n’aura d’impact que sur la possibilité de se connecter à Miro à l’aide de l’adresse e-mail d’entreprise. L’utilisateur semble actif dans d’autres abonnements, mais ne peut pas se connecter avec son adresse e-mail d’entreprise.

**Si un utilisateur est désactivé et supprimé, verra-t-il son accès à Miro bloqué une fois le paramètre activé ?**

Les utilisateurs resteront bloqués une fois que vous les aurez [supprimés de votre abonnement](01-deactivated-users.md). La suppression de l’utilisateur aura certaines conséquences. Pour plus d’informations, consultez nos scénarios d’utilisateurs bloqués et désactivés. La seule façon de débloquer un utilisateur supprimé est de le réinviter dans l’abonnement avec le domaine vérifié. Si l’utilisateur est supprimé de l’abonnement avant l’activation du paramètre, celui-ci ne s’applique pas à lui.

**Ce paramètre a-t-il un impact sur les utilisateurs non gérés ?**

Non. Seuls les utilisateurs gérés sont impactés par ce paramètre.
