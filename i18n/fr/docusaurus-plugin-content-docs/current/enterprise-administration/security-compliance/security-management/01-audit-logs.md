---
title: Journaux d’audit
article_id: 360017571434
translation_id: 360017571434
locale: fr
sidebar_position: 1
created_at: '2019-02-11T10:09:04Z'
updated_at: '2026-03-12T09:21:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible pour: Forfait Enterprise Configuration par: Admins d’entreprise'
---

Les journaux d’audit permettent aux admins de l’organisation disposant des privilèges appropriés de suivre l’activité des utilisateurs dans leur organisation Miro. Les journaux sont extrêmement utiles pour enquêter sur un problème ou obtenir un rapport détaillé sur des événements importants (par exemple, les modifications apportées aux paramètres de sécurité globaux, les invitations de nouveaux utilisateurs ou la création de nouveaux tableaux).

:::note
Actuellement, les événements sont enregistrés à partir du moment où l’abonnement Enterprise est créé et sont stockés pendant 180 jours par défaut :
a) Si vous changez de forfait pour Enterprise à partir d’un autre forfait, les événements seront enregistrés dès le moment du changement de forfait.
b) Si vous migrez certaines équipes vers l’abonnement Enterprise, leurs données ne seront enregistrées que lorsqu’elles feront partie de l’abonnement.
:::

## Accès aux journaux d’audit

Pour accéder aux journaux d’audit, procédez comme suit :

1. Accédez à **Paramètres d'entreprise**.
2. Dans le panneau de gauche, cliquez sur **Sécurité** > **Journaux d’audit**.
3. Vous pouvez filtrer les journaux d’audit en choisissant une **Période**, un **Auteur**, une **Catégorie d’événement** et un **Événement** spécifique.

Cliquez sur le bouton Afficher les événements pour visualiser les événements correspondant à vos critères de filtrage. L'heure est affichée au format **ISO 8601**, dans le fuseau horaire **local**. Vous pouvez consulter les détails d’un événement particulier en cliquant sur les trois points de la colonne **Détails**.

:::note
Seuls les événements survenus au cours des 90 derniers jours sont disponibles pour la prévisualisation.
:::

## Exporter les journaux d’audit

Vous pouvez exporter les journaux au format **CSV**.

Dans le fichier d’exportation CSV, la date et l’heure de l’événement sont fournies au format ISO 8601, fuseau horaire UTC. Il n’y a pas de limite au nombre d’enregistrements à exporter à la fois ; cependant, plus vous exportez de données, plus il faut de temps pour préparer le fichier à télécharger. N’oubliez pas non plus que les applications courantes permettant de travailler avec des tables ont leurs limites quant au volume de données qu’elles peuvent ouvrir.

Pour exporter les journaux, cliquez sur le bouton **Exporter au format CSV**.

La barre contenant les détails de votre fichier d’exportation apparaît ci-dessous. Lorsque le fichier est prêt à être téléchargé, vous pouvez cliquer sur le bouton Télécharger CSV. Le fichier sera disponible au téléchargement pendant 24 heures.

:::note
Actuellement, un seul fichier d’exportation peut être téléchargé par organisation à la fois. En cliquant sur le bouton **Exporter vers CSV**, vous remplacerez le fichier d’exportation actuel.
:::

## Accéder aux journaux d’audit via l’API

Les admins peuvent utiliser l'[API des journaux d’audit](https://developers.miro.com/reference/audit-logs) ou les [Intégrations SIEM](https://help.miro.com/hc/sections/4404757427090-Security-information-and-event-management-SIEM) prises en charge pour accéder de manière programmée et collecter les données des journaux d’audit.

## Suppression des journaux d’audit

Les admins peuvent définir une politique de conservation des journaux d’audit. Vous pouvez choisir entre 30, 90, 180 ou 365 jours.

:::warning
Une fois les journaux d’audit supprimés, ils ne peuvent pas être récupérés.
:::

:::note
La conservation indéfinie des journaux d’audit a été supprimée.
:::

Pour définir une période de suppression, procédez comme suit :

1. Allez dans les **Paramètres de l’entreprise**.
2. Dans le panneau de gauche, cliquez sur **Sécurité** > **Journaux d’audit**.
3. Sous **Journaux d’audit**, cliquez sur l’onglet **Paramètres**.
4. Choisissez une option dans la liste déroulante. Il vous sera demandé de confirmer votre choix.

## Les événements dans les journaux d’audit

Les journaux d’audit comprennent des enregistrements concernant les catégories d’événements suivantes :

**Administration**

