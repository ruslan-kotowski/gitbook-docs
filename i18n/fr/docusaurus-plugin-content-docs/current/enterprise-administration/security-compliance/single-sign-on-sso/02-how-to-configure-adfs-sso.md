---
title: Comment configurer l’authentification unique ADFS
article_id: 360022411353
translation_id: 360022411353
locale: fr
sidebar_position: 2
created_at: '2019-04-29T20:13:47Z'
updated_at: '2025-11-25T16:04:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible pour: [Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md),
    Plans d''[affaires](../../../plans-billing/miro-plans/06-business-plan.md) Installation
    par: les admins d’entreprise'
---

Miro prend en charge les authentifications uniques (SSO) via SAML 2.0.

Un fournisseur d’identité SAML 2.0 peut prendre de nombreuses formes, y compris un serveur ADFS (Active Directory Federation Services) auto-hébergé. Un ADFS est un service fourni par Microsoft en tant que rôle standard pour Windows Server, qui fournit une connexion Web établie à l’aide des identifiants Active Directory existants.

Ce guide se fonde sur des captures d’écran de **Server 2012R2**, mais les étapes à suivre devraient être similaires sur d’autres versions.

Tout d’abord, vous devez installer l’ADFS sur votre serveur. Ce guide n’est pas axé sur la configuration et l’installation d’ADFS mais vous trouverez des instructions détaillées dans cet [article de Microsoft](http://msdn.microsoft.com/library/gg188612.aspx).

Pendant le test, assurez-vous que l’authentification de votre poste de travail est paramétrée sur la même adresse e-mail que celle que vous utilisez pour le test. Sinon, l’ADFS ne vous permettra pas de vous connecter même si la configuration et le profil sont corrects.

> *Il est fortement recommandé de configurer l’authentification unique dans une fenêtre indépendante de votre navigateur, en mode navigation privée.* De cette façon, votre session reste active dans la fenêtre standard, ce qui vous permet de désactiver l’autorisation de l’authentification unique si quelque chose est mal configuré.

Si vous souhaitez configurer une instance de test avant d’activer l’authentification unique en production, veuillez en faire la demande auprès de votre responsable de compte ou de votre représentant commercial ou représentante commerciale. Seules les personnes qui configurent l’authentification unique seront ajoutées à cette instance de test.

> **⚠️ Consultez notre article principal sur l’authentification unique** [**ici**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **pour découvrir les règles, les fonctionnalités prises en charge et les configurations optionnelles du côté de Miro.**

## Étape 1 - Ajout d’une approbation de partie de confiance

1) Connectez-vous au serveur de l’ADFS et lancez la **ADFS Management Console** (Console de gestion de l’ADFS).

2) Sélectionnez le dossier **Relying Party Trusts** (Approbations de partie de confiance) dans **AD FS Management** (Gestion AD FS) et ajoutez une nouvelle **Standard Relying Party Trust** (Approbation de partie de confiance standard) à partir de la barre latérale **Actions**. L’assistant de configuration démarre pour la création d’une nouvelle partie de confiance.

add_a_party_trust.jpg
Ajout d’une approbation de partie de confiance

3) Dans l’écran **Select Data Source** (Sélectionner la source de données), sélectionnez la dernière option, **Enter Data About the Party Manually** (Saisir les données relatives à la partie manuellement).

step_3.jpg
**Choix de l’option Enter Data About the Party Manually (Saisir les données relatives à la partie manuellement)**

4) Saisissez un **Display name (Nom d’affichage)** que vous pourrez reconnaître à l’avenir ainsi que toutes les notes que vous souhaitez faire.

display_name.jpg
Ajout d’un nom d’affichage

5) Sélectionnez le bouton **AD FS profile** (Profil AD FS) (ADFS 2.0).

step_5.jpg

next.jpg
Une invite de commande vous enjoindra à rechercher un certificat pour chiffrer et déchiffrer les revendications. Cette option est facultative et peut être ignorée en appuyant sur **Next** (Suivant).

6) Cochez la case **Activer la prise en charge du protocole SAML 2.0 WebSSO**.
L'URL du service sera https://miro.com/sso/saml.

**Notez** qu’aucune barre oblique n’est présente à la fin de l’URL.

