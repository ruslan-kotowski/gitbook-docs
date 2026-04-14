---
title: Copropriétaires des tableaux et des espaces
article_id: 360021580759
translation_id: 360021580759
locale: fr
sidebar_position: 6
created_at: '2021-05-12T07:36:28Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
availability:
  notes: 'Qui peut le faire: Propriétaires de tableau, Copropriétaires de tableau,
    Propriétaires d’espace, Copropriétaires d’espace, Admins d’équipe, Admins d’entreprise
    Quels forfaits: Business, Enterprise Quelles plateformes: Navigateur, Bureau,
    Mobile'
---

Le rôle de copropriétaire améliore la collaboration en permettant aux propriétaires de tableaux de déléguer les responsabilités de préparation et de facilitation du travail sur un tableau, que ce soit pour des sessions en direct ou asynchrones.

Un copropriétaire assure un flux de travail fluide, même si le propriétaire principal du tableau est indisponible, car les copropriétaires peuvent effectuer presque toutes les actions de niveau propriétaire, de la gestion des paramètres du tableau au contrôle de la visibilité du contenu. Un copropriétaire aide à répartir la charge de travail et assure une sauvegarde fiable pour la gestion du tableau.

Pour savoir quelles autorisations un copropriétaire a pour un tableau ou un espace, consultez la référence des copropriétaires.

## Activer le rôle de copropriétaire pour l'organisation

En tant qu'administrateur de l'entreprise, suivez ces étapes :

1. Depuis votre tableau de bord Miro, cliquez sur votre avatar dans le coin supérieur droit et cliquez sur **Console d'administration**.
2. Allez à **Sécurité** > **Partage** > **Rôles et autorisations**.
3. Basculez **Autoriser le rôle de copropriétaire** en position activée.

Les admins peuvent désormais activer le rôle de copropriétaire pour leurs équipes.

## Activer le rôle de copropriétaire pour une équipe

En tant qu'admin d'entreprise ou d'équipe, suivez ces étapes :

1. Depuis votre tableau de bord Miro, cliquez sur votre avatar dans le coin supérieur droit et cliquez sur **Console d'administration** | **Paramètres**.
2. Allez dans **Équipes** > **\{team name\}** > **Paramètres**.
3. Sous **Paramètres de collaboration**, activez **Activer le rôle de copropriétaire sur les tableaux et les Espaces** en position marche.

## Ajouter des copropriétaires aux tableaux

En tant que propriétaire ou copropriétaire existant d'un tableau, suivez ces étapes :

1. Depuis votre tableau de bord Miro, effectuez l’une des opérations suivantes :
   1. Pour un tableau, cliquez sur les trois points (**...**) et cliquez sur **Partager**.
   2. Ouvrez un tableau, puis cliquez sur **Partager** en haut à droite.
2. Saisissez l’adresse e-mail du ou des utilisateurs que vous souhaitez ajouter en tant que co-propriétaire.
3. Pour leurs droits d'accès, cliquez sur **Est copropriétaire**.
4. (Facultatif) Ajouter un message personnalisé.
5. Cliquez sur **Envoyer les invitations**.

> Vous pouvez attribuer le rôle de copropriétaire uniquement aux membres de l’équipe. Pour ajouter un co-propriétaire de l'extérieur de l'équipe, invitez-le d'abord à rejoindre l'équipe.

## Ajouter des copropriétaires aux Espaces

En tant que propriétaire d’un espace, ou co-propriétaire existant, suivez ces étapes :

1. Depuis votre tableau de bord Miro, effectuez l'une des opérations suivantes :
   1. Pour un Espace dans la barre latérale, cliquez sur les trois points (**...**) puis cliquez sur **Partager**.
   2. Ouvrez un espace, puis cliquez sur le libellé en haut qui indique le nombre de membres.
2. Cliquez sur **Gérer l’accès**.
3. Pour un membre de l’espace, mettez à jour ses droits d’accès en **Co-propriétaire.**

> Vous pouvez attribuer le rôle de copropriétaire uniquement aux membres de l’Espace. Pour ajouter un copropriétaire de l'extérieur de l'Espace, commencez par l'inviter à rejoindre l'Espace.

