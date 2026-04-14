---
title: Comment configurer Auth0 SSO
article_id: 360022496573
translation_id: 360022496573
locale: fr
sidebar_position: 3
created_at: '2019-05-01T18:33:32Z'
updated_at: '2025-02-26T11:43:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible pour: les forfaits Business et Enterprise Installation par: les
    admins d’entreprise'
---

*Il est fortement recommandé de configurer cette fonctionnalité dans une fenêtre distincte de votre navigateur, en navigation privée.* *Ainsi, vous conservez la session dans la fenêtre standard, ce qui vous permet de désactiver l’autorisation du SSO au cas où quelque chose serait mal configuré.*

Si vous souhaitez configurer une instance de test avant d’activer l’authentification unique (SSO) en production, veuillez en faire la demande auprès de votre responsable de compte ou de votre représentant commercial ou représentante commerciale Miro. Seules les personnes qui configurent l’authentification unique seront ajoutées à cette instance de test.

## Créer l’application Miro au sein de votre hébergeur

1. Créez l’application dans votre liste d’**Applications**.
   create_application_button.jpg
   *Section des applications Auth0*
2. Sélectionnez le type d'application **Applications Web régulières**.
   application_types_list.jpg
   *Liste des types d'application*
3. Accédez à l’onglet **Settings (Paramètres)** et assurez-vous que les options répertoriées sont sélectionnées exactement de la manière décrite ci-dessous.
   ![mceclip0.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017725482002_mceclip0.png)


   |  |  |
   | --- | --- |
   | **Token Endpoint Authentication Method** | POST |
   | **Allowed Callback URLs** | `https://miro.com/sso/saml` |
   | **Application Login URI** | `https://miro.com/sso/saml` |
   | **Origines autorisées (CORS)** | `https://miro.com/` |
   | **Expiration JWT** | 36000 (Défini par défaut) |
4. Cliquez sur **Afficher les paramètres avancés**:
   ![mceclip1.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017725485074_mceclip1.png)

   puis allez dans **Certificats** et copiez votre certificat de signature x509 :
   copy_the_certificate.jpg
   *Onglet Paramètres avancés dans Auth0*
5. Passez à Miro et ouvrez vos paramètres SSO (les administrateurs du plan Business trouveront les paramètres dans l'onglet **Sécurité**, les administrateurs du plan Enterprise devront aller dans l'onglet **Intégrations Enterprise** ), puis collez le **certificat de signature x509** dans le champ correspondant, comme indiqué dans la capture d'écran ci-dessous :
   certificate_in_Miro_SSO_settings.jpg
   *Onglet **Sécurité** Miro avec paramètres SAML*

## Paramétrer SAML pour l’application

1. Retournez à la page de configuration de l'application Auth0 et choisissez l'onglet **Addons** et l'addon **SAML2**:
   add-ons_catalog.jpg
   *Catalogue d'add-ons Auth0*Une fenêtre contextuelle s'affiche avec les paramètres de la demande et l'URL de rappel de l'application **:
   add-on_settings.jpg***Onglet Addon **Settings***
2. Veillez à ce que l'**URL** soit définie comme suit : **`https://miro.com/sso/saml`**Les **paramètres de** la demande doivent être définis comme suit :

   ```
    "nameIdentifierFormat" : "urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress",
    "nameIdentifierProbes" : [
    "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress"
   ```
3. Basculez les onglets sur **Usage** et copiez l'URL de connexion du fournisseur d'identité **:**![](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017695812626_mceclip2.png)mceclip2.png
   *Champ de l'URL de connexion du fournisseur d'identité dans Auth0*
4. Passez à nouveau sur Miro et collez l’URL dans le champ **SAML Sign-in URL** (URL de connexion SAML).
5. Cliquez sur **Save** (Enregistrer) pour appliquer les paramètres à votre plan Miro.

## Vérification de la configuration

Vous pouvez maintenant revenir sur la console Auth0 et basculer sur l’onglet **Settings** (Paramètres) du module complémentaire.  Cliquez sur Debug pour déclencher la tentative de connexion.

debug.jpg
Déclenchement de la tentative de connexion

Cela initiera la tentative de connexion de l’IdP et vous permettra de voir les résultats.

En cas de difficultés - n’hésitez pas à [contacter l’équipe de notre Service d’assistance](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)

## Test de la configuration SSO dans Miro

1. Suivez les étapes ci-dessus pour configurer vos paramètres SSO.
2. Cliquez sur le bouton **Tester la configuration SSO**.
3. Examinez les résultats :

- Si aucun problème n’est détecté, un message de confirmation indiquant que **le test de configuration SSO a réussi s’** affiche.
- Si des problèmes sont détectés, un message de confirmation indiquant que **le test de configuration SSO a échoué s’** affiche, suivi de messages d’erreur détaillés pour vous indiquer ce qui doit être corrigé.

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Test de la configuration SSO dans Miro*
