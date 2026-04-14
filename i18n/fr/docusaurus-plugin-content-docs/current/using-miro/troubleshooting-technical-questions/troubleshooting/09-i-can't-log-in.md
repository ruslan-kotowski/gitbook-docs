---
title: Je ne peux pas me connecter
article_id: 360020993079
translation_id: 360020993079
locale: fr
sidebar_position: 9
created_at: '2021-04-09T06:31:47Z'
updated_at: '2025-11-25T16:04:24Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Suivez ce guide si vous rencontrez des problèmes pour vous connecter à votre profil Miro.

## Problèmes relatifs à l’adresse e-mail et/ou au mot de passe

Mon adresse e-mail/mot de passe ne fonctionne pas

Voici deux solutions que vous pouvez explorer :

1. Vérifiez que l’adresse e-mail/le mot de passe que vous utilisez pour vous connecter ne comporte pas de fautes de frappe.
2. Si les identifiants que vous saisissez sont corrects, [réinitialisez votre mot de passe](../../managing-your-profile/05-how-to-change-your-password.md).
3. Si votre adresse e-mail ou votre mot de passe comprend l’un des symboles **& " < >**, [contactez notre service d’assistance.](https://help.miro.com/hc/requests/new?)

:::warning
Notez que votre **profil est verrouillé** après 10 tentatives infructueuses de saisie de votre adresse e-mail et de votre mot de passe. Vous devrez peut-être d’abord [déverrouiller votre profil](../../tools/troubleshooting/14-profile-lockout.md), puis réinitialiser votre mot de passe.
:::

Je ne peux pas réinitialiser mon mot de passe

Trois raisons peuvent expliquer pourquoi vous ne recevez pas d’e-mail de réinitialisation de mot de passe :

1. **L’adresse e-mail est incorrecte**
Assurez-vous que l’adresse e-mail que vous avez fournie ne contient pas de faute de frappe. Tentez de refaire une demande de réinitialisation si vous trouvez une faute de frappe.