> Un copropriétaire d'Espace dispose des autorisations d'éditeur pour tout le contenu de cet Espace.

## Copropriétaires

### Autorisations du copropriétaire de tableau

En plus de toutes les autorisations d'éditeur, un copropriétaire de tableau dispose des autorisations suivantes :

- **Gérer les paramètres du contenu du tableau et les paramètres des outils de collaboration**
  Contrôler qui peut copier le contenu du tableau et gérer des outils comme le minuteur, le vote, le chat vidéo, le partage d’écran et la gestion de l’attention.
- **Masquer et révéler les cadres**
  Contrôlez la visibilité du contenu des cadres pendant les présentations ou ateliers.
- **Ajouter un verrouillage protégé**
  Empêchez le déplacement ou la suppression accidentelle de contenu pendant la collaboration.
- **Ajouter un mot de passe au tableau**
  Protégez les tableaux publics en exigeant un mot de passe pour l'accès.
- **Télécharger une sauvegarde du tableau**
  Créer des copies archivées des tableaux. Les copropriétaires peuvent également restaurer des tableaux à partir de sauvegardes.
- **Ajouter des copropriétaires**
  Attribuer le statut de co-propriétaire à d'autres utilisateurs.
- **Modifier les détails du tableau**
  Modifier la couverture et renommer le tableau
- **Partager le tableau**
  Modifier les droits d’accès de l’équipe et des autres utilisateurs sur le tableau
- **Configurer les autorisations avancées de partage du tableau**
  Préciser si le tableau peut être partagé en dehors de l’équipe ou de l’organisation

:::note
Dans les forfaits Enterprise, les copropriétaires de tableau et les administrateurs de contenu peuvent déplacer des tableaux en utilisant l'[API REST de Miro](https://developers.miro.com/reference/update-board), ce qui diffère intentionnellement de l'expérience de l'interface utilisateur de Miro, où seuls les propriétaires peuvent déplacer leurs tableaux.
:::

Un copropriétaire d'un tableau ne peut pas effectuer les opérations suivantes :

- Supprimer le tableau
- Déplacez le tableau vers une autre équipe.
- Changer le propriétaire du tableau

### Autorisations du copropriétaire de l'espace

En plus de toutes les autorisations d'éditeur, un copropriétaire de l'espace dispose des autorisations suivantes :

- Renommer l’espace
- Partager l’espace
- Modifier les droits d’accès de l’équipe et des autres utilisateurs dans l’Espace
- Ajouter des copropriétaires à l'Espace

Un copropriétaire de l'espace ne peut pas effectuer les opérations suivantes :

- Supprimer l’Espace
- Modifier le propriétaire de l’espace

## Foire aux questions

**Je n’ai pas la possibilité de désigner un copropriétaire. Pourquoi?**

La fonctionnalité de co-propriétaire est disponible sur les forfaits Business et Enterprise. L'administrateur de votre entreprise doit activer cette fonctionnalité dans les paramètres de l'équipe ou de l'entreprise. Seuls les membres existants de l’équipe peuvent être promus au rang de copropriétaires. Assurez-vous que l’utilisateur a été invité au tableau par e-mail avant de tenter d'assigner le rôle de copropriétaire.

**Je suis un admin avec les permissions d’administration du contenu activées. Pourquoi ne puis-je pas ajouter des copropriétaires au tableau ?**

Les admins disposant d’autorisations d’admin de contenu (CAP) doivent d’abord s’ajouter eux-mêmes comme propriétaires au tableau spécifique. Une fois qu'ils sont propriétaires d'un tableau, ils peuvent alors désigner des copropriétaires.

**Dois-je payer des frais supplémentaires pour les copropriétaires invités à mes tableaux ?**

Seuls les membres existants de l’équipe peuvent être désignés comme copropriétaires. Si l'utilisateur que vous souhaitez désigner comme co-propriétaire ne fait pas déjà partie de votre équipe, vous devez d'abord l'inviter à rejoindre l'équipe, ce qui peut nécessiter l'achat d'une place supplémentaire, en fonction de votre forfait et du nombre actuel d'utilisateurs. Après qu'ils sont membres de l'équipe, vous pouvez leur attribuer le rôle de copropriétaire.
