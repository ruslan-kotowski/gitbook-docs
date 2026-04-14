---
title: "Param\xE8tres d\u2019invitation du forfait Enterprise"
article_id: 4412315533842
translation_id: 4412315533842
locale: fr
sidebar_position: 3
created_at: '2021-12-13T04:56:26Z'
updated_at: '2026-02-19T10:56:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
---

Configurez les paramètres d’invitation de votre forfait Enterprise pour gérer qui est autorisé à inviter de nouveaux utilisateurs à rejoindre votre forfait. Vous pouvez personnaliser vos paramètres d’invitation pour répondre aux exigences de vos équipes et de toute l’entreprise.

> **Disponible pour** : le forfait Enterprise
> **Qui peut le faire :** les admins d’entreprise

:::tip
Si vous êtes nouveau sur Miro, découvrez-en plus sur [les paramètres d'équipe et entreprise](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md).
:::

## Paramètres d’invitation de l’équipe

Pour une collaboration plus fluide, autorisez **tous les membres de l'équipe** à inviter de nouveaux membres dans l'équipe. Si vous préférez un plus grand contrôle des invitations de l’équipe, vous pouvez restreindre cette option aux admins d’entreprise et/ou d’équipe afin que toutes les demandes d’invitation soient envoyées via [la gestion des demandes](09-request-management-on-enterprise-plan.md). Vous pouvez également contrôler si les utilisateurs peuvent inviter des [invités](../../using-miro/sharing-boards/07-collaboration-with-guests.md) dans les équipes.

### Comment configurer les paramètres d’invitation de l’équipe

Pour gérer vos paramètres d’invitation de l'équipe, allez dans la console d’admin, puis dans **Équipes** et sélectionnez votre équipe. Le panneau de votre équipe s'ouvre. Sous **Invitation**, sélectionnez l'une des options suivantes :

- **Admins d’entreprise seulement**
  Seuls les admins d’entreprise peuvent ajouter de nouveaux membres à l’équipe.
- **Admins d’entreprise et admins d’équipe**
  Les admins d’entreprise et les admins d’équipe peuvent inviter de nouveaux membres dans l’équipe.
- **Tous les membres de l’équipe**
  Tous les membres de l’équipe peuvent inviter de nouveaux membres dans l’équipe.

:::note
Dans les abonnements au [programme de licences flexibles (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md), les paramètres d'invitation d'équipe sont complétés par les paramètres d'invitation de l'entreprise.
:::

### Comment configurer les invitations aux invités

Les admins d’entreprise peuvent autoriser ou restreindre l'option permettant aux membres d'inviter des [invités](../../using-miro/sharing-boards/07-collaboration-with-guests.md). Les invités ne peuvent accéder qu’aux tableaux auxquels ils sont invités et n’ont pas besoin d’une licence.

Mettez à jour les paramètres d'invitation des invités dans **Équipes** > choisissez votre équipe > **Paramètres** > **Autoriser les invités pour l’équipe [Nom].**

:::note
Les admins d’entreprise peuvent activer la désactivation automatique des invités après 30 jours d'inactivité.
:::

## Scénarios d’invitation

:::tip
Selon les [paramètres de gestion des demandes](09-request-management-on-enterprise-plan.md), les demandes de partage d’un tableau ou d’invitation d’un utilisateur dans une équipe peuvent soit être envoyées directement aux admins d’entreprise, à des personnes spécifiques par e-mail, ou bien un ticket d’assistance est créé.
:::

**Inviter de nouveaux membres dans une équipe**

Si les invités ne sont pas autorisés et que les membres ne sont pas autorisés à inviter de nouveaux membres, la notification ci-dessous s’affichera lorsqu’ils essayeront de partager un tableau et ils devront soumettre une demande.

**Octroyer le rôle de propriétaire ou de copropriétaire**

Si les membres ne sont pas autorisés à inviter de nouveaux membres et tentent d’assigner le rôle de propriétaire ou de copropriétaire sur un tableau spécifique à un invité ou à un membre sous licence [gratuite restreinte](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md), la notification ci-dessous s’affichera et ils devront soumettre une demande.

**Inviter un utilisateur externe ou un invité à modifier un tableau**

:::note
Les invités externes sont des invités hors domaine de votre entreprise. Ils ont une adresse e-mail externe à l’entreprise.
:::

Si les membres ne sont pas autorisés à inviter de nouveaux membres dans l’équipe et que les invités avec droit de modification n’ont pas été activés pour l’équipe, les personnes qui tentent d’inviter un utilisateur externe pour modifier un tableau verront s’afficher la notification ci-dessous et devront soumettre une demande. Une fois la demande soumise, la personne invitée sera ajoutée au tableau avec droit de commenter, ce qui lui permettra d’ajouter des commentaires sur le tableau mais pas d’en modifier le contenu.

## Paramètres d’invitation de l’entreprise

Les paramètres d’invitation de l’entreprise permettent de déterminer qui peut inviter de nouveaux membres dans votre abonnement Enterprise. Tous les nouveaux membres reçoivent une licence Avancée, Standard, Complète (ancienne version), Free, ou Free Restreinte selon votre [modèle de licence](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md) et [licence par défaut](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

### Comment configurer les paramètres d’invitation de l’entreprise

> **Disponible pour** : [programme de licences flexibles (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)

Pour gérer les paramètres d'invitation de l’entreprise, rendez-vous dans **Entreprise** > **Sécurité** > **Partage** > **Invitation** et sélectionnez l'une des options suivantes :

**Admins d’entreprise uniquement**
Seuls les admins d’entreprise peuvent accorder des licences aux nouveaux membres. Les admins d’équipe et les membres peuvent uniquement inviter les membres existants de l’entreprise dans leurs équipes, et ils ne peuvent pas activer de nouvelles licences.

**Admins d’entreprise et admins d’équipe**
Les admins d’entreprise et les admins d’équipe peuvent inviter de nouveaux membres et ajouter de nouvelles licences. Les admins d’équipe ne peuvent inviter de nouveaux membres que dans les équipes où ils sont admin d’équipe.

**Tous les membres**
Chaque membre de l’abonnement Enterprise peut ajouter de nouvelles licences en invitant des personnes dans son équipe, tant que les invitations sont autorisées pour **tous les membres de l’équipe** dans les paramètres d’invitation de l’équipe.

## Comment les paramètres de l’entreprise et de l’équipe fonctionnent ensemble

Les paramètres de l’entreprise complètent les paramètres d’invitation de l’équipe. Les admins d’entreprise peuvent, dans les paramètres de l’équipe, configurer qui peut inviter des utilisateurs dans une équipe spécifique. Cela signifie que les admins d’entreprise peuvent autoriser les membres et les admins d’équipe à gérer leurs propres invitations et la collaboration de l’équipe, mais les licences sont toujours sous le contrôle des admins d’entreprise dans les paramètres de l’entreprise.

## Désactivation automatique des invités

Paramétrez la désactivation automatique des invités après 30 jours d’inactivité. Utilisez cette fonctionnalité pour supprimer des invités et garder votre abonnement sécurisé.

Lorsque la fonctionnalité est activée, tous les invités (quel que soit leur domaine) qui n’ont pas été actifs dans vos équipes Enterprise au cours des 30 derniers jours seront automatiquement désactivés. Il n’est pas possible de personnaliser la période de 30 jours.

Ce paramètre est appliqué à toutes les équipes au sein de l’organisation.

Allez dans vos paramètres de **l'entreprise** > **Sécurité** > **Partage** et activez **Désactiver automatiquement les invités**.

:::tip
Dès que le paramètre est activé, l'action est enregistrée dans les [journaux d'audit](../security-integrations/security-management/01-audit-logs.md) comme **Paramètre d'expiration des utilisateurs externes activé/désactivé**. Les événements de désactivation seront également consignés dans les [journaux d'audit](../security-integrations/security-management/01-audit-logs.md). L'acteur apparaîtra comme **Miro Automation**.
:::
