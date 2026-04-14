---
title: "Configurer Asana pour votre \xE9quipe"
article_id: 28252196453778
translation_id: 28252196453778
locale: fr
sidebar_position: 2
created_at: '2025-07-22T13:30:20Z'
updated_at: '2026-02-20T09:00:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Cette section fournit des détails techniques et administratifs complets, essentiels pour les professionnels de l'informatique et de la sécurité responsables du déploiement, de la sécurité et de la gestion continue de l'intégration Asana au sein de leur organisation.

## Aperçu technique

L'intégration Asana est techniquement mise en œuvre via une API REST. À des fins d'authentification et d'autorisation, l'intégration utilise le protocole OAuth 2.0, qui est un standard de l'industrie. Un élément clé de cette architecture est l'utilisation d'une plateforme API unifiée en tant que sous-traitant de données tierces. Cette plateforme fournit des API unifiées qui sont responsables de l'authentification, de la normalisation et de la synchronisation des données entre divers fournisseurs d'API.

## Flux de données

Une compréhension approfondie du flux de données est essentielle pour gérer la sécurité et la conformité au sein de votre organisation.

### Diagramme de séquence général

Création d'une carte Asana

![image (7).png](images/30597105764498_image%20(7).png)

Mise à jour d'une carte Asana

![image (8).png](images/30597084630930_image%20(8).png)

### Données Asana dans Miro

Lorsque les utilisateurs importent des tâches Asana sur un tableau Miro, les données pertinentes des tâches deviennent partie intégrante des données du canevas Miro. Miro stocke les points de données spécifiques suivants pour les tâches importées, à condition qu'ils soient disponibles dans Asana :

- Titre
- Description
- Attributaire (y compris le nom et/ou l'e-mail de l'utilisateur)
- État
- Priorité

L'énumération explicite des types de données stockées est cruciale pour la gouvernance des données organisationnelles et la conformité. Elle permet aux administrateurs d'évaluer avec précision quelles informations, notamment celles potentiellement sensibles, sont répliquées dans l'environnement Miro. Cette transparence garantit l'alignement sur les politiques internes de gestion des données de leur organisation. Il est également à noter que, comme mentionné dans la section "Limitations", les champs personnalisés ne sont pas pris en charge et ne sont donc pas stockés, ce qui est un détail clé pour la cartographie des données et les évaluations de conformité. Miro utilise une approche hybride du stockage des données, minimisant les données stockées directement sur le widget carte et récupérant des détails supplémentaires lorsque l'utilisateur ouvre la vue de modification.

### Conservation des informations stockées chez Miro

Toutes les données importées d'Asana qui sont stockées dans Miro respectent strictement la politique standard de conservation des données de Miro. Cette politique est appliquée de manière homogène à toutes les données des clients, garantissant une approche uniforme de la gestion du cycle de vie des données.

## Authentification et autorisation

L'intégration Asana déclenche un flux d'authentification lorsque l'utilisateur interagit pour la première fois avec l'intégration. L'autorisation au sein d'Asana est gérée par le service d'intégration. Pour chaque utilisateur individuel, Miro établit un compte avec le service d'intégration, et ces identifiants sont ensuite utilisés pour toutes les interactions de l'utilisateur avec l'intégration.

L'intégration nécessite généralement l'approbation d'un administrateur Asana (ou d'un administrateur Microsoft Entra, si Asana est géré via Azure AD) pour autoriser l'application d'intégration au sein de l'écosystème de leur organisation. De plus, les utilisateurs individuels doivent également autoriser l'intégration Miro Asana via la page d'autorisation OAuth d'Asana lorsqu'ils tentent pour la première fois d'intégrer un lien Asana.

### Autorisations requises

Le champ d'autorisation peut varier en fonction du système tiers spécifique. Cependant, pour les intégrations de billetterie comme Asana, Miro nécessite généralement l'accès aux données suivantes :

| Portée | Description |
| --- | --- |
| Billets (lecture et écriture) | Octroie à l'intégration la permission de lire les tâches existantes et de créer ou modifier des tâches dans Asana. |
| Utilisateurs (lecture) | Octroie à l'intégration la permission de lire les informations des utilisateurs dans Asana, généralement pour assigner des tâches ou afficher les noms des personnes assignées. |
| Étiquettes (lecture) | Accorde à l'intégration la permission de lire les étiquettes associées aux tâches dans Asana. |
| Collections (lecture) | Accorde à l'intégration la permission de lire les collections de tâches ou de projets dans Asana. |

### Qu'est-ce qui est stocké dans Miro et comment

Miro stocke de manière sécurisée des données liées à l'autorisation et au déploiement pour l'intégration Asana :

- **Données liées à l'autorisation :** Cela comprend les jetons d'accès et les valeurs de jetons d'actualisation, qui sont stockés dans la base de données de Miro pour une durée limitée de plusieurs jours. Ces jetons sont automatiquement actualisés à expiration grâce au jeton d'actualisation afin d'assurer un accès continu. Toutes les données stockées dans la base de données pour cette intégration sont cryptées en utilisant la norme de chiffrement avancé 256 bits, offrant une couche robuste de sécurité des données.
- **Données liées au déploiement :** Cela inclut les titres des tâches, qui sont stockés dans les tableaux Miro eux-mêmes. De plus, les titres et les références chiffrées à ces éléments sont stockés dans un service interne, encore sécurisé grâce à la gestion des clés de chiffrement (EKM).

### Révoquer un jeton