- Modifier le nom de l’entreprise
- Modifier, supprimer le logo de l’entreprise
- Demande d’accès créée
- Demande d’accès refusée
- Activer, désactiver les métriques d'activité des utilisateurs dans Analytics
- Activer, désactiver ou modifier les paramètres de SSO/SAML
- Activer, désactiver le SCIM
- Générer un jeton pour l’API SCIM
- Activer, désactiver les notifications SCIM
- Activer, désactiver, modifier la [liste autorisée](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Activer, désactiver le partage avec les invités en dehors des domaines autorisés
- Activer, désactiver le partage [via un lien public](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Activer, désactiver le partage [via un lien public pour modification](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Activer, désactiver la [confidentialité de l’équipe](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Activer, désactiver, mettre à jour les paramètres de [contrôle de domaine](../../canvas-25-admin-features/domain-control/01-domain-control.md)
- Activer, désactiver [Bloquer les utilisateurs désactivés](../../user-management/02-block-deactivated-users.md)
- Modifier les [paramètres de gestion des demandes](../../user-management/09-request-management-on-enterprise-plan.md) (y compris le changement de l'e-mail ServiceNow ou de l'URL du service d'assistance)
- Créer, supprimer une équipe
- Modifier le nom de l’équipe
- Modifier, supprimer le logo de l’équipe
- Changer les [paramètres d'invitation de l'équipe](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Changer la [découverte de l'équipe](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Activer, désactiver les [invités pour une équipe](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Changer les [paramètres de partage par défaut du tableau](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Modifier [les paramètres de partage par défaut des projets](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Installer, désinstaller une application
- [Approuver, restreindre une application](../../../integrations-apps/integrations-basics/04-how-to-install-apps.md)
- [Modération de Miro IA](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md)

**Gestion des utilisateurs**

- Inviter un nouveau membre dans l’équipe
- Convertir un membre en invité
- Convertir un utilisateur en membre avec un accès complet
- Promouvoir un utilisateur au rôle d’admin d’entreprise, révoquer un admin d’entreprise
- Promouvoir un utilisateur au rôle d’admin d’équipe, révoquer un admin d’équipe
- Supprimer un utilisateur d’une équipe ou d’une entreprise (si un utilisateur quitte une équipe, il aura à la fois un rôle d’acteur et d’objet affecté)
- Révoquer une invitation
- Désactiver, réactiver un utilisateur
- Un utilisateur rejoint une équipe/une entreprise

**Tableaux**

- Ouvrir un tableau
- Créer, supprimer, restaurer un tableau
- Renommer un tableau
- Modifier la description d’un tableau
- Modifier la couverture d’un tableau
- Déplacer un tableau vers une autre équipe
- Ajouter un tableau à un projet, le supprimer d’un projet, le déplacer vers un autre projet
- Modifier le propriétaire d’un tableau
- Partager un tableau avec un lecteur/commentateur/éditeur
- Supprimer un utilisateur d’un tableau
- Activer, désactiver, changer le [lien public](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#partage-de-tableaux-via-un-lien-public) du tableau
- Activer, désactiver, changer le [mot de passe d'un tableau public](../../../using-miro/sharing-boards/13-password-protection-for-public-boards.md)
- Activer, désactiver, changer le [partage d’un tableau avec l’entreprise](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Activer, désactiver, changer le [partage d’un tableau avec l’équipe](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Exporter un tableau, télécharger un fichier depuis un tableau.
- État créé
- État mis à jour
- État supprimé
- Charger un fichier (obsolète, disponible dans le [journal de contenu](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md))

Veuillez noter que le journal d’audit **n’enregistre pas** d’informations relatives aux modifications apportées aux tableaux.

**Modèles**

- Ouvrir un modèle
- Créer, supprimer, restaurer un modèle
- Renommer un modèle
- Modifier le propriétaire d’un modèle
- État créé
- État mis à jour
- État supprimé

**Projets**

- Créer, supprimer un projet
- Renommer un projet
- Partager un projet avec un utilisateur, supprimer un utilisateur participant au projet
- Activer, désactiver le partage d’équipe pour un projet
- Modifier le propriétaire d’un projet

**Connexions**

- Se connecter
- Échec de la connexion
- Se déconnecter
- Profil verrouillé, déverrouillé

:::warning
Les événements relatifs aux connexions comprendront l’activité des [utilisateurs désactivés](../../user-management/01-deactivated-users.md).
:::

**Détails du profil**

- Modifier les détails du profil
- Demander un changement d’adresse e-mail
- Modifier l’adresse e-mail

**Plans d’action**

- Créer un plan d’action
- Supprimer un plan d’action
- Créer une section de plan d’action
- Supprimer une section de plan d’action
- Changer le propriétaire du plan d’action

**Miro IA**

- Utiliser la fonctionnalité Miro IA

### Foire aux questions

Existe-t-il un moyen d’extraire automatiquement les journaux d’audit ?

Oui, vous pouvez configurer l’[application Miro pour Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md) afin d'accéder aux journaux Miro depuis Splunk.