step_6.jpg
Enable Support for the SAML 2.0 WebSSO protocol (Activer la prise en charge du protocole WebSSO SAML 2.0)

7) Ajoutez un **Relying party trust identifier** (Identificateur pour la partie de confiance), comme `https://miro.com/`

step_7.jpg
**Ajout d’un Relying party trust identifier (Identificateur pour la partie de confiance)**

*Sur l’écran suivant, vous pouvez configurer l’authentification multifactorielle. Ce guide n’est cependant pas axé sur cette configuration.*

rejecting_on_step_7.jpg
*Rejet de la configuration de l’authentification multifacteur*

8) Sélectionnez le bouton **Permit all users to access this relying party** (Autoriser tous les utilisateurs à accéder à cette partie de confiance).

step_8.jpg
Autoriser l’accès de tous les utilisateurs à la partie de confiance

Sur les deux écrans suivants, l’assistant affiche un aperçu de vos paramètres.

Sur l’écran final, cliquez sur le bouton **Close**(Fermer) pour quitter et ouvrir l’éditeur **Claim Rules** (Règles de revendication).

final_step.jpg
Finition de l’ajout d’une approbation de partie de confiance

Veuillez également vous assurer que votre configuration comprend une **assertion signée**.

## Étape 2 - Création de règles de revendication

Une fois que la fiducie de confiance a été créée, vous pouvez créer les règles de réclamation.
Par défaut, l'éditeur de règles de réclamation s'ouvre une fois que vous avez créé la fiducie.

1) Pour créer une règle, cliquez sur **Add Rule** (Ajouter une règle).

adding_a_rule.jpg
Ajout d’une nouvelle règle

2) Créez une règle **Send LDAP Attributes as Claims** (Envoyer les attributs LDAP sous forme de revendications).

claim_rule_template.jpg
Création d’une règle

3) Sur l’écran suivant, nommez votre règle et utilisez **Active Directory** comme votre magasin d’attributs, à mapper comme suit :

| LDAP Attribute (Attribut LDAP) | Type de revendication sortante |
| --- | --- |
| E-Mail-Addresses (Adresses e-mail) | E-Mail Address (Adresse e-mail) |
| Given-Name (Prénom) | FirstName (Prénom) |
| Surname (Nom de famille) | LastName (Nom de famille) |

map_LDAP_attributes.jpg
Mappage des attributs LDAP

Cliquez sur **OK**pour enregistrer la nouvelle règle.

4) Créez une nouvelle règle en cliquant sur**Add Rule** (Ajouter une règle) et cette fois, sélectionnez le modèle **Transform an Incoming Claim** (Transformer une revendication entrante).

add_another_rule.jpg
**Sélection du modèle Transform an Incoming Claim (Transformer une revendication entrante)**

5) Nommez ensuite la règle et définissez les paramètres suivants :

|  |  |
| --- | --- |
| **Incoming Claim Type (Type de revendication entrante)** | E-mail Address (Adresse e-mail) |
| **Type de revendication sortante** | Name ID (ID de nom) |
| **Outgoing Name ID Format (Format d’ID de nom sortant)** | E-mail |

set_rule_parameters.jpg
Configuration des paramètres de la règle

Enfin, cliquez sur **OK**pour créer la règle de revendication, puis cliquez à nouveau sur **OK** pour terminer la création des règles.

La configuration d’ADFS est maintenant terminée ! Après cela, il vous suffit d’[activer la fonctionnalité SSO pour votre plan Miro](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) et vos utilisateurs finaux pourront commencer à utiliser SAML pour s’authentifier dans Miro.

## Test de la configuration SSO dans Miro

1. Suivez les étapes ci-dessus pour configurer vos paramètres SSO.
2. Cliquez sur le bouton **Tester la configuration SSO**.
3. Examinez les résultats :

1. Si aucun problème n’est détecté, un message de confirmation indiquant que **le test de configuration SSO a réussi s’** affiche.
2. Si des problèmes sont détectés, un message de confirmation indiquant que **le test de configuration SSO a échoué s’** affiche, suivi de messages d’erreur détaillés pour vous indiquer ce qui doit être corrigé.

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*Test de la configuration SSO dans Miro*
