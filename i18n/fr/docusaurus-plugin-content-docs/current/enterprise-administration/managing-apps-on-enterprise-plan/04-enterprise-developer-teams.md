---
title: "\xC9quipes de d\xE9veloppement Enterprise"
article_id: 4766759572114
translation_id: 4766759572114
locale: fr
sidebar_position: 4
created_at: '2022-03-22T14:13:15Z'
updated_at: '2025-04-29T13:25:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: developer-teams
---

Découvrez l’option permettant de configurer des équipes de développement au sein des abonnements Enterprise, un moyen facile et sécurisé de créer des applications personnalisées pour votre plan Enterprise.

> **Disponible pour** : [Plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Installation par :** les admins d’entreprise
> Les utilisateurs d'autres plans Miro peuvent créer des équipes de développeurs à partir de [cette page.](https://developers.miro.com/docs/rest-api-build-your-first-hello-world-app#step-1-create-a-developer-team-in-miro)

### Création d’une équipe de développement

Pour configurer une équipe de développement, rendez-vous dans les paramètres **Company** (Entreprise) > **Teams** (Équipes) et cliquez sur **Create new team** (Créer une équipe) dans le coin supérieur droit.

Dans la fenêtre contextuelle suivante, insérez le nom de l’équipe et [choisissez son niveau d’accès : vous pouvez définir les paramètres d’accès par défaut ou sélectionner une équipe et copier ses autorisations (en savoir plus sur les](../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md) autorisations et les paramètres par défaut).  Cochez la case **Équipe de développeurs**, confirmez votre autorisation et cliquez sur **Créer une équipe**.

![create-dev-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803173266_create-dev-team.png)
Créer une équipe de développement

### Autorisations d’une équipe de développement Enterprise

Vous pouvez créer des applications en toute sécurité pour l’équipe de développement Enterprise, qui vous offre toutes les fonctionnalités de sécurité Enterprise tout en faisant partie de votre abonnement Enterprise.

L’équipe de développement Enterprise dispose d’un nombre illimité de tableaux et de membres.

Les tableaux créés dans cette équipe seront dotés d’un filigrane qui les différenciera des autres équipes de l’organisation.

L’équipe dispose des paramètres standard permettant de configurer les autorisations des utilisateurs sur un forfait Enterprise : vous pouvez autoriser/interdire les membres de l’équipe à/de inviter de nouveaux utilisateurs, partager des tableaux avec l’équipe/l’entreprise/via un lien public, déplacer des tableaux, restreindre l’accès aux domaines autorisés, etc. Pour plus d’informations, consultez [cet article](../managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md).

### Créer et installer des applications

> **Installation par :** admins d’équipe
> Si vous souhaitez inviter des développeurs à créer une application dans l'équipe, veillez à [leur accorder les droits d'admin d'équipe.](../../administration/user-management/06-how-to-manage-admin-roles.md)

[Pour créer une nouvelle application sur votre compte Miro Enterprise via une équipe de développement Enterprise, rendez-vous dans](../../using-miro/managing-your-profile/01-profile-settings.md) ****Profile settings** (Détails du profil) > Your apps (Vos applications),** **acceptez les conditions générales et cliquez sur** Create new app (Créer une application).

![profil-creer-nouvelle-application.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780634770_profile-create-new-app.png)
Vos applications dans les détails du profil

:::tip
Vous pouvez également accéder à la page en cliquant sur **Construire une application** dans le coin supérieur droit du tableau de bord de l'équipe des développeurs.
:::

![dev-team-build-an-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780641298_dev-team-build-an-app.png)
L’option permettant de créer des applications personnalisées

**Insérez le nom de l’application, sélectionnez votre équipe de développement pour l’application et cliquez sur** Create app (Créer l’application).

create_a_new_app.jpg
Création d’une application pour une équipe de développement Enterprise

**Sur la page de l’application, faites défiler vers le bas et sélectionnez les accès que vous souhaitez accorder à votre application, puis cliquez sur** Install app and get OAuth token (Installer l’application et obtenir un jeton OAuth).

app_permissions.jpg
Autorisations de l’application

Lors de l’installation de l’application, sélectionnez une équipe (différente de l’équipe de développement) dans le compte Enterprise de votre organisation et cliquez sur **Install & authorize** (Installer et autoriser). Le jeton d’accès sera affiché à l’étape suivante.

installing_the_app.jpg
Installer l’application

### Supprimer une équipe de développement

Vous pouvez supprimer l’équipe de développement comme toute autre équipe de votre organisation souscrite au forfait Enterprise mais vous devez d’abord supprimer toutes les applications créées dans cette équipe. Une fois les applications supprimées, accédez à [**Équipes**](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md), cliquez sur le nom de l'équipe, sélectionnez l'onglet **Profil**, puis **Supprimer l'équipe**.

:::warning
Notez qu’une fois l’équipe de développement du forfait Enterprise supprimée, les jetons associés à celle-ci ne seront plus valides.
:::

![delete-dev-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803181586_delete-dev-team.png)*Supprimer l'équipe de développeurs Enterprise*
