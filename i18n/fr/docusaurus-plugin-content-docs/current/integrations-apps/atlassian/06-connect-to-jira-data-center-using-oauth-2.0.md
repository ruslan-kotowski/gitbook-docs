---
title: Se connecter au Jira Data Center en utilisant OAuth 2.0
article_id: 25753304280466
translation_id: 26513439039506
locale: fr
sidebar_position: 8
created_at: '2025-05-06T09:05:36Z'
updated_at: '2025-05-21T09:27:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Qui peut le faire: Admins d''entreprise ayant des autorisations d''administrateur
    système Jira Quels forfaits: Entreprise Quelles plateformes: Navigateur, Bureau'
---

> La connexion au Centre de données Jira à l'aide d'OAuth 2.0 n'est activée qu'au niveau de l'organisation.

## Prérequis

- Assurez-vous d'avoir les autorisations suivantes :
  - Autorisations d’administration système Jira
  - Rôle d'admin d’entreprise Miro
- Créer un lien d'application OAuth 2.0 sur Jira Data Center. Pour en savoir plus, consultez le [support des applications Atlassian Jira](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Create%20an%20incoming%20link%20using%20application%20links).
  - Utilisez l'URL de redirection suivante lorsqu'elle est demandée :
    https://integrations.miro.com/api/external-auth/oauth2/callback
  - Pour utiliser les webhooks automatiques, assurez-vous de sélectionner **Admin** pour votre périmètre.

## Connecter Miro à Jira Data Center en utilisant OAuth 2.0

1. Depuis votre tableau de bord Miro, sélectionnez votre avatar dans le coin supérieur droit et accédez à la (Enterprise) **console d'administration**, ou(Starter et Business) **Paramètres**.
2. Dans la barre latérale gauche, allez à **Applications et intégrations ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** >  **Applications** >  **Gérer les applications** .
3. Assurez-vous que **Autoriser uniquement les applications de la liste ci-dessous** est activé.
4. Sous la colonne **Application**, pour les **cartes Jira**, sélectionnez **Paramètres.**
5. Sélectionnez **Établir une nouvelle connexion**.
6. Dans **Configuration de Jira**, sélectionnez **Jira Data Center**.
7. Sous **Méthode d’authentification**, sélectionnez **OAuth 2.0**.
8. Pour **URL Jira**, entrez l'URL de votre instance Jira.
9. (Facultatif) Pour faire de cette connexion la connexion par défaut pour toutes les équipes de votre organisation, cliquez sur **Définir par défaut**.
10. Saisir l’identifiant **client Jira**.
    **En savoir plus**: Consultez (Externe) [Configurer un lien entrant](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
11. Saisir le **secret du client** Jira.
    **En savoir plus** : Voir (Externe) [Configurer un lien entrant](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
12. Choisissez votre périmètre.
    Pour utiliser les webhooks automatiques, choisissez **Admin** ou **Admin du système**.
13. Pour obtenir des mises à jour en temps réel de Jira dans Miro, cochez **Créer un webhook automatiquement**.
    > ✏️ Vous pouvez éventuellement ajouter manuellement le webhook ultérieurement.
14. Sélectionner **Connecter**.
    > La première fois qu'un utilisateur tente une action liée à Jira, il est invité à s'authentifier. Il n'est pas nécessaire qu'ils se réauthentifient.

## Et ensuite ?

Pour afficher et gérer vos instances Jira connectées, accédez à la **console d'administration** | **Paramètres** > **Applications et intégrations ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Gérer les applications**. Ensuite, sous la colonne **Application**, pour **Cartes Jira**, sélectionnez **Paramètres**.

Pour apprendre comment connecter vos équipes à l'instance Jira par défaut, consultez [Connecter des équipes dans une organisation aux paramètres Jira par défaut.](https://help.miro.com/hc/articles/26438407676434)

## FAQ

**Le choix d'Admin pour l'étendue nécessite-t-il que tous les utilisateurs aient des privilèges d'admin dans Jira ?**

Non. Le statut d'Admin signifie que l'Admin a le niveau d'autorisation le plus élevé qu'un utilisateur puisse avoir dans Miro. Le périmètre est de toute façon limité par utilisateur, en fonction de leurs autorisations dans Jira.

**Puis-je connecter Jira Data Center avec OAuth 2.0 au niveau de l’équipe ?**

Non. Uniquement au niveau de l'organisation.
