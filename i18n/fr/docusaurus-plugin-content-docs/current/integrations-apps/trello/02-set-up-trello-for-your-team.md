---
title: "Configurer Trello pour votre \xE9quipe"
article_id: 30634093325842
translation_id: 30634093325842
locale: fr
sidebar_position: 2
created_at: '2025-10-29T15:59:48Z'
updated_at: '2026-02-23T11:40:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

L'intégration de Trello est techniquement mise en œuvre via une API REST. Pour l'authentification et l'autorisation, l'intégration utilise le protocole standard de l'industrie OAuth 2.0. Un élément clé de cette architecture est l'utilisation d'une plateforme API unifiée en tant que sous-traitant pour les données tierces. Cette plateforme fournit des API unifiées responsables de l'authentification, de la normalisation et de la synchronisation des données entre divers fournisseurs d'API.

## Flux de données

Une compréhension approfondie du flux de données est primordiale pour gérer la sécurité et la conformité au sein de votre organisation.

### Diagramme de séquence de haut niveau

Création d'un widget de carte Trello

![Trello (BETA) 2.jpg](images/30634984722578_Trello%20(BETA) 2.jpg)

Mise à jour d’un widget de carte Trello

![Trello (BETA) 2.jpg](images/30634984722578_Trello%20(BETA) 2.jpg)

### Données Trello dans Miro

Lorsque les utilisateurs importent des cartes Trello sur un tableau Miro, les données pertinentes des cartes deviennent partie intégrante des données du canevas Miro. Miro stocke les points de données spécifiques suivants pour les cartes importées, à condition qu'ils soient disponibles dans Trello :

- Titre
- Description
- Membres (y compris les noms d'utilisateur et les e-mails)
- Liste
- Badges

L'énumération explicite des types de données stockées est cruciale pour la gouvernance des données organisationnelles et la conformité. Elle permet aux administrateurs d'évaluer précisément quelles informations, notamment les données potentiellement sensibles, sont répliquées dans l'environnement Miro. Cette transparence garantit l'alignement avec les politiques internes de gestion des données de leur organisation. Il est également à noter que, conformément à la section "Limitations", les champs personnalisés ne sont pas pris en charge et donc non stockés, un détail clé pour la cartographie des données et les évaluations de conformité. Miro utilise une approche hybride pour le stockage des données, minimisant celles stockées directement sur le widget de carte et récupérant des détails supplémentaires lorsque l'utilisateur ouvre la vue de modification.

### Conservation des données stockées chez Miro

Toutes les données importées de Trello qui sont stockées dans Miro adhèrent strictement à la politique de conservation des données de Miro. Cette politique est appliquée uniformément à toutes les données clients, assurant une approche cohérente de la gestion du cycle de vie des données.

## Authentification et autorisation

L'intégration Trello initie un flux d'authentification lorsque l'utilisateur interagit pour la première fois avec l'intégration. L'autorisation au sein de Trello est gérée par le service d'intégration. Pour chaque utilisateur individuel, Miro établit un compte avec le service d'intégration, et ces identifiants sont ensuite utilisés pour toutes les interactions utilisateur avec l'intégration.

L'intégration nécessite généralement l'approbation d'un administrateur Trello pour autoriser l'application d'intégration au sein de l'écosystème de leur organisation. De plus, les utilisateurs individuels doivent également autoriser l'intégration Trello de Miro via la page d'autorisation OAuth de Trello lors de leur première tentative d'intégrer un lien Trello.

### Portées d'autorisation requises

La portée d'autorisation peut varier en fonction du système tiers spécifique. Cependant, pour les intégrations de gestion de cartes comme Trello, Miro exige généralement l'accès aux données suivantes :

| Portée | Description |
| --- | --- |
| Cartes (lecture et écriture) | Octroie à l'intégration l'autorisation de lire les cartes existantes et de créer ou modifier des cartes dans Trello. |
| Utilisateurs (lecture) | Octroie à l'intégration l'autorisation de lire les informations utilisateur dans Trello, généralement pour assigner des cartes ou afficher les noms des membres. |
| Collections (lecture) | Octroie à l'intégration l'autorisation de lire les collections, tableaux et listes dans Trello. |

### Que est stocké dans Miro et comment

Miro stocke de manière sécurisée les données liées à l'autorisation et au dépliage pour l'intégration Trello :

- **Données liées à l'autorisation :** Cela comprend les jetons d'accès et les valeurs de jetons d'actualisation, qui sont stockés dans la base de données de Miro pour une durée limitée de plusieurs jours. Ces jetons sont automatiquement actualisés à l'expiration en utilisant le jeton d'actualisation pour garantir un accès continu. Toutes les données stockées dans la base de données pour cette intégration sont chiffrées à l'aide de la norme de cryptage avancée 256 bits, offrant un niveau de sécurité des données robuste.
- **Données liées au déploiement :** Cela inclut les titres des cartes, qui sont stockés en tant que partie intégrante des tableaux Miro eux-mêmes. De plus, les titres et les références chiffrées à ces éléments sont stockés dans un service interne, sécurisés davantage par chiffrement (gestion des clés de chiffrement).

### Révocation d'un jeton

Si nécessaire, les administrateurs ou les utilisateurs individuels peuvent révoquer les jetons accordés à l'intégration Trello. Les utilisateurs peuvent accéder aux paramètres de l'intégration en ouvrant le sélecteur de carte d'intégrations, en cliquant sur le menu à trois points en haut à droite et en sélectionnant **Paramètres de l'intégration**, ou en accédant à l'onglet **Applications** de l'équipe dans les paramètres de l'équipe Miro, en trouvant l'intégration spécifique et en cliquant dessus. Sur la page des paramètres, l'autorisation peut être révoquée en cliquant sur le bouton **Déconnecter**. Suite à cette action, Miro révoquera l'accès à Trello et supprimera le compte utilisateur associé. Pour la désinstallation au niveau de l'équipe, les administrateurs peuvent suivre les étapes spécifiques décrites dans la section « Dépannage et FAQ (Admin) ».

## Comment configurer l'intégration Trello

Le processus d'intégration Miro + Trello se compose d'étapes distinctes pour les administrateurs et les utilisateurs finaux, garantissant un déploiement contrôlé au sein d'une organisation.

1. **Assurez-vous que les comptes sont actifs :** Avant de commencer l'installation, assurez-vous que des comptes Miro et Trello actifs sont disponibles.
2. **Installation au niveau de l'équipe (Action de l'admin) :**
   - Les administrateurs peuvent avoir besoin d'autoriser explicitement l'intégration Trello pour leur équipe Miro. Les membres de l'équipe peuvent seulement utiliser l'intégration si elle a été installée au niveau de l'équipe.
   - Un administrateur d'équipe Miro peut installer directement l'application en ouvrant un tableau Miro, en sélectionnant **Outils Média & Intégrations (+)**, en recherchant "Trello", et en cliquant sur **Connecter** pour autoriser l'intégration. Si un administrateur d'équipe Miro effectue cette action, l'application sera automatiquement autorisée et installée sans nécessiter d'approbation administrative supplémentaire.
