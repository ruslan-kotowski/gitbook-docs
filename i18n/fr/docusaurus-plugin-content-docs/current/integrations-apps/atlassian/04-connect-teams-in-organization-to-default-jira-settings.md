---
title: Connecter les équipes de l'organisation aux paramètres Jira par défaut
article_id: 26438407676434
translation_id: 26442006352530
locale: fr
sidebar_position: 6
created_at: '2025-05-02T14:36:29Z'
updated_at: '2025-10-21T12:08:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Qui peut le faire: admin d’entreprise Quels forfaits: Enterprise Quelles
    plateformes: Navigateur, Bureau'
---

Les admins d’entreprise peuvent connecter en masse les équipes de leur organisation pour utiliser les paramètres Jira globaux, ce qui remplace les paramètres spécifiés au niveau de l'équipe.

## Prérequis

- Assurez-vous d'avoir le rôle d’admin d’entreprise dans Miro.
- Assurez-vous d'avoir une connexion par défaut à un [Centre de données Jira utilisant OAuth 2.0](https://help.miro.com/hc/articles/25753304280466).

## Connecter les équipes aux paramètres Jira par défaut

1. Depuis votre tableau de bord Miro, sélectionnez votre avatar en haut à droite et allez dans **Console d'administration** | **Paramètres**.
2. Dans la barre latérale gauche, allez à **Applications et intégrations ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Applications** > onglet **Gérer les applications**.
3. Assurez-vous que **N'autoriser que les applications de la liste ci-dessous** est activé.
4. Sous la colonne **Application**, pour **Cartes Jira**, sélectionnez **Paramètres**.
5. Sous **Ajouter des équipes à l'instance par défaut**, sélectionnez chaque équipe que vous voulez connecter, ou cliquez sur **Sélectionner tout**.

   > ✏️ La liste montre uniquement les équipes qui n'utilisent pas les paramètres globaux de l'organisation.
6. Cliquez sur **Ajouter <nombre d'équipes> à défaut**.

   > ✏️ Les utilisateurs qui n'utilisent pas déjà l'instance globale de Jira dans votre organisation sont migrés, et doivent se réauthentifier.

   > ✏️ Les utilisateurs migrés depuis une autre instance Jira sont invités à se réauthentifier la première fois qu'ils tentent une action liée à Jira dans Miro.

## FAQ

**Les équipes vont-elles continuer à utiliser la connexion globale à Jira indéfiniment ?**

Non. Vous pouvez modifier ultérieurement les paramètres Jira pour une équipe donnée.

**Quelles équipes devraient utiliser la connexion globale à Jira ?**

Il est généralement préférable d'utiliser les paramètres de l'organisation car cela nécessite moins de gestion de votre part. Si l'une de vos connexions à une équipe partage les mêmes paramètres que l'organisation, nous conseillons d'intégrer les équipes aux paramètres par défaut de l'organisation pour cette raison.
