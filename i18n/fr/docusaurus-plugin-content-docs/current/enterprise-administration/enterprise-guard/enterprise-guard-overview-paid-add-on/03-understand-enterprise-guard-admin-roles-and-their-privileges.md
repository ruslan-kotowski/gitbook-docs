---
title: "Comprendre les r\xF4les d'admin Enterprise Guard et leurs privil\xE8ges"
article_id: 15695755655954
translation_id: 15695755655954
locale: fr
sidebar_position: 1
created_at: '2023-12-11T18:33:53Z'
updated_at: '2026-03-12T22:21:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Les fonctionnalités d'Enterprise Guard sont contrôlées via des privilèges d'admin. Ces privilèges peuvent être accordés grâce à des rôles d'admin prédéfinis ou à des rôles d'admin personnalisés configurés avec les privilèges nécessaires.

Le tableau suivant liste les privilèges disponibles pour chaque fonctionnalité et montre quels rôles d'admin prédéfinis les incluent par défaut. Lors de la création de rôles d'admin personnalisés, les admins d’entreprise peuvent attribuer ces privilèges pour autoriser l'accès à des fonctionnalités spécifiques d'Enterprise Guard.

Le tableau suivant liste les privilèges détaillés et le matrice de rôles d'admin pour chaque fonctionnalité.

|  |  |  |  |
| --- | --- | --- | --- |
| **Gestion du cycle de vie du contenu** | | | |
| **Privilège** | **Admin de gouvernance des données** | **Admin de contenu sensible** | **Admin eDiscovery** |
| Consulter les paramètres de la corbeille | ✅ | ❌ | ❌ |
| Modifier les paramètres de la corbeille | ✅ | ❌ | ❌ |
| Ajouter une politique de conservation | ✅ | ❌ | ❌ |
| Modifier la politique de conservation | ✅ | ❌ | ❌ |
| Supprimer la politique de conservation | ✅ | ❌ | ❌ |
| Ajouter une politique de suppression | ✅ | ❌ | ❌ |
| Modifier la politique de suppression | ✅ | ❌ | ❌ |
| Supprimer la politique de suppression | ✅ | ❌ | ❌ |
| **Classification des données** | | | |
| **Privilège** | **Admin de gouvernance des données** | **Admin de contenu sensible** | **Admin eDiscovery** |
| Consulter les paramètres de classification des données | ❌ | ✅ | ❌ |
| Modifier les niveaux de classification | ❌ | ✅ | ❌ |
| Modifier les paramètres de classification automatique | ❌ | ✅ | ❌ |
| Modifier les paramètres des garde-fous de classification | ❌ | ✅ | ❌ |
| Modifier le niveau de classification par défaut | ❌ | ✅ | ❌ |
| **Découverte des données** | | | |
| **Privilège** | **Admin de gouvernance des données** | **Admin de contenu sensible** | **Admin eDiscovery** |
| Consulter les badges de confidentialité | ❌ | ✅ | ❌ |
| Activer/désactiver la détection de données personnelles | ❌ | ✅ | ❌ |
| Consulter le nombre de correspondances - badges de confidentialité | ❌ | ✅ | ❌ |
| Consulter les correspondances biffées - badges de confidentialité | ❌ | ✅ | ❌ |
| Consulter l’intégralité des correspondances - badges de confidentialité | ❌ | ✅ | ❌ |
| **eDiscovery** | | | |
| **Privilège** | **Admin de gouvernance des données** | **Admin de contenu sensible** | **Admin eDiscovery** |
| Gérer les paramètres de mise en suspens juridique | ❌ | ❌ | ✅ |
| Consulter les paramètres de mise en suspens juridique | ❌ | ❌ | ✅ |

*Matrice détaillée des privilèges et rôles d'admin prédéfinis pour chaque fonctionnalité*

> **REMARQUE :** Les fonctionnalités Enterprise Guard peuvent être accordées via les rôles d'admin prédéfinis ou via des rôles d'admin personnalisés configurés avec les privilèges requis.

## Attribuer un rôle d'admin Enterprise Guard

:::note
Pour attribuer un rôle d'admin Enterprise Guard à un utilisateur, vous devez être un **admin d’entreprise**.
:::

1. Allez dans vos **paramètres du profil** :

   - À partir d’un tableau : **Menu principal > Préférences > Paramètres du profil**.
   - Depuis le tableau de bord : Cliquez sur votre **avatar** dans le coin supérieur droit et cliquez sur **Paramètres**.
   - Depuis l'URL : Rendez-vous sur `https://miro.com/app/settings`, et choisissez votre **Entreprise** dans la liste en haut à gauche.
