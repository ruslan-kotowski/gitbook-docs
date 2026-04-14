---
title: Miro pour Microsoft Teams (guide d'admin)
article_id: 4406387610002
translation_id: 4406387610002
locale: fr
sidebar_position: 1
created_at: '2021-09-09T10:28:14Z'
updated_at: '2025-11-25T16:07:14Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
availability:
  notes: 'Disponible pour: Free, Starter, Business, Education, Enterprise plans, et
    tous les plans Microsoft 365.'
---

:::note
Les paramètres d'autorisation et d'accès varient en fonction du type de plan. Pour en savoir plus sur les utilisateurs externes dans Microsoft Teams, veuillez consulter la [politique de Microsoft en matière d'applications](https://learn.microsoft.com/microsoftteams/apps-external-users).
:::

Activez l'intégration de Miro pour Microsoft Teams afin d'accélérer la collaboration au sein de votre équipe. Miro pour Microsoft Teams offre un certain nombre d'expériences qui permettent aux utilisateurs de recevoir des notifications en temps réel ainsi que de collaborer sur des tableaux Miro intégrés dans les réunions Teams, les canaux, les chats et les invitations du calendrier.

Miro prend également en charge les cartes adaptatives grâce au déploiement de liens et aux extensions de messages de recherche, ce qui donne aux utilisateurs plus de contexte sur les tableaux partagés et permet de gérer rapidement l'accès aux tableaux, le tout sans quitter leur espace Microsoft Teams.

:::tip
En savoir plus sur l'[intégration de Microsoft Teams](..) par Miro.
:::

<iframe allowfullscreen="" frameborder="0" height="315" src="//www.youtube-nocookie.com/embed/6xab9nSnmAA" width="560"></iframe>
 *Miro pour les équipes Microsoft*

## Gestion des applications

:::warning
Les administrateurs de Microsoft devront activer l'intégration de Miro pour Microsoft Teams à partir du catalogue de gestion des applications Microsoft. Les administrateurs de Miro Enterprise devront également activer l'intégration à partir du panneau de gestion des applications Miro.
:::

### Gestion des applications dans Microsoft Teams

Les paramètres peuvent varier en fonction des comptes. En savoir plus sur [la gestion des applications dans Microsoft Teams](https://learn.microsoft.com/microsoftteams/manage-apps).

Pour que votre organisation tire le meilleur parti de l'intégration, installez en masse et épinglez l'application Miro à l'aide de la [politique de configuration des applications de Microsoft](https://learn.microsoft.com/microsoftteams/teams-app-setup-policies).

### Gestion des applications dans Miro

Dans les paramètres de votre société Miro > **Applications**, vous verrez deux applications Microsoft Teams :

- Miro pour Microsoft Teams (intégration des onglets) - intégrez Miro dans le calendrier, les réunions Teams, les canaux et les chats.
- Microsoft Teams (intégration des robots) - notifications des utilisateurs

Si vous désactivez Microsoft Teams (intégration par bot), les utilisateurs ne recevront plus de notifications Miro dans Microsoft Teams.

![Microsoft-Teams-Bot-Tab-Applications.png](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21017606037010_Microsoft-Teams-Bot-Tab-Apps.png)*Applications Microsoft Teams*

## Comprendre les paramètres d’accès de partage du tableau

Lors de l'ajout d'un tableau en tant qu'onglet dans les réunions, les invitations au calendrier, les chats et les canaux, les utilisateurs peuvent définir les autorisations de partage appropriées. Pour ajouter un tableau en tant qu'onglet dans Microsoft Teams, visitez Ajouter Miro en tant qu'onglet dans Microsoft Teams. En savoir plus sur les [paramètres d'accès à un tableau embarqué](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

### Configuration des paramètres d’accès pour votre tableau

Les options des paramètres d’accès suivront les contrôles d’accès à l’échelle de l’organisation.  Si vous avez un forfait Enterprise et que vous avez restreint le partage des tableaux intégrés, cette option ne sera pas disponible pour les utilisateurs. Pour en savoir plus, consultez le[site](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md) [Managing Enterprise sharing policy for embed integrations (Gestion de la politique de partage de l'Enterprise pour les intégrations)](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).

![publi__editing_is_turned_off.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21017593055506_publi%D1%81%20editing%20is%20turned%20off.jpg)*Exemple de désactivation de l'édition publique par l'admin d'entreprise*
