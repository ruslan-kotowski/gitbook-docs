---
title: Configurer Glean pour Miro (guide de l'admin)
article_id: 27581463837330
translation_id: 27581463837330
locale: fr
sidebar_position: 2
created_at: '2025-06-23T10:52:57Z'
updated_at: '2026-01-02T09:57:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Prérequis

1. Vous êtes un **admin de l’organisation Miro** et un **admin Glean**.
2. Dans Glean, **enregistrez un ID client OAuth.** Consultez la [documentation Glean](https://developers.glean.com/api-info/client/authentication/oauth) pour plus de détails.
3. Activez le paramètre de confidentialité au niveau utilisateur **Autoriser l'historique des chats à être sauvegardé jusqu'à 30 jours**.

## Installer l'application Glean

Pour commencer, installez l'application Glean depuis le Marketplace de Miro pour les équipes pertinentes de votre organisation.

1. Accédez aux paramètres de votre **Entreprise** et cliquez sur **Applications & Intégrations**.
2. Sous l'onglet **Applications**, cliquez sur **Ajouter des applications** pour ouvrir le Marketplace.
3. Recherchez "Glean". Vous pouvez aussi le trouver en collant son ID client dans la barre de recherche : `1202342442818548396`.
4. Depuis le profil de l'application, sélectionnez où ajouter l'application : soit pour **Toutes les équipes** soit sélectionnez **Équipes spécifiques...**.
5. Examinez la page des autorisations. L'application Glean est développée et maintenue par Miro et ne nécessite pas de permissions spécifiques.
6. Sélectionnez **Ajouter** pour terminer l'installation.

## Configuration de l'authentification unique (Okta)

Si votre organisation utilise Okta comme fournisseur d'authentification unique (SSO), vous devez créer une application Web Okta OpenID Connect (OIDC) avant de passer aux sections suivantes.

1. Créez une nouvelle application Okta en suivant les étapes mentionnées dans la documentation [ici](https://help.okta.com/en-us/content/topics/apps/apps_app_integration_wizard_oidc.htm).
   1. Sélectionnez **OIDC - OpenID Connect** comme méthode de **connexion**.
   2. Sélectionnez **Application Web** comme type d'application.
   3. Assurez-vous que le **Jeton de rafraîchissement** est **activé** dans les paramètres **Grant type** > **Core grants**.
   4. Ajoutez `https://integrations.miro.com/api/external-auth/oauth2/callback` dans les **URIs de redirection à la connexion**.
   5. Sélectionnez **Enregistrer**.
2. Copiez l'**identifiant client** et le **secret client** de la section Identifiants du client. Ceux-ci seront nécessaires dans les prochaines sections pour terminer la configuration de l'intégration.

## Configurer l'authentification unique (SSO)

Suivez ces étapes pour configurer l'application :

1. Depuis la page **Applications et intégrations**, accédez à **Gérer les applications**.
2. Trouvez "Glean" dans votre liste d'applications installées et cliquez sur ses **Paramètres**. Si vous ne voyez pas l'application, cherchez-la par identifiant client (`1202342442818548396`) et approuvez-la d'abord.
3. Dans les paramètres de configuration, sélectionnez le **fournisseur d'authentification unique (SSO)**.
   1. Okta
   2. Azure
   3. Google
4. Entrez les détails requis pour l'authentification unique.
   1. Okta : **URL de base Glean, détails de l'application Okta (URL du serveur d'autorisation**, **URL du token d'accès**, **ID client**, **Secret client**).
   2. Azure : **URL de base Glean**.
   3. Google : **URL de base Glean**.
5. Cliquez sur **Enregistrer** pour appliquer la configuration.

:::note
Si vous utilisez Azure, assurez-vous que votre admin Microsoft Entra a sélectionné « Consentir au nom de votre organisation » pour l'application Glean dans le centre d'admin Microsoft Entra afin de permettre aux utilisateurs de s'authentifier correctement.
:::

## Configurer la console d’admin Glean

Avant d'utiliser Glean dans Miro, vous devez configurer l'accès basé sur un jeton OAuth dans votre console d’admin Glean.

1. Ouvrez votre **console d'admin Glean** et allez dans **Paramètres** > **Accès tiers (OAuth)**.
2. Dans la section **OAuth configuré par l'IdP**, activez **Activer l'OAuth de l'IdP pour l'accès API**.
3. Cliquez sur **Gérer les paramètres**, sélectionnez votre **fournisseur SSO**.
4. Remplissez les détails du fournisseur selon votre fournisseur SSO.
   - **Okta**
     - URL du serveur d'autorisation : `https://<sous-domaine>.okta.com`
     - Identifiant(s) client autorisé(s) : Identifiant client de l'application Okta créée dans la section précédente.
     - Le reste des champs du formulaire peut être laissé vide.
   - **Azure**
     - Sous-domaine de l'émetteur : `https://login.microsoftonline.com/<tenant-id>/v2.0`
     - Identifiant(s) client autorisé(s) : `a49fdb25-3b5f-4d3b-bedf-6da7be2b4bf4`
   - **GSuite**
     - Identifiant(s) client autorisé(s) : `1062019541050-pf2ndc9f3o4lrmkupj3cj0fep5hkecns.apps.googleusercontent.com`
5. Sélectionnez **Enregistrer** pour appliquer les paramètres.

> ⏰ **Remarque :** Les modifications peuvent prendre jusqu'à 30 minutes pour être prises en compte dans la console d’admin de Glean.

## Utiliser l’application Glean

Une fois que vous avez installé et configuré l'application, les utilisateurs des équipes désignées peuvent commencer à l'utiliser. La première fois qu'un utilisateur ouvre l’application Glean dans Miro, il sera invité à s'authentifier.

1. Ouvrez un tableau Miro et cliquez sur l'icône Glean dans la barre d'outils pour ouvrir le panneau latéral.
2. Cliquez sur **Connecter Glean** pour démarrer l'autorisation.
3. Une boîte de dialogue d'autorisation SSO apparaîtra.
4. Après une authentification réussie, l'interface utilisateur de Glean s'affichera, prête à l'emploi.

## Sécurité

Pour plus d’informations sur les données et la sécurité, consultez ce [document de sécurité](https://docs.google.com/document/d/1lGLF7eASQb2uMRmMEAaH-GzFhyz4UKfwMeqSQOSYPdM/edit?tab=t.0#heading=h.gu9ng058yy7y).