Si nécessaire, les administrateurs ou les utilisateurs individuels peuvent révoquer les jetons accordés à l'intégration Asana. Les utilisateurs peuvent accéder aux paramètres de l'intégration soit en ouvrant le sélecteur de tâches d'intégration, en cliquant sur le menu à trois points en haut à droite et en sélectionnant **Paramètres d'intégration**, soit en accédant à l'onglet **Apps** de l'équipe dans les paramètres de l'équipe Miro, en trouvant l'intégration spécifique et en cliquant dessus. Sur la page des paramètres, l'autorisation peut être révoquée en cliquant sur le bouton **Déconnecter**. Suite à cette action, Miro révoquera l'accès à Asana et supprimera le compte associé de l'utilisateur. Pour la désinstallation au niveau de l'équipe, les administrateurs peuvent suivre les étapes spécifiques décrites dans la section « Dépannage et FAQ (Admin) ».

## Comment configurer l’intégration Asana

Le processus d'installation de l'intégration Miro + Asana implique des étapes distinctes pour les administrateurs et les utilisateurs finaux, garantissant un déploiement contrôlé au sein d'une organisation.

1. **Assurez-vous d'avoir des comptes actifs :** Avant de commencer l'installation, assurez-vous que des comptes Miro et Asana actifs sont disponibles.
2. **Installation au niveau de l'équipe (Action de l’admin) :**
   - Les admins peuvent avoir besoin d’autoriser explicitement l’intégration Asana pour leur équipe Miro. Les membres de l’équipe ne peuvent utiliser l’intégration que si elle a été installée au niveau de l’équipe.
   - Un admin de l’équipe Miro peut installer directement l'application en ouvrant un tableau Miro, en sélectionnant **Outils Médias & Intégrations (+)**, en recherchant "Asana" et en cliquant sur **Connecter** pour autoriser l’intégration. Si un admin de l’équipe Miro effectue cette action, l'application sera automatiquement autorisée et installée sans nécessiter d'approbation administrative supplémentaire.
3. **Flux de demande utilisateur et approbation par l'admin (si applicable) :**
   - Dans les organisations où un consentement administratif strict est requis, un utilisateur non-admin au sein d'une équipe Miro configurée pour l'intégration Asana peut coller un lien Asana sur un tableau Miro. Cette action peut déclencher une boîte de dialogue « demande d’installation de l’appli » pour l’utilisateur, l'incitant à demander l'approbation de l'administration.
   - Les administrateurs désignés peuvent ensuite examiner et approuver cette demande en attente via leurs consoles administratives Miro ou Asana, en fonction du flux de consentement spécifique configuré.
4. **Connexion individuelle de l'utilisateur :**
   - Une fois l'intégration installée et autorisée avec succès au niveau de l'équipe par un administrateur, les utilisateurs individuels cliqueront sur **Connecter** dans le widget Asana qui apparaît sur le tableau Miro.
   - Les utilisateurs seront ensuite redirigés vers une page d'autorisation Asana où ils accorderont à Miro l'accès à leur compte Asana individuel, confirmant ainsi leur autorisation personnelle d'intégrer et d'interagir avec le contenu.

## Considérations de sécurité et de conformité

### Restriction d'accès au fichier source

Pour garantir que l'accès aux données intégrées d'Asana reste restreint aux mêmes individus que dans le fichier source Asana, les administrateurs de l'organisation Miro doivent maintenir un contrôle strict sur le partage et l'export du contenu des tableaux. Bien que l'intégration principale d'Asana respecte les autorisations individuelles pour l'interaction en direct, tout export ou instantané statique du contenu du tableau pourrait potentiellement exposer les données à des personnes non autorisées si le tableau Miro lui-même n'est pas géré de manière sécurisée.

### Gestion des erreurs

L'intégration est conçue avec un retour utilisateur élégant et une gestion des erreurs dans les cas où la mise à jour des données de la carte échoue en raison du rejet par des tiers.

### Addendum sur le traitement des données Miro (DPA)

Pour des détails juridiques et de conformité complets concernant les pratiques de traitement des données de Miro, les administrateurs sont invités à consulter le [Contrat de traitement des données Miro](https://miro.com/legal/customer-data-processing-addendum/).

## Dépannage & FAQs

### Comment désactiver l'intégration (désinstallation au niveau de l'équipe) ?

Un administrateur d'équipe Miro peut désinstaller l'intégration Asana au niveau de l'équipe. Cette action désactive l'intégration pour tous les membres de l'équipe. Pour ce faire, allez dans **Paramètres de l'équipe Apps & Intégrations**. Trouvez "Asana Ticketing" dans la liste des applications installées, descendez et cliquez sur **Désinstaller pour l'équipe**.

### Comment désactiver l'intégration (désinstallation individuelle) ?

Les utilisateurs individuels peuvent désinstaller l'intégration pour eux-mêmes. Allez dans **Applications & Intégrations** dans vos paramètres Miro. Recherchez "Asana Ticketing" et cliquez sur **Désinstaller pour moi**.

### Quels administrateurs peuvent installer l'intégration Asana pour leur équipe ?

Seuls les administrateurs d'équipes Miro peuvent installer directement l'application. Si un administrateur d'équipe Miro colle une URL Asana sur un tableau Miro, l'application sera automatiquement autorisée et installée sans nécessiter d'autres actions.

### Quelles sont les exigences de disponibilité pour l'intégration Asana ?

L'intégration Asana est disponible pour les forfaits Business et Enterprise de Miro.

### Les administrateurs doivent-ils autoriser l'intégration Asana pour leur équipe ?

Oui, les administrateurs peuvent avoir besoin d'autoriser l'intégration Asana pour leur équipe Miro. Les membres de l'équipe peuvent uniquement utiliser l'intégration Asana si elle a été installée au niveau de l'équipe.
