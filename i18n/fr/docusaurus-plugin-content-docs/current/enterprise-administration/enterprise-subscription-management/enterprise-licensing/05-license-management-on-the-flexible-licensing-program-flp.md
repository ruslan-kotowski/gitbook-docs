---
title: Gestion des licences dans le cadre du programme de licences flexible (FLP)
article_id: 360018622159
translation_id: 360018622159
locale: fr
sidebar_position: 5
created_at: '2020-12-29T10:44:01Z'
updated_at: '2026-02-23T18:22:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'Pertinent pour: : le forfait Enterprise'
---

Consultez la gestion des licences dans le cadre du programme de licences flexibles (FLP), notamment les options de gestion des licences disponibles pour les nouveaux utilisateurs et le processus de conversion des licences existantes.

:::tip
Si vous êtes novice en matière de licences FLP, nous vous recommandons de lire d’abord le [programme de licences flexibles](03-flexible-licensing-program-flp.md) et [les niveaux d’accès des utilisateurs dans le forfait Enterprise](../../user-management/11-user-access-levels-on-enterprise-plan.md) afin de comprendre comment nos modèles de licence, nos types de licences et nos rôles Miro fonctionnent ensemble.
:::

## Attribuer des licences à de nouveaux utilisateurs

Membres Invités Visiteurs

En fonction des paramètres de licence par défaut de votre entreprise, les nouveaux membres se voient attribuer soit une licence Free (gratuite), soit une licence gratuite restreinte. Pour définir une licence par défaut pour les nouveaux membres de votre abonnement, contactez votre personne-ressource chez Miro.

Les nouveaux membres se voient attribuer la licence par défaut :

- lorsqu’ils sont invités par des membres non admin
- automatiquement via le [provisionnement Just-in-Time](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), le [contrôle de domaine](../../canvas-25-admin-features/domain-control/01-domain-control.md) ou le [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)

Les admins d’entreprise ont également la possibilité de sélectionner une licence pour les membres invités.

- selectionnez **Free** si vous souhaitez que les utilisateurs aient la possibilité de modifier (ils seront changés de forfait à une licence Standard ou Complète (legacy) dès qu’ils modifient ou créent un tableau, sont invités à modifier un tableau, se voient accorder la copropriété du tableau ou sont ajoutés à un [projet](../../../using-miro/sharing-boards/16-projects.md) en tant qu'éditeur)
- sélectionnez **Free Restricted** pour inviter le membre sans droits de modification

Les invités envoyés à un tableau se voient toujours attribuer une licence **Free**. Découvrez comment [inviter des invités sur un forfait Enterprise](../../../using-miro/sharing-boards/07-collaboration-with-guests.md).

[Les visiteurs](../../../using-miro/sharing-boards/08-collaboration-with-visitors.md) des tableaux partagés publiquement sont gratuits et n'ont pas besoin de licences.

## Comment mettre à niveau ou rétrograder des licences

> **Qui peut le faire :** Admins d'entreprise

Les licences **Free** sont automatiquement mises à niveau vers une licence Standard ou une licence complète (legacy) dès que l'utilisateur crée ou modifie un tableau.

Free Restricted à Standard ou Complet (ancien)  Standard ou Complet (ancien) à Free Restricted Conversion groupée de licences

Les licences gratuites restreintes peuvent être changées manuellement par les admins d’entreprise vers un forfait Standard ou une licence complète (ancien modèle), ou dans le cadre du [workflow d'Enterprise](../enterprise-workflow-automation/01-enterprise-workflow-automation.md).

Pour mettre à niveau une licence gratuite restreinte vers une licence complète :

1. Ouvrez **Équipes** ou allez dans **Paramètres de l’organisation** > **Utilisateurs** > **Tous les utilisateurs** > **Utilisateurs actifs**.
2. Cliquez sur l'icône **trois points** (**...**) à côté d’un utilisateur de licence gratuite restreinte.
3. Sélectionnez **Changer pour membre Standard**.

Des licences complètes peuvent être rétrogradées vers des licences gratuites restreintes si les admins d’entreprise souhaitent limiter l’accès de certains utilisateurs et libérer des licences complètes supplémentaires.

Les membres complets ne peuvent pas être rétrogradés vers des licences gratuites, étant donné que celles-ci ne sont attribuées qu’aux nouveaux utilisateurs.

Pour rétrograder une licence complète vers une licence gratuite restreinte :

1. Ouvrez **Équipes** ou **Paramètres de l'organisation** > **Utilisateurs** > **Tous les utilisateurs** >**Utilisateurs actifs**.
2. Cliquez sur l’icône **trois points** (**...**) à côté d'un utilisateur complet.
3. Sélectionnez **Passer à la licence Free Restricted**.

Pour convertir plusieurs licences à la fois:

1. Ouvrez **Paramètres de l'organisation** > **Utilisateurs** > **Tous les utilisateurs** > **Utilisateurs actifs**.
2. Sélectionnez individuellement tous les utilisateurs dont vous souhaitez convertir les licences ou appliquez des filtres pour les sélectionner. Vous pouvez sélectionner jusqu'à 50 utilisateurs.
3. Cliquez sur **Actions groupées** et sélectionnez une nouvelle option de licence
