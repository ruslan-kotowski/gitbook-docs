---
title: Licence gratuite restreinte
article_id: 360011746739
translation_id: 360011746739
locale: fr
sidebar_position: 4
created_at: '2020-02-05T07:29:16Z'
updated_at: '2026-02-19T10:40:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Lorsque de nouveaux utilisateurs rejoignent un abonnement Miro, ils peuvent se voir attribuer une licence gratuite restreinte selon le [modèle de licence Enterprise](02-enterprise-licensing.md).

> **Pertinent pour :** forfait Enterprise

## Quand les utilisateurs se voient-ils attribuer une licence gratuite restreinte ?

**Sur le programme de licences flexibles (FLP)**, un utilisateur peut se voir attribuer une licence gratuite restreinte dans les conditions suivantes :

- La licence par défaut des nouveaux utilisateurs est définie sur Licence gratuite restreinte
- Un admin d’entreprise invite l'utilisateur et lui attribue une licence gratuite restreinte dans la fenêtre d'invitation
- Un admin d’entreprise convertit la licence de l’utilisateur en licence gratuite restreinte dans **Paramètres de l’entreprise > Utilisateurs actifs**

:::note
En savoir plus sur le [programme de licences flexibles (FLP)](03-flexible-licensing-program-flp.md) et sur la [gestion des licences sur le FLP](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

**Sur une licence non flexible (non-FLP)**, un utilisateur peut se voir attribuer une licence gratuite restreinte dans les conditions suivantes :

- L'utilisateur est automatiquement capturé (par le [contrôle de domaine](../../canvas-25-admin-features/domain-control/01-domain-control.md) ou le [provisionnement à la demande](../../user-management/13-user-provisioning-on-enterprise-plan.md)) dans une organisation qui n'a pas suffisamment de licences Avancées, Standard ou Complètes (Legacy) lors de son inscription sur Miro.
- L'utilisateur est invité dans une équipe de l'organisation qui ne dispose pas de suffisamment de licences Avancées, Standard ou Complètes (Legacy).

Lorsque plusieurs utilisateurs sont invités en même temps, les licences leur sont attribuées dans l’ordre dans lequel apparaissent les adresses e-mail dans la liste des invités. Si l’organisation ne dispose pas d’un nombre suffisant de licences, les utilisateurs figurant en fin de liste recevront une licence gratuite restreinte. Dans ce cas, la personne chargée d’envoyer les invitations recevra une notification contextuelle lui indiquant que certains utilisateurs auront un accès limité au compte.

## Comment les licences gratuites restreintes fonctionnent pour les utilisateurs

Les utilisateurs disposant d’une licence gratuite restreinte peuvent consulter et commenter les tableaux des équipes dans lesquels ils participent et demander l’accès aux droits de modification ainsi qu'une licence standard ou une licence complète (anciennement). Ils peuvent également découvrir et rejoindre d’autres équipes de l’entreprise comme les autres membres.

:::note
Les admins d’entreprise peuvent [configurer les paramètres de gestion des demandes](../../user-management/09-request-management-on-enterprise-plan.md).
:::

### Accès restreint gratuit aux tableaux

Les autorisations d’accès suivantes pour consulter, commenter ou modifier s’appliquent aux utilisateurs disposant d’une licence gratuite restreinte :

|  |  |
| --- | --- |
| **Comment le tableau a-t-il été partagé** | **Niveau d’accès** |
| Lien public | Les utilisateurs sous licence gratuite restreinte peuvent consulter et/ou modifier en fonction du niveau d’accès qui leur est accordé. |
| Lien d’équipe ou d’entreprise | Les utilisateurs sous licence gratuite restreinte peuvent consulter et/ou commenter en fonction du niveau d’accès qui leur est accordé. |
| [Lien intégré](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md) | Les utilisateurs sous licence gratuite restreinte peuvent consulter et/ou commenter en fonction du niveau d’accès qui leur est accordé.  Les utilisateurs sous licence gratuite restreinte ne pourront pas modifier ou demander l’accès à la modification, même si l’accès à la modification est accordé par le biais des autorisations intégrées. |

## Comment gérer les licences gratuites restreintes

> **Qui peut le faire :** les admins d’entreprise

L’admin d’entreprise peut, quel que soit l’abonnement, convertir une licence gratuite restreinte en une licence standard ou complète (ancienne version) dans la section **Utilisateurs actifs** des paramètres de son équipe ou de son entreprise.

**Programme de licences flexibles (FLP)**

Sur les abonnements FLP, l’admin d’entreprise peut également à tout moment rétrograder une licence avancée, standard ou complète (ancienne version) en licence gratuite restreinte.

Lorsqu’un utilisateur disposant d’une licence gratuite restreinte demande des droits de modification, les admins d’entreprise reçoivent la demande en fonction de leurs [paramètres de gestion des demandes](../../user-management/09-request-management-on-enterprise-plan.md).

:::note
En savoir plus sur [la gestion des licences dans le cadre du programme de licences flexible](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

## Foire aux questions

**Qu'advient-il de mes licences gratuites restreintes lorsque j’ajoute des licences standard ou complètes (ancien modèle) à mon forfait non FLP ?**

Les utilisateurs auxquels vous avez attribué une licence gratuite restreinte ne sont pas automatiquement transférés sur de nouvelles licences standard ou complètes (ancien modèle). Les admins d’entreprise peuvent mettre à niveau les licences manuellement.
