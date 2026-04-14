---
title: Comment installer des applications
article_id: 360017731093
translation_id: 360017731093
locale: fr
sidebar_position: 4
created_at: '2019-02-11T10:12:46Z'
updated_at: '2025-08-05T07:54:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'Personnes: Tous les utilisateurs Forfaits: Tous les forfaits Plateformes:
    Navigateur, application de bureau Les admins d’équipe peuvent restreindre l’installation
    pour les non-admins. Les admins d’entreprise sur le forfait Enterprise peuvent
    restreindre davantage aux seules applications approuvées.'
---

Vous pouvez étendre les fonctionnalités de Miro en installant des applications depuis le Marketplace de Miro. Cet article vous guide à travers l'installation et la désinstallation d'applications, la compréhension des autorisations des applications, et fournit un aperçu de la création d'intégrations personnalisées.

## Installer des applications depuis le Marketplace de Miro

Le [Marketplace de Miro](https://miro.com/marketplace/) est votre hub central pour découvrir et ajouter des applications afin d'améliorer votre expérience Miro. Vous pouvez installer des applications directement depuis votre tableau ou en visitant le site du Marketplace.

![Miro_marketplace.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021611044242_Miro%20marketplace.jpg)*Marketplace de Miro*

Il existe deux façons principales pour les utilisateurs d'ajouter des applications :

1. **Depuis votre tableau :** Cliquez sur l’icône **Outils, médias et intégrations (+)** dans la barre d’outils de création, puis utilisez le champ de recherche "Rechercher des intégrations" dans l’onglet Marketplace. Si votre application figure déjà dans la liste, cliquez simplement pour l’ajouter. Vous pouvez également parcourir les applications disponibles depuis ce panneau.
   ![marketplace-add-apps.png](../../../../../../docs/integrations-apps/integrations-basics/images/21260776452626_marketplace-add-apps.png)*Marketplace dans la barre d’outils de création*
2. **Depuis le site du Marketplace :** Vous pouvez également aller directement sur le site du [Marketplace de Miro](https://miro.com/marketplace/) pour parcourir et installer des applications à partir de leurs listes respectives.

**Pour les admins d’entreprise :**
Les admins d’entreprise sur les forfaits applicables peuvent également installer des applications pour leur équipe entière via les paramètres de l’équipe. Pour ce faire, accédez à **Paramètres de l’équipe** > **Applications et intégrations** > **Installer des applications**. Cette section permet une gestion et un déploiement centralisés des applications dans toute l’équipe.

![apps_and_integrations_page.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021832338450_apps%20and%20integrations%20page.jpg)*Section des applications installées dans les paramètres de l’équipe pour les admins*

## Désinstaller des applications

Vous pouvez gérer et désinstaller des applications depuis les paramètres de votre équipe. Notez que les utilisateurs non admins peuvent avoir des restrictions sur la désinstallation des applications, selon la configuration de l'équipe.

:::warning
Les utilisateurs qui ne sont pas admins ne peuvent pas désinstaller des applications s'ils ne sont pas autorisés à les installer par un admin dans les paramètres de l'équipe.
:::

Pour gérer les applications de votre équipe, accédez à **Paramètres de l’équipe > Applications et intégrations**. Cette page répertorie toutes les applications actuellement installées pour votre équipe ou par vous personnellement.

![apps_settings.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021898097682_apps%20settings.jpg)*Applications et intégrations dans les paramètres de l’équipe*

Pour désinstaller une application, suivez ces étapes :

1. Dans la liste **Applications et intégrations**, sélectionnez l'application que vous souhaitez supprimer.
2. Cliquez sur **Désinstaller pour l'équipe** ou **Désinstaller pour moi**. L'option disponible dépendra de la manière dont l'application a été installée et de vos droits administratifs.

![uninstall_an_app.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021797466258_uninstall%20an%20app.jpg)*L’option pour désinstaller une application*

## Autorisations d'installation d'applications

Les admins d’entreprise et d’équipe disposent de divers contrôles pour gérer qui peut installer des applications et quelles applications sont disponibles pour leur organisation, garantissant ainsi la sécurité et la conformité.

Les admins d’équipe peuvent configurer si les membres de l’équipe qui ne sont pas admins sont autorisés à installer des applications. Ce paramètre se trouve dans **Paramètres de l’équipe > Applications et intégrations** sous les options de gestion d'application.

![allow_non-admins_to_install_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021903025170_allow%20non-admins%20to%20install%20apps.jpg)*Option "Permettre aux non-admins d’installer des applications" dans les paramètres de l’équipe*

Pour les utilisateurs sur le [forfait Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), les admins d’entreprise ont accès à des contrôles plus granuleux. Ils peuvent gérer les **applications approuvées** via **Paramètres de l’entreprise** > **Applications**. Cette fonctionnalité permet aux admins de créer une liste d'applications approuvées par l'entreprise, empêchant ainsi les utilisateurs d'installer des applications qui ne figurent pas sur cette liste approuvée. [En savoir plus sur la gestion de la découverte et des paramètres d'installation d'applications pour les forfaits Enterprise](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).

![Enterprise_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021890162962_Enterprise%20apps.jpg)*Gestion des applications approuvées dans les paramètres de l'entreprise Enterprise*

## Intégrations personnalisées et plateforme de développement

Si vous avez besoin de fonctionnalités spécifiques qui ne sont pas disponibles dans le Marketplace de Miro, vous pouvez créer vos propres solutions personnalisées en utilisant la [plateforme de développement Miro](https://miro.com/api/). Cette plateforme offre des outils robustes, y compris des API REST, des plugins web et des intégrations, pour vous aider à créer des intégrations puissantes adaptées à vos besoins.

Voici les points clés à considérer lors du développement d'intégrations personnalisées :

- **Pour commencer :** Vous pouvez commencer à développer votre application en [créant une équipe de développement](https://developers.miro.com/). Les équipes de développement standard sont destinées à des fins de développement et de test et ont certaines limitations :
  - Jusqu’à 5 utilisateurs dans l’équipe.
  - Jusqu’à 3 tableaux dans l’équipe.
  - Un filigrane est affiché sur les tableaux.
  - La fonctionnalité d'exportation de tableau n'est pas disponible.
- **Développeurs du forfait Enterprise :** Si votre organisation est sur un [forfait Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), vous pouvez créer une équipe de développement dans le cadre de votre abonnement. Ces équipes de développement ne sont pas soumises aux limitations des équipes standard et bénéficient de toutes les fonctionnalités de sécurité de niveau Enterprise. [En savoir plus sur les équipes de développement pour les forfaits Enterprise](../../enterprise-administration/managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md).

Pour des informations supplémentaires, de l'assistance et pour vous connecter avec d'autres développeurs, vous pouvez explorer le [forum de la plateforme de développement](https://community.miro.com/developer-platform-forum-57).
