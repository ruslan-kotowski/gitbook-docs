---
title: "Je ne parviens pas \xE0 me connecter via l\u2019authentification unique"
article_id: 360019271654
translation_id: 360019271654
locale: fr
sidebar_position: 10
created_at: '2019-03-07T15:50:03Z'
updated_at: '2025-11-25T16:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Vous et vos responsables IT trouverez ci-dessous des conseils sur la résolution des problèmes relatifs à l’authentification unique.

> **✏️** En savoir plus sur la [configuration de l’authentification unique Miro](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) et du [SCIM Miro](https://developers.miro.com/docs/scim).

## Messages d’erreur de Miro relatifs à l’authentification unique

Si vous recevez l’un des messages d’erreur suivants relatifs à l’authentification unique, essayez les solutions ci-dessous.  Il se peut que vous ayez besoin de l’aide de votre service informatique ou des admins d’entreprise.

Votre adresse e-mail n’est pas associée à un compte avec authentification unique.

Ce message apparaît lorsque l’adresse e-mail que vous avez saisie dans Miro n’est pas reconnue comme le nom d’un utilisateur supposé être authentifié via l’authentification unique.

Causes possibles :

- **Vous n’êtes membre d’aucun abonnement qui utilise l’authentification unique comme méthode de connexion**.  Connectez-vous à l’aide des options standard (adresse e-mail et mot de passe) ou contactez votre admin pour recevoir une invitation et rejoindre l’abonnement de votre entreprise.
- **Vous devez vous connecter via l’authentification unique, mais il y a un problème avec votre adresse e-mail**.  Il est possible que vous ayez plusieurs adresses e-mail (ou alias) et que l’invitation au forfait nécessitant l’authentification unique ait été envoyée à une autre adresse e-mail. Connectez-vous avec une autre adresse e-mail.

Votre adresse e-mail n’est pas associée au compte avec authentification unique. Demandez l’accès à votre admin d’entreprise.

Ce message s’affiche généralement dans deux cas de figure :

- **Votre profil d’utilisateur enregistré dans le système du fournisseur d’identité n’est pas autorisé à se connecter à Miro (vous n’avez pas de rôle assigné)**.  Le cas échéant, vous ne verrez probablement pas d’icône Miro sur le tableau de bord des applications de votre fournisseur. Contactez l’admin de votre fournisseur pour obtenir les autorisations nécessaires. /span>
- **Vous avez récemment changé votre adresse e-mail** (en raison d’un mariage par exemple) et cette modification n’a pas été correctement mise à jour dans tous les systèmes, ce qui crée des conflits.  Contactez votre admin pour clarifier la situation et il prendra contact avec nous, le cas échéant, pour approuver les changements nécessaires.

Si vous ne parvenez pas à vous connecter à Miro via l’authentification unique, vous pouvez demander un accès auprès des admins d’entreprise en cliquant sur le bouton correspondant sur la [page de connexion par authentification unique de Miro](https://miro.com/sso/login/).

![sso-new-sign-in.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/20463017477778_sso-new-sign-in.png)*L'option permettant de demander l'accès aux admins d'entreprise*

Vous devrez saisir le code de confirmation envoyé à votre adresse e-mail.  Une fois le code renseigné, les admins de l’abonnement de votre entreprise recevront une notification les informant que vous avez besoin d’aide.

Something went wrong. » (Erreur de connexion. Une erreur est survenue.) La validation de la signature de la réponse n'a pas abouti

Ce message signifie que des éléments ont mal été configurés dans les paramètres d’authentification unique de Miro ou du côté de votre fournisseur d’identité.  Il est probable qu’aucun de vos collègues ne puisse se connecter. Contactez votre service informatique ou l’admin du fournisseur d’identité pour qu’ils puissent vérifier les points suivants.

- La réponse SAML doit contenir *l’assertion* signée.  Il s’agit d’une exigence de Miro.
- Il se peut que votre fournisseur d’identité traite les réponses signées de manière spécifique.  Par exemple, l’authentification unique de Google *désactive*/span> la signature de l’assertion lorsque la *réponse* est signée.  Si tel est le cas, désactivez la signature de la réponse.
- La réponse SAML contient l’assertion signée requise, mais la valeur du certificat X.509 qui est censée la valider n’est pas présente (cela peut également se produire si votre VPN/pare-feu [interrompt certaines parties du transfert de données](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)).  Assurez-vous que la valeur du certificat X.509 est transmise dans le trafic SAML vers Miro.
- La réponse SAML contient une valeur de certificat X.509 *différente* de celle ajoutée dans les [paramètres de Miro](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), ce qui crée un défaut de correspondance et un échec de la validation.  Vérifiez que les valeurs du certificat du côté du fournisseur d’identité et du côté de Miro correspondent.

Something went wrong. » (Erreur de connexion. Une erreur est survenue.) L’utilisateur n’a pas été renseigné dans la réponse SAML.

Cela indique un problème de configuration du côté de votre fournisseur d’identité. Soit au niveau de la configuration générale, soit au niveau de votre profil d’utilisateur spécifique.  Contactez votre service informatique ou l’admin du fournisseur d’identité pour qu’ils puissent vérifier les points suivants.

- Le format de nom d’utilisateur (NameID, identifiant d’utilisateur unique) de votre configuration d’authentification unique n’est pas spécifié ou est défini sur un attribut autre qu’une adresse e-mail, de sorte que la valeur utilisateur envoyée à Miro ne peut pas être reconnue.  Donnez l’attribut EmailAddress /span>**au nom d’utilisateur du côté du fournisseur d’identité (ou tout autre attribut dans un format d’adresse e-mail).**
- La réponse SAML ne contient pas la valeur e-mail de l’utilisateur, qui ne peut donc pas être reconnu (cela peut également se produire si votre VPN/pare-feu [interrompt certaines parties du transfert de données](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)).  Assurez-vous que l’adresse e-mail est transmise dans le trafic SAML vers Miro.
- La réponse SAML est chiffrée.  N’utilisez pas de chiffrement, car Miro ne le prend pas en charge.

Something went wrong. » (Erreur de connexion. Une erreur est survenue.) La réponse SAML n'est pas correcte

Ce message s’affiche généralement lorsqu’il y a des problèmes avec votre profil du côté du fournisseur d’identité.
Causes possibles :/span>

- **Votre profil d’utilisateur est mal configuré dans le système du fournisseur d’identité**.  Par exemple, vous n’avez pas la permission de vous connecter à Miro (vous n’avez pas de rôle assigné). Le cas échéant, vous ne verrez probablement pas d’icône Miro sur le tableau de bord des applications de votre fournisseur. Contactez l’admin de votre fournisseur pour obtenir les autorisations nécessaires.
- **Votre profil d’utilisateur est correctement configuré dans le système du fournisseur d’identité, mais des restrictions s’appliquent**.  Par exemple, des restrictions relatives à l’IP s’appliquent et vous ne pouvez vous connecter que depuis certains endroits. Contactez l’admin de votre fournisseur d’identité et demandez-lui des informations sur vos autorisations.

Pour autoriser avec l’authentification unique, utilisez le lien URL fourni par votre employeur.

Ce message signifie que vous n’avez pas le droit d’accéder à Miro depuis cette page ou que la configuration de l’authentification unique dans votre forfait Miro Enterprise n’est pas terminée.  Dans ce cas, vous pourrez peut-être vous connecter à partir de votre tableau de bord MyApps.
Causes possibles :/span>

- **Votre fournisseur d’identité est configuré pour une** [connexion initiée par le fournisseur d’identité](https://blogs.oracle.com/dcarru/sp-vs-idp-initiated-sso) **uniquement et vous ne devriez pas être en mesure de vous connecter à partir de la page de connexion de Miro.**  Connectez-vous via le lien fourni à partir du tableau de bord de vos applications, ou contactez votre admin d’entreprise pour obtenir davantage d’instructions.
- **L’authentification unique est activée dans votre forfait Miro Enterprise, mais la configuration n’a pas été finie**.  Contactez votre service informatique ou l’admin de votre fournisseur d’identité afin qu’ils terminent la configuration conformément à ces instructions./span>

## Erreurs Entra ou ADFS

La configuration de l’authentification unique n’est pas disponible pour cette application dans l’expérience Applications d’entreprise.

Le texte intégral du message : La configuration de l’authentification unique n’est pas disponible pour cette application dans l’expérience Applications d’entreprise. Miro (anciennement RealtimeBoard) est une application multi-locataires et l'application appartient à un autre locataire.
*Pour modifier des propriétés telles que l'URL de réponse et les identifiants, contactez le propriétaire de l'application.*Contactez votre service informatique et demandez-lui de vérifier la configuration du SSO. Il est très probable qu'il existe déjà une application Miro configurée dans votre ID Entra où notre identifiant (`https://miro.com/)` est utilisé et donc pris. Entra est plus ou moins unique en ce sens que ce fournisseur d'identité exige que l'identifiant (Entity ID) soit unique.
Pour éventuellement résoudre la situation, nous vous conseillons de vérifier les applications Enterprise de votre instance Entra et d'utiliser celle que vous avez déjà configurée pour vos paramètres Miro.
Si vous êtes sûr qu'il n'y a pas d'autres applications Miro dans vos applications Enterprise, essayez d'obtenir une nouvelle copie de l'application Miro à partir de la galerie Entra.

Une erreur s’est produite. Contactez votre administrateur pour obtenir plus d’informations.

Partagez cet article de la communauté avec votre service informatique : Une erreur s’est produite. Contactez votre administrateur pour plus d’informations. »

Aucun accès accordé : erreur AADSTS50105

![mceclip3.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044185746_mceclip3.png)
Partagez cet article de la communauté avec votre service informatique : ["Erreur "Rôle non attribué](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50105-user-not-assigned-role)

Application mal configurée : erreur AADSTS650056

![mceclip2.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044184722_mceclip2.png)
Nous avons consulté la documentation de Microsoft relative à l’erreur AADSTS650056 (ainsi que quelques suggestions de la communauté) et il semble que l’erreur pourrait être causée par les modifications que vous avez apportées aux autorisations de l’application. Il se peut que votre admin Entra doive donner son accord à l'application Miro pour permettre aux utilisateurs finaux de s'authentifier dans Miro. Ce tutoriel Microsoft devrait être utile pour résoudre ce problème.

Lisez [l’article sur support.microsoft.com à propos des autres erreurs d’authentification unique possibles](https://support.office.com/article/how-to-troubleshoot-issues-that-you-encounter-when-you-sign-in-to-office-apps-for-mac-ipad-iphone-or-ipod-touch-when-using-active-directory-federation-services-e44357b4-c9c4-4580-a946-ef5dabdb98cd?ui=en-US&rs=en-US&ad=US).

## Messages d’erreur relatifs au SAML Google

Veuillez vous référer à [cette section de la documentation de Google](https://support.google.com/a/answer/6301076?hl=en) qui énumère les erreurs possibles ainsi que les instructions pour les résoudre.

## Problèmes de connexion à l’application Miro via l’authentification unique sur l’application de bureau, pour tablette ou mobile

Si vous ne parvenez pas à vous connecter à l’application Miro via l’authentification unique depuis un ordinateur/une tablette/un appareil mobile, mais que vous pouvez vous connecter à la [version sur navigateur](https://miro.com/app/), procédez comme suit :

1. Supprimez l’application de l’appareil et réinstallez-la.  Pour l’application de bureau, assurez-vous de supprimer tous les dossiers de l’application en suivant les instructions suivantes/span>. Ce problème est le plus souvent dû à un mauvais cache. Vous devez donc tout effacer et réinstaller à partir de zéro.
2. Essayez de changer le navigateur par défaut de votre appareil pour voir si vous pouvez alors terminer le processus.  Assurez-vous que votre navigateur préféré autorise les cookies tiers/span>.
3. Vérifiez si votre fournisseur d’identité ne gère *pas* le paramètre **RelayState**. Il s’agit d’un jeton unique que Miro génère et utilise pour reconnaître que l’utilisateur est censé être renvoyé vers l’application plutôt que de rester sur la page du navigateur. Vérifiez que tous les champs de votre configuration IdP qui gèrent le RelayState sont laissés vides (le champ peut être nommé différemment : par exemple, ce serait **Default RelayState** dans Okta, ou *Start URL* dans Google SSO).
4. Si le problème persiste, il est possible que l’appareil en question ne puisse pas accéder à l’environnement d’authentification unique de l’entreprise.  Vérifiez auprès de votre service informatique s’il existe des restrictions quant aux appareils autorisés à utiliser l’authentification unique. Par exemple, pour les solutions de gestion des appareils mobiles (MDM), des problèmes peuvent survenir si Miro n’est pas correctement autorisé/span>[.](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)
5. Pour l’application de bureau Miro spécifiquement : vérifiez que le schéma de notre application fonctionne et n’est pas cassé.  Pour ce faire, saisissez **miroapp://** dans la barre d’adresse de votre navigateur préféré et cliquez sur *Ouvrir en tant que site Web* (ne pas appuyer simplement sur Entrée sous peine de lancer une recherche).
   ![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)
   À ce moment-là, vous êtes censé recevoir un ​vous invite à ouvrir l'application Miro. Si ce n’est pas le cas, le schéma est peut-être cassé. Pour vérifier si le schéma est correctement installé, suivez les instructions pour Windows ou Mac (cela ne s’applique pas à la version Microsoft Store de l’application Miro).

   Pour Windows Pour Mac

   1. Allez dans l’[application Éditeur du registre](https://support.microsoft.com/windows/how-to-open-registry-editor-in-windows-10-deab38e6-91d6-e0aa-4b7c-8878d9e07b11).
   2. Appuyez sur Ctrl + F et cherchez **miroapp.**  Votre registre devrait ressembler à ceci :/strong>
      ![registry_editor_map.png](images/21016057564306_registry editor map.png)

   1. Exécutez la commande suivante dans l’application Terminal :

      **sudo /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/Support/lsregister -dump URLSchemeBinding | grep miroapp**

      Le résultat doit ressembler à ceci :

      ![](/attachments/token/I53o1MUemZ9TqkRlz9dQ7ndsr/?name=image.png)

Si votre situation diffère (par exemple si le rapport du schéma n’est pas affiché dans le registre ou s’affiche selon un chemin différent), essayez de réinstaller l’application [à partir de notre site Web](https://miro.com/apps/).

Si cela ne résout pas le problème, contactez votre équipe informatique et demandez-lui de vérifier la situation, notamment les points suivants :

- Est-ce que les protocoles d’URI personnalisés sont autorisés ?  S’ils sont bloqués, il se peut que notre schéma ne se soit pas installé pendant le processus d’installation de l’application.
- Est-ce que le registre fait l’objet d’autres restrictions ou politiques susceptibles d’empêcher ou de modifier l’installation standard ?

## Mon adresse e-mail a changé et je ne peux pas me connecter à mon profil via l’authentification unique

Veuillez noter que si votre organisation utilise l’authentification unique, la modification de l’adresse e-mail doit être effectuée du côté de Miro et du côté du fournisseur d’identité avant qu’un utilisateur final puisse utiliser ses nouveaux identifiants pour se connecter à Miro.  Si les modifications n’ont pas été effectuées avant la prochaine connexion, votre adresse e-mail sera reconnue comme un nouvel utilisateur et vous pourriez rencontrer des problèmes pour vous connecter à Miro.

Contactez votre admin pour clarifier la situation.  Vous et votre admin devrez peut-être contacter le service d’assistance de Miro/span> [afin que nous puissions supprimer votre nouveau profil vide et modifier l’adresse e-mail du profil existant.](../../tools/troubleshooting/06-contacting-miro-support.md)  Veuillez fournir les informations suivantes :

- Votre nouvelle et votre ancienne adresses e-mail
- Placez l’admin Miro de votre entreprise en copie et demandez-lui d’envoyer une confirmation comme quoi nous pouvons procéder au changement (obligatoire pour des raisons de sécurité).

:::note
Si vous n’avez pas trouvé la solution à votre problème dans cet article, [contactez le service d’assistance de Miro](https://miro.com/contact/recover/).
:::