3. **Flux de demande utilisateur et approbation admin (si applicable) :**
   - Dans les organisations où un consentement administratif strict est requis, un utilisateur non-admin d'une équipe Miro configurée pour l'intégration Trello peut coller un lien Trello sur un tableau Miro. Cette action pourrait déclencher un dialogue de "demande d'installation d'application" pour l'utilisateur, l'incitant à demander une approbation administrative.
   - Les admins désignés peuvent alors examiner et approuver cette demande en attente à travers leurs consoles administratives Miro ou Trello, en fonction du flux de consentement spécifique configuré.
4. **Connexion utilisateur individuel :**
   - Une fois l'intégration installée et autorisée au niveau de l'équipe par un administrateur, les utilisateurs individuels cliqueront sur **Connecter** sur le widget Trello qui apparaît sur le tableau Miro.
   - Les utilisateurs seront ensuite redirigés vers une page d'autorisation Trello où ils accorderont à Miro l'accès à leur compte Trello individuel, confirmant ainsi leur autorisation personnelle pour intégrer et interagir avec le contenu.

## Considérations de sécurité et de conformité

### Restriction d'accès au fichier source

Pour garantir que l'accès aux données Trello intégrées reste restreint aux mêmes personnes que celles du tableau Trello source, les administrateurs de l'organisation Miro doivent maintenir des contrôles stricts sur le partage des tableaux et l'export des contenus. Bien que l'intégration principale de Trello respecte les autorisations individuelles pour l'interaction en direct, toute exportation ou capture statique du contenu du tableau pourrait potentiellement exposer des données à des personnes non autorisées si le tableau Miro lui-même n'est pas géré de manière sécurisée.

### Gestion des erreurs

L'intégration est conçue avec une UI de secours élégante et une gestion des erreurs dans les cas où les mises à jour des données de carte échouent en raison d'un rejet par un tiers.

### Addendum sur le traitement des données Miro (DPA)

Pour des informations juridiques et de conformité détaillées sur les pratiques de traitement des données de Miro, les administrateurs sont invités à consulter le [Complément de traitement des données de Miro](https://miro.com/legal/customer-data-processing-addendum/).

## Dépannage & FAQ

### Comment désactiver l'intégration (désinstallation au niveau de l'équipe) ?

Un administrateur d'équipe Miro peut désinstaller l'intégration Trello au niveau de l'équipe. Cette action désactive l'intégration pour tous les membres de l'équipe. Pour ce faire, accédez à **Paramètres de l'équipe Apps & Intégrations**. Trouvez "Trello" ou "Gestion des cartes Trello" dans la liste des applications installées, faites défiler vers le bas, puis cliquez sur **Désinstaller pour l'équipe**.

### Comment désactiver l'intégration (désinstallation individuelle) ?

Les utilisateurs individuels peuvent désinstaller l'intégration pour eux-mêmes. Accédez à **Applications & intégrations** dans vos paramètres Miro. Localisez "Trello" ou "Gestion de cartes Trello" et cliquez sur **Désinstaller pour moi**.

### Quels administrateurs peuvent installer l'intégration Trello pour leur équipe ?

Seuls les administrateurs d'équipe Miro peuvent installer directement l'application. Si un administrateur d'équipe Miro colle une URL Trello sur un tableau Miro, l'application sera automatiquement autorisée et installée sans nécessiter d'action supplémentaire.

### Quelles sont les conditions de disponibilité pour l'intégration Trello ?

L'intégration Trello est disponible pour les forfaits Business et Enterprise de Miro.

### Les administrateurs doivent-ils autoriser l'intégration Trello pour leur équipe ?

Oui, les administrateurs peuvent devoir autoriser l'intégration de Trello pour leur équipe Miro. Les membres de l'équipe ne peuvent utiliser l'intégration Trello que si elle a été installée au niveau de l'équipe.
