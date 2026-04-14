---
title: Comment configurer l’authentification unique OKTA
article_id: 360023901054
translation_id: 360023901054
locale: fr
sidebar_position: 7
created_at: '2019-05-31T11:32:41Z'
updated_at: '2025-11-25T16:05:05Z'
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

[Si vous souhaitez paramétrer une instance de test avant d’activer l’authentification unique pour la production, veuillez contacter l’équipe du service d’assistance pour obtenir de l’aide.](https://help.miro.com/hc/requests/new?referer=help-center-article) Seules les personnes qui configurent l’authentification unique seront ajoutées à cette instance de test.

> **⚠️ Consultez notre article principal sur l’authentification unique** [**ici**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **pour découvrir les règles, les fonctionnalités prises en charge et les configurations optionnelles du côté de Miro.**

## Configuration d’Okta

### Ajouter et configurer l’application

Cliquez sur l’onglet **Applications** et choisissez **Catalogue des applications du navigateur** :

browse_app_catalog.jpg
Section des applications dans Okta

Recherchez notre application préconfigurée pour une configuration facile et cliquez sur **Ajouter** :

Miro_pre-configured_app.jpg
Miro dans le catalogue de l’application Okta

Donnez à l’application dans votre galerie le badge de votre choix (les autres étapes sont facultatives) et cliquez sur **Suivant** pour basculer sur l’onglet **Options de connexion** :

general_settings.jpg
Les paramètres généraux de l’application Miro

Dans **Options de connexion**, toutes les valeurs attendues sont déjà remplies et aucune donnée supplémentaire n’est requise.

:::warning
Vous pouvez ajouter des valeurs personnalisées si vous le souhaitez, mais assurez-vous que l’**État du relais par défaut** reste *vide* : nos applications autonomes utilisent la redirection vers le navigateur de l’utilisateur final pendant la procédure d’authentification et génèrent pour cela des valeurs RelayState uniques. Si vous utilisez une valeur par défaut, Okta écrasera nos données et vos utilisateurs ne pourront accéder qu’à la version de navigateur de Miro, et pas aux applications autonomes (bureau, tablette, mobile).
:::

sign-on_options.jpg
Méthodes de connexion

Cliquez sur **Terminer**. Vous pourrez revenir et modifier d’autres champs plus tard si nécessaire.

### Format du nom d’utilisateur

> Le **format du nom d’utilisateur de l’application** est défini par défaut sur **Nom d’utilisateur Okta**, ce qui est suffisant si votre nom d’utilisateur est au format adresse e-mail. Autrement, définissez le nom d’utilisateur comme étant une **adresse e-mail.**

:::warning
L’adresse e-mail est l’identifiant principal par lequel l’utilisateur est reconnu dans Miro. Elle ne doit pas être mise à jour du côté d’Okta, sauf si vous avez activé le SCIM. Si vous n’utilisez pas le SCIM, mais que vous avez besoin de mettre à jour les adresses e-mail de vos utilisateurs finaux, veuillez contacter notre [service d’assistance](https://help.miro.com/hc/requests/new?).
:::

### Configuration des images de profil (facultatif)

La configuration d’un attribut personnalisé comme ProfilePicture (Image de profil) peut être considérée comme un processus à part entière. Veuillez suivre ce [guide](https://drive.google.com/file/d/1go4BJWzFpQS5R04WdN1Q4O5Dy93k4wGp/view) pour configurer l’attribut du côté d’Okta et activer par la suite l’[exigence de ProfilePicture (Image de profil)](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) du côté de Miro.

## Configuration de Miro

Faites défiler la page jusqu’à **Certificats de signature SAML** pour obtenir les métadonnées du fournisseur d’identité (IdP). Si vous n’avez pas de certificats émis, commencez par en créer un.

Après cela, cliquez sur **Actions** et choisissez **Consulter les métadonnées de l’IdP** comme suit :

view_Idp_metadata.jpg
Obtention des métadonnées de l’IdP

Un onglet séparé contenant toutes les informations s’ouvrira.  Copiez le certificat à partir de la ligne commençant par &lt;ds:X509Certificate&gt; et collez-le dans les paramètres d’authentification unique de Miro dans le champ Clé certificat x509/span>**.**

certificate_in_Miro_SSO_settings.jpg
 /span>Clé certificat x509 dans les paramètres d’authentification unique de Miro

Revenez à la page des métadonnées et copiez l’URL à partir de la ligne **SingleSignOnService** après **Location=** et collez-la sur l’**URL de connexion SAML**.

Tout est prêt !

L’étape finale des paramètres Miro consiste à ajouter vos domaines et [à les vérifier](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Vous pouvez également configurer les paramètres facultatifs.

Si vous rencontrez un problème, veuillez consulter [notre liste des cas usuels et comment les résoudre.](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)

## Test de la configuration SSO dans Miro

1. Suivez les étapes ci-dessus pour configurer vos paramètres SSO.
2. Cliquez sur le bouton **Tester la configuration SSO**.
3. Examinez les résultats :

- Si aucun problème n’est détecté, un message de confirmation indiquant que **le test de configuration SSO a réussi s’** affiche.
- Si des problèmes sont détectés, un message de confirmation indiquant que **le test de configuration SSO a échoué s’** affiche, suivi de messages d’erreur détaillés pour vous indiquer ce qui doit être corrigé.

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Test de la configuration SSO dans Miro*
