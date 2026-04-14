---
title: Comment configurer l’authentification unique Entra ID
article_id: 360022722233
translation_id: 360022722233
locale: fr
sidebar_position: 5
created_at: '2019-05-07T12:03:08Z'
updated_at: '2025-11-25T16:04:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible pour: les forfaits Business et Enterprise Rôle requis: Admins
    d’entreprise'
---

> *💡 Il est fortement recommandé de configurer l’authentification unique dans une fenêtre indépendante de votre navigateur, en mode navigation privée.* De cette façon, votre session reste active dans la fenêtre standard, ce qui vous permet de désactiver l’autorisation de l’authentification unique si quelque chose est mal configuré.

Si vous souhaitez paramétrer une instance de test avant d’activer l’authentification unique en production, veuillez [contacter l’équipe du service d’assistance](https://help.miro.com/hc/requests/new?referer=help-center-article) pour obtenir de l’aide. Seules les personnes qui configurent l’authentification unique seront ajoutées à cette instance de test.

> **⚠️ Consultez notre article principal sur l’authentification unique** [**ici**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **pour découvrir les règles, les fonctionnalités prises en charge et les configurations optionnelles du côté de Miro.**

## Ajouter et configurer l’application

 1. Recherchez l’application préconfigurée Miro dans la Galerie d’applications d’Entreprise Entra ID ([Applications d'entreprise](https://portal.Entra.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/) > +Nouvelle application).

2. Créez l’application et cliquez sur **2.** **Configurer l’authentification unique** (ou sélectionnez **Authentification unique** sur le côté gauche et sélectionnez la méthode d’authentification **SAML**).

3. Vous verrez que la **configuration SAML de base** est déjà en place:

:::warning
Si une fois que tout est configuré, la connexion par SSO échoue, essayez de changer l’identifiant d’entité pour passer de `https://miro.com` à `https://miro.com/`
:::

:::warning
Les champs URL de connexion, État du relais et URL de déconnexion (pour la déconnexion unique) doivent être laissés vides, car ces fonctionnalités ne sont pas prises en charge.
:::

Les **Attributs et revendications** sont également déjà en place :

:::warning
Notez que :
a) l'UPN deviendra le paramètre principal par lequel un utilisateur dans Miro sera reconnu et ce paramètre ne pourra pas être mis à jour du côté Entra. Lorsque vous devez mettre à jour les adresses e-mail des utilisateurs dans Miro sans utiliser SCIM, veuillez [contacter notre équipe du service d’assistance](https://help.miro.com/hc/requests/new?referer=help-center-article).
b) Miro acceptera les attributs [**GivenName (Prénom),** **Surname (Nom de famille),** **DisplayName (Nom d’affichage)** et **ProfilePicture (Photo de profil)**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Les autres attributs ne sont pas pris en charge via SSO, mais ils peuvent être transférés par [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).
:::

### Créer le certificat

1. Dans Microsoft Entra, assurez-vous que **Certificat de signature SAML** >**Option de signature** est soit **Signer l'assertion SAML** soit **Signer la réponse et l'assertion SAML**.

2. **Télécharger** le fichier **Base64**.

## Configurer l’authentification unique dans votre forfait Miro

1. Ouvrez le fichier téléchargé **Base64** dans un éditeur de texte, puis copiez le certificat **x509** du fichier.

2. Dans Miro, sous **Sécurité > Authentification**, collez le certificat **x509** copié dans le champ **Clé certificat x509**.

3. Dans l'interface des paramètres de Microsoft Entra, copiez l'**URL de connexion**, puis allez à la page **Sécurité > Authentification** de Miro et collez-la dans le champ **URL de connexion SAML**.

4. Dans la page **Sécurité >** **Authentification** de Miro, dans la section **Les utilisateurs de ces domaines se connecteront en utilisant l’authentification unique**, assurez-vous d’ajouter au moins un domaine d’entreprise.

:::warning
Dans Miro, assurez-vous que **Synchroniser les photos de profil depuis l'IdP** n'est pas coché. Entra ID ne prend pas en charge la synchronisation des photos de profil utilisateur. Lorsque **Synchroniser les photos de profil depuis l'IdP** n'est pas coché, les utilisateurs peuvent définir leurs propres photos de profil.
:::

4. Cliquez sur **Enregistrer**.

La configuration de l’authentification unique est maintenant terminée.

## Configuration des revendications lorsque l’UPN et l’adresse e-mail diffèrent

Vous pouvez configurer les paramètres pour utiliser n’importe quel attribut Entra au format e-mail en tant qu’**NameID** dans Miro.

#### **Connexions initiées par l’IDP et le SP**

*En cas de connexion initiée par l’IDP*, Entra envoie à Miro la valeur que vous décidez d’utiliser comme **NameID** (**user.mail** dans l’exemple ci-dessous).

Avec ce flux, vos utilisateurs finaux accèdent à Miro via l’icône sur leur console de portail (par exemple à `https://myapplications.microsoft.com/`). De là, une demande est envoyée à Miro et *l’utilisateur est connecté à l’aide de l’**identifiant de nom** que vous avez défini.*Miro s’attend à ce que cet attribut corresponde à l’**adresse e-mail** de l’utilisateur dans Miro. Une non-concordance entraînera un échec de l’authentification.

*En cas de connexion initiée par le SP*, Miro enverra une demande spécifique pour l’**UPN** de l’utilisateur et s’attendra à ce qu’elle corresponde à l’**adresse e-mail** de l’utilisateur dans Miro. Une non-concordance entraînera un échec de l’authentification.

Désormais, le champ **URL de connexion SAML** dans vos paramètres Miro devrait contenir l'**URL de connexion** de l'application Miro de votre instance Entra. Il s’agit de l’URL vers laquelle Miro dirigera l’utilisateur à partir de la [page de connexion Miro](https://miro.com/sso/login/).

Lorsque l’utilisateur est dirigé vers l’URL de connexion depuis l’application, la demande SAML est générée. Avec ce flux, l’utilisateur est connecté avec l’adresse e-mail qu’il a saisie sur la page de connexion de Miro et que Miro demande ensuite à Entra en exigeant qu’il s’agisse de l’attribut UPN.

#### **Comment configurer**

Pour permettre à vos utilisateurs d’accéder à Miro avec leur **adresse e-mail** Entra plutôt qu’avec l’**UPN**, vous pouvez remplir le champ **URL de connexion SAML** dans Miro avec l’URL de l’application à partir de la console Entra. Ensuite, le flux initié par le SP sera le suivant :

1. L’utilisateur accède à Miro en saisissant son adresse e-mail Miro, soit l’adresse e-mail qu’il a dans Miro. Miro comprend que la personne doit être connectée au profil d’utilisateur défini.
2. L’utilisateur est dirigé vers le lien de son application qui est utilisé pour la connexion initiée par l’IDP.
3. Le lien utilise l’attribut  **NameID**  *que vous avez défini* et l’envoie à Miro.
4. L’utilisateur est donc connecté à Miro dans le profil utilisateur précédemment défini avec l’**NameID** que vous avez défini.

Veuillez consulter [cet article](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md) si vous souhaitez également activer le provisionnement automatique pour Miro.

Veuillez consulter [cet article](../../../using-miro/tools/troubleshooting/10-i-can't-log-in-via-sso.md) si vous avez rencontré des problèmes lors de la configuration.

## Outil de test Entra

Pour accéder à l’outil de test, choisissez l’onglet **Connexion unique** dans les paramètres de votre application et faites défiler la page jusqu’au bas de la section.

Entra suggère d’utiliser le processus de connexion test pour vérifier la connexion et résoudre un message d’erreur. Après le test, vous recevrez des instructions sur la façon de résoudre le problème.

Veuillez garder à l’esprit les identifiants gérés par Entra/ADFS avec lesquels votre poste de travail est authentifié. Si vous essayez d’utiliser un ensemble d’identifiants différent pour vous connecter à Miro, la tentative de connexion risque d’échouer, car le fournisseur d’identité transférera votre ensemble principal d’identifiants et il y aura une non-concordance. Cela peut se produire par exemple si vous êtes l’administrateur SSO et que vous testez la procédure de connexion avec différents identifiants d’utilisateur.

## Vous pouvez également tester dans Miro

1. Suivez les étapes ci-dessus pour configurer vos paramètres SSO.
2. Cliquez sur le bouton **Tester la configuration SSO**.
3. Examinez les résultats :
   1. Si aucun problème n’est détecté, un message de confirmation **le test de configuration SSO a réussi** sera affiché.
   2. Si des problèmes sont détectés, un message de confirmation **le test de configuration SSO a échoué** sera affiché, suivi de messages d’erreur détaillés pour vous indiquer ce qui doit être corrigé.

##
