---
title: "Enterprise Guard Deployment Guide Part 1 : Configurer les r\xF4les d'admin."
article_id: 17120595534994
translation_id: 17120595534994
locale: fr
sidebar_position: 1
created_at: '2024-02-19T09:19:59Z'
updated_at: '2025-11-25T15:41:04Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Les administrateurs d'entreprise peuvent s'attribuer, ainsi qu'à d'autres personnes, des rôles d'administrateur supplémentaires une fois qu'Enterprise Guard est activé. Par conséquent, le nombre d'administrateurs d'entreprise dans votre organisation doit être réduit au minimum. Examinez attentivement votre configuration d'administration existante et déplacez les admin d'entreprise vers d'autres rôles (tels que l'admin d'équipe ou d'utilisateur) lorsque cela est approprié pour équilibrer la sécurité, la conformité et l'efficacité opérationnelle.

Bien que recommandée, une réévaluation globale de votre configuration admin n'est pas nécessaire pour déployer Enterprise Guard. Passez à [Partie 2 : Déployez le site](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md) à votre convenance.

## Aperçu des rôles de l'administrateur Miro

Voici une liste des rôles d'admin disponibles dans Miro, avec une description des responsabilités et des personnes auxquelles ils conviennent dans une organisation type.

:::note
Notes :
- Il s'agit d'une liste évolutive de rôles et de privilèges. Consultez régulièrement cette page pour des mises à jour.
- Pour attribuer le rôle d'admin de gouvernance des données ou d'admin de contenu sensible à un utilisateur, vous devez être administrateur d'entreprise.
:::

|  |  |  |
| --- | --- | --- |
| **Rôle d'admin.** | **Responsabilités** | **Recommandé pour** |
| **les admins d’entreprise** | Responsable de la gestion globale et de la délégation de responsabilités spécifiques à d'autres rôles d'admin. Il doit avoir une large compréhension des besoins opérationnels de l'organisation et de ses obligations en matière de conformité. | - Administrateurs informatiques seniors - Chefs de service - Gestionnaires de projet - Chefs d'équipe - Directeurs des opérations - Responsables des technologies de l'entreprise - Miro Propriétaire de produit |
| **admins d’équipe** | Gérer les paramètres spécifiques à l'équipe et l'accès des utilisateurs au sein de leurs équipes respectives. Assurer l'autonomie de l'équipe tout en s'alignant sur les politiques générales de l'organisation. | - Chefs de service - Gestionnaires de projet - Chefs d'équipe - Directeurs des opérations |
| **Admins utilisateurs** | Gérer la gestion des utilisateurs et des licences. Idéal pour gérer les accès et les comptes des employés. Gérez efficacement les utilisateurs sans surcharger les administrateurs d'entreprise ou d'équipe. | - Responsable informatique - Administrateurs informatiques - Service d'assistance informatique |
| **Admins gouvernance des données (Enterprise Guard)** | Responsable de la conformité et de la gouvernance des données. Doit comprendre le paysage juridique et réglementaire relatif aux données de l'organisation, y compris les politiques de conservation et de suppression de l'organisation. | - Responsable de la conformité (CCO) - Responsable de la gouvernance des données - Responsable de la conformité - Responsable des affaires réglementaires - Risk Manager - Gestionnaire des dossiers - Analyste eDiscovery - Analyste en criminalistique |
| **Administrateurs eDiscovery (Enterprise Guard)** | Gérez les paramètres de conservation inaltérable afin de préserver les tableaux pertinents pour les enquêtes ou les affaires judiciaires en cours. Cela inclut la création, la modification et la libération de conservations inaltérables ou d'affaires pour empêcher la suppression permanente de contenu, en assurant la conformité avec les obligations légales et réglementaires. Ce rôle est crucial pour les organisations qui exigent une préservation rigoureuse des données pour soutenir les procédures judiciaires et les mandats de conformité. | - Conseiller juridique - Spécialistes de l'administration de la preuve électronique - Agents de conformité - Gestionnaires de risques - Analystes en criminalistique - Responsable de la sécurité de l'information (CISO) - Délégué à la protection des données (DPD) - Responsable de la protection de la vie privée |
| **Administrateurs de contenus sensibles (Enterprise Guard)** | Responsable de la protection des données et de la vie privée. Il est essentiel de classer, de gérer et de protéger les informations sensibles dans l'ensemble de l'organisation. Important pour le traitement des PII, PHI, PCI ou de la propriété intellectuelle. | - Responsable de la sécurité de l'information (CISO) - Délégué à la protection des données (DPD) - Responsable de la protection de la vie privée - Analyste en cybersécurité - Consultant en sécurité informatique |

:::tip
En savoir plus sur les [rôles d’administrateur et leurs privilèges](../enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) dans le forfait Enterprise.
:::

## Matrice détaillée des privilèges et des rôles d'administrateur d'Enterprise Guard

Le tableau suivant répertorie les privilèges détaillés et la matrice des rôles d'admin pour chaque fonctionnalité.

|  |  |  |  |
| --- | --- | --- | --- |
| **Gestion du cycle de vie du contenu** | | |  |
| **Privilège** | **Admin de gouvernance des données** | **Admin de contenu sensible** | **admin eDiscovery** |
| Consulter les paramètres de la corbeille |  |  |  |
| Modifier les paramètres de la corbeille |  |  |  |
| Ajouter une politique de conservation |  |  |  |
| Modifier la politique de conservation |  |  |  |
| Supprimer la politique de conservation |  |  |  |
| Ajouter une politique de suppression |  |  |  |
| Modifier la politique de suppression |  |  |  |
| Supprimer la politique de suppression |  |  |  |
| **Classification des données** | | |  |
| **Privilège** | **Admin de gouvernance des données** | Admin de contenu sensible | **admin eDiscovery** |
| Consulter les paramètres de classification des données |  |  |  |
| Modifier les niveaux de classification |  |  |  |
| Modifier les paramètres de classification automatique |  |  |  |
| Modifier les paramètres des garde-fous de classification |  |  |  |
| Modifier le niveau de classification par défaut |  |  |  |
| **Découverte de données** | | |  |
| **Privilège** | **Admin de gouvernance des données** | **Admin de contenu sensible** | **admin eDiscovery** |
| Consulter les badges de confidentialité |  |  |  |
| Activer/désactiver la détection des données confidentielles |  |  |  |
| Consulter le nombre de résultats : badges de confidentialité |  |  |  |
| Consulter les résultats biffés : badges de confidentialité |  |  |  |
| Consulter l’intégralité des résultats : badges de confidentialité |  |  |  |
| **eDiscovery** | | |  |
| **Privilège** | **Admin de gouvernance des données** | **Admin de contenu sensible** | **admin eDiscovery** |
| Gérer les paramètres de mise en suspens juridique |  |  |  |
| Consulter les paramètres de mise en suspens juridique |  |  |  |

</table> Privilèges détaillés et matrice des rôles d'admin pour chaque fonctionnalité

## Transition de votre configuration admin

### Auditer votre configuration admin actuelle

Passez en revue la liste des utilisateurs qui disposent de droits d'administration dans Miro et leurs responsabilités. Utilisez l'outil d'évaluation de la configuration admin pour générer un résumé de l'état actuel.

- Filtrez la liste des utilisateurs de la section **Utilisateurs actifs** des paramètres de l'entreprise pour afficher les administrateurs de l'entreprise.
- Consultez la liste des administrateurs d'utilisateurs, des administrateurs de gouvernance des données et des administrateurs de contenu sensible à l'aide de la section **Rôle d'administrateur des** paramètres de l'entreprise.

### Établir une nouvelle configuration de l'admin.

Comparez votre configuration admin actuelle au tableau ci-dessus et aux politiques de votre entreprise. Utilisez l'outil d'évaluation de la configuration admin pour générer une nouvelle configuration.

Réfléchissez à des questions telles que

- Qui a besoin d'un rôle de gouvernance des données ?
- Qui a besoin du rôle "Contenu sensible" ?
- Quels sont les administrateurs d'entreprise qui peuvent être transformés en administrateurs d'utilisateur ?
- Quels sont les administrateurs d'entreprise qui peuvent être transformés en administrateurs d'équipe ?

### Réattribuer les rôles et informer les utilisateurs

Les articles du Centre d'assistance ci-dessous expliquent comment attribuer les différents rôles. Pour vous faciliter la tâche, personnalisez les modèles d'e-mail fournis pour informer les utilisateurs des transitions.

- [Comment attribuer des administrateurs d'entreprise et des administrateurs d'équipe ?](../../../administration/user-management/06-how-to-manage-admin-roles.md)
- [Comment désigner des administrateurs d'utilisateurs, des administrateurs de gouvernance des données et des administrateurs de contenu sensible ?](../enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)

### Attribuez le rôle d'admin de gouvernance de données à la gouvernance des données

:::note
Pour attribuer le rôle d'admin de gouvernance à un utilisateur, vous devez être un admin d'entreprise.
:::

1. Allez dans les paramètres de votre profil.
   - A partir d’un tableau : **Menu principal > Préférences > Paramètres du profil**.- Depuis le tableau de bord : cliquez sur votre avatar dans le coin supérieur droit et cliquez sur **Paramètres**.
   - A partir de l'URL `https://miro.com/app/settings`: Choisissez votre entreprise dans la liste située dans le coin supérieur gauche.
2. Sous « Gestion des utilisateurs », cliquez sur Rôles d’admin.
3. Dans le volet de droite, cliquez sur l'**ellipse** **Data Governance Admin** **(****...)**puis sélectionnez **Attribuer un rôle**.
4. Choisissez l'utilisateur auquel vous souhaitez attribuer le rôle d'administrateur de la gouvernance des données, faites défiler la fenêtre jusqu'en bas, puis cliquez sur **Attribuer**.

### Attribuez le rôle d'admin. de contenu sensible rôle

:::note
Pour attribuer le rôle d'administrateur de contenu sensible à un utilisateur, vous devez être administrateur d'entreprise.
:::

1. Allez dans les paramètres de votre profil.
   - A partir d’un tableau : **Menu principal > Préférences > Paramètres du profil**.- Depuis le tableau de bord : cliquez sur votre avatar dans le coin supérieur droit et cliquez sur **Paramètres**.
   - A partir de l'URL `https://miro.com/app/settings`: Choisissez votre entreprise dans la liste située dans le coin supérieur gauche.
2. Sous « Gestion des utilisateurs », cliquez sur Rôles d’admin.
3. Oans le volet de droite, cliquez sur l'**ellipse** **Sensitive Content Admin** **(****...)**puis sélectionnez **Attribuer un rôle**.
4. Choisissez l'utilisateur auquel vous souhaitez attribuer le rôle d'administrateur de contenu sensible, faites défiler la fenêtre jusqu'en bas, puis cliquez sur **Attribuer**.

### Attribuer le rôle d'admin eDiscovery au rôle d'administrateur d'eDiscovery

:::note
Pour attribuer le rôle d'administrateur d'eDiscovery à un utilisateur, vous devez être administrateur d'entreprise.
:::

1. Allez dans les paramètres de votre profil.
   - A partir d’un tableau : **Menu principal > Préférences > Paramètres du profil**.- Depuis le tableau de bord : cliquez sur votre avatar dans le coin supérieur droit et cliquez sur **Paramètres**.
   - A partir de l'URL `https://miro.com/app/settings`: Choisissez votre entreprise dans la liste située dans le coin supérieur gauche.
2. Sous « Gestion des utilisateurs », cliquez sur Rôles d’admin.
3. Oans le volet de droite, cliquez sur l'**ellipse** **eDiscovery Admin** **(****...)**puis sélectionnez **Attribuer un rôle**.
4. Choisissez l'utilisateur auquel vous souhaitez attribuer le rôle d'administrateur eDiscovery, faites défiler la fenêtre jusqu'en bas, puis cliquez sur **Attribuer**.

### Ressources

- [Outil d'évaluation de la configuration admin](https://docs.google.com/spreadsheets/d/1a0WQc-fBpuVwfnoY8VCx66PjOXS76q7DJ__xDYcp8rk/edit?usp=sharing) (faites une copie)
- [Modèles d'e-mail | Configuration admin Communications](https://docs.google.com/document/d/18Kw4GNPq7GnAx8R8co5PaZ04peVogfVDgsdKK2MuARM/edit?usp=sharing) (faites une copie)
