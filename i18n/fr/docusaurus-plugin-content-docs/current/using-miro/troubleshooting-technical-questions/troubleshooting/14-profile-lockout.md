---
title: Verrouillage de profil
article_id: 360017571374
translation_id: 360017571374
locale: fr
sidebar_position: 14
created_at: '2019-02-11T10:08:55Z'
updated_at: '2026-02-24T12:02:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Le verrouillage de profil se fait par défaut pourtous les utilisateurs et tous les forfaits Miro, la personnalisation n'est pas disponible. Les utilisateurs qui tentent de [s’authentifier par le biais de fournisseurs d’identité externes](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) ne seront pas affectés par cette fonctionnalité.

Après un mauvais mot de passe pour votre profil, vous avez **10 tentatives** pour entrer le bon mot de passe pour une paire e-mail/mot-de-passe. Les 5 premières tentatives sont classiques et sans complexité supplémentaire.

Les tentatives suivantes comprennent un captcha (uniquement pour les applications web et de bureau). Si vous ne parvenez pas à fournir le bon mot de passe **10 fois de suite** pour une paire e-mail/mot-de-passe, votre profil utilisateur est verrouillé pendant**1 heure**, durant laquelle toutes les tentatives de connexion au profil échoueront même si un mot de passe correct est fourni.

:::tip
Pendant l'heure de verrouillage, vous pouvez essayer de vous connecter sans mot de passe ou avec un fournisseur social.
:::

Si votre profil utilisateur est verrouillé, Miro vous envoie un e-mail avec un code à six chiffres pour déverrouiller votre profil. Le lien dans l’e-mail vous redirige vers la page de confirmation où vous devrez fournir le code à six chiffres. Si le code fourni est correct, votre profil est déverrouillé et les tentatives de connexion sont réinitialisées. L’e-mail vous invite également à remplacer votre mot de passe.

Le profil verrouillé est déverrouillé **automatiquement** après 1 heure et le nombre de tentatives échouées est réinitialisé.

### Que faire si vous ne recevez pas le code ?

Si vous ne trouvez pas l’e-mail dans votre boîte de réception, essayez ces étapes de dépannage :

- Assurez-vous que l’adresse e-mail que vous avez fournie ne contient pas de faute de frappe. Si vous trouvez une faute de frappe, essayez de vous connecter avec l’adresse correcte
- Ouvrez vos dossiers **Spam, Promotions, Indésirables, Réseaux sociaux** et **Mises à jour** et vérifiez si votre e-mail de confirmation Miro s’y trouve
- Vérifiez si votre boîte de réception est pleine pour vous assurer que vous n’avez pas atteint la limite de mémoire de votre boîte de messagerie. S’il est plein, vous devrez peut-être supprimer certains e-mails pour en recevoir de nouveaux. Après la suppression des e-mails, cliquez sur **Send code again (Envoyer le code à nouveau)** pour recevoir un e-mail d’inscription
- Il se peut qu’un pare-feu empêche l’e-mail d’atteindre votre boîte de réception. Veuillez contacter l’*administrateur système* et lui demander d’ajouter nos domaines et sous-domaines à la liste d'autorisations : [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) et [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). [Voici un article](../../tools/troubleshooting/02-allowlist-miro-mailers.md) contenant plus d’informations sur les expéditeurs à autoriser
- Utilisateurs AOL/CompuServe : assurez-vous que vos Mail Controls (Contrôles d’E-Mail) sont configurés pour recevoir des e-mails depuis l’Internet. Si votre e-mail Internet est bloqué, veuillez changer vos Mail Controls en accédant à **Mail Controls** dans AOL ou CompuServe. Ensuite, retournez sur notre formulaire d’inscription pour renvoyer votre code de confirmation
- Le code devrait normalement arriver instantanément, mais en raison des particularités de votre système de messagerie, vous pourrez devoir attendre jusqu’à 24 heures
- Si aucune des solutions ne fonctionne, [signalez le problème au service d’assistance de Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
