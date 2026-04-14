---
title: Connectez-vous à Jira on-premise avec des serveurs d’autorisation tiers en
  utilisant OAuth2.0
article_id: 25692796700306
translation_id: 26751270491410
locale: fr
sidebar_position: 9
created_at: '2025-05-16T09:14:02Z'
updated_at: '2025-11-25T15:50:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Qui peut le faire: les admins d’entreprise Quels forfaits: Entreprise'
---

> *✏️* La connexion de Jira via un serveur d'autorisation est uniquement activée au niveau de l'organisation.

Cet article fournit les étapes pour connecter Miro à Jira avec un serveur d'autorisation tiers sur site utilisant OAuth2.0.

Pour apprendre les détails techniques de cette configuration, consultez l'article de référence pour [Jira sur site avec autorisation tierce utilisant OAuth 2.0](https://help.miro.com/hc/articles/26726425696530).

## Prérequis

- Assurez-vous de disposer des autorisations suivantes :
  - Admin d’entreprise Miro
  - (Facultatif) Administrateur système Jira, si vous souhaitez utiliser des webhooks automatiques.
- Sur votre serveur d’autorisation, créez une application OAuth 2.0.
- Configurez l'URL de redirection dans votre application OAuth 2.0 vers l'URL suivante :
  https://integrations.miro.com/api/external-auth/oauth2/callback
- Assurez-vous d'avoir les détails suivants de votre application OAuth 2.0 prêts à être configurés dans Miro :
  - URL d’autorisation
  - URL du jeton
  - Identifiant client
  - Secret client
  - Portée

## Se connecter à Jira sur site avec des serveurs tiers en utilisant OAuth 2.0

1. Sur votre tableau de bord Miro, sélectionnez votre avatar dans le coin supérieur droit et allez dans **Console d'administration** | **Paramètres**.
2. Aller dans **Applications et intégrations ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)**> **Applications** > **Onglet Gérer les applications**.
3. Assurez-vous que **Autoriser uniquement les applications de la liste ci-dessous** est activée.
4. Dans la colonne **App**, pour les **cartes Jira**, sélectionnez **Paramètres**.
5. Cliquez sur **Établir une nouvelle connexion**.
6. Sous **configuration de Jira**, cliquez sur **Jira Data Center**.
7. Sous **Méthode d’authentification**, sélectionnez **OAuth2.0 via un serveur d'autorisation tiers**.
8. Sous **URL Jira**, entrez l'URL de votre instance Jira.
   > *✏️* Vous pouvez ajouter votre URL de base Jira externe ou votre URL Jira interne. Si vous utilisez une URL interne Jira, vous devez alors spécifier votre URL de passerelle API externe à l'étape 10.

   > *✏️* En général, l'utilisation d'une URL interne vous permet d'ajuster la fonctionnalité de navigation vers la source.
9. (Facultatif) Pour faire de cette connexion la connexion par défaut pour toutes les équipes de votre organisation, cochez **Définir par défaut**.
10. (Optionnel) Si vous utilisez une passerelle API pour faire des requêtes à Jira, alors pour l'**URL de base de la passerelle d’API Jira**, saisissez l'URL de votre passerelle API externe.
11. Saisissez les détails suivants de votre application OAuth 2.0 :
    - URL d’autorisation
    - URL du jeton
    - Identifiant client
    - Clé secrète client
    - Portée
12. (Facultatif) Pour obtenir des mises à jour en temps réel de Jira dans Miro, cochez **Créer un webhook automatiquement**.
    > *✏️ Vous pouvez ajouter le webhook manuellement plus tard.*
13. Cliquez sur **Connecter**.
14. Suivez le flux d'authentification pour votre serveur d'autorisation. Si vous y êtes invité, connectez-vous à votre environnement.
    Lorsque votre connexion est terminée, votre instance Jira est répertoriée sous **Instances connectées** avec l'étiquette suivante : **Serveur d’authentification**.

## Assurez-vous que votre équipe puisse s'authentifier

