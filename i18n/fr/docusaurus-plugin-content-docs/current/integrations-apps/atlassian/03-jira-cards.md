---
title: Cartes Jira
article_id: 360017572434
translation_id: 6634753575954
locale: fr
sidebar_position: 5
created_at: '2022-07-15T14:23:14Z'
updated_at: '2025-11-25T15:59:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  plans: starter, business, education, enterprise
  notes: 'Utilisateurs: Tous les utilisateurs Plateformes: Navigateur, Bureau, Mobile
    Jira: Jira Cloud, Jira Server (sur site), Jira Data Center'
---

Les cartes Jira vous permettent de travailler sur des tickets Jira directement dans les tableaux Miro. Cette intégration simplifie le workflow de votre équipe en intégrant les tickets Jira dans votre espace collaboratif pour les rétrospectives, l'estimation des user stories, la priorisation du backlog, la cartographie des user stories et d'autres activités de l'équipe.

![Jira cards in user story mapping](../../../../../../docs/integrations-apps/atlassian/images/21017348097170_Jira%20cards%20in%20USM.png)

## Importer des tickets Jira sur votre tableau

Vous pouvez importer des tickets Jira sur votre tableau de deux façons :

1. Copiez l’URL du ticket Jira et collez-la sur le tableau.
2. Cliquez sur l’icône **Outils, Médias et Intégrations** (**+**) dans la barre d'outils de création, sélectionnez **Jira Cards**, choisissez un ou plusieurs tickets, puis cliquez sur **Ajouter**.

Lors de l'importation de tickets pour la première fois, vous devrez connecter votre compte Jira :

1. Cliquez sur **Autoriser** dans la boîte de dialogue qui apparaît.
2. Connectez-vous à votre compte Jira avec vos identifiants.
3. Autorisez la connexion entre Miro et Jira.

Après autorisation, vous verrez tous les tickets Jira auxquels vous avez accès dans le sélecteur de cartes Jira.

:::note
Les utilisateurs qui n'ont pas autorisé leur compte Jira verront une vue simplifiée des cartes sans les avatars des assignés.
:::

## Créer de nouveaux tickets Jira

Vous pouvez créer des tickets Jira directement depuis Miro de deux manières.

### Créer en utilisant l’application Jira

1. Cliquez sur l’icône **Outils, médias et intégrations** (**+**) dans la barre d’outils de création
2. Sélectionnez **Cartes Jira**.
3. Cliquez sur **Créer un ticket**.
4. Remplissez les champs requis.
5. Cliquez sur **Créer**.

### Convertir des éléments existants en tickets Jira

Vous pouvez convertir les cartes et pense-bêtes existants sur votre tableau en tickets Jira.

1. Sélectionnez jusqu’à 50 pense-bêtes ou cartes.
2. Cliquez sur **Convertir en** > **Jira** dans le menu contextuel.
3. Définissez les valeurs par défaut (type de ticket, priorité, personne assignée, etc.).
4. Cliquez sur **Convertir**.

:::warning
Remarque :

- Les cartes de la ligne des tâches USM ne peuvent pas être converties en tickets Jira.
- Lors de la conversion, les étiquettes et la date de début des cartes Miro ne seront pas conservées.
- Les informations concernant l’assignation doivent être redéfinies après la conversion.
:::

## Consulter et modifier les tickets Jira

:::warning
La modification des cartes Jira n'est pas prise en charge dans l'application de bureau ou l'application mobile.
:::

Vous pouvez consulter les cartes Jira de deux façons :

- Vue latérale
- Vue centrée

### Modifier les tickets dans Miro

1. Cliquez sur l'icône **Ouvrir dans le panneau latéral** ou **Ouvrir dans le panneau central**.
2. Effectuez vos modifications.
3. Cliquez sur **Mettre à jour** pour enregistrer.

### Modifier l'état du ticket

1. Cliquez sur l'icône **Workflow**.
2. Sélectionnez l'**État** et le **Commentaire** souhaités.
3. Cliquez sur **Mettre à jour** pour enregistrer.

### Modifier dans Jira

1. Sélectionnez une carte et cliquez sur l’icône **Source**.
2. Modifiez le ticket dans Jira dans le nouvel onglet du navigateur.
3. Les modifications se synchroniseront automatiquement avec la carte Miro.

## Synchronisation entre Miro et Jira

|  |  |
| --- | --- |
| **Mise à jour de l’instance Jira vs mise à jour de la carte Miro** | **Quand la mise à jour a-t-elle lieu ?** |
| Mise à jour dans Jira via OAuth 1.0 et OAuth 2.0 | La carte Miro Jira est mise à jour immédiatement via [webhook](https://help.miro.com/hc/articles/360017731113). |
| Mise à jour dans Miro | La carte Jira de Miro est immédiatement mise à jour et le ticket Jira correspondant est mis à jour simultanément. |

## Personnaliser les cartes Jira

### Changer les couleurs des cartes

1. Sélectionnez une ou plusieurs cartes Jira.
2. Cliquez sur **Couleur de remplissage** dans le menu contextuel.
3. Choisissez votre couleur désirée.

### Configurer des champs personnalisés

1. Cliquez sur l’icône **Outils, Médias et Intégrations** (**+**) dans la barre d’outils de création
2. Sélectionnez **Cartes Jira**.
3. Sélectionnez **Configurer les cartes**.
4. Sélectionnez les champs que vous souhaitez afficher.
5. Cliquez sur **Enregistrer**.

:::note
Notes importantes concernant les champs :

- Les paramètres s'appliquent uniquement au tableau actuel.
- Les champs par défaut (Assigné, Type de ticket, Priorité, État) ne peuvent pas être supprimés.
- Les champs peuvent ne pas s'afficher s'ils n'ont pas de valeur ou ne sont pas disponibles pour le type de ticket.
- Certains types de champs (comme les champs personnalisés de couleur) ne sont pas pris en charge.
:::

## Rechercher des tickets Jira

Le sélecteur de cartes Jira affiche d'abord les tâches récentes et offre plusieurs options de tri :

- Type de ticket
- Priorité
- Clé
- Résumé
- Destinataire
- État

Utilisez des mots-clés pour trouver des tickets spécifiques ou utilisez le **Jira Query Language** (JQL) pour des recherches complexes :

1. Sélectionnez l’option **Recherche avancée** dans la barre de recherche.
2. Entrez votre requête JQL.

Les résultats seront mis à jour en fonction de votre requête.

## Articles relatifs

- [FAQ sur les cartes Jira](https://help.miro.com/hc/articles/360013463739)
- [Configurer et désinstaller les cartes Jira](https://help.miro.com/hc/articles/360019501754)
- [Configurer des webhooks pour les cartes Jira](https://help.miro.com/hc/articles/360017731113)
- [Résoudre les problèmes des cartes Jira](https://help.miro.com/hc/articles/360017572654)
