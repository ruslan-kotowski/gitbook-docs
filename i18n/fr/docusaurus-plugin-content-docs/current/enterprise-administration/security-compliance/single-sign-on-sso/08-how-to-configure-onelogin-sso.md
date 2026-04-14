---
title: Comment configurer l’authentification unique OneLogin
article_id: 360022547134
translation_id: 360022547134
locale: fr
sidebar_position: 8
created_at: '2019-05-07T13:32:16Z'
updated_at: '2025-02-26T11:22:04Z'
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

## Configuration de Onelogin

### Ajouter et configurer l’application

La configuration de OneLogin dans Miro est simple car OneLogin propose une application Miro fonctionnelle préconfigurée dans son catalogue d’**applications**.

Miro_in_OneLogin_apps.jpg
Miro dans le catalogue d’applications OneLogin

Cliquez sur le bouton **Enregistrer**.

save_button.jpg
Onglet de configuration de l’application dans OneLogin

## Configuration de Miro

Après avoir enregistré la configuration, la section des paramètres de l’application s’ouvrira immédiatement. Passez sur l’onglet **SSO** pour obtenir votre **URL de connexion** et votre **certificat x509**.

sso_tab.jpg
Onglet SSO

Vous verrez ci-dessous une liste dURLs. Copiez l’URL **SAML 2.0 Endpoint (HTTP)** :

SAML_endpoint.jpg

et ***collez***-la dans le champ **URL de connexion SAML** de Miro :

sign-in_URL.jpg
**Champ URL de connexion SAML Miro**

Retournez sur l’onglet SSO de l’application OneLogin et cliquez sur **Consulter les détails** pour copier le **certificat x509**.

view_details.jpg
Bouton Consulter les détails

copy_certificate.jpg
**Copie du certificat x509**

Collez le certificat dans le champ **certificat x509** de Miro.

certificate_in_Miro_SSO_settings.jpg
**Champ certificat x509 dans les paramètres d’authentification unique de Miro**

L’étape finale des paramètres Miro consiste à ajouter vos domaines et [à les vérifier](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Vous pouvez également configurer les paramètres facultatifs.

Tout est prêt et maintenant vos utilisateurs pourront s’authentifier dans Miro via l’authentification unique !

Si vous rencontrez un problème, veuillez consulter [notre liste des cas usuels et comment les résoudre.](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)

## Test de la configuration SSO dans Miro

1. Suivez les étapes ci-dessus pour configurer vos paramètres SSO.
2. Cliquez sur le bouton **Tester la configuration SSO**.
3. Examinez les résultats :

- Si aucun problème n’est détecté, un message de confirmation indiquant que **le test de configuration SSO a réussi s’** affiche.
- Si des problèmes sont détectés, un message de confirmation indiquant que **le test de configuration SSO a échoué s’** affiche, suivi de messages d’erreur détaillés pour vous indiquer ce qui doit être corrigé.

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Test de la configuration SSO dans Miro*