Maintenant que vous avez connecté votre instance Jira au niveau de l'organisation, vous pouvez commencer à utiliser Jira au niveau de l'équipe.

1. Sur votre tableau de bord Miro, sélectionnez votre avatar en haut à droite et allez à **Console d’administration**.
2. Sélectionnez **Équipes** > **Votre équipe**.
   Le curseur **Votre équipe** s'ouvre.
3. Sélectionnez l'onglet **Applications**.
4. Dans la liste des applications, sélectionnez **cartes Jira**.
5. Sous **Paramètres d'administration**, vérifiez si votre configuration Jira affiche l'étiquette **CONNEXION GLOBALE**, et affiche l'URL correcte de l'instance Jira, puis faites l'une des actions suivantes :
   - Si c'est le cas, vous avez terminé cette procédure. Vous pouvez passer à [Et ensuite ?](https://help.miro.com/hc/articles/25699264170386)
   - Si non, sélectionnez **Modifier la configuration** > **Paramètres généraux de l’organisation** > **votre instance Jira**.
6. Sélectionner **Enregistrer les paramètres**.

## Et ensuite ?

Chaque membre de l'équipe doit autoriser son compte utilisateur. Pour s'assurer que chaque utilisateur obtienne des jetons d'accès et de rafraîchissement, lorsqu'un membre de l'équipe tente d'effectuer une action liée à Jira sur un tableau Miro, il sera invité à autoriser son compte.

## FAQ

**Quels serveurs d’autorisation puis-je utiliser ?**

Vous pouvez utiliser n'importe quel serveur d'autorisation qui prend en charge les protocoles standard OAuth 2.0 pour les environnements sur site. Par exemple, Azure Active Directory (Entra ID) et Okta.

**Puis-je utiliser le même serveur d'autorisation pour plusieurs organisations ?**

Oui, mais vous devez ajouter manuellement le serveur à chaque organisation.

**Puis-je mettre à jour le secret client pour un serveur d’autorisation&nbsp;?**

Non. Si vous devez changer le secret du client, vous devez alors déconnecter et reconnecter votre instance.

**Les admins de l'organisation et d'équipe peuvent-ils encore utiliser l'autorisation native dans Jira ?**

Oui. Selon la configuration sélectionnée, les administrateurs peuvent continuer à utiliser le processus d'autorisation natif dans Jira.

**Que se passe-t-il si une équipe est déjà connectée à une autre instance Jira ?**

Vous pouvez mettre à jour les équipes de votre organisation avec les [paramètres Jira par défaut](https://help.miro.com/hc/articles/26438407676434).

**Miro contrôle-t-il le mappage entre les utilisateurs autorisés et les utilisateurs Jira ?**

Non. La cartographie entre les utilisateurs autorisés et les utilisateurs Jira relève de la responsabilité de l'environnement client via leur passerelle API. Miro ne contrôle pas cette passerelle.

**Comment savoir si OAuth 2.0 via un serveur d'autorisation tiers est la bonne solution pour mon organisation ?**

Si toutes les conditions suivantes sont remplies, alors OAuth 2.0 via un serveur d'autorisation tiers est une bonne option :

- Votre instance Jira est hébergée sur vos serveurs.
- L'accès externe à Jira n'est possible qu'avec une passerelle API.
- La passerelle API applique l'autorisation en utilisant un serveur d'autorisation personnalisé.
- Vous devez connecter Miro à Jira sans exposer l'URL de base publique de Jira.

**Quel problème cette solution résout-elle ?**

Cette solution est conçue pour les organisations qui hébergent Jira en interne et acheminent le trafic API externe via une passerelle API. Dans cette configuration, Jira n'est pas accessible au public et l'accès est contrôlé via un serveur d'autorisation personnalisé. Au lieu d'avoir une URL de base publique pour Jira, cette solution vous permet de connecter vos instances Jira sur site en configurant Miro pour s'authentifier via votre propre serveur d'autorisation.
