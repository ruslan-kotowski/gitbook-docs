---
title: Se connecter à Jira en utilisant OAuth 1.0 (Mis à jour)
article_id: 27689156602514
translation_id: 27689200297618
locale: fr
sidebar_position: 12
created_at: '2025-06-27T13:20:33Z'
updated_at: '2025-11-25T15:52:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Qui peut le faire: Admins d''entreprise, Admins d’équipe Quels forfaits:
    Starter, Business, Enterprise, Éducation Quelles plateformes: Navigateur, Bureau'
---

Les organisations qui ne sont pas prêtes à migrer vers OAuth 2.0 peuvent utiliser la procédure suivante pour connecter Miro à Jira en utilisant OAuth 1.0.

Atlassian a [déprécié OAuth 1.0](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively), et la méthode fournie dans cet article est une solution provisoire. Pour éviter les problèmes, et pour s'aligner sur les meilleures pratiques en matière de sécurité et de compatibilité, Miro recommande fortement de migrer vers OAuth 2.0 dès que possible.

:::note
La méthode d'authentification OAuth 1.0 précédente [est obsolète](https://help.miro.com/hc/articles/360019501754-Set-up-and-disable-Jira-Cards-OAuth-1-0) et sera retirée le 31 juillet 2025.
:::

Cet article explique également comment utiliser une instance Jira pour plusieurs équipes Miro et comment désactiver les cartes Jira au niveau de l'organisation et de l'équipe.

## Prérequis

- Assurez-vous de disposer des autorisations suivantes :
  - (Business, Enterprise) admin de l'entreprise Miro
    (Starter, Education) admin d’équipe Miro
  - Admin du système Jira

    > ✏️ Pour terminer la procédure, vous devez être en mesure de créer un lien applicatif dans Jira.
- Dans Jira, supprimez tout lien applicatif existant vers Miro.

## Procédure

Pour vous connecter à Jira en utilisant OAuth1.0, suivez ces étapes :

1. Depuis votre tableau de bord Miro, sélectionnez votre avatar en haut à droite et cliquez sur **Console d’admin**.
2. Dans la barre latérale gauche, allez à **Apps et intégrations** > **Apps** > onglet **Gérer les apps**.
3. Assurez-vous que **N'autoriser que les apps de la liste ci-dessous** est activé.
4. Dans la colonne **App**, pour **Cartes Jira**, sélectionnez **Paramètres**.
5. Dans l'onglet **Paramètres par défaut**, sélectionnez **Ajouter une nouvelle connexion**.
6. Sous **Configuration de Jira**, sélectionnez soit **Jira Cloud** soit **Jira Data Center**.
7. Sous **Méthode d’authentification**, sélectionnez **OAuth 1.0x (Mis à jour)**.
8. Sous **URL Jira**, saisissez l’URL de votre instance Jira.
9. (Facultatif) Pour faire de cette connexion la connexion par défaut pour toutes les équipes de votre organisation, cochez **Définir comme par défaut**.
10. Sous **Instructions d’installation**, vérifiez que vous avez les propriétés suivantes :
    - URL
    - Clé consommateur
    - Nom du consommateur
    - Clé publique
11. Dans Jira, créez un lien d'application.
    1. (Cloud) Allez dans **Paramètres** > **Produits** > **Liens d'application**.
       (Data Center) Dans les paramètres d'administration de Jira, allez dans **Produits** > **Liens d'application**.
    2. Cliquez sur **Créer un lien**.
    3. (Cloud) Pour **Type d'application**, sélectionnez **Application directe**.
       (Data Center) Pour **Type d'application**, sélectionnez **Produit Atlassian**.
    4. Pour **URL de l'application**, collez l'URL des instructions de configuration de Miro. Voir étape 10.
    5. Cliquez sur **Continuer**.
    6. Pour **Nom de l'application**, nommez votre application.

       > **⚠️** N'entrez pas de données dans d'autres champs. Vous fournirez les données Miro dans une étape suivante.
    7. Cochez **Créer un lien entrant**.
    8. Cliquez sur **Continuer**.
    9. Copiez et collez votre clé client, nom de client, et clé publique à partir des instructions de configuration de Miro. Voir l'étape 10.
    10. Cliquez sur **Continuer**.
        Vous avez créé votre lien d'application.
12. Dans Miro, cliquez sur **Se connecter**.
    Vous avez connecté Miro à Jira à l'aide d'OAuth 1.0.

## Et ensuite ?

Vous avez configuré et connecté votre intégration Jira avec Miro en utilisant OAuth1.0 de Jira. Lorsqu’un utilisateur tente pour la première fois une action liée à Jira dans Miro, il doit s’authentifier.

**Plus d’informations :** Voir [Comment utiliser les cartes Jira](https://help.miro.com/hc/articles/360017572434).

## Une instance Jira pour plusieurs équipes Miro

Vous pouvez installer les cartes Jira au niveau de l’organisation ou au niveau de l’équipe. Si vous avez plusieurs équipes, vous pouvez spécifier des paramètres au niveau de l’organisation pour éviter une configuration répétée pour chaque équipe. Le lien d’application existant est alors utilisé pour toutes les équipes.

:::note
La connexion de plusieurs instances Jira à une seule équipe Miro n’est pas prise en charge.
:::

Pour les demandes de mise à jour, après avoir connecté votre organisation ou équipe à une instance Jira, un webhook est ajouté aux webhooks de Jira pour cette organisation ou équipe Miro.

:::tip
Donnez un nom unique à chaque webhook par équipe. Allez sur votre page des webhooks Jira et modifiez chaque webhook nouvellement créé.
:::

Si vous spécifiez des paramètres au niveau de l'organisation, les équipes qui ont déjà leurs propres paramètres d'équipe conservent leur configuration. Toute équipe ayant sa propre configuration peut passer à tout moment aux paramètres au niveau de l'organisation.

Inversement, toute équipe peut outrepasser les paramètres au niveau de l'organisation pour se connecter à une instance Jira distincte.

## Désactiver les cartes Jira

### Niveau de l'organisation

Pour désactiver les cartes Jira au niveau de l'organisation, suivez ces étapes :

1. Depuis votre tableau de bord Miro, cliquez sur votre avatar dans le coin supérieur droit et sélectionnez **Console d’admin**.
2. Allez dans **Applications et Intégrations** > **Gérer les applications**.
3. Trouvez **Jira Cards**.
4. Pour Jira Cards, basculez **Autorisé** en position désactivée.

:::warning
Si vous désactivez Jira Cards pour l'organisation, alors les membres de toutes les équipes Enterprise ne pourront pas utiliser les cartes Jira. Pour en savoir plus sur la gestion des applications, consultez [Gestion des applications](https://help.miro.com/hc/articles/4404659741458).
:::

### Niveau équipe

Pour désactiver Jira Cards au niveau de l'équipe, suivez ces étapes:

1. Depuis votre tableau de bord Miro, cliquez sur votre avatar dans le coin supérieur droit et cliquez sur **Console d’admin**.
2. Accédez à **Équipes**.
3. Cliquez sur la ligne de l’équipe que vous souhaitez gérer.
   Le panneau des paramètres de l’équipe s’ouvre.
4. Cliquez sur l’onglet **Apps**.
5. Localisez et cliquez sur **Jira Cards**.
6. Cliquez sur **Supprimer pour l’équipe**.
