---
title: Authentification à deux facteurs (2FA) pour entreprise – guide de l'utilisateur
article_id: 7935469290002
translation_id: 7935469290002
locale: fr
sidebar_position: 2
created_at: '2022-10-04T09:00:42Z'
updated_at: '2025-11-06T13:50:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Utile pour: Starter, Business, Education, Enterprise'
---

## Qu’est-ce que l’authentification à deux facteurs (2FA)

L’authentification à deux facteurs (2FA) renforce la sécurité de vos comptes en ligne. Lorsque votre admin d’entreprise active l’authentification à deux facteurs (2FA), chaque connexion à Miro à l’aide de votre e-mail et de votre mot de passe sera suivie d’une couche de sécurité supplémentaire. Cette étape supplémentaire assure une protection accrue de votre compte, en exigeant une vérification au-delà de vos identifiants de connexion habituels.

:::tip
Apprenez comment activer l'authentification à 2 facteurs (2FA) pour votre organisation pour les [forfaits Enterprise](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md), et [tous les autres forfaits](../../../administration/security-compliance/01-two-factor-authentication-2fa.md).
:::

## Comment mettre en place l’authentification à deux facteurs (2FA)

**Nouveaux utilisateurs :** Lors de la [procédure d'inscription](https://miro.com/signup/) initiale avec votre adresse e-mail d’entreprise, vous serez invité à activer la fonction 2FA.
**Utilisateurs existants :** Lors de votre prochaine [connexion](https://miro.com/login/), si votre organisation exige l’authentification à deux facteurs (2FA) et que vous n’utilisez pas l’authentification unique (SSO), vous serez invité à configurer l’authentification à deux facteurs.

1. Téléchargez une application d’authentification sur votre appareil mobile. Les applications d’authentification, telles que Google Authenticator, Microsoft Authenticator et Authy, génèrent un code à usage unique basé sur le temps (TOTP) pour les connexions sécurisées à Miro. Pour savoir quelle application d’authentification choisir, adressez-vous à votre admin d’entreprise ou à votre administrateur informatique.

2. Cliquez sur **J'ai une application d'authentification** dans l'écran de configuration de la 2FA de Miro.

   ![2FA-setup-step-1-Confirmation-of-authenticator-app-download.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653633554_2FA-setup-step-1-Confirmation-of-authenticator-app-download.png)
   *Confirmation de l'application d'authentification*
3. En utilisant l’application d’authentification, vous avez maintenant deux options :


   Scannez le code QR

   1. Ouvrez votre application d’authentification.
   2. Utilisez l’application pour scanner le code QR.
   3. Après la numérisation, cliquez sur **J’ai numérisé le code**
      dans Miro.

      ![2FA-setup-step-2-Scan-QR-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683263122_2FA-setup-step-2-Scan-QR-code.png)*Numérisation du code QR*

   Saisir manuellement le code Miro

   1. Si vous ne parvenez pas à scanner le code QR, cliquez sur **Can’t scan QR code?** dans Miro.
   2. Miro vous fournira alors un code d’authentification. **Copiez** ce code.
   3. Ouvrez votre application d'authentification et collez le code copié.
   4. Après avoir ajouté le code à l’application, cliquez sur **J’ai ajouté le code** dans Miro.

      ![2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653636754_2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png)*Copie du code Miro pour le coller dans l’application d'authentification*
4. L’application authentificateur génère un code de vérification à 6 chiffres. Saisissez ce code dans Miro et cliquez sur **Vérifier le code**.

   ![2FA-setup-step-3-enter-6-digit-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653634706_2FA-setup-step-3-enter-6-digit-code.png)
   *Vérification du code à 6 chiffres*
5. Après avoir vérifié votre compte avec le code à 6 chiffres, Miro vous fournira un code de récupération. Cliquez **Copier** pour enregistrer ce code en toute sécurité. Il est crucial d’avoir ce code car il vous permet de réinitialiser votre 2FA au cas où vous perdriez l’accès à votre application d’authentification.

   Pour confirmer que vous avez enregistré le code, sélectionnez **J’ai enregistré ce code**, puis cliquez sur **Continuer** pour terminer le processus.

   ![Save-2FA-recovery-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683265554_Save-2FA-recovery-code.png)*Enregistrement du code de récupération*

## Connexion avec l’authentification à deux facteurs (2FA)

Une fois que vous avez réussi à configurer l’authentification à deux facteurs (2FA) pour votre compte, chaque fois que vous tenterez de vous connecter, Miro vous invitera à saisir un code unique à 6 chiffres basé sur le temps (TOTP).

Ce code est généré par votre application d’authentification et fournit une couche de sécurité supplémentaire pour votre compte. Il suffit d’ouvrir votre application d’authentification, de récupérer le code actuel et de le saisir sur la page de connexion pour accéder à votre compte.

![2fa-user-guide.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/20847806879634_2fa-user-guide.png)
*Connexion à Miro avec 2FA*

Vous disposez de trois tentatives avant d’être invité à redémarrer la procédure de connexion.

![Too-many-attempts.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683267346_Too-many-attempts.png)*Trop de tentatives de connexion avec l'authentification à deux facteurs*

### Faire confiance aux dispositifs d’authentification à deux facteurs (2FA)

Si votre administrateur l’a configuré, vous pouvez cocher la case **Faire confiance à cet appareil** lors de la connexion à votre compte avec 2FA lorsque vous utilisez un appareil sécurisé (n’utilisez pas **Faire confiance à cet appareil** si vous vous connectez à partir d’un ordinateur partagé ou accessible au public). Dans ce cas, vous pourrez vous connecter sans saisir votre deuxième facteur, jusqu’à ce qu’une période de temps déterminée se soit écoulée. Cette période est fixée par votre administrateur entre 7 et 90 jours.

![2FA-signin.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/19612606396818_2FA-signin.png)

*La durée de confiance d’un appareil est affichée à côté de la case à cocher lors de la connexion avec l’authentification à deux facteurs*

Si vous ne voyez pas l’option "Faire confiance à ce périphérique", c’est que votre administrateur ne l’a pas activée pour votre organisation.

Si vous vous connectez avec un nouvel appareil, ou après avoir effacé les cookies de votre appareil de confiance, l’authentification à deux facteurs sera de nouveau nécessaire.

## Comment réinitialiser l’authentification à deux facteurs (2FA) ?

Si vous rencontrez des problèmes avec votre application d’authentification, si vous perdez votre appareil ou si vous devez réinitialiser votre 2FA pour toute autre raison, suivez ces étapes :

### J’ai un code de récupération

1. Cliquez sur **Réinitialiser l’authentification à deux facteurs**.
2. Utilisez le code de récupération enregistré lors de votre configuration initiale de 2FA. Vous serez à nouveau guidé à travers le processus de configuration pour reconfigurer votre application d'authentification.

![Reset-two-factor-authentication.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683268114_Reset-two-factor-authentication.png)*L’option de réinitialisation de l'authentification à deux facteurs.*

### Je n’ai pas de code de récupération

Si vous avez perdu votre code de récupération ou que vous ne pouvez pas utiliser le flux d’auto-récupération, vous devrez demander à votre admin de réinitialiser votre 2FA.

Si votre domaine de messagerie ne fait pas partie des domaines vérifiés de votre organisation, votre admin ne pourra pas initier de réinitialisation pour vous. Vous devrez demander vous-même une réinitialisation de l'authentification à deux facteurs - votre admin pourra alors l'approuver.

Les admins peuvent réinitialiser l'authentification à deux facteurs uniquement pour les utilisateurs dont les domaines de messagerie sont vérifiés dans leur organisation, si l’admin initie la réinitialisation. Si l'utilisateur demande une réinitialisation, tout admin de l'organisation peut l'approuver.

Suivez les étapes suivantes :

1. Cliquez sur **Demandez à votre admin de réinitialiser**.
   ![2fa-user-reset.png](https://help.miro.com/hc/article_attachments/24650844819602)
   *Demandez à votre admin de réinitialiser votre 2FA si vous n'avez pas de code de récupération*
2. Si vous appartenez à plusieurs organisations utilisant le 2FA, vous devrez sélectionner à quel admin d'organisation vous souhaitez faire la demande.
3. Vous recevrez un e-mail avec un code de vérification.
4. Saisissez le code de vérification.
5. Une confirmation que la demande a été envoyée à l'admin choisi vous sera affichée.
6. Lorsque l'admin réinitialise votre 2FA, vous devrez passer par le processus de configuration de la 2FA lors de votre prochaine connexion.

## Foire aux questions

Pourquoi dois-je configurer 2FA ?

L’authentification à deux facteurs renforce la sécurité de votre organisation. Tous les utilisateurs non-SSO doivent utiliser l’authentification à deux facteurs pour se connecter si cette exigence est appliquée par votre admin d'entreprise.

Dois-je utiliser 2FA à chaque connexion ?

Oui. Après avoir effectué la configuration initiale, vous devez utiliser votre application d’authentification pour chaque connexion afin de garantir la sécurité de votre compte.

J’ai essayé de configurer 2FA mais j’ai reçu un message d’erreur "Code invalide", alors que mon code est correct. Que dois-je faire ?

Assurez-vous que le fuseau horaire, la date et l’heure de votre appareil sont correctement réglés. Si le problème persiste, essayez de configurer 2FA sur un autre appareil.

Que se passe-t-il si je fais accidentellement confiance à un appareil partagé ?

Si vous faites accidentellement confiance à un appareil partagé, vous devrez effacer les cookies de Miro sur cet appareil. C’est très simple :

1. Cliquez sur l’icône du curseur à gauche de la barre d’adresse de votre navigateur.
2. Cliquez sur "Cookies et données du site" dans le menu.
3. Cliquez ensuite sur "Gérer les données du site sur l’appareil".
4. Cliquez sur l’icône de la corbeille à côté de chaque URL répertoriée pour effacer les cookies et les données du site.

Notez qu’une fois les données du site effacées de l’appareil, vous devrez vous connecter à nouveau à l’aide de l’authentification à deux facteurs.

Que se passe-t-il si je perds l’accès à un appareil de confiance ?

Si vous perdez l’accès à un appareil de confiance avant l’expiration de la période de confiance, vous pouvez utiliser l’option **Se déconnecter partout** pour supprimer l’accès à tous les appareils connectés (à l’exception de l’appareil que vous utilisez actuellement). Cela vous déconnectera de tous les autres appareils et révoquera l’option 2FA de tous les appareils de confiance. Vous trouverez le lien **Se déconnecter partout** dans les paramètres de votre profil d’utilisateur. Vous devrez ensuite repasser par la procédure de connexion 2FA sur les appareils auxquels vous avez accès.
