---
title: Authentification à deux facteurs (2FA)
article_id: 27356474050834
translation_id: 27356474050834
locale: fr
sidebar_position: 1
created_at: '2025-06-12T12:01:03Z'
updated_at: '2025-06-24T08:19:34Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  notes: 'Qui peut le faire: Admins d’équipe, admins d’entreprise Quels forfaits:
    Starter, Business, Education, Enterprise Quelles plateformes: Navigateur, Bureau,
    Mobile'
---

L'authentification à deux facteurs (2FA) ajoute une couche de sécurité supplémentaire aux comptes en ligne en exigeant des utilisateurs qu'ils fournissent deux méthodes de vérification uniques avant d'accéder à leurs comptes.

Les admins Miro peuvent activer l'authentification à deux facteurs (2FA) pour leurs équipes et réinitialiser la 2FA pour les membres de l'équipe. Les utilisateurs ont la possibilité de faire confiance à un appareil pendant 30 jours.

:::note
Cet article explique l'authentification à deux facteurs (2FA) pour les forfaits Starter, Business et Education. Pour en savoir plus sur l'authentification à deux facteurs pour Enterprise, consultez le [guide admin de l'authentification à deux facteurs (2FA).](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)
:::

## Activer l’authentification à deux facteurs

Pour les forfaits Starter et Education, assurez-vous d'avoir le rôle d'admin d’équipe.

Pour un forfait Business, assurez-vous d'avoir le rôle d'admin d'entreprise.

Suivez les étapes suivantes :

1. Depuis votre tableau de bord Miro, cliquez sur votre avatar dans le coin supérieur droit et sélectionnez **Console d'administration**.
2. (Starter) Rendez-vous dans **Sécurité**>**Autorisations**.
   (Éducation) Allez à **Permissions**.
   Rendez-vous dans **Sécurité** > **Authentification**.
3. Sous **Authentification à deux facteurs (2FA)**, activez **Exiger l’authentification à deux facteurs lors de la connexion**.

## Configuration de l’authentification à deux facteurs (2FA) pour les utilisateurs

Pour les équipes qui ont activé l'authentification à deux facteurs (2FA), les utilisateurs doivent s'authentifier en utilisant une application d'authentification, en plus de leur e-mail et de leur mot de passe.

Pour apprendre à configurer l'authentification à deux facteurs (2FA) en tant qu'utilisateur, consultez le [guide de l’utilisateur sur l’authentification à deux facteurs (2FA)](02-two-factor-authentication-2fa-–-user-guide.md).

## Appareils de confiance

Un utilisateur se connectant à Miro avec l'authentification à deux facteurs (2FA) peut choisir de faire confiance à son appareil.

Lors de l'utilisation d'un appareil de confiance pour se connecter, l'utilisateur ne sera invité à s'authentifier qu'avec son premier facteur, en sautant le deuxième facteur, car l'appareil est de confiance.

![](../../../../../../docs/administration/security-compliance/images/27358547112978_image.png)

*Le dispositif de confiance pour l’authentification à deux facteurs (2FA) est activé par défaut.*

Lors de la connexion, **Faire confiance à cet appareil pendant 30 jours** est sélectionné par défaut, ce que l'utilisateur peut désélectionner.

:::note
La période de confiance du dispositif ne peut être modifiée que sur un forfait Enterprise. Pour plus d'informations, consultez le [guide d’administration sur l'authentification à deux facteurs (2FA)](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md).
:::

Pour ne plus faire confiance à un appareil auquel on a accidentellement fait confiance, un utilisateur peut se déconnecter de partout. Allez dans **Profil**, sous **Paramètres du profil**, cliquez sur **Se déconnecter partout**.

## Réinitialiser l’authentification à 2 facteurs

Si un utilisateur perd l'accès à son deuxième facteur, il peut demander à son admin de réinitialiser son 2FA.

Pour réinitialiser la 2FA pour les utilisateurs des forfaits Starter et Education, assurez-vous d'avoir le rôle d'admin d’équipe.

Pour réinitialiser l'A2F pour les utilisateurs d'un forfait Business, assurez-vous que vous avez le rôle d'admin d'entreprise.

Suivez les étapes suivantes :

1. Cliquez sur votre avatar dans le coin supérieur droit de votre tableau de bord Miro et sélectionnez **Console d'admin**.
2. Allez à **Utilisateurs** > **Tous les utilisateurs**.
3. Localisez l’utilisateur, puis sélectionnez les trois points (**...**) à la fin de la ligne.
4. Cliquez sur **Réinitialiser l'authentification à deux facteurs**.
   L'utilisateur reçoit des instructions de réinitialisation par e-mail.