2. **L’adresse e-mail n’est pas encore enregistrée auprès de Miro**
Dans ce cas, le lien de réinitialisation du mot de passe ne sera pas envoyé à votre adresse e-mail. Enregistrez un nouveau profil sur la [page d’inscription](https://miro.com/signup/). Si votre adresse e-mail est enregistrée, vous verrez le message correspondant :
![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)

3. **La livraison de l’e-mail rencontre des problèmes**

- Ouvrez vos dossiers **Spam, Promotions, Courrier indésirable, Réseaux sociaux** et **Notifications** et vérifiez si l’e-mail de demande de réinitialisation s’y trouve.
- Il se peut également qu’un pare-feu empêche l’e-mail d’atteindre votre boite de réception.

  Demandez à votre *admin système* d’autoriser nos domaines et sous-domaines : [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) et [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/), puis ajoutez l’IPS de notre système d’envoi d’e-mails dans votre liste d’autorisations.

  Voici la liste des IP dédiées : 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. [Voici un article](../../tools/troubleshooting/02-allowlist-miro-mailers.md) contenant plus d’informations sur les expéditeurs que vous devez autoriser.

J’ai réinitialisé mon mot de passe, mais je n’arrive toujours pas à me connecter

Si vous ne parvenez toujours pas à accéder à votre profil :

1. Assurez-vous d’entrer le nouveau mot de passe.
2. Connectez-vous à partir du mode privé (incognito) de votre navigateur ou essayez un autre navigateur.

Je me connecte avec une adresse e-mail, mais l’interface me redirige et me connecte avec une autre adresse e-mail

Le problème peut survenir si vous utilisez une méthode d’authentification alternative pour vous connecter (Google, Slack, Office 365, Apple ID, Facebook).

![new-sing-in-third-party.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)
*Autres options de connexion sur la page de connexion*

Vous avez peut-être accidentellement lié votre adresse e-mail Google/Office 365/etc. à votre profil Miro enregistré sous une autre adresse e-mail. Dans ce cas, essayez ce qui suit :

1. Supprimez l’association erronée avec l’adresse e-mail en allant dans **Paramètres du profil** > **Intégrations** et en cliquant sur **Se déconnecter** à côté de Google/Office 365/etc.
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Supprimer l’association avec la connexion Google*
2. Déconnectez-vous et connectez-vous à nouveau avec votre adresse e-mail.

:::note
Configurez une connexion avec l’adresse e-mail Google/Office 365/Slack qui correspond à l’adresse e-mail de votre profil Miro pour éviter de rencontrer ce problème.
:::

## La connexion via SSO ne fonctionne pas

Consultez l’article : [Je ne parviens pas à me connecter via l’authentification unique](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## Chargement sans fin lors de la connexion

Pour les utilisateurs qui rencontrent des problèmes de chargement sans fin après avoir entré leurs informations d’identification Miro, nous recommandons ce qui suit :

1. Connectez-vous depuis un **autre navigateur**.
2. Connectez-vous en utilisant le **mode de navigation privée de votre navigateur.** Si le problème ne survient pas en navigation privée ou depuis un autre navigateur, videz le cache de votre navigateur.

   Comment vider le cache de Chrome

   1. Rendez-vous sur `https://miro.com/` et ouvrez les **Outils de développement**de Chrome (**Commande + Option + J** *sur Mac*, **Ctrl + Shift + J***sur Windows*).
   2. Choisissez l’onglet **Appli > Stockage**. Vous verrez le bouton bleu **Effacer les données des sites.**  Cliquez sur le bouton et cela devrait supprimer toutes les données Miro enregistrées dans votre navigateur Chrome pour que vous puissiez commencer une nouvelle session de travail.
   ![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
   *L’option permettant de supprimer les données des sites dans Chrome*
3. Si vous utilisez un **VPN**, activez/désactivez-le.
4. Vérifiez auprès de votre service informatique si votre entreprise utilise des pare-feux ou un proxy susceptibles de bloquer Miro. Suivez [ces directives](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md) pour **autoriser Miro** ou fournir une méthode de contournement.
5. Vérifiez votre connexion Internet. Si la bande passante de votre réseau n’atteint pas le minimum de 8 Mbit/s, **passez sur un autre réseau, de préférence** **plus rapide**.
6. Essayez de vous connecter à un **hotspot mobile**, si possible. Reconnectez-vous ensuite à votre réseau d’origine.
7. Si cela ne résout pas le problème, [soumettez une demande](https://miro.com/contact/recover/) et [envoyez les journaux de la console de votre navigateur au service d’assistance](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

## Problèmes de connexion sur l’application de bureau Miro

1. Si vous ne pouvez pas accéder à Miro sur l’application de bureau, connectez-vous depuis votre navigateur. Si vous ne parvenez toujours pas à vous connecter, suivez les étapes ci-dessus. Suivez les étapes ci-dessous si vous pouvez accéder à Miro dans le navigateur.
2. Réinitialisez les données de l’application.

Réinitialiser les données de l’application sur Windows

Appuyez sur **Alt > Help (Aide)** et choisissez de réinitialiser les données de l’application comme indiqué dans la capture d’écran ci-dessous :

​​![reset_app_data_on_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725434514_reset%20app%20data%20on%20Windows.jpg)
*Réinitialiser les données de l’application sur l’application de bureau pour Windows*

Si vous ne trouvez pas le menu, vous utilisez probablement l’application téléchargée depuis le MS Store. Dans ce cas, pour réinitialiser les données de l’application, ouvrez Windows **Settings** (Paramètres Windows) > **Apps** (Applications) > **Apps and Features** (Applications et fonctionnalités) > recherchez **Miro** dans la liste > **Advanced options**(Options avancées) > **Reset** (Réinitialiser).

Si cela ne vous aide pas immédiatement, supprimez tous les fichiers de l’application situés dans **C:\Users\username\AppData\Roaming\RealtimeBoard** et **C:\Users\username\AppData\Local\RealtimeBoard**

> **✏️** Si le dossier **Appdata** est masqué, découvrez [ici](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) comment l’afficher.

Comment réinitialiser les données de l’application sur Mac

Cliquez sur Miro dans le menu supérieur et choisissez **Reset application data** (Réinitialiser les données de l’application) comme indiqué dans la capture d’écran ci-dessous :

![reset_app_data_on_Mac.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
*Réinitialiser les données de l’application sur Mac*

Après cela, essayez de vous reconnecter à l’application et vérifiez si le problème est résolu.

Si la réinitialisation ne vous aide pas immédiatement, ouvrez une fenêtre de recherche > appuyez sur **Commande + Maj + G**> collez **~/Library/Application Support/RealtimeBoard**et supprimez tous les fichiers de l’application.

3. Si le problème persiste, assurez-vous que vous utilisez la dernière version de l’application téléchargée [depuis notre site Web.](https://miro.com/apps/)

## Connexion Google/Office 365/Slack/etc.

Je ne peux pas me connecter via Google/Office/Slack/etc.

1. Connectez-vous à Miro en utilisant vos identifiants standards (adresse e-mail et mot de passe). Si vous ne vous souvenez pas de votre mot de passe ou si vous ne le connaissez pas, [réinitialisez-le](../../managing-your-profile/05-how-to-change-your-password.md).
2. Allez dans **Paramètres du profil** > **Intégrations**, cliquez sur **Se déconnecter** en regard de Google/Office 365/etc. et reconfigurez la connexion.
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Supprimer l’association avec la connexion Google*

Je ne peux pas me connecter via Google/Office/Slack/etc. sur l’application de bureau

Consultez ces étapes de dépannage.

J’avais l’habitude de me connecter à Miro via Google/Office 365/etc., mais mon service de messagerie a changé. Comment puis-je me connecter maintenant ?

Connectez-vous à Miro en utilisant vos nouveaux identifiants de service (adresse e-mail et mot de passe). Si vous ne vous souvenez pas du mot de passe ou si vous ne le connaissez pas, [réinitialisez-le](../../managing-your-profile/05-how-to-change-your-password.md).

## Problèmes de connexion sur tablette/mobile

1. Vérifiez si vous pouvez vous connecter à la version du navigateur. Si ce n’est pas le cas, nous vous recommandons de suivre ces étapes de dépannage.
2. Si la connexion fonctionne pour vous dans le navigateur, il se peut que les données d’authentification de votre appareil soient corrompues. Allez dans **Paramètres de l’application > Stockage > Effacer le stockage** ou réinstallez l’application Miro sur votre appareil.

## Astuces de dépannage

Si aucune des solutions proposées ci-dessus ne fonctionne pour vous, connectez-vous à Miro en utilisant **un autre navigateur** ou **en mode de navigation privée**. Si tout va bien dans le mode incognito de votre navigateur, effacez le cache et les cookies du navigateur et connectez-vous à Miro en mode standard.

Comment vider le cache de Chrome

1. Rendez-vous sur `https://miro.com/` et ouvrez les **Outils de développement**de Chrome (**Commande + Option + J** *sur Mac*, **Ctrl + Shift + J***sur Windows*).
2. Choisissez l’onglet **Appli > Stockage**. Vous verrez le bouton bleu **Effacer les données des sites.**  Cliquez sur le bouton et cela devrait supprimer toutes les données Miro enregistrées dans votre navigateur Chrome pour que vous puissiez commencer une nouvelle session de travail.

![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
*L’option permettant de supprimer les données des sites dans Chrome*

Si cette opération ne résout pas le problème, [contactez le service d’assistance Miro](https://miro.com/contact/recover/). Décrivez le problème en détail.

:::note
Si vous rencontrez des problèmes lors de votre inscription avec Miro, consultez [Problèmes avec les e-mails de code de confirmation](../../tools/troubleshooting/12-issues-with-confirmation-code-or-password-reset-emails.md).
:::
