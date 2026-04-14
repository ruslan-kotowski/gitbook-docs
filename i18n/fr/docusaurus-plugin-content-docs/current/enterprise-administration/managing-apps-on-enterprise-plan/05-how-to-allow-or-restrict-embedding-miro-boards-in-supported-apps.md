---
title: "Comment autoriser ou restreindre l\u2019int\xE9gration de tableaux Miro dans\
  \ les applications prises en charge"
article_id: 4405088016274
translation_id: 4405088016274
locale: fr
sidebar_position: 5
created_at: '2021-08-13T05:51:25Z'
updated_at: '2025-11-25T16:06:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: live-embed
---

Miro dispose de plusieurs intégrations permettant aux utilisateurs de partager facilement un tableau dans des applications externes telles que [Zoom](../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md), [Microsoft Teams](../../integrations-apps/microsoft/microsoft-teams/05-embed-miro-boards-in-microsoft-teams.md), [Jira](../../integrations-apps/atlassian/02-miro-for-jira-cloud.md), [Confluence](../../integrations-apps/atlassian/01-miro-for-confluence.md), et [bien d’autres](https://miro.com/marketplace/category/embed-miro/).  Les admins de comptes Enterprise peuvent autoriser ou restreindre l’intégration des tableaux dans les applications prises en charge.

> **Concerne :** [le forfait Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)

### Intégration de tableaux Miro dans les applications prises en charge

Lorsque vous intégrez un tableau Miro dans une application prise en charge, vous pouvez autoriser les utilisateurs de l’application à accéder au tableau même s’ils n’ont pas de profils Miro.

Le partage d’un tableau dans une application prise en charge n’affecte pas les paramètres de partage dans Miro.  En savoir plus sur l’Accès aux tableaux intégrés dans les applications prises en charge/span>[.](../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)

![allow_restrict_embed_customize_embed.gif](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/21019705471122_allow_restrict_embed_customize_embed.gif)*Intégration d'un tableau Miro avec accès restreint*

### Comment restreindre ou autoriser l’intégration de tableaux dans les applications prises en charge

> **Qui peut le faire ? les admins d’entreprise**

Les admins d’entreprise bénéficiant du forfait Enterprise peuvent configurer la possibilité d’intégrer des tableaux Miro aux applications prises en charge**.**  Une fois ce paramètre activé, les utilisateurs peuvent intégrer leurs tableaux Miro même si le partage public est restreint au sein de votre organisation ou de vos équipes/strong>.

Pour autoriser ou restreindre le partage avec des utilisateurs non connectés dans les applications prises en charge :

1. Allez dans les **paramètres de l'** **organisation**.
2. Sous **Sécurité**, cliquez sur **Partage.**
3. Faites défiler la page jusqu'à la section Contenu et activez/désactivez l'option **Autoriser le partage via l'intégration**.

:::note
En savoir plus sur [l’accès aux tableaux intégrés pour les utilisateurs disposant de licences gratuites restreintes](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
:::

![allow-embedding.pngAutoriser le](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803639826_allow-embedding.png)
*partage via embed sur le plan Enterprise*

Si vous désactivez ce paramètre, les tableaux précédemment intégrés deviendront indisponibles. Les nouveaux tableaux peuvent toujours être intégrés mais exigeront que chaque visiteur y ait accès.

Les utilisateurs ont une vue complète de toutes les applications dans lesquelles un tableau spécifique a été intégré, avec la possibilité de révoquer l’accès à tout moment, à partir des paramètres de partage du tableau.  En savoir plus sur la manière de gérer et de révoquer l’accès aux tableaux intégrés/span>[.](../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)

### Les tableaux intégrés dans les applications prises en charge peuvent-ils être protégés par un mot de passe ?

Dans les paramètres de l'entreprise, les administrateurs ont la possibilité d'exiger des mots de passe pour les tableaux Miro qui sont partagés par un lien public.

Lorsque vous [partagez un tableau Miro protégé par un mot de passe à l’aide d’un lien public](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), ces paramètres ne sont pas conservés dans les tableaux intégrés aux applications prises en charge.  La protection par mot de passe n’est pas appliquée lorsque vous intégrez un tableau dans Microsoft Teams, Zoom/span> [ou toute autre application.](../../integrations-apps/microsoft/microsoft-teams/05-embed-miro-boards-in-microsoft-teams.md)

Nous nous assurons par contre que l’accès à un tableau intégré est uniquement possible depuis l’application prise en charge et pas en dehors de l’application (par exemple, depuis un navigateur web), sauf si le tableau est [partagé dans Miro](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).
