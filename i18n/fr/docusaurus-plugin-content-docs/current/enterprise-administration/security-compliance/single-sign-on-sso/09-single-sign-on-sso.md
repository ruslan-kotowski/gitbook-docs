---
title: Authentification unique (SSO)
article_id: 360017571414
translation_id: 360017571414
locale: fr
sidebar_position: 9
created_at: '2019-02-11T10:08:59Z'
updated_at: '2026-01-07T13:25:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Grâce à l’authentification unique (SSO) basée sur SAML, les utilisateurs peuvent accéder à Miro par l’intermédiaire d’un fournisseur d’identité (IdP) de leur choix.

> **Disponible pour :** les forfaits Business et Enterprise
> **Rôle requis :** Admin d’entreprise

## Comment fonctionne l’authentification unique SAML

1. Lorsqu’un utilisateur Miro tente de se connecter à Miro à l’aide de l’authentification unique, Miro envoie une demande SAML (Security Assertion Markup Language) au fournisseur d’identité (IdP).
2. Le fournisseur d’identité valide les identifiants de l’utilisateur et envoie une réponse à Miro pour valider l’identité du membre.
3. Miro prend acte de la réponse et accorde l’accès, ce qui permet au membre de se connecter à son compte Miro.

## Que se passe-t-il après l’activation de l’authentification unique ?

**Activation de l’authentification unique pour la première fois**

La première fois que vous configurez l’authentification unique, les utilisateurs existants peuvent continuer à travailler dans Miro sans interruption. Cependant, la prochaine fois qu’ils se déconnectent, que leur session expire ou qu’ils tentent de se connecter à partir d’un nouvel appareil, ils devront se connecter via l’authentification unique.

Les autres options d’ouverture de session seront désactivées pour les utilisateurs, y compris la combinaison identifiant + mot de passe, Google, Facebook, Slack, AppleID et O365.

**Délai d’inactivité de la session**

Si vous avez activé le [délai d’inactivité de la session](../../security-integrations/security-management/02-idle-session-timeout.md), les utilisateurs seront automatiquement déconnectés de leur profil Miro et devront à nouveau se connecter, cette fois à l’aide de l’authentification unique.

**Plusieurs équipes et organisations**

Si vos utilisateurs font partie de plusieurs équipes ou organisations Miro, vous pouvez configurer l’utilisation du même fournisseur d’identité (IdP) pour l’authentification.

**Qui doit se connecter avec SSO ?**

L’authentification unique est obligatoire pour les utilisateurs actifs qui font partie de votre abonnement Enterprise *et* possèdent un domaine répertorié dans vos paramètres d’authentification unique.

- Les utilisateurs qui accèdent à Miro à partir de domaines qui n’ont pas été ajoutés à vos paramètres d’authentification unique ne sont pas tenus de se connecter avec. À la place, ils doivent se connecter à l’aide des méthodes d’authentification standards.
- Les utilisateurs d’un domaine vérifié, qui ne font pas partie de votre abonnement Miro Enterprise, doivent se connecter via l’authentification unique (SSO) uniquement si le [provisionnement juste à temps (JIT)](../../user-management/13-user-provisioning-on-enterprise-plan.md) est activé. Ces utilisateurs seront automatiquement ajoutés à une équipe préconfigurée et devront utiliser le SSO pour se connecter.
- [Utilisateurs gérés](../../user-management/06-managed-users-on-enterprise-plan.md)Il  s'agit de tout utilisateur à l'intérieur de votre (vos) domaine(s) vérifié(s), y compris tout utilisateur géré qui est également membre d'une équipe en dehors de votre abonnement Enterprise. Pour restreindre l’accès à des équipes spécifiques, mettez à jour les paramètres de [contrôle de votre domaine](../../canvas-25-admin-features/domain-control/01-domain-control.md).
  > ✏️ Pour un abonnement Enterprise, une organisation peut avoir des domaines vérifiés et non vérifiés. Pour les domaines vérifiés, les utilisateurs deviennent des utilisateurs gérés qui doivent s'authentifier avec SSO. Pour les utilisateurs de domaine non vérifiés de la même organisation, l'e-mail et le mot de passe sont requis pour l'authentification.

**Gestion des coordonnées des utilisateurs**

