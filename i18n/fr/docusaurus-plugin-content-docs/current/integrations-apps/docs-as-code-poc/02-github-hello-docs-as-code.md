---
title: '[GitHub] Bonjour, documents comme du code !'
article_id: 29239655610258
translation_id: 29239655610258
locale: fr
sidebar_position: 2
created_at: '2025-09-04T17:11:12Z'
updated_at: '2026-01-23T15:01:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Cette section fournit des détails techniques et administratifs complets, essentiels pour les professionnels de l'IT et de la sécurité responsables du déploiement, de la sécurité et de la gestion continue de l'intégration Trello au sein de leur organisation.

## Vue d'ensemble technique

L'intégration Trello est techniquement mise en œuvre par le biais d'une API REST. Pour l'authentification et l'autorisation, l'intégration utilise le protocole OAuth 2.0, reconnu dans l'industrie comme norme. Un composant clé de cette architecture est l'utilisation d'une plateforme API unifiée en tant que sous-processeur pour les données tierces. Cette plateforme fournit des API unifiées chargées d'authentifier, de normaliser et de synchroniser les données à travers divers fournisseurs d'API.

## Flux de données

Une compréhension approfondie du flux de données est essentielle pour gérer la sécurité et la conformité au sein de votre organisation.

### Diagramme de séquence haut niveau

Créer un widget de carte Trello

![image (7).png](images/32777076293650_image%20(7).png)

Mettre à jour un widget de carte Trello

![image (8).png](images/32777120530578_image%20(8).png)

### Données Trello dans Miro

Lorsque les utilisateurs importent des cartes Trello sur un tableau Miro, les données pertinentes de la carte deviennent une partie intégrante des données du canevas Miro. Miro stocke les points de données spécifiques suivants pour les cartes importées, à condition qu'ils soient disponibles dans Trello :