2. Sous **Gestion des utilisateurs**, cliquez sur **Rôles d'admin**.
3. Dans le volet droit, trouvez le rôle d'admin que vous souhaitez attribuer (par exemple, **Admin de gouvernance des données**, **Admin de contenu sensible**, ou **Admin eDiscovery**).
4. Cliquez sur le **menu à trois points (…)** à côté du rôle et sélectionnez **Attribuer un rôle**.
5. Choisissez l'utilisateur à qui vous souhaitez attribuer le rôle.
6. Faites défiler jusqu'en bas de la fenêtre et cliquez sur **Attribuer**.

## Rôles d'admin personnalisés pour Enterprise Guard

Les rôles d'admin personnalisés permettent aux admins d’entreprise de donner accès à des fonctionnalités individuelles d'Enterprise Guard sans attribuer de rôles administratifs plus larges. Cela permet aux organisations d'adapter l'accès en fonction des responsabilités internes en matière de gouvernance, de sécurité ou de conformité.

Lors de la création ou de la modification d'un rôle d'admin personnalisé, les admins d’entreprise peuvent sélectionner les privilèges qui déterminent quelles fonctionnalités d'Enterprise Guard le rôle peut accéder et gérer. Ces privilèges s'étendent à plusieurs domaines d'Enterprise Guard, tels que la classification des données, la découverte de données, la gestion du cycle de vie du contenu, eDiscovery.

En n'attribuant que les privilèges requis, les organisations peuvent déléguer des tâches administratives, telles que l'examen des conclusions sur le contenu sensible, la gestion des paramètres de classification, la configuration des politiques de cycle de vie ou l'accès aux outils d'eDiscovery, aux équipes appropriées. La table ci-dessous répertorie les privilèges qui peuvent être attribués lors de la configuration des rôles d'admin personnalisés.

|  |  |  |
| --- | --- | --- |
| **Capacité** | **Privilège** | **Description** |
| **Classification des données** | Consulter les paramètres de classification des données | L’admin peut consulter les paramètres de classification de l’organisation. |
| Modifier les paramètres de classification automatique | L’admin peut modifier les paramètres de classification automatique de l’organisation. |
| **Découverte de données** | Consulter les paramètres de découverte de données | L’admin peut consulter les paramètres de découverte de données de l’organisation. |
| Gérer les paramètres de découverte de données | L’admin peut gérer les paramètres de découverte de données de l’organisation. |
| Consulter les résultats liés à la découverte de données | L’admin peut consulter les résultats liés à la découverte de données. |
| Gérer les résultats liés à la découverte de données | L’admin peut gérer les résultats liés à la découverte de données. |
| **eDiscovery** | Consulter les paramètres de mise en suspens juridique | L’admin peut consulter les mises en suspens juridiques sur la page des paramètres d’enquête eDiscovery. |
| Gérer les paramètres de mise en suspens juridique | L’admin peut gérer les mises en suspens juridiques sur la page des paramètres d’enquête eDiscovery. |
| Consulter les exports de tableaux | L’admin peut consulter les exports de tableaux dans le cadre de l'eDiscovery. |
| Gérer les exports de tableaux | L’admin peut gérer les exports de tableaux dans le cadre de l'eDiscovery. |
| **Gestion du cycle de vie du contenu** | Consulter les paramètres de la corbeille | L’admin peut consulter les paramètres de la corbeille des tableaux de l’organisation. |
| Gérer les paramètres de la corbeille | L’admin peut gérer la durée de conservation des tableaux de l’organisation dans la corbeille et les autorisations. |
| Consulter les paramètres de conservation du cycle de vie du contenu | L’admin peut consulter la page des paramètres de conservation du cycle de vie du contenu. |
| Gérer les paramètres de conservation du cycle de vie du contenu | L’admin peut gérer la page des paramètres de conservation du cycle de vie du contenu. |
| Consulter les paramètres de suppression du cycle de vie du contenu | L’admin peut consulter la page des paramètres de suppression du cycle de vie du contenu. |
| Gérer les paramètres de suppression du cycle de vie du contenu | L’admin peut gérer la page des paramètres de suppression du cycle de vie du contenu. |
| Consulter le contenu sous conservation ou suppression | Permet à l’utilisateur de consulter le contenu qui est affecté par les politiques de conservation ou de suppression. |
