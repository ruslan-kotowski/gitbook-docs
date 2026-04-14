---
title: Guide pour les admins - Authentification à deux facteurs (2FA) pour l'enterprise
article_id: 7935391125394
translation_id: 7935391125394
locale: fr
sidebar_position: 1
created_at: '2022-10-04T08:57:18Z'
updated_at: '2026-01-13T13:35:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Pertinent pour: Plan Enterprise Mis en place par: Admins d’entreprise'
---

## Authentification à deux facteurs (2FA) pour les organisations

La 2FA ajoute une couche supplémentaire de sécurité aux profils en ligne, allant au-delà du simple nom d'utilisateur et mot de passe. Les admins d’entreprise peuvent exiger une preuve d'identité supplémentaire lorsque les utilisateurs accèdent à l'abonnement Miro de leur organisation. Cette exigence s'applique à toutes les connexions utilisant un e-mail et un mot de passe.

Pour les entreprises utilisant la SSO, la 2FA inclut uniquement les collaborateurs externes non-SSO. Pour les entreprises n'utilisant pas la SSO, la 2FA s'étend à tous les utilisateurs.

:::note
Cet article explique l'authentification à deux facteurs (2FA) pour les forfaits Enterprise. Pour tous les autres forfaits, voir [Authentification à deux facteurs (2FA)](../../../administration/security-compliance/01-two-factor-authentication-2fa.md) dans Administration.
:::

## Configuration de l’authentification à deux facteurs forcée pour votre organisation

:::note
Avant d'activer l’authentification à deux facteurs (2FA), il est important d'informer tous les utilisateurs concernés, y compris les membres de votre organisation et les collaborateurs externes. Pour assurer une transition en douceur, nous vous suggérons de partager notre [guide utilisateur 2FA](../../security-integrations/two-factor-authentication-2fa/02-enterprise-two-factor-authentication-2fa-–-user-guide.md) pour les aider à traverser ce processus.
:::

## Activer l’authentification à deux facteurs pour vos utilisateurs

1. Allez dans la console d'admin > **Sécurité** > **Authentification**.
2. Activez **Appliquer l'authentification à deux facteurs pour les utilisateurs non-SSO**.

![2FA-enable.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24790277317394_2FA-enable.png)*Appliquer l'authentification 2FA pour les utilisateurs non-SSO*

### Faire confiance aux appareils 2FA

Lorsqu'elle est activée, vos utilisateurs 2FA verront une case à cocher leur permettant de sauter la 2FA à chaque connexion sur cet appareil pour les X prochains jours, où "X" est la période définie par l'administrateur. Vous pouvez permettre que les appareils des utilisateurs soient approuvés pour une durée de 7 à 90 jours. Par défaut, l'approbation des appareils 2FA est activée, mais vous pouvez désactiver cette fonctionnalité dans votre console d’admin.

![2FA-trusted-devices.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24790277323410_2FA-trusted-devices.png)

:::warning
Si l'approbation des appareils 2FA est désactivée, les utilisateurs devront saisir un code 2FA à chaque connexion. Cela ralentira leur expérience de connexion.
:::

La 2FA sera à nouveau requise après la période d'approbation passée.

La 2FA ne sera pas sautée si les utilisateurs se connectent sur un nouvel appareil ou navigateur, ou s'ils effacent les cookies de leur navigateur.

## Réinitialisation de la 2FA pour les utilisateurs

Si un utilisateur perd l'accès à sa méthode d'authentification à deux facteurs (2FA), les admins peuvent réinitialiser leur 2FA. Une fois qu'un utilisateur demande à ce que sa méthode 2FA soit réinitialisée, l'admin concerné recevra une notification par e-mail.

:::note
Les admins peuvent réinitialiser l'authentification à deux facteurs uniquement pour les utilisateurs dont les domaines de messagerie sont vérifiés au sein de leur organisation, si l'admin est à l'origine de la réinitialisation. Si l'utilisateur demande une réinitialisation, tout admin de l'organisation peut l'approuver.
:::

Pour réinitialiser la méthode 2FA de l'utilisateur :

1. Allez dans **console d’admin** > **Utilisateurs** > **Utilisateurs actifs** tab.
2. Trouvez l'utilisateur qui doit réinitialiser sa méthode d'authentification à 2 facteurs.
3. Cliquez sur l'icône des **trois points** (**...**) sur la ligne de l'utilisateur.
   ![reset-2fa.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24650686629138_reset-2fa.png)
   *Réinitialisation de l'authentification à deux facteurs dans la console d’admin*
4. Cliquez sur **Réinitialiser l’authentification à deux facteurs**.
   Une boîte de dialogue s'ouvrira pour demander une confirmation.
5. Cliquez sur le bouton **Réinitialiser la 2FA** dans la boîte de dialogue.
6. Un message de confirmation apparaîtra en haut de votre écran confirmant que les instructions de réinitialisation ont été envoyées à l'utilisateur.

## Impact sur l’expérience utilisateur

- Les utilisateurs sans authentification unique seront invités à configurer leur deuxième facteur lors de leur prochaine connexion. Ce processus ne les déconnectera pas des sessions en cours.
- Les utilisateurs doivent configurer l’authentification à deux facteurs à l’aide de leur appareil mobile et de toute application de mot de passe unique limité dans le temps (TOTP), comme Microsoft Authenticator, Google Authenticator ou Authy.
- Pour les utilisateurs utilisant l’authentification à deux facteurs, il y a une limite de 3 tentatives pour entrer un code TOTP valide. Si cette limite est dépassée, ils devront recommencer le processus d’authentification.
- Bien que la connexion via l’authentification à deux facteurs soit disponible sur les applications mobiles et tablettes, le processus d’enregistrement initial n’est pris en charge que sur les applications de navigateur et de bureau.

## Important à savoir

L'application de l'authentification à deux facteurs concerne uniquement *les utilisateurs s'authentifiant avec leur e-mail et mot de passe ou via des liens magiques (envoyés par e-mail)*.

- La 2FA n'est pas activée pour les collaborateurs externes qui s'authentifient à l'aide de SSO.
- Si un collaborateur ou une collaboratrice externe à votre organisation sur forfait Enterprise s’authentifie déjà grâce au SSO de sa propre organisation, ils continueront d’accéder à toutes les équipes et tous les tableaux Miro à l’aide du SSO.
- Lorsqu'un utilisateur s'authentifie via une intégration de connexion tierce (par exemple, Google, Microsoft, Slack), il continuera d'accéder à toutes les équipes et tous les tableaux dans Miro via cette méthode de connexion. Les administrateurs ont la possibilité d'encourager ces utilisateurs à configurer un second facteur au sein de leur intégration de connexion respectif. Cependant, le processus d'authentification de Miro ne demandera pas à ces utilisateurs de configurer un second facteur.

## Journaux d’audit

Les administrateurs peuvent suivre les utilisateurs ayant configuré l’authentification à deux facteurs ainsi que les réussites et échecs de connexion avec les événements de journal d’audit suivants :

- ’mfa_setup_succeeded’ - si un utilisateur a configuré avec succès son second facteur
- Mise à jour vers l'événement 'sign_in_succeeded' pour inclure l'attribut MfaFactorType si une connexion réussie a lieu avec l'authentification à deux facteurs
- Mise à jour vers l'évènement 'sign_in_failed' pour inclure l'attribut MfaFactorType si une connexion avec l’authentification à deux facteurs a échoué en raison de l’utilisateur ayant dépassé le nombre maximum de tentatives (échec non technique)
