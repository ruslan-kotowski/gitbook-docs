---
title: Jira OAuth 1.0 obsolète dans Miro
article_id: 28738797627538
translation_id: 28739445491986
locale: fr
sidebar_position: 13
created_at: '2025-08-13T12:34:39Z'
updated_at: '2025-10-20T14:49:04Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  plans: starter, business, enterprise, education
  notes: 'Personnes: Admins d’entreprise Plateformes: Navigateur, Bureau'
---

L'authentification Jira OAuth 1.0 sera obsolète à partir d'août 2025.

Si votre organisation a déjà migré vers Jira OAuth 2.0, vous pouvez ignorer cet article. Aucune action n'est requise de la part de votre admin d’entreprise. Vous pouvez vérifier avec votre admin d’entreprise que votre organisation utilise OAuth 2.0.

:::warning
Si votre organisation n'a pas migré vers OAuth 2.0, alors votre intégration de Jira avec Miro, y compris Jira Cloud, Server, et Data Center, peut être perturbée.
:::

Seuls les admins d’entreprise peuvent mettre à jour les équipes de leur organisation.

En cas de perturbation, la synchronisation entre Miro et Jira s'arrête jusqu'à ce que votre organisation mette à jour vers l'authentification OAuth 2.0. Les cartes Jira existantes restent sur vos tableaux Miro.

Une perturbation signifie que l’importation est indisponible, les cartes ne sont pas mises à jour, les détails ne peuvent pas être chargés, et la création ou la mise à jour d’une planification est impossible.

Pour éviter toute perturbation, Miro recommande que vos admin d'entreprise procèdent immédiatement à la mise à jour vers Jira OAuth 2.0.

:::tip
Les admins peuvent vérifier votre version OAuth.
:::

## Pourquoi OAuth 1.0 est-il déprécié ?

Atlassian a déprécié et ne supporte plus le protocole d’authentification OAuth 1.0.

**Plus d’informations :** Voir (Externe) [OAuth 1.0a pour les API REST (Obsolète)](https://developer.atlassian.com/cloud/jira/platform/jira-rest-api-oauth-authentication/).

## Vérifiez votre version OAuth

En tant qu'admin d’équipe Enterprise ou d’un forfait Starter ou Business, vous pouvez vérifier si votre équipe utilise OAuth 1.0 ou OAuth 2.0.

Suivez les étapes suivantes :

1. Depuis votre tableau de bord Miro, cliquez sur votre avatar dans le coin supérieur droit et sélectionnez **Console d’admin**.
2. Allez à **Équipes** > **[Nom de l’équipe]**.
3. Cliquez sur **Applications**.
4. Trouvez et cliquez sur **Cartes Jira**.
5. Allez à **Paramètres admin** > **Configuration Jira**.
   La configuration indique quelle version d'OAuth votre équipe utilise.
6. (Facultatif) Répétez les étapes 1-5 pour les autres équipes que vous souhaitez vérifier.
7. Informez votre/vos admin(s) d’entreprise sur les équipes n'utilisant pas OAuth 2.0.

## Trouver votre admin d’entreprise

Pour identifier votre ou vos admins d’entreprise, suivez ces étapes :

:::note
(Enterprise) Si la confidentialité de l’équipe est activée, les non-admins d’entreprise ne peuvent pas consulter les listes de membres.
:::

1. Accédez aux **Paramètres du profil de l’équipe** dans Miro.
2. Ouvrez la page des **Membres**.
3. Cliquez sur **Rôles supplémentaires**.
4. Recherchez les utilisateurs ayant le rôle d’**Admin d’entreprise**.

:::tip
Pour vous assurer que votre équipe passe à OAuth 2.0 et évite toute interruption, partagez cet article avec votre ou vos admins d’entreprise.
:::

## Passer à OAuth 2.0 pour les admins d’entreprise

En tant qu'admin d’entreprise, vous disposez des ressources suivantes pour vous aider à faire passer votre organisation à OAuth 2.0 :

- [Connexion à Jira Cloud en utilisant OAuth 2.0](https://help.miro.com/hc/articles/8588617184402)
- [Connexion à Jira Data Center en utilisant OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
- [Connecter les équipes de l'organisation aux paramètres par défaut de Jira](https://help.miro.com/hc/articles/26438407676434)

## Solution intérimaire

Si OAuth 2.0 n'est pas une option pour votre organisation pour le moment, Miro propose une [solution intermédiaire utilisant OAuth 1.0](https://help.miro.com/hc/articles/27689156602514).

Toutefois, Miro recommande de passer à OAuth 2.0 pour une méthode d'authentification plus sécurisée et pérenne qui suit les normes actuelles d'Atlassian.

## Aide supplémentaire

Si vous ou votre admin d’entreprise avez des questions, contactez le [service d’assistance Miro](https://help.miro.com/hc/articles/360020185799).
