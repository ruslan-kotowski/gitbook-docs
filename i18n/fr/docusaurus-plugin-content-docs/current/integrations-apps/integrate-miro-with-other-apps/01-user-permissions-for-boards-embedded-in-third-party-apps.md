---
title: Autorisations de l’utilisateur pour les tableaux intégrés dans des applications
  tierces
article_id: 4411883577618
translation_id: 4411883577618
locale: fr
sidebar_position: 1
created_at: '2021-12-08T10:13:42Z'
updated_at: '2025-11-25T16:07:55Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: 'Personnes: Propriétaires du tableau, copropriétaires du tableau Forfaits:
    Tous les forfaits Plateformes: Navigateur, application de bureau'
---

Miro propose plusieurs intégrations qui vous permettent de collaborer facilement avec des tableaux dans des environnements tiers, tels que [Microsoft Teams](../microsoft), [Confluence](../atlassian/01-miro-for-confluence.md), Notion et Google Meet. Vous pouvez découvrir d'autres applications prises en charge dans le [Marketplace de Miro](https://miro.com/marketplace/category/embed-miro/). Lorsque vous intégrez des tableaux, vous pouvez définir différents niveaux d'accès utilisateur et gérer ces autorisations depuis Miro.

## Comprendre l'accès intégré

Lorsque vous partagez un tableau dans une application externe, vous pouvez accorder un accès pour consultation, commentaire ou modification spécifiquement aux utilisateurs de cette application pour une collaboration unique, quel que soit leur accès à Miro. Ces utilisateurs n'auront pas besoin d'avoir un profil Miro pour accéder au tableau dans l'application. Cela vous permet de définir certains droits d'accès au tableau pour les utilisateurs de l'application qui ne sont pas inscrits sur Miro sans rendre le tableau accessible au public.

Pour une sécurité maximale, nous déconseillons l'utilisation de cette méthode en dehors d'une collaboration ponctuelle (comme un atelier) et recommandons à votre organisation d'attribuer l'accès à Miro de manière appropriée aux personnes qui en ont besoin.

![embed_Miro_in_Zoom.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020254296722_embed%20Miro%20in%20Zoom.gif) *Configuration des droits d'accès pour l'intégration d'un tableau*

Le tableau devient accessible uniquement dans l’application où il a été intégré. Le niveau d’accès que vous définissez pour un tableau intégré dans l’application n’affecte pas les paramètres de partage du tableau en dehors de l’application. Par exemple, si un [tableau privé](../../using-miro/sharing-boards/15-make-a-miro-board-private.md) est intégré dans un canal Microsoft Teams avec un accès "Toute personne peut lire", les utilisateurs de ce canal Microsoft Teams peuvent consulter le tableau sans connexion à Miro. Si les mêmes utilisateurs tentent d’accéder au tableau en dehors du canal Microsoft Teams en suivant le lien du tableau, ils n’y auront pas accès.

Notez toutefois que les paramètres de partage des tableaux du côté de Miro priment sur le niveau d'accès défini dans l'application externe. Par exemple, si un tableau est [partagé publiquement du côté de Miro](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), il sera disponible pour tous dans Microsoft Teams, même si vous avez intégré le tableau en tant que Privé.

## Gérer et révoquer l'accès intégré

Vous pouvez facilement suivre, gérer et révoquer l'accès aux tableaux intégrés dans des applications externes prises en charge.

Pour gérer et révoquer l'accès aux tableaux intégrés :

1. Cliquez sur le bouton **Share** pour ouvrir les paramètres de partage d’un tableau Miro.
2. Sélectionnez **Sharing settings** (Paramètres de partage).
3. Ouvrez l’onglet **Embeds** (Intégrations).
4. Vous verrez les applications externes dans lesquelles le tableau est intégré, y compris le nom de l'intégration, quand et par qui il a été intégré, ainsi que les paramètres d'accès au tableau dans l'application.
5. Pour révoquer l’accès au tableau dans une application, cliquez sur **Révoquer l’accès** en regard de l’application. Notez que cette action est irréversible.

ol

![remove_an_access_link.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020265344914_remove%20an%20access%20link.gif)
*Suppression d’un lien d’accès*

Une fois l'accès intégré révoqué, l'accès au tableau sera limité dans l'application. Notez que le tableau peut toujours être accessible dans l’application s’il est partagé dans Miro. Par exemple :

- Si tout le monde pouvait **modifier** le tableau au sein de l’application et que le même tableau est [publiquement partagé](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) pour **consultation** dans Miro, tout le monde pourra toujours **consulter** le tableau dans l’application.
- Si le tableau est privé et uniquement partagé [avec d’autres utilisateurs par e-mail](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), les utilisateurs devront **se connecter** pour accéder au tableau intégré dans l’application.

## Règles et limitations d'intégration

Veuillez noter les règles et limitations suivantes lors de l'intégration de tableaux :

- Vous ne pouvez pas intégrer un tableau s'il est [inactif](../../using-miro/tools/troubleshooting/15-the-board-is-locked.md) ou si vous avez un accès en lecture seule au tableau.
- Les tableaux stockés dans des [équipes du plan Free](../../plans-billing/miro-plans/09-free-plan.md) ne peuvent pas être intégrés avec un accès en commentaires.
- Pour les utilisateurs du [forfait Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), vos paramètres d’accès suivront les contrôles d’accès à l’échelle de l’organisation, ce qui peut impliquer que certaines options de partage peuvent être restreintes. En savoir plus : [Gérer la politique de partage pour les intégrations embarquées sur un compte Enterprise](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- Pour certains anciens liens, vous ne verrez que le niveau d'accès et l'application, mais pas le nom de la personne qui a créé le tableau ni quand il a été intégré.
- Si vous souhaitez limiter la capacité d’intégrer des tableaux Miro dans des applications externes pour le compte Enterprise de votre organisation, consultez l’article [Gérer la politique de partage pour les intégrations embarquées sur un compte Enterprise](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- La gestion des liens d’accès des tableaux intégrés n’est pas encore prise en charge sur les appareils mobiles et les tablettes.

En savoir plus sur [l'accès aux tableaux intégrés pour les utilisateurs disposant de licences gratuites restreintes](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
