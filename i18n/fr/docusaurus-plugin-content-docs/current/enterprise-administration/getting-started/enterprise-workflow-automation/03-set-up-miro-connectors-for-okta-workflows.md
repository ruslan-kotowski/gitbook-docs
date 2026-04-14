---
title: Configurer les connecteurs Miro pour Okta Workflows
article_id: 8166481458706
translation_id: 8166481458706
locale: fr
sidebar_position: 2
created_at: '2022-10-19T06:52:05Z'
updated_at: '2025-02-26T11:59:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: okta-workflows
---

Les connecteurs Miro pour Okta Workflows vous permettent d’automatiser facilement les tâches administratives répétitives et à plusieurs étapes dans Miro. Découvrez comment configurer l’automatisation des workflows et simplifier la gestion des équipes et des utilisateurs.

> **Pertinent pour :** Forfait Enterprise

## Connecteur Miro User Management Connector (gestion des utilisateurs de Miro)

Le connecteur User Management (Gestion des utilisateurs) de Miro permet aux comptes Miro Entreprise pour lesquels SCIM est configuré d’ajouter des utilisateurs à leur organisation et de gérer les licences et les statuts des utilisateurs.

**Autoriser votre connecteur Miro User Management :**

Lorsque vous ajoutez une carte Miro User Management (Gestion d’utilisateur Miro) à un flux pour la première fois, une invite vous demande de configurer une connexion pour votre organisation.  Voir la section Autorisation/span>.

**Les cartes d’action du connecteur Miro User Management :**