- Titre
- Description
- Membres (y compris noms d'utilisateurs et e-mails)
- Liste
- Badges

L'énumération explicite des types de données stockées est cruciale pour la gouvernance des données organisationnelles et la conformité. Elle permet aux administrateurs d'évaluer avec précision quelles informations, notamment les données potentiellement sensibles, sont répliquées dans l'environnement Miro. Cette transparence garantit l'alignement avec les politiques internes de gestion des données de l'organisation. Il est également à noter que, comme indiqué dans la section "Limitations", les champs personnalisés ne sont pas pris en charge et ne sont donc pas stockés, ce qui est un point clé pour la cartographie des données et l'évaluation de la conformité. Miro adopte une approche hybride du stockage des données, minimisant les données stockées directement sur le widget de la carte et récupérant des détails supplémentaires lorsque l'utilisateur ouvre le mode de modification.

### Conservation des données stockées chez Miro

Toutes les données Trello importées et stockées dans Miro respectent strictement la politique de conservation des données standard de Miro. Cette politique est appliquée de manière cohérente à toutes les données des clients, garantissant une approche uniforme de la gestion du cycle de vie des données.

## Authentification et autorisation

L'intégration Trello initie un flux d'authentification lorsque qu'un utilisateur interagit pour la première fois avec l'intégration. L'autorisation au sein de Trello est gérée par le service d'intégration. Pour chaque utilisateur, Miro établit un compte avec le service d'intégration, et ces identifiants sont ensuite utilisés pour toutes les interactions de l'utilisateur avec l'intégration.

L'intégration nécessite généralement l'approbation d'un administrateur Trello pour autoriser l'application d'intégration dans l'écosystème de leur organisation. De plus, les utilisateurs individuels doivent également autoriser l'intégration Miro Trello via la page d'autorisation OAuth de Trello lorsqu'ils tentent pour la première fois d'intégrer un lien Trello.

### Portées d'autorisation requises

La portée d'autorisation peut varier en fonction du système tiers spécifique. Cependant, pour les intégrations de gestion de cartes comme Trello, Miro nécessite généralement l'accès aux données suivantes :

| Portée | Description |
| --- | --- |
| Cartes (lecture et écriture) | Accorde à l'intégration l'autorisation de lire les cartes existantes et de créer ou modifier des cartes dans Trello. |
| Membres (lecture) | Accorde à l'intégration l'autorisation de lire les informations des membres dans Trello, généralement pour l'assignation de cartes ou l'affichage des noms des membres. |
| Badges (lecture) | Accorde à l'intégration l'autorisation de lire les badges associés aux cartes dans Trello. |
| Tableaux (lecture) | Accorde à l'intégration l'autorisation de lire les informations des tableaux et des listes dans Trello. |

### Ce qui est stocké dans Miro et comment

Miro stocke en toute sécurité à la fois les données liées à l'autorisation et celles liées au déploiement pour l'intégration Trello :

- **Données liées à l'autorisation :** Cela comprend les jetons d'accès et les valeurs de jetons de rafraîchissement, qui sont stockés dans la base de données de Miro pour une durée limitée de plusieurs jours. Ces jetons sont automatiquement renouvelés à leur expiration à l'aide du jeton de rafraîchissement pour garantir un accès continu. Toutes ces données stockées dans la base de données pour cette intégration sont cryptées à l'aide de l'Advanced Encryption Standard 256 bits, fournissant une couche robuste de sécurité des données.
- **Données liées au déploiement :** Cela inclut les titres des cartes, qui sont stockés en tant que partie des tableaux Miro eux-mêmes. De plus, les titres et les références chiffrées à ces éléments sont stockés dans un service interne, sécurisé en outre par un cryptage (gestion des clés de chiffrement).

### Révoquer un jeton

En cas de nécessité, les administrateurs ou les utilisateurs individuels peuvent révoquer les jetons accordés à l'intégration Trello. Les utilisateurs peuvent accéder aux paramètres d'intégration soit en ouvrant un sélecteur de carte d'intégrations, en cliquant sur le menu à trois points en haut à droite et en sélectionnant **Paramètres d'intégration**, soit en accédant à l'onglet **Applications** dans les paramètres de l'équipe Miro, en trouvant l'intégration spécifique et en cliquant dessus. Sur la page des paramètres, l'autorisation peut être révoquée en cliquant sur le bouton **Déconnecter**. Suite à cette action, Miro révoquera l'accès à Trello et supprimera le compte associé de l'utilisateur. Pour désinstaller au niveau de l'équipe, les administrateurs peuvent suivre les étapes spécifiques décrites dans la section "Dépannage & FAQs (Admin)".

## Comment configurer l'intégration Trello

Le processus d'installation de l'intégration Miro + Trello implique des étapes distinctes pour les administrateurs et les utilisateurs, assurant un déploiement contrôlé au sein d'une organisation.

1. **Assurez-vous que les comptes sont actifs :**  Avant de commencer l'installation, vérifiez que des comptes actifs pour Miro et Trello sont disponibles.
2. **Installation au niveau de l’équipe (Action d’admin) :**
   - Les admins peuvent avoir besoin d’autoriser explicitement l’intégration Trello pour leur équipe Miro. Les membres de l’équipe ne peuvent utiliser l’intégration que si elle a été installée au niveau de l’équipe.
   - Un admin de l’équipe Miro peut installer directement l’application en ouvrant un tableau Miro, en sélectionnant **Outils Médias & Intégrations (+)**, en recherchant "Trello", puis en cliquant sur **Connecter** pour autoriser l’intégration. Si un admin de l’équipe Miro effectue cette action, l’application sera automatiquement autorisée et installée sans nécessiter d’approbation administrative supplémentaire.
3. **Processus de demande utilisateur et d'approbation admin (si applicable) :**
   - Dans les organisations où un consentement administratif strict est requis, un utilisateur non-admin d'une équipe Miro configurée pour l'intégration Trello peut coller un lien Trello sur un tableau Miro. Cette action peut déclencher une boîte de dialogue "demande d'installation de l'application" pour l'utilisateur, l'incitant à solliciter l'approbation administrative.
   - Les administrateurs désignés peuvent alors examiner et approuver cette demande en attente via leurs consoles administratives Miro ou Trello, en fonction du flux de consentement spécifique configuré.
4. **Connexion de l'utilisateur individuel :**
   - Une fois l'intégration installée et autorisée au niveau de l'équipe par un administrateur, les utilisateurs individuels cliqueront sur **Connecter** sur le widget Trello qui apparaît sur le tableau Miro.
   - Les utilisateurs seront alors redirigés vers une page d'autorisation Trello où ils accorderont à Miro l'accès à leur compte Trello individuel, confirmant ainsi leur autorisation personnelle pour intégrer et interagir avec le contenu.

## Considérations de sécurité et de conformité

### Restriction d'accès au fichier source

Pour s'assurer que l'accès aux données Trello intégrées reste limité aux mêmes individus que sur le tableau Trello source, les administrateurs de l'organisation Miro doivent maintenir un contrôle strict sur le partage des tableaux et l'export de contenu. Bien que l'intégration principale de Trello respecte les permissions individuelles pour une interaction en direct, toute exportation ou capture statique du contenu du tableau pourrait potentiellement exposer les données à des personnes non autorisées si le tableau Miro lui-même n'est pas géré de manière sécurisée.

### Gestion des erreurs

L'intégration est conçue avec une interface utilisateur à récupération élégante et une gestion des erreurs dans les cas où les mises à jour des données des cartes échouent en raison du rejet par des tiers.

### Ajout à l'accord de traitement des données de Miro (DPA)

Pour des détails complets sur les aspects légaux et de conformité des pratiques de traitement des données de Miro, les administrateurs sont invités à consulter le [Miro Data Processing Addendum](https://miro.com/legal/customer-data-processing-addendum/).

## Dépannage & FAQs

### Comment désactiver l'intégration (désinstallation au niveau de l'équipe) ?

Un administrateur d'équipe Miro peut désinstaller l'intégration Trello au niveau de l'équipe. Cette action désactive l'intégration pour tous les membres de l'équipe. Pour ce faire, accédez à **Paramètres de l'équipe - Applications & Intégrations**. Trouvez "Trello" ou "Gestion des cartes Trello" dans la liste des applications installées, descendez et cliquez sur **Désinstaller pour l'équipe**.

### Comment désactiver l'intégration (désinstallation individuelle) ?

Les utilisateurs peuvent désinstaller l'intégration pour eux-mêmes. Rendez-vous dans **Applications et intégrations** dans vos réglages Miro. Trouvez "Trello" ou "Gestion des cartes Trello" et cliquez sur **Désinstaller pour moi**.

### Quels administrateurs peuvent installer l'intégration Trello pour leur équipe ?

Seuls les administrateurs d'équipe Miro peuvent installer directement l'application. Si un administrateur d'équipe Miro colle une URL Trello sur un tableau Miro, l'application sera automatiquement autorisée et installée sans nécessiter d'action supplémentaire.

### Quelles sont les exigences de disponibilité pour l'intégration Trello ?

L'intégration Trello est disponible pour les forfaits Business et Enterprise de Miro. API REST

### Les administrateurs doivent-ils autoriser l'intégration Trello pour leur équipe ?

Oui, les administrateurs peuvent avoir besoin d'autoriser l'intégration Trello pour leur équipe Miro. Les membres de l'équipe ne peuvent utiliser l'intégration Trello que si elle a été installée au niveau de l'équipe.