Les données des utilisateurs sont automatiquement attribuées dans Miro par votre fournisseur d’identité après une ouverture de session réussie. Certains paramètres, tels que le nom et le mot de passe, ne peuvent pas être modifiés. D’autres paramètres, tels que le service et les photos de profil, sont optionnels.  /span>

- Les noms d’utilisateur Miro sont mis à jour après chaque authentification réussie des utilisateurs. Pour plus d’informations sur la façon de paramétrer les noms d’utilisateur Miro, reportez-vous aux paramètres d’authentification unique avancés. Si vous devez modifier l’adresse e-mail d’un utilisateur, vous ne pouvez le faire que via le [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md). Si vous n’utilisez pas le SCIM, [veuillez contacter l’équipe du service d’assistance](https://help.miro.com/hc/requests/new?referer=help-center-article).

![sso-settings-2.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21027132582290_sso-settings-2.png)
*Sélection du domaine dans les paramètres de l’authentification unique*

> Pour éviter tout verrouillage, créez un « utilisateur d’urgence » dont le domaine de messagerie se trouve en dehors du domaine répertorié dans les paramètres d’authentification unique, comme utilisateurdesecours@gmail.com. Autrement, vous pouvez contacter le service d’assistance qui peut désactiver l’authentification unique pour toute l’organisation.

## Configuration du SSO

### Fournisseurs d’identité (IdP)

Vous pouvez utiliser le fournisseur d’identité de votre choix. Voici les noms des plateformes de fourniture d’identité les plus populaires :

- [OKTA](../../security-integrations/single-sign-on-sso/07-how-to-configure-okta-sso.md)
- [Entra ID de](../../security-integrations/single-sign-on-sso/05-how-to-configure-entra-id-sso.md) Microsoft
- [OneLogin](../../security-integrations/single-sign-on-sso/08-how-to-configure-onelogin-sso.md)
- [ADFS](../../security-integrations/single-sign-on-sso/02-how-to-configure-adfs-sso.md) de Microsoft
- [Auth0](../../security-integrations/single-sign-on-sso/03-how-to-сonfigure-auth0-sso.md)
- [Google SSO](../../security-integrations/single-sign-on-sso/06-how-to-configure-google-sso.md)
- [Jumpcloud SSO](https://support.jumpcloud.com/support/s/article/single-sign-on-sso-with-miro)

### Comment configurer votre IdP

> **💡** [Si votre organisation Enterprise souhaite ajouter plusieurs fournisseurs d’identité](../../security-integrations/single-sign-on-sso/01-adding-multiple-identity-providers.md) , inscrivez-vous à notre [version bêta privée](https://coda.io/form/Miro-Multi-IdP-Private-Beta-Sign-Up_dkoTJMza_jV).

1. Rendez-vous sur le panneau de configuration de votre fournisseur d’identité et suivez ses instructions pour configurer l’authentification unique.

2. Ajoutez les métadonnées suivantes. Nous vous recommandons d’ignorer tous les champs optionnels et de laisser les valeurs par défaut telles quelles.

#### Spécifications (métadonnées)

|  |  |
| --- | --- |
| **Protocole** | SAML 2.0 |
| **Liaison** | Redirection HTTP pour SP vers IdP HTTP Post pour IdP vers SP |
| **URL de service** (URL initiée par le SP)  Également appelée URL de lancement, URL de réponse, URL de service d’authentification unique de la partie utilisatrice, URL cible, URL de connexion par authentification unique, point de terminaison du fournisseur d’identité, etc. | https://miro.com/sso/saml |
| **URL du service consommateur d’assertion**    Également appelée URL de rappel autorisé, URL ACS personnalisée, URL de réponse | https://miro.com/sso/saml |
| **ID de l’entité**    Également appelé identificateur, identificateur d’approbation de partie de confiance | https://miro.com/ |
| **État du relais par défaut** | doit être laissévide dans votre configuration |
| [**Conditions de signature**](https://developers.onelogin.com/saml/examples/response) | Une réponse SAML non signée avec uneassertion signée  Une réponse SAML signée avec une assertionsignée |
| **Méthode SubjectConfirmation** | « urn:oasis:names:tc:SAML:2.0:cm:bearer » |
| La réponse SAML du fournisseur d’identité doit contenirle certificat de clé publique x509 émis par le fournisseur d’identité.  Voirdes exemples SAML détaillés. Télécharger le [fichier de métadonnées Miro SP](https://drive.google.com/file/d/1BN58fiwC062F5MC-PsO3QN7JlCbKNCSJ/view) (XML). | |

:::warning
Le chiffrement et la déconnexion unique ne sont pas pris en charge.
:::

#### Identifiants des utilisateurs

Les champs autres que les champs ci-dessous ne sont pas obligatoires. Nous vous recommandons d’ignorer tous les champs optionnels et de laisser les valeurs par défaut telles quelles.

|  |  |
| --- | --- |
| Attributs de l’identifiant de l’utilisateur obligatoires | |
| **NameID** (équivaut à l’adresse e-mail d’un utilisateur)  Également appelé SAML_Subject, clé principale, nom d’ouverture de session, format du nom d’utilisateur de l’application, etc. | &lt;NameID Format="urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress"&gt; |
| **Attributs facultatifs à envoyer avec l’assertion**  (mis à jour à chaque nouvelle authentification via l’authentification unique, utilisés lorsqu’ils sont présents/disponibles) | - "DisplayName" ou"http://schemas.microsoft.com/identity/claims/displayname"(utilisé comme nom préféré)  [mceclip0.png](http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname)  - "Prénom", "FirstName" ou "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname"; - "Nom de famille", "Nom de famille" ou "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname"; - « ProfilePicture » : l’URL codée de l’image |

### Comment activer l’authentification unique dans vos paramètres Miro

Forfait Business Forfait Enterprise

1. Allez dans les paramètres de votre **entreprise** > **Sécurité** > **Authentification** unique
2. Activez **SSO/SAML

*![](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20889990489874_security-sso.png)
*security-sso.png****

1. Allez dans les **paramètres de votre entreprise** > **Sécurité et conformité** > **Authentification** > **Authentification unique**
2. Activez **SSO/SAML

*![](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366644626_sso-enterprise.png)
*sso-enterprise.png****

:::note
L’activation de l’authentification unique dans vos paramètres ne l’active pas immédiatement pour les utilisateurs. Le login SSO est disponible après la [vérification de](../../canvas-25-admin-features/domain-control/01-domain-control.md) vos [domaines](../../canvas-25-admin-features/domain-control/01-domain-control.md). Ensuite, lorsque vous configurez SSO dans la section suivante, assurez-vous d'ajouter vos domaines vérifiés.
:::

### Comment configurer l’authentification unique dans vos paramètres Miro

Après avoir activé la fonction SSO/SAML dans les paramètres d'authentification unique, remplissez les champs suivants :

1. **URL de connexion SAML** (dans la plupart des cas, elle ouvre la page de votre fournisseur d’identité où vos utilisateurs finaux doivent entrer leurs identifiants).
2. **Certificat à clé publique x.509** (émis par votre fournisseur d’identité).
3. Tous les domaines et sous-domaines autorisés ou obligés (ACME.com ou ACME.dev.com) de s’authentifier via votre serveur SAML.
4. Ajoutez votre/vos domaine(s) vérifié(s). Pour **Les utilisateurs de ces domaines se connecteront à l'aide du SSO**, cliquez sur ***Sélectionner un domaine***et sélectionnez l'un de vos domaines à ajouter à la liste.

![sso-settings.pngParamètres](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366648082_sso-settings.png)
*SSO de*

### Renouveler votre certificat SSO/SAML

Si votre certificat à clé publique x.509 a expiré, l’authentification unique continuera de fonctionner, mais il est fortement recommandé de le renouveler afin de poursuivre l’utilisation de Miro en toute sécurité. Les certificats x.509 à clé publique garantissent la sécurité, la conformité, l’authenticité et l’intégrité des informations partagées entre votre fournisseur d’identité et Miro.

Ces certificats ne sont valables que pour une période donnée, qui peut être spécifiée (et vérifiée) auprès de votre fournisseur d’identité. Veuillez vérifier la date d’expiration auprès de votre fournisseur d’identité.

Ce processus se déroule en deux étapes :

1. Renouvelez le certificat auprès de votre fournisseur d’identité. Vérifiez leurs instructions concernant la marche à suivre.
2. Ajoutez le certificat renouvelé à votre configuration de l’authentification unique Miro.

#### Ajout de certificats renouvelés à Miro

:::warning
Nous vous recommandons de remplacer votre certificat x.509 pendant les périodes moins chargées dans votre organisation (par exemple, le week-end ou après les heures de bureau) pour éviter les interruptions de connexion.
:::

1. Allez dans les **Paramètres de l’entreprise** > **Authentification** > **Authentification unique**.
2. Supprimez le contenu dans le champ **certificat à clé x.509**.
3. Collez la nouvelle clé dans ce champ.
4. Faites défiler la page et cliquez sur **Save (Enregistrer)**.
   ![sso-gif-2.gifRenouvellement d'](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21027132584850_sso-gif-2.gif)
*un certificat x.509 dans Miro*

## Tester votre configuration SSO

Testez votre configuration SSO avant de l’activer afin de réduire les risques de problèmes de connexion pour vos utilisateurs.

1. Suivez les étapes ci-dessus pour configurer vos paramètres SSO.
2. Cliquez sur le bouton **Tester la configuration SSO**.
3. Examinez les résultats :

- Si aucun problème n’est détecté, un message de confirmation indiquant que **le test de configuration SSO a réussi s’** affiche.
- Si des problèmes sont détectés, un message de confirmation indiquant que **le test de configuration SSO a échoué s’** affiche, suivi de messages d’erreur détaillés pour vous indiquer ce qui doit être corrigé.

![sso-test.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366649618_sso-test.png)
*Tester la configuration SSO*

## Paramètres d’authentification unique avancés facultatifs

La section des paramètres facultatifs est utilisée par les utilisateurs avancés qui s’y connaissent en matière de configuration de l’authentification unique.

### Provisionnement juste à temps (JIT) pour les nouveaux utilisateurs

Facilitez la tâche de vos utilisateurs pour qu’ils puissent commencer à utiliser Miro immédiatement, sans avoir à attendre une invitation ou à passer par un long processus d’intégration. Assurez-vous également qu’aucune équipe gratuite n’est créée en dehors de votre abonnement géré (nécessite le contrôle de domaine). L’authentification unique est nécessaire pour activer le provisionnement Juste-à-temps (JIT) de nouveaux utilisateurs. Tous les utilisateurs approvisionnés en Juste-à-temps se voient attribuer la licence par défaut de votre abonnement :

|  |  |  |
| --- | --- | --- |
| **Type d’abonnement** | **Type de licence** | **Comportement lorsque les licences sont épuisées** |
| Forfait Business | Licence complète | Les utilisateurs ne sont pas automatiquement ajoutés ; la fonctionnalité JIT cesse de fonctionner. |
| Forfait Enterprise (sans le [programme de licences flexibles](../../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)) | Licence complète | Utilisateurs approvisionnés sous la licence [gratuite restreinte](../../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md). |
| Forfait Enterprise (avec le programme de licences flexibles) | Licence gratuite restreinte ou Free | Dépend des paramètres de [licence par défaut](../../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md). |

### Comment activer le provisionnement Juste-à-temps

Une fois activé, le provisionnement Juste-à-temps s’appliquera automatiquement à tous les nouveaux utilisateurs qui s’inscrivent sur Miro. En revanche, les utilisateurs Miro existants devront être invités à rejoindre votre forfait.

1. Rendez-vous dans les paramètres de l’authentification unique.
2. Cochez la case **Ajouter automatiquement à votre compte Enterprise tous les utilisateurs nouvellement enregistrés des domaines répertoriés**.
3. **Choisissez une équipe par défaut pour les utilisateurs nouvellement enregistrés** dans le menu déroulant.
4. Cliquez sur **Enregistrer**.

Lorsque vous répertoriez des domaines spécifiques dans vos paramètres d’authentification unique, tous les utilisateurs qui s’inscrivent avec ces domaines seront automatiquement ajoutés à votre abonnement Enterprise. Ils seront assignés à l’équipe que vous avez sélectionnée dans les paramètres Juste-à-temps (JIT).

![Copie de user_provisioning_jit_provisioning.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528391698_Copy%20of%20user_provisioning_jit_provisioning.png)*Activez la fonctionnalité de provisionnement juste à temps sur la page des intégrations Enterprise.*

Tous**les utilisateurs nouvellement enregistrés** avec les domaines que vous avez énumérés dans les paramètres seront automatiquement ajoutés à votre compte Enterprise dans cette équipe en particulier lorsqu’ils s’inscriront à Miro.

:::warning
Dans le forfait Enterprise, cette équipe sera également affichée dans la liste des équipes pouvant être trouvées si vous activez l’option dedécouverte de l’équipe.
:::

### Définition de DisplayName comme nom d’utilisateur par défaut

Par défaut, Miro utilisera les attributs **FirstName (Prénom)** + **LastName (Nom)**. Vous pouvez à la place demander à utiliser l’attribut **DisplayName (Nom d’affichage)**. Dans ce cas, Miro utilisera **DisplayName (Nom d’affichage)** *lorsqu’il est présent* dans la réponse SAML de l’utilisateur.

Si l’attribut **DisplayName (Nom d’affichage)** n’est pas présent mais que les attributs **FirstName (Prénom)** + **LastName (Nom)** le sont, Miro utilisera les attributs **FirstName (Prénom)** + **LastName (Nom).** Contactez le service d’assistance de Miro pour faire de l’attribut **DisplayName (Nom d’affichage)** votre nom d’utilisateur SSO préféré.

Si aucun des trois attributs n’est présent dans votre communication SAML, Miro affichera l’adresse e-mail de l’utilisateur comme nom d’utilisateur.

|  |  |
| --- | --- |
| **Paramètres** | **Nom d’utilisateur par défaut** |
| Nom d’utilisateur Miro | FirstName (Prénom) + LastName (Nom) |
| Paramètres alternatifs | DisplayName (Nom d’affichage) (s’il est présent dans la demande SAML de l’utilisateur) |
| Solution de secours | FirstName (Prénom) + LastName (Nom) (si DisplayName (Nom d’affichage) n’est pas présent) |
| Nom d’utilisateur préféré pour l’authentification unique | DisplayName (Nom d’affichage) ([contactez le service d’assistance Miro](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)) |
| Aucun attribut présent | Adresse e-mail affichée comme nom d’utilisateur |

Si vous voyez quelque chose qui ne correspond pas à ce que vous attendiez, vous devrez peut-être vous authentifier via l’authentification unique. Il est aussi possible que la réponse SAML ne contienne pas les valeurs nécessaires pour la mise à jour.

### Synchronisation des images de profil d’utilisateur à partir de l’IdP

:::warning
En général, il est recommandé d’activer cette option si vous n’activez pas le SCIM ou si votre IdP ne prend pas en charge l’**attribut** **ProfilePicture (Photo de profil)** (c’est le cas d’Azure par exemple). Dans les autres cas, il est recommandé de passer ProfilePicture (Photo de profil)viale SCIM avec des mises à jour immédiates.
:::

Lorsque ce paramètre est activé :

- l’image de profil définie du côté de l’IdP sera définie comme l’image de profil de l’utilisateur dans Miro.
- les utilisateurs ne seront pas en mesure changer ou de supprimer eux-mêmes leur image de profil.

:::warning
À l’instar de l’attribut nom d’utilisateur, les utilisateurs ne pourront pas modifier immédiatement leurs données du côté de Miro, mais la *synchronisation*des données n’est pas immédiate. En effet, l’IdP envoie une mise à jour à Miro uniquement lors de la*prochaine* authentification par authentification unique de l’utilisateur (à condition que le paramètre « Synchroniser les photos de profil d’utilisateur à partir de l’IdP » soit toujours activé à ce moment-là).
:::

Si l’image de profil est définie dans l’IdP et que vous souhaitez que l’attribut soit transféré dans la communication SAML, Miro attendra le schéma suivant :

```
<saml2:Attribute Name="ImageProfil"NameFormat="urn:oasis:names:tc:SAML:2.0:attrname-format:uri">
<saml2:AttributeValue
xmlns:xs="http://www.w3.org/2001/XMLSchema"
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">https://images.app.goo.gl/cfdeBqKfDKsap1icxecsaHF
</saml2:AttributeValue>
</saml2:Attribute>
```

## SSO et résidence des données

Si vous utilisez le service de [résidence des données de](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md) Miro et que vous disposez d'une URL dédiée (workspacedomain.miro.com), vous devez ajuster la configuration de votre fournisseur d'identité.

:::note
Pour les organisations dont les données résident en Australie et aux États-Unis, la connexion sociale n'est pas disponible. Pour plus d'informations sur la résidence des données, consultez la rubrique [Résidence des données à Miro](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md).
:::

Pour ce faire, vous devrez ajouter votre [ORGANIZATION_ID] à l’URL.

Vous trouverez votre ORGANIZATION_ID sur le tableau de bord Miro, en cliquant sur votre **Profil** dans le coin supérieur droit > **Paramètres** > il est affiché dans l’URL dans la barre d’adresse.

|  | Valeur normale | Valeur en cas de résidence des données |
| --- | --- | --- |
| **URL du service consommateur d’assertion** (aussi appelée URL de rappel autorisé, URL ACS personnalisée, URL de réponse) : | https://miro.com/sso/saml | https://workspace-domain.miro.com/ sso/saml/ORGANIZATION_ID |
| **ID de l’entité** (identificateur, identificateur d’approbation de partie de confiance) :  https://miro.com/ | https://miro.com/ | https://workspace-domain.miro.com/ IDENTIFIANT DE L’ORGANISATION |

## Mise en place de l’authentification multifacteur (2FA) pour les utilisateurs extérieurs à l’authentification unique

L’authentification à deux facteurs (2FA) fournit une couche de sécurité supplémentaire. Avec l’authentification à deux facteurs, les utilisateurs doivent passer par une étape supplémentaire lorsqu’ils se connectent, afin de vérifier leur identité. Cette mesure supplémentaire permet de s’assurer que seules les personnes autorisées peuvent accéder à votre abonnement.
Pour en savoir plus, consultez notre [guide d’administration de l’authentification à deux facteurs](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md).

## Foire aux questions et résolution des problèmes éventuels

Les adresses de mon domaine ne sont pas acceptées dans les paramètres de l’authentification unique. Message affiché : « Le nom de domaine est occupé ».

Pour des raisons de sécurité, nous ne prenons en charge le(s) domaine(s) d’une organisation que dans le cadre *d’un seul et même compte entreprise (abonnement Enterprise)*. Il est possible que vos domaines soient déjà configurés dans un autre forfait Business ou [Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md), ce qui vous empêche d’activer l’authentification unique pour le domaine souhaité. N’hésitez pas à vérifier auprès de vos collègues à l’avance.

Mon domaine n'apparaît pas dans la liste déroulante des domaines disponibles.

Vous devez d'abord réclamer et vérifier vos domaines dans les [paramètres de Managed Domain.](../../canvas-25-admin-features/domain-control/01-domain-control.md)

Nous devons modifier les adresses e-mail de nos utilisateurs finaux/Nous avons modifié les adresses e-mail de nos utilisateurs et ils ne peuvent plus accéder à leurs tableaux.

Si votre entreprise change de nom de domaine et que les adresses e-mail des utilisateurs finaux ont donc besoin de modifier leurs identifiants pour l’authentification unique, [contactez notre équipe du service d’assistance](https://help.miro.com/hc/requests/new?referer=help-center-article) pour obtenir de l’aide.

Nous aimerions utiliser une passerelle distincte (par exemple, une authentification multifacteur, comme Duo Dag) pour la procédure d’authentification unique.

C’est tout à fait possible. Miro prend en charge votre solution préférée tant qu’elle fonctionne sous SAML 2.0.

Nous avons activé l’authentification unique, mais les données des profils des utilisateurs (noms, photos de profil si prises en charge par votre IdP) dans Miro ne sont pas synchronisées avec celles du fournisseur d’identité.

Le nom d’utilisateur et la photo de profil Miro sont mis à jour après chaque authentification réussie de l’utilisateur, *si et seulement si* SAMLResponse contient de nouvelles valeurs non vides. Pour plus d’informations sur la façon de paramétrer les noms d’utilisateur Miro, reportez-vous aux paramètres d’authentification unique avancés facultatifs.

Quelle est la procédure à suivre pour changer de fournisseur SSO ?

Lorsque vous changez de fournisseur SSO, vous devez configurer le nouvel IDP à partir de zéro, comme vous le feriez lors d'une première installation.

Si un ou tous vos utilisateurs rencontrent une erreur lorsqu’ils essaient de se connecter à Miro, consultezla liste des erreurs courantes et leurs solutions.