|  |  |
| --- | --- |
| **Action** | **Description** |
| Create User (Créer un utilisateur) | Crée un nouvel utilisateur. |
| Read User (Lire un utilisateur) | Recherche un utilisateur existant dans l’organisation par adresse e-mail. |
| Upgrade User License Type to Full (Mettre à niveau la licence de l’utilisateur vers une licence complète) | Met à niveau une ressource utilisateur existante, en modifiant son type de licence utilisateur vers une licence **complète**. |
| Update User Status (Mettre à jour le statut de l'utilisateur) | Met à jour une ressource utilisateur existante, en changeant son statut actif en une valeur de true ou false.Le connecteur de gestion des utilisateurs Miro fonctionne à l'aide de votre jeton SCIM. La gestion des utilisateurs de Miro n’est disponible que pour les entreprises ayant activé le SSO et le SCIM. |

## Permission

Vous pouvez créer et gérer plusieurs connexions à partir de la page **Connexions** vous pouvez créer et gérer plusieurs connexions.
Cette fonction est utile si vous prévoyez d'opérer avec plusieurs organisations. Chaque connexion du connecteur Miro !User Management/span> ne peut pointer que vers une seule organisation Miro.

Pour activer le SCIM et obtenir un nouveau token, ou pour copier un token existant, suivez les instructions de la rubrique [Comment activer le SCIM](https://developers.miro.com/docs/how-to-enable-scim).
Pour créer une nouvelle connexion à partir d’une carte Action :

1. Cliquez sur **New Connection** (Nouvelle connexion).
2. Entrez un **Connection Nickname** (Pseudo de connexion). Nous vous recommandons de choisir un nom qui représente l’organisation.
3. Activez le provisionnement SCIM depuis [la page Miro Enterprise integration (Intégration Enterprise) en suivant ces](https://developers.miro.com/docs/how-to-enable-scim) instructions (uniquement disponibles en anglais).
   1. Copiez l’**URL de base** depuis Miro et collez-la dans le champ **Base URL** (URL de base) dans Connection (Connexion).
   2. Copiez le **jeton API** depuis Miro et collez-le dans le champ **Access Token** (Jeton d’accès) dans Connection (Connexion).
4. Cliquez sur **Create** (Créer).  Cela enregistre votre connexion et vous ramène à votre flux.

### Create user (Créer un utilisateur)

Crée un utilisateur au sein de l’organisation.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| **User Details (Détails utilisateur)** |  |  |  |
| Email (Adresse e-mail) | L’adresse e-mail de l’utilisateur. | Chaîne de caractères | VRAI |
| Active (Actif) | Statut de l’utilisateur.   - **True** (Vrai) : l’utilisateur est actif. - **False** (Faux) : l’utilisateur est inactif.    Lorsque le statut n’est pas précisé, il est **false** (faux) par défaut. | Liste déroulante | FALSE (FAUX) |
| User License Type (Type de licence utilisateur) | Type de licence de l’utilisateur.   - **Complète** - **Free**    Lorsque la licence de l’utilisateur n’est pas précisée, elle est définie selon la logique interne de Miro, qui dépend du plan de l’organisation. | Liste déroulante | FALSE (FAUX) |
| Role (Rôle) | Le rôle de l’utilisateur au sein de l’organisation.   - **Organization Member** (Membre de l’organisation) : membre standard sans privilèges d’admin. - **Organization Admin** (Admin de l’organisation) : membre doté de privilèges d’admin au niveau de l’organisation.   Lorsque le rôle de l’utilisateur n’est pas précisé, il est défini comme **Membre de l’organisation** par défaut. | Liste déroulante | FALSE (FAUX) |
| **Name (Nom)** |  |  |  |
| Family Name (Nom de famille) | Le nom de famille de l’utilisateur. | Chaîne de caractères | FALSE (FAUX) |
| Given Name (Prénom) | Le prénom de l’utilisateur. | Chaîne de caractères | FALSE (FAUX) |
| Display Name (Nom affiché) | Le nom qui sera affiché dans Miro. | Chaîne de caractères | FALSE (FAUX) |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **User (Utilisateur)** |  |  |
| User ID (ID utilisateur) | L’identifiant du nouvel utilisateur. | Chaîne de caractères |

### Read User (Lire un utilisateur)

Recherche un utilisateur existant dans l’organisation par adresse e-mail.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| **Requête** |  |  |  |
| Email (Adresse e-mail) | L'adresse e-mail de l'utilisateur à rechercher | Chaîne de caractères | VRAI |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **User (Utilisateur)** |  |  |
| User ID (ID utilisateur) | L’identifiant de l’utilisateur. | Number (Numéro) |
| User License Type (Type de licence utilisateur) | Le type de licence de l’utilisateur. | Number (Numéro) |
| Active (Actif) | Le statut de l’utilisateur.  - **True** (Vrai) : l’utilisateur est actif. - **False** (Faux) : l’utilisateur est inactif. | Number (Numéro) |
| **Name (Nom)** |  |  |
| Username (Pseudonyme) | L’adresse e-mail de l’utilisateur. | Number (Numéro) |
| Family Name (Nom de famille) | Le nom de famille de l’utilisateur. | Number (Numéro) |
| Given Name (Prénom) | Le prénom de l’utilisateur. | Number (Numéro) |
| Display Name (Nom affiché) | Le nom affiché dans Miro. | Number (Numéro) |

### Upgrade user license type to Full (Mettre à niveau la licence de l’utilisateur vers une licence complète)

Met à niveau une ressource utilisateur existante, modifiant son type de licence utilisateur vers une licence **Full** (Complète).

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| utilisateur |  |  |  |
| User ID (ID utilisateur) | L’identifiant de l’utilisateur. | Chaîne de caractères | VRAI |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Réponse** |  |  |
| Status Code (Code de statut) | Statut HTTP de la demande.  Codes indiquant que la mise à jour de la licence est réussie :   - 200. OK   Codes indiquant que la mise à jour de la licence a échoué :   - 400. 400 : Malformed request (Requête mal formée) - 401. 401 : Unauthorized (Non autorisé) - 403. 403 : Forbidden (Interdit) - 404. introuvable - 409. 409 : Conflict (Conflit) - 429. 429 : Too many requests (Trop de requêtes) | Number (Numéro) |

### Update user status (Mettre à jour le statut de l’utilisateur)

Met à jour une ressource utilisateur existante en modifiant la valeur de son **état actif** : soit vraie, soit fausse.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| utilisateur |  |  |  |
| User ID (ID utilisateur) | L’identifiant de l’utilisateur. | Chaîne de caractères | VRAI |
| Active (Actif) | Le nouveau statut de l’utilisateur.  - **True** (Vrai) : l’utilisateur est actif. - **False** (Faux) : l’utilisateur est inactif. | Liste déroulante | VRAI |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Réponse** |  |  |
| Code de statut | Statut HTTP de la demande.  Codes indiquant que la mise à jour du statut actif est réussie :   - 200. OK    Codes indiquant que la mise à jour du statut actif a échoué :   - 400. 400 : Malformed request (Requête mal formée) - 401. 401 : Unauthorized (Non autorisé) - 403. 403 : Forbidden (Interdit) - 404. introuvable - 409. 409 : Conflict (Conflit) - 429. 429 : Too many requests (Trop de requêtes) | Number (Numéro) |

## Miro Administration Connector

Le connecteur Miro Administration permet aux entreprises clientes de créer des équipes et de gérer les paramètres et les membres de ces équipes.

**Autoriser votre connecteur Miro Administration** :

Lorsque vous ajoutez une carte Miro à un flux pour la première fois, une invite vous demande de configurer une connexion pour votre organisation.  Voir la section Autorisation/span>.

**Cartes d’action du** **Miro Administration Connector :**

|  |  |
| --- | --- |
| **Action** | **Description** |
| Create Team (Créer une équipe) | Crée une nouvelle équipe dans une organisation existante. |
| Search Teams (Rechercher des équipes) | Recherche des équipes existantes dans une organisation.  Les 10 premières correspondances sont sélectionnées dans les résultats de recherche. |
| Add Member to Team (Ajouter un membre à l’équipe) | Ajoute un nouveau membre à une équipe existante. |
| Update Team Member Role (Mettre à jour le rôle du membre de l’équipe) | Met à jour le rôle d’un membre dans une équipe existante. |
| Get Team Settings (Récupérer les paramètres de l’équipe) | Récupère les paramètres d’une équipe existante. |
| Update Team Sharing Policies Settings (Mettre à jour les paramètres des politiques de partage de l’équipe) | Met à jour les paramètres de la politique de partage d’une équipe existante. |
| Update Team Invitation Settings (Mettre à jour les paramètres d’invitation de l’équipe) | Met à jour les paramètres de la politique d’invitation d’une équipe existante. |
| Update Team Collaboration Settings (Mettre à jour les paramètres de collaboration de l’équipe) | Met à jour les paramètres de collaboration d’une équipe existante. |
| Update Team Discovery Settings (Mettre à jour les paramètres de découverte de l’équipe) | Met à jour les paramètres de la politique de découverte d’une équipe existante. |
| Update Team Copy Access Settings (Mettre à jour les paramètres de copie de l’équipe) | Met à jour les paramètres de la politique en matière de copie d’une équipe existante. |
| Suppression de la session utilisateur (BETA) | Efface toutes les sessions d'utilisateurs pour une adresse e-mail donnée. |

## Permission

Le connecteur Miro Administration fonctionne à l’aide du jeton API OAuth.  Le connecteur Miro Administration n’est disponible que pour les clients d’un plan Enterprise. Pour créer une nouvelle connexion, les utilisateurs doivent disposer des permissions nécessaires pour installer des applications avec les portées prises en charge détaillées ci-dessous.

Vous pouvez créer et gérer plusieurs connexions à partir de la page **Connexions** vous pouvez créer et gérer plusieurs connexions.
Cette fonction est utile si vous prévoyez d'opérer avec plusieurs organisations. Chaque connexion du connecteur Miro Administration ne peut pointer que vers une seule organisation Miro.

Pour créer une nouvelle connexion à partir d’une carte Action :

1. Cliquez sur **New Connection** (Nouvelle connexion).
2. Entrez un **Connection Nickname** (Pseudo de connexion). Nous vous recommandons de choisir un nom qui représente l’organisation.
3. Obtenez l’**identifiant de l’organisation** et le **jeton d’accès** depuis la page Enterprise integration (Intégration Enterprise) en suivant les [instructions](02-miro-connector-for-okta-workflows.md).
4. Cliquez sur **Create** (Créer).  Cela enregistre votre connexion et vous ramène à votre flux.

Portées prises en charge :

- organizations:teams:write
- organizations:teams:read

### Create team (Créer une équipe)

Crée une nouvelle équipe dans une organisation existante.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| Équipe : |  |  |  |
| Team name (Nom de l’équipe) | Le nom de l’équipe. | chaîne de caractères | VRAI |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Réponse** |  |  |
| Team ID (Identifiant de l’équipe) | L’identifiant de la nouvelle équipe. | Chaîne de caractères |

### Search Teams (Rechercher des équipes)

Recherche des équipes existantes dans une organisation.  Les 10 premières correspondances sont sélectionnées dans les résultats de recherche.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| **Requête** |  |  |  |
| Le nom de l’équipe | Les mots à faire correspondre avec un nom d’équipe.  Toute équipe dont le nom comprend ces mots exacts sera affichée dans les résultats de la recherche. Les équipes dont les noms correspondent entièrement à la requête se trouveront en tête de la liste des résultats. | Chaîne de caractères | FALSE (FAUX) |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Réponse** |  |  |
| **Équipes** | Liste des 10 premières équipes trouvées. Chaque équipe comprend les champs ci-dessous. | List (Liste) |
| Team ID (Identifiant de l’équipe) | L’identifiant de l’équipe | Chaîne de caractères |
| Nom | Nom de l’équipe | Chaîne de caractères |

### Add member to team (Ajouter un membre à l’équipe)

Ajoute un nouveau membre à une équipe existante.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| **Team** |  |  |  |
| Team ID (Identifiant de l’équipe) | L’identifiant de l’équipe. | Chaîne de caractères | VRAI |
| Membre |  |  |  |
| User Email (Adresse e-mail de l’utilisateur) | L’adresse e-mail de l’utilisateur que vous souhaitez ajouter à l’équipe. | Chaîne de caractères | VRAI |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Réponse** |  |  |
| Member ID (Identifiant du membre) | Identifiant du nouveau membre de l’équipe. | Chaîne de caractères |

### Update team member role (Mettre à jour le rôle du membre de l’équipe)

Met à jour le rôle d’un membre d’une équipe existante.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| **Team** |  |  |  |
| Team ID (Identifiant de l’équipe) | L’identifiant de l’équipe. | Chaîne de caractères | VRAI |
| Membre |  |  |  |
| Member ID (Identifiant du membre) | L’identifiant du membre de l’équipe. | Chaîne de caractères | VRAI |
| Role (Rôle) | Le nouveau rôle du membre au sein de l’équipe.  - **Member** (Membre) : membre standard. - **Admin** : membre ayant des privilèges d’admin au sein de l’équipe. - **Team Guest** (Invité de l’équipe) : invité disposant de privilèges limités. | Liste déroulante | VRAI |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Réponse** |  |  |
| Member ID (Identifiant du membre) | L’identifiant du membre de l’équipe. | Chaîne de caractères |
| Role (Rôle) | Le nouveau rôle assigné au membre de l’équipe.  - **member** (membre) : membre standard. - **admin** : membre disposant de privilèges d’admin au sein de l’équipe. - **team_guest** (invité de l’équipe) : invité disposant de privilèges limités. | Chaîne de caractères |

### Get Team settings (Obtenir les paramètres de l’équipe)

Récupère les paramètres d’équipe d’une équipe existante.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| Équipe : |  |  |  |
| Team ID (Identifiant de l’équipe) | L’identifiant de l’équipe. | Chaîne de caractères | VRAI |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| Paramètres d’invitation de l’équipe |  |  |
| Who can Invite (Qui peut inviter) | - **only_org_admins** : les admins d’entreprise sont les seuls à pouvoir inviter des collaborateurs. - **admins** : les admins d’entreprise et les admins d’équipes peuvent inviter des collaborateurs. - **all_members** : tous les membres de l’équipe peuvent inviter des collaborateurs. | Chaîne de caractères |
| Invite External Users (Inviter des utilisateurs extérieurs) | - **allowed** : autorise les collaborateurs qui ne sont pas membres de l’équipe. - **Not_allowed** : n’autorise pas les collaborateurs qui ne sont pas membres de l’équipe. | Chaîne de caractères |
| **Paramètres de collaboration de l’équipe** |  |  |
| Co-Owner Role (Rôle de copropriétaire) | - **enabled** : le rôle de copropriétaire pour les tableaux et les projets est actif. - **disabled** : le rôle de copropriétaire pour les tableaux et les projets est inactif. | Chaîne de caractères |
| **Paramètres du niveau d’accès à la copie de l’équipe** |  |  |
| Copy Access Level (Niveau d’accès à la copie) | - **anyone** (tout le monde) : toutes les personnes ayant accès au tableau peuvent copier le contenu du tableau existant vers des tableaux nouvellement créés. ATTENTION : cette option n'est disponible que si **Limitation du niveau d'accès à la copie** est réglé sur **n'importe qui**. - **team_members** (membres de l’équipe) : les membres de l’équipe peuvent copier le contenu d’un tableau existant vers des tableaux nouvellement créés. - **team_editors** (éditeurs de l’équipe) : les membres de l’équipe dotés de droits de modification peuvent copier le contenu d’un tableau existant vers des tableaux nouvellement créés. - **board_owner** (propriétaire du tableau) : seuls les propriétaires du tableau peuvent copier le contenu d’un tableau existant vers des tableaux nouvellement créés. | Chaîne de caractères |
| Copy Access Level Limitation (Limite du niveau d’accès à la copie) | - **anyone** (tout le monde) : les membres de l’équipe et les utilisateurs ne faisant pas partie de l’équipe peuvent être autorisés à copier le contenu du tableau. - **team_members** (membres de l’équipe) : seuls les membres de l’équipe peuvent être autorisés à copier le contenu du tableau. | Chaîne de caractères |
| Paramètres de découverte de l’équipe |  |  |
| Discovery (Découverte) | - **hidden** (cachée) : seuls les utilisateurs invités à l’équipe peuvent voir l’équipe et y accéder. - **request** (demande) : les membres de l’organisation peuvent trouver l’équipe et demander à un admin de la rejoindre. - **join** (rejoindre) : les membres de l’organisation peuvent trouver l’équipe et la rejoindre. | Chaîne de caractères |
| **Paramètres de la politique de partage de l’équipe** |  |  |
| Default Board Access (Accès au tableau par défaut) | - **private** (privé) : seuls les propriétaires des tableaux peuvent accéder à ceux-ci. - **view** (afficher) : les membres de l’équipe peuvent afficher les tableaux. - **comment** (commenter) : les membres de l’équipe peuvent ajouter des commentaires aux tableaux. - **edit** (modifier) : tous les membres de l’équipe peuvent modifier les tableaux. | Chaîne de caractères |
| Accès par défaut de l’organisation | - **private** (privé) : seuls les propriétaires des tableaux peuvent accéder à ceux-ci. - **view** (consulter) : les membres de l’organisation peuvent consulter les tableaux. - **comment** (commenter) : tous les membres de l’organisation peuvent ajouter des commentaires sur les tableaux. - **edit** (modifier) : tous les membres de l’organisation peuvent modifier les tableaux. | Chaîne de caractères |
| Sharing on Organization (Partage avec l’organisation) | - - **allowed** (autorisé) : le partage au niveau de l’organisation est autorisé. - **allowed_with_editing** (autorisé avec droits de modification) : le partage avec droits de modification au niveau de l’organisation est autorisé. - **not_allowed** (non autorisé) : le partage au niveau de l’organisation n’est pas autorisé. | Chaîne de caractères |
| Sharing on Team (Partage avec l’équipe) | - - **allowed** (autorisé) : le partage au niveau de l’équipe est autorisé. - **allowed_with_editing** (autorisé avec droits de modifications) : le partage avec droits de modification au niveau de l’équipe est autorisé. - **not_allowed** (non autorisé) : le partage au niveau de l’équipe n’est pas autorisé. | Chaîne de caractères |
| Sharing via Public Link (Partage via lien public) | - **Allowed** (autorisé) : **le partage via un lien public est autorisé.** - **allowed_with_editing** (autorisé avec droits de modification) : le partage avec droits de modification via un lien public est autorisé. - **not_allowed** (non autorisé) : le partage via un lien public n’est pas autorisé. | Chaîne de caractères |
| Move Board to Team (Déplacer le tableau vers l’équipe) | - **allowed** (autorisé) : le déplacement des tableaux vers une équipe différente est autorisé. - **not_allowed** (non autorisé) : le déplacement des tableaux vers une équipe différente n’est pas autorisé. | Chaîne de caractères |

### Update Team Sharing Policy settings (Mettre à jour les paramètres de la politique de partage de l’équipe)

Met à jour les paramètres de la politique de partage d’une équipe existante.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| **Team** |  |  |  |
| Team ID (Identifiant de l’équipe) | L’identifiant de l’équipe. | Chaîne de caractères | VRAI |
| Default Board Access (Accès au tableau par défaut) | - **Private** (Privé) : seuls les propriétaires des tableaux peuvent accéder à ceux-ci. - **View** (Consulter) : les membres de l’équipe peuvent consulter les tableaux. - **Comment** (Commenter) : tous les membres de l’équipe peuvent ajouter des commentaires aux tableaux. - **Edit** (Modifier) : tous les membres de l’équipe peuvent modifier les tableaux. | Liste déroulante | FALSE (FAUX) |
| Default Organization Access (Accès par défaut de l’organisation) | - **Private** (Privé) : seuls les propriétaires des tableaux peuvent accéder aux tableaux. - **View** (Consulter) : les membres de l’équipe peuvent consulter les tableaux. - **Comment** (Commenter) : tous les membres de l’équipe peuvent ajouter des commentaires aux tableaux. - **Edit** (Modifier) : tous les membres de l’équipe peuvent modifier les tableaux. | Liste déroulante | FALSE (FAUX) |
| Sharing via Public Link (Partage via lien public) | - **Allowed** (autorisé) : le partage via un lien public est autorisé. - **allowed_with_editing** (autorisé avec droits de modification) : le partage avec droits de modification via un lien public est autorisé. - **Not Allowed** (non autorisé) : le partage via un lien public n’est pas autorisé. | Liste déroulante | FALSE (FAUX) |
| Sharing on Team (Partage avec l’équipe) | - **allowed** (autorisé) : le partage au niveau de l’équipe est autorisé. - **allowed_with_editing** (autorisé avec droits de modifications) : le partage avec droits de modification au niveau de l’équipe est autorisé. - **not_allowed** (non autorisé) : le partage au niveau de l’équipe n’est pas autorisé. | Liste déroulante | FALSE (FAUX) |
| Sharing on Organization (Partage avec l’organisation) | - **allowed** (autorisé) : le partage au niveau de l’organisation est autorisé. - **allowed_with_editing** (autorisé avec droits de modification) : le partage avec droits de modification au niveau de l’organisation est autorisé. - **not_allowed** (non autorisé) : le partage au niveau de l’organisation n’est pas autorisé. | Liste déroulante | FALSE (FAUX) |
| Move Board to Team (Déplacer le tableau vers l’équipe) | - **Allowed** (autorisé) : le déplacement des tableaux vers une équipe différente est autorisé. - **Not Allowed** (non autorisé) : le déplacement des tableaux vers une équipe différente n’est pas autorisé. | Liste déroulante | FALSE (FAUX) |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Paramètres de la politique de partage de l’équipe** |  |  |
| Default Board Access (Accès au tableau par défaut) | - **private** (privé) : seuls les propriétaires des tableaux peuvent accéder à ceux-ci. - **view** (afficher) : les membres de l’équipe peuvent afficher les tableaux. - **comment** (commenter) : les membres de l’équipe peuvent ajouter des commentaires aux tableaux. - **edit** (modifier) : tous les membres de l’équipe peuvent modifier les tableaux. | Chaîne de caractères |
| Default Organization Access (Accès par défaut de l’organisation) | - **private** (privé) : seuls les propriétaires des tableaux peuvent accéder à ceux-ci. - **view** (consulter) : les membres de l’organisation peuvent consulter les tableaux. - **comment** (commenter) : les membres de l’organisation peuvent ajouter des commentaires sur les tableaux. - **edit** (modifier) : tous les membres de l’organisation peuvent modifier les tableaux. | Chaîne de caractères |
| Sharing on Organization (Partage avec l’organisation) | - - **allowed** (autorisé) : le partage au niveau de l’organisation est autorisé. - **allowed_with_editing** (autorisé avec droits de modification) : le partage avec droits de modification au niveau de l’organisation est autorisé. - **not_allowed** (non autorisé) : le partage au niveau de l’organisation n’est pas autorisé. | Chaîne de caractères |
| Sharing on Team (Partage avec l’équipe) | - - **allowed** (autorisé) : le partage au niveau de l’équipe est autorisé. - **allowed_with_editing** (autorisé avec droits de modifications) : le partage avec droits de modification au niveau de l’équipe est autorisé. - **not_allowed** (non autorisé) : le partage au niveau de l’équipe n’est pas autorisé. | Chaîne de caractères |
| Sharing via Public Link (Partage via lien public) | - - **Allowed** (autorisé) : le partage via un lien public est autorisé. - **allowed_with_editing** (autorisé avec droits de modification) : le partage avec droits de modification via un lien public est autorisé. - **not_allowed** (non autorisé) : le partage via un lien public n’est pas autorisé. | Chaîne de caractères |
| Move Board to Team (Déplacer le tableau vers l’équipe) | - **allowed** (autorisé) : le déplacement des tableaux vers une équipe différente est autorisé. - **not_allowed** (non autorisé) : le déplacement des tableaux vers une équipe différente n’est pas autorisé. | Chaîne de caractères |

### Update Team Invitation settings (Mettre à jour les paramètres d’invitation de l’équipe)

Met à jour les paramètres de la politique d’invitation d’une équipe existante.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| **Team** |  |  |  |
| Team ID (Identifiant de l’équipe) | L’identifiant de l’équipe. | Chaîne de caractères | VRAI |
| Invite External Users (Inviter des utilisateurs extérieurs) | - **Allowed** : autorise les collaborateurs qui ne sont pas membres de l’équipe. - **Not_allowed** : n’autorise pas les collaborateurs qui ne sont pas membres de l’équipe. | Liste déroulante | FALSE (FAUX) |
| Who can Invite (Qui peut inviter) | - **Only Organization Admins** (Admins d’entreprise uniquement) : seuls les admins d’entreprise peuvent inviter des collaborateurs. - **Admins** : les admins d’entreprise et les admins d’équipes peuvent inviter des collaborateurs. - **All Members** (Tous les membres) : tous les membres de l’équipe peuvent inviter des collaborateurs. | Liste déroulante | FALSE (FAUX) |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Paramètres d’invitation de l’équipe** |  |  |
| Invite External Users (Inviter des utilisateurs extérieurs) | - **allowed** : autorise les collaborateurs qui ne sont pas membres de l’équipe. - **not_allowed** (non autorisé) : n’autorise pas les collaborateurs qui ne sont pas membres de l’équipe. | Chaîne de caractères |
| Who can Invite (Qui peut inviter) | - **only_org_admins** : les admins d’entreprise sont les seuls à pouvoir inviter des collaborateurs. - **admins** : les admins d’entreprise et les admins d’équipes peuvent inviter des collaborateurs. - **all_members** : tous les membres de l’équipe peuvent inviter des collaborateurs. | Chaîne de caractères |

### Update Team copy access settings (Mettre à jour les paramètres de copie de l’équipe)

Met à jour les paramètres de la politique de copie d’une équipe existante.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| **Team** |  |  |  |
| Team ID (Identifiant de l’équipe) | L’identifiant de l’équipe. | Chaîne de caractères | VRAI |
| Copy Access Level (Niveau d’accès à la copie) | - **anyone** (tout le monde) : toutes les personnes ayant accès au tableau peuvent copier le contenu du tableau existant vers des tableaux nouvellement créés. - **Team Members** (Membres de l’équipe) : les membres de l’équipe peuvent copier le contenu d’un tableau existant vers des tableaux nouvellement créés. - **Team Editors** (Éditeurs de l’équipe) : les membres de l’équipe dotés de droits de modification peuvent copier le contenu d’un tableau existant vers des tableaux nouvellement créés. - **board_owner** (propriétaire du tableau) : seuls les propriétaires du tableau peuvent copier le contenu d’un tableau existant vers des tableaux nouvellement créés. | Liste déroulante | FALSE (FAUX) |
| Copy Access Level Limitation (Limite du niveau d’accès à la copie) | - **Anyone** (Tout le monde) : les membres de l’équipe et les utilisateurs ne faisant pas partie de l’équipe peuvent être autorisés à copier le contenu du tableau. - **Team Members** (Membres de l’équipe) : seuls les membres de l’équipe peuvent être autorisés à copier le contenu du tableau. | Liste déroulante | FALSE (FAUX) |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Paramètres d’accès à la copie de l’équipe** |  |  |
| Copy Access Level (Niveau d’accès à la copie) | - **anyone** (tout le monde) : toutes les personnes ayant accès au tableau peuvent copier le contenu du tableau existant vers des tableaux nouvellement créés. - **team_members** (membres de l’équipe) : les membres de l’équipe peuvent copier le contenu d’un tableau existant vers des tableaux nouvellement créés. - **team_editors** (éditeurs de l’équipe) : les membres de l’équipe dotés de droits de modification peuvent copier le contenu d’un tableau existant vers des tableaux nouvellement créés. - **board_owner** (propriétaire du tableau) : seuls les propriétaires du tableau peuvent copier le contenu d’un tableau existant vers des tableaux nouvellement créés. | Chaîne de caractères |
| Copy Access Level Limitation (Limite du niveau d’accès à la copie) | - **anyone** (tout le monde) : les membres de l’équipe et les utilisateurs ne faisant pas partie de l’équipe peuvent être autorisés à copier le contenu du tableau. - **team_members** (membres de l’équipe) : seuls les membres de l’équipe peuvent être autorisés à copier le contenu du tableau. | Chaîne de caractères |

### Update Team Collaboration settings (Mettre à jour les paramètres de collaboration de l’équipe)

Met à jour les paramètres de la politique de collaboration d’une équipe existante.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| **Team** |  |  |  |
| Team ID (Identifiant de l’équipe) | L’identifiant de l’équipe. | Chaîne de caractères | VRAI |
| Co-Owner Role (Rôle de copropriétaire) | - **Enabled** (activé) : le rôle de copropriétaire pour les tableaux et les projets est actif. - **Disabled** (désactivé) : le rôle de copropriétaire pour les tableaux et les projets est inactif | Liste déroulante | FALSE (FAUX) |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Paramètres de collaboration de l’équipe** |  |  |
| Co-Owner Role (Rôle de copropriétaire) | - **enabled** : le rôle de copropriétaire pour les tableaux et les projets est actif. - **disabled** : le rôle de copropriétaire pour les tableaux et les projets est inactif. | Chaîne de caractères |

### Update Team Discovery settings (Mettre à jour les paramètres de découverte de l’équipe)

Met à jour les paramètres de la politique de découverte d’une équipe existante.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| **Team** |  |  |  |
| Team ID (Identifiant de l’équipe) | L’identifiant de l’équipe. | Chaîne de caractères | VRAI |
| Discovery (Découverte) | - **Hidden** (Cachée) : seuls les utilisateurs invités à l’équipe peuvent voir l’équipe et y accéder. - **Request** (Demande) : les membres de l’organisation peuvent trouver l’équipe et demander à un admin de la rejoindre. - **Join** (rejoindre) : les membres de l’organisation peuvent trouver l’équipe et la rejoindre. | Liste déroulante | FALSE (FAUX) |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Paramètres de découverte de l’équipe** |  |  |
| Discovery (Découverte) | - **hidden** (cachée) : seuls les utilisateurs invités à l’équipe peuvent voir l’équipe et y accéder. - **request** (demande) : les membres de l’organisation peuvent trouver l’équipe et demander à un admin de la rejoindre. - **join** (rejoindre) : les membres de l’organisation peuvent trouver l’équipe et la rejoindre. | Chaîne de caractères |

### Effacement de la session de l'utilisateur

Efface toutes les sessions d'utilisateurs pour une adresse e-mail donnée.

Entrée

|  |  |  |  |
| --- | --- | --- | --- |
| **Champ** | **Définition** | **Type** | **Requis** |
| User Details (Détails utilisateur) |  |  |  |
| Email (Adresse e-mail) | L'adresse e-mail de l'utilisateur dont les sessions doivent être effacées. | Chaîne de caractères | VRAI |

Sortie

|  |  |  |
| --- | --- | --- |
| **Champ** | **Définition** | **Type** |
| **Réponse** |  |  |
| Code de statut | Statut HTTP de la demande.   Codes indiquant la réussite de la mise à jour de l'effacement de la session de l'utilisateur :   - 200. Session utilisateur supprimée    Codes indiquant l'échec de la mise à jour de l'effacement de la session de l'utilisateur :   - 400. 400 : Malformed request (Requête mal formée) - 401. 401 : Unauthorized (Non autorisé) - 403. 403 : Forbidden (Interdit) - 404. introuvable - 409. 409 : Conflict (Conflit) - 429. 429 : Too many requests (Trop de requêtes) | Number (Numéro) |
