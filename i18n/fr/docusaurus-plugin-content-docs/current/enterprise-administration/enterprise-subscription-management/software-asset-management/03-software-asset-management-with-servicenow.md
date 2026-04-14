---
title: Gestion des actifs logiciels avec ServiceNow
article_id: 360021758459
translation_id: 360021758459
locale: fr
sidebar_position: 3
created_at: '2021-05-20T05:00:32Z'
updated_at: '2025-02-26T11:53:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Analysez et personnalisez l’utilisation de votre abonnement à grande échelle à l’aide de l’intégration ServiceNow & Miro. Cette intégration vous permet d’obtenir la liste des utilisateurs non actifs et de les désactiver à partir de l’application de gestion des ressources.

> **Disponible pour** : [Plan Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Installation par :** les admins d’entreprise

## Fonctionnalités prises en charge

L’intégration vous donne accès aux fonctionnalités suivantes :

- **Téléchargement des abonnements**
  - Obtenez la liste de l’usage que les utilisateurs font de votre abonnement ainsi que la liste des licences allouées dans votre abonnement Miro Enterprise.
- **Récupération des abonnements**
  - Désactivez des utilisateurs de votre plan Miro Enterprise en fonction de leur utilisation de l’abonnement.

## Étapes de configuration

### intégration

1. Dans ServiceNow, accédez au module **SaaS License** (Licence SaaS) et sélectionnez l’option **Direct Integration Profiles** (Profils d’intégration directe), puis cliquez sur **New** (Nouveau) :

   saas_license_module.jpg
   Module SaaS License (Licence SaaS)

   > ✏️ Si le module **Saas License** n'est pas présent dans votre instance ServiceNow, vous devrez l'installer en suivant ces .
2. Recherchez **Miro Enterprise Integration Profile** (Profil d’intégration Miro Enterprise) :

   Miro_Enterprise_integration_profile.jpg
   Le profil d’intégration Miro Enterprise
3. Vous verrez deux flux secondaires prédéfinis pour **télécharger les abonnements** et **réclamer les abonnements**:
   download_subscription_sybflow.jpg
   *Télécharger Subscription Subflow*

   reclaim.jpg
   *Sous-flux de récupération des abonnements*

### Comment créer une nouvelle connexion

1. Pour créer une nouvelle connexion, allez dans **Identifiants et connexions** > **Alias de connexion et d'identifiant et** cliquez sur **Nouveau.**
   new_alias.jpg
   *La possibilité de créer un nouvel alias de connexion et d'identifiants*

  Cliquez sur le lien **Create New Connection (Créer une connexion)** :

create_connection.jpg
Connexion et alias

Pour le sous-flux **Download Subscriptions** (Télécharger les abonnements), vous devrez fournir le **Client ID** (ID client) et le **Client Secret** (Secret du client).

create_connection_modal.jpg
Création d’une connexion et d’un identifiant

2. Pour obtenir l'**ID client** et le **secret client de**  **,** du côté de Miro, allez dans **Paramètres > Paramètres du profil > Vos applications** et sélectionnez **Créer une nouvelle application.**

![](../../../../../../../docs/enterprise-administration/enterprise-subscription-management/software-asset-management/images/23921803379090_image.png)*Créez une nouvelle application dans les paramètres de votre profil*

3. Définissez le **nom de l'application**, sélectionnez une équipe et cliquez sur **Create app.** Notez que vous devez disposer d'une [équipe de développeurs](../../managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md).

4. 4. Sur la page de l’application, dans la section **Permissions** (Autorisations), vous devrez cocher l’option **organizations:read** et cliquer sur **Install app and get OAuth Token** (Installer l’application et obtenir le jeton OAuth).

5. 5. Sélectionnez une équipe faisant partie du compte Enterprise de votre organisation et installez l’application.

6. Copiez l'**identifiant** et le **secret du client sur****le site**  .

Pour le sous-flux **Récupérer les abonnements** , vous devrez fournir un jeton **API SCIM**. Pour obtenir un jeton API SCIM, dans Miro, accédez à la console d'administration et allez dans **Applications et intégrations** > **Intégrations Enterprise** > **SCIM Provisioning** et copiez le jeton sous **Jeton API.**

## Personnalisation de l’utilisation de l’abonnement

Par défaut, la valeur **Last activity threshold** (Limite de la dernière activité en date) est définie sur 60 jours.  Pour la modifier, rendez-vous sur Reclamation Rules (Règles de récupération) et sélectionnez la règle Miro, vous pourrez ensuite modifier la limite de la dernière activité en date comme suit :

last_activity_treshold.jpg
Limite de la dernière activité en date

## Problèmes éventuels et comment les résoudre

Lorsque vous essayez d'installer l'application pour une équipe, vous voyez apparaître le message d'erreur "We couldn't install this app. Vous ne pouvez pas installer cette application. Ses champs d'application ne sont pas disponibles dans votre plan actuel".
- C'est le comportement attendu lors de l'installation de l'application dans une équipe de développement, car l'équipe de développement n'a pas accès aux champs d'application au niveau de l'organisation. Vous devrez installer l’application dans l’une de vos équipes Enterprise dotée d’un accès à l’échelle de l’organisation pour l’intégration de ServiceNow.

install_app_error.jpg
L’erreur s’affichant lors de l’installation de l’application pour une équipe de développement
