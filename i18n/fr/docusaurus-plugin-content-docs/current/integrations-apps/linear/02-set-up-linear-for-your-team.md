---
title: "Configurer Linear (b\xEAta) pour votre \xE9quipe"
article_id: 30630697364626
translation_id: 30630697364626
locale: fr
sidebar_position: 2
created_at: '2025-10-29T14:09:41Z'
updated_at: '2026-02-23T11:23:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

L’intégration Linear est techniquement mise en œuvre via une API REST. Pour l'authentification et l'autorisation, elle utilise le protocole standard de l'industrie OAuth 2.0. Un composant central de cette architecture est une plateforme API unifiée utilisée comme sous-traitant pour les données tierces — gérant l'authentification, la normalisation et la synchronisation entre différents fournisseurs d'API.

## Flux de données

Comprendre le flux de données est crucial pour gérer la sécurité et la conformité.

### Diagramme de séquence de haut niveau

Créer un widget de carte Linear

![Asana Cards (BETA) (1).jpg](images/30631672805522_Asana%20Cards%20(BETA) (1).jpg)

Mettre à jour un widget de carte Linear

![Asana Cards (BETA) (1).jpg](images/30631672805522_Asana%20Cards%20(BETA) (1).jpg)

### Données Linear dans Miro

Lorsque les utilisateurs importent des tickets Linear dans un tableau Miro, les données suivantes sont intégrées au canevas Miro :

- Titre
- Description
- Attributaire (nom/e-mail)
- État
- Priorité

Cette énumération est essentielle pour la gouvernance des données, confirmant quelles données sensibles entrent dans l'environnement Miro. Notez que les champs personnalisés ne sont pas pris en charge.

### Conservation des données

Toutes les données importées de Linear respectent strictement la politique standard de conservation des données de Miro, appliquée de manière cohérente à toutes les données clients.

## Authentification et autorisation

Lors de la première interaction, l'intégration de Linear initie un flux d'authentification. Pour chaque utilisateur, Miro crée des identifiants avec le service d'intégration pour les interactions ultérieures.

L'intégration nécessite généralement l'approbation d'un administrateur Linear.

### Champs d'autorisation requis

| Portée | Description |
| --- | --- |
| Collections | Accéder aux collections de tickets. |
| Utilisateurs | Lire les informations des utilisateurs pour l'assignation/affichage. |
| Tickets | Lire, créer, modifier des tickets dans Linear. |

## Qu'est-ce qui est stocké dans Miro et comment

- **Données liées à l’autorisation :** Les jetons sont stockés dans la base de données de Miro pendant plusieurs jours, chiffrés avec AES-256.
- **Données liées au déploiement :** Les titres des tickets sont stockés avec des références chiffrées.

### Révocation d'un jeton

La révocation des jetons peut se faire via les onglets **Paramètres d’intégration** ou **Applications** en sélectionnant **Déconnecter**. Cette action supprime l'accès à Linear et efface les identifiants.

## Comment configurer l’intégration Linear

Des étapes pour les administrateurs et les utilisateurs finaux garantissent un déploiement contrôlé.

1. **Assurez-vous que les comptes sont actifs :** les comptes Miro et Linear doivent être actifs.
2. **Installation au niveau de l’équipe (Action admin) :**
   - Les administrateurs doivent autoriser l'intégration de Linear au niveau de l'équipe.
   - Installation via **Outils médias et intégrations**, en recherchant "Linear" et en connectant.
3. **Demande utilisateur et approbation par un admin :**
   - Dans les organisations à consentement strict, coller un lien Linear peut déclencher une demande d'approbation par un admin.
   - Les admins peuvent approuver via les consoles Miro ou Linear.
4. **Connexion utilisateur individuelle :**
   - Les utilisateurs se connectent via le widget Linear et l'autorisation OAuth.

## Sécurité et conformité

### Restriction d'accès au fichier source

Le maintien de contrôles stricts de partage de tableau aligne les permissions Linear avec Miro.

### Gestion des erreurs

L'intégration dispose d'un retour à l'interface utilisateur élégant en cas de rejet par des tiers.

### Addendum de traitement des données de Miro (DPA)

Consultez [l'Addendum de traitement des données de Miro](https://miro.com/legal/customer-data-processing-addendum/) pour des informations détaillées sur les aspects légaux et la conformité.

## Résolution des problèmes & FAQs

### Comment désactiver l'intégration (Niveau d'équipe)

Les administrateurs peuvent désinstaller à partir de **Paramètres de l'équipe Applications & Intégrations** en sélectionnant "Linear" et en cliquant sur **Désinstaller pour l'équipe**.

### Comment désactiver l'intégration (Individuel)

Les utilisateurs peuvent se rendre sur **Applications & Intégrations** et sélectionner "Désinstaller pour moi" pour Linear.

### Permissions de l'administrateur

Seuls les administrateurs de l'équipe Miro peuvent installer l'application directement. Les installations automatiques se produisent lors du collage d'une URL Linear sur un tableau.

### Exigences de disponibilité

L'intégration Linear est disponible pour les forfaits Business et Enterprise.

### Exigence d'autorisation de l'administrateur

Oui, une autorisation au niveau de l'équipe par les administrateurs est nécessaire pour l'accès de l'équipe.
