---
title: Comment configurer l’authentification unique AWS
article_id: 360014798100
translation_id: 360014798100
locale: fr
sidebar_position: 4
created_at: '2020-07-01T20:03:44Z'
updated_at: '2025-02-26T11:33:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible pour: [Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md),
    Plans d''[affaires](../../../plans-billing/miro-plans/06-business-plan.md) Installation
    par: les admins d’entreprise'
---

> *Il est fortement recommandé de configurer l’authentification unique dans une fenêtre indépendante de votre navigateur, en mode navigation privée.* De cette façon, votre session reste active dans la fenêtre standard, ce qui vous permet de désactiver l’autorisation de l’authentification unique si quelque chose est mal configuré.

Si vous souhaitez configurer une instance de test avant d’activer l’authentification unique en production, veuillez en faire la demande auprès de votre responsable de compte ou de votre représentant commercial ou représentante commerciale. Seules les personnes qui configurent l’authentification unique seront ajoutées à cette instance de test.

> **⚠️ Consultez notre article principal sur l’authentification unique** [**ici**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **pour découvrir les règles, les fonctionnalités prises en charge et les configurations optionnelles du côté de Miro.**

## Prérequis

Vous aurez besoin des éléments suivants pour configurer l’authentification unique AWS pour accéder à Miro :

1. Accès à la console d’authentification unique AWS avec les autorisations IAM pour gérer les applications
2. Des autorisations d’admin d’entreprise dans les forfaits Enterprise ou Business de Miro

## Instructions d’installation

1. Sur la page de configuration de l’authentification unique AWS, ajoutez une nouvelle application et recherchez **Miro**.    Lors de l'ajout de l'application Miro, le nom d'affichage et la description peuvent être mis à jour.
   application_catalog.jpg
   Catalogue d'applications AWS SSO
2. Connectez-vous au tableau de bord Miro dans une autre fenêtre du navigateur.  Nous vous recommandons d’utiliser une fenêtre de navigation privée indépendante./span>
3. En haut à droite, cliquez sur l’icône de votre profil, puis rendez-vous dans **Paramètres**.  Dans le panneau de gauche, assurez-vous que la bonne équipe est sélectionnée dans le menu déroulant dans le coin supérieur gauche.
4. Dans le panneau de gauche, rendez-vous dans **Intégrations Enterprise** (Les utilisateurs du forfait Business doivent aller dans **Sécurité**) et activez l’option **Activer SSO/SAML**.  Saisissez la valeur suivante pour l’URL de connexion SAML à partir de l’authentification unique AWS.

application_configuration_page.jpg
Page de configuration de l’application d’authentification unique AWS

5. Téléchargez le fichier des métadonnées SAML d’authentification unique AWS et copiez-collez le certificat X509 dans **Clé certificat x509**.  Votre configuration dans Miro devrait maintenant ressembler à la configuration ci-dessous.

Miro_SSO_settings.jpg
Paramètres de configuration de l’authentification unique de Miro

6. Dans la configuration de l’authentification unique de Miro, saisissez le nom de domaine de l’adresse e-mail de votre entreprise dans **Domaines**.  Assurez-vous d’avoir ajouté au moins un domaine d’entreprise.
7. Cliquez sur **Enregistrer** pour enregistrer les modifications.
8. Revenez à votre application pour Miro dans la console web de l’authentification unique AWS.  Dans les métadonnées de l’application, vérifiez que les valeurs suivantes ont été saisies. Elles devraient automatiquement s’afficher si vous avez recherché et ajouté l’application Miro au lieu de créer une application personnalisée.
9. |  |  |
   | --- | --- |
   | **Champ** | **Valeur** |
   | URL de l’application ACS | [https://miro.com/sso/saml](https://Miro.com/sso/saml) |
   | Audience de d’application SAML | https://miro.com/ |
10. Choisissez **Enregistrez les modifications**.
11. [Assignez un utilisateur](https://docs.aws.amazon.com/singlesignon/latest/userguide/assignuserstoapp.html) à l’application dans les Utilisateurs assignés à l’application de la console de l’authentification unique AWS.

Et c’est tout ! La configuration de l’authentification unique est maintenant terminée.

Veuillez consulter [cet article](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md) si vous souhaitez également activer le provisionnement automatique pour Miro.

## test

Utilisez la section suivante pour vérifier l’intégration de l’authentification unique.  Avant la vérification et d’effectuer les étapes ci-dessous, assurez-vous que l’utilisateur qui l’effectue est déconnecté à la fois de l’authentification unique AWS et Miro. Les utilisateurs ne pourront se connecter à l’aide de l’authentification unique que si l’utilisateur existe dans votre répertoire, qu’il est membre de votre forfait Miro Enterprise ou Business et que l’utilisateur est affecté à l’application./span>

### Vérification de l’authentification unique initiée par l’IdP à partir de l’authentification unique AWS

1. Accédez au portail de l’utilisateur final de l’authentification unique AWS à l’aide des identifiants d’un utilisateur affecté à l’application Miro.
2. Dans la liste des applications, choisissez l’application Miro pour lancer une connexion sur Miro.
3. Si la connexion est réussie, vous arriverez sur le tableau de bord de Miro.

### Vérification de l’authentification unique lancée par le fournisseur de services à partir de Miro.

1. Rendez-vous sur [https://miro.com/login/](https://Miro.com/login/) et choisissez **Se connecter avec l’authentification unique**.  Saisissez ensuite votre adresse e-mail professionnelle.
2. Vous serez redirigé(e) vers le portail d’authentification unique AWS, dans lequel vous saisirez les identifiants d’un utilisateur affecté à l’application dans la console d’authentification unique AWS.
3. Si la connexion est réussie, vous arriverez sur le tableau de bord Miro.

### Vous pouvez également tester dans Miro

1. Suivez les étapes ci-dessus pour configurer vos paramètres SSO.
2. Cliquez sur le bouton **Tester la configuration SSO**.
3. Examinez les résultats :
   1. Si aucun problème n’est détecté, un message de confirmation indiquant que **le test de configuration SSO a réussi s’** affiche.
   2. Si des problèmes sont détectés, un message de confirmation indiquant que **le test de configuration SSO a échoué s’** affiche, suivi de messages d’erreur détaillés pour vous indiquer ce qui doit être corrigé.![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)*Test de la configuration SSO à partir de Miro*

## Résolution des problèmes

Pour la résolution des problèmes génériques, veuillez consulter le [Guide de résolution des problèmes liés à l’authentification unique AWS](http://docs.aws.amazon.com/singlesignon/latest/userguide/troubleshooting.html).
