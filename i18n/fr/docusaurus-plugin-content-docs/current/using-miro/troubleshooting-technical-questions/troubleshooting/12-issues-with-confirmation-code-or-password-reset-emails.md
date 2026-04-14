---
title: "Probl\xE8mes avec les e-mails de code de confirmation ou de r\xE9initialisation\
  \ de mot de passe"
article_id: 360017731373
translation_id: 360017731373
locale: fr
sidebar_position: 12
created_at: '2019-02-11T10:14:22Z'
updated_at: '2024-10-25T14:25:54Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Si vous n’avez pas reçu de code de confirmation ou d’e-mail de réinitialisation du mot de passe, cela peut être dû à plusieurs raisons. Les informations ci-dessous peuvent vous aider à résoudre la situation en vous proposant des options à essayer.

## Raisons courantes pour lesquelles les codes ou les e-mails ne parviennent pas au destinataire

Les deux raisons les plus communes pour lesquelles vous ne recevez pas d’e-mail de réinitialisation de mot de passe ou ne pouvez pas demander un nouveau code de confirmation sont les suivantes :

1. Votre entreprise utilise un pare-feu qui bloque les e-mails provenant des domaines miro.com. Demandez à votre administrateur informatique d’autoriser les e-mails provenant des [domaines](http://miro.com/)miro.com.  Si vous êtes l’administrateur, consultez la section ci-dessous pour obtenir des instructions sur la façon d’autoriser les domaines Miro.
2. Votre entreprise utilise l’authentification unique (SSO). Voir la section ci-dessous pour des instructions sur comment résoudre ce problème.

## Comment résoudre les problèmes liés aux e-mails et aux codes de confirmation perdus

1. Si votre entreprise utilise l’authentification unique (SSO), vous devez vous connecter avec les identifiants SSO de votre entreprise. Si vous essayez de réinitialiser votre mot de passe avec Miro, vous serez simplement redirigé vers la page de connexion SSO. Si cela se produit, essayez d’utiliser les identifiants SSO de votre entreprise. Si cela ne fonctionne pas, poursuivez le diagnostic de pannes ci-dessous.
2. Il se peut qu’un pare-feu empêche l’e-mail d’atteindre votre boite de réception. Veuillez contacter votre administrateur système et demandez-lui d’autoriser nos domaines et sous-domaines : Miro.com*, *.Miro.com, mirostatic.com*, *.mirostatic.com et realtimeboard.com*, *.realtimeboard.com.

   Voici la liste des IP dédiées : 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. En savoir plus sur [la liste des adresses e-mail Miro à autoriser](../../tools/troubleshooting/02-allowlist-miro-mailers.md).
3. Assurez-vous que l’adresse e-mail que vous avez fournie ne contient pas de faute de frappe. [Si vous trouvez une faute de frappe,](../../../getting-started/start-here/02-how-to-register-with-miro.md) enregistrez à nouveau votre profil / réinitialisez votre mot de passe en vous servant d’une adresse e-mail valide.
4. Vérifiez les dossiers **Spam, Promotions,** **Courrier indésirable, Social** et **Mises à jour** de votre fournisseur de messagerie.
5. Vous pouvez également vous inscrire ou vous connecter en utilisant d’autres options d’inscription ou de connexion : connectez-vous/inscrivez-vous avec Google, Slack, Office 365, Apple ou Facebook.
   > ⚠️ Notez que les identifiants alternatifs ne sont **pas** connectés aux logins SSO de l’entreprise. Si vous utilisez Miro en entreprise, veuillez utiliser les informations d’identification que votre administrateur Miro a configurées pour vous.

   ![nouveau-chant-en-troisième-partie.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)
   Méthodes d’authentification disponibles

Si vous ne parvenez pas à vous inscrire ou à vous connecter à l’aide d’autres méthodes d’authentification :

- Vérifiez que votre boîte de réception ne soit pas pleine et que vous n’avez pas atteint la limite de stockage d’e-mails. Si elle est pleine, vous pouvez supprimer des e-mails pour pouvoir en recevoir à nouveau. Après avoir supprimé les e-mails, retournez sur notre page d’inscription et cliquez sur **Send code again (Envoyer le code à nouveau).**
- Vous devriez recevoir l’e-mail immédiatement. Si ce n’est pas le cas, vous devrez patienter jusqu’à 24 heures.
- Si vous utilisez vos identifiants d’authentification unique d’entreprise et que vous ne pouvez pas vous connecter, vous pouvez en apprendre plus sur les [erreurs courantes d’authentification unique et comment les résoudre](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

### Autres problèmes de confirmation

Mon code n’est pas valide

Si le code saisi n’est **pas valide :**

1. Vérifiez votre boîte de réception et assurez-vous que vous saisissez le code que vous avez reçu en dernier. **Si le code n’est toujours pas valide, cliquez sur** Send code again (Envoyer le code à nouveau) et saisissez le code reçu dans le nouvel e-mail.
2. Une autre façon de finaliser l’inscription est de cliquer sur **Confirm your email (Confirmer votre e-mail)** dans l’e-mail contenant le code de confirmation. Dans ce cas, vous n’aurez pas besoin du code de confirmation.
   ![bouton de confirmation de l'e-mail.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725339026_confirm%20email%20button.png)
   *L’option permettant de confirmer votre e-mail*

J’ai dépassé le nombre de tentatives de confirmation d’e-mail

Si vous ne parvenez pas à confirmer votre e-mail après 4 tentatives, vous verrez le message  **Email confirmation attempts exceeded (Nombre de tentatives de confirmation d’e-mail dépassé)** sur la page d’inscription.

Attendez 60 secondes et cliquez sur **Send code again (Envoyer le code à nouveau)** - cela vous générera un nouveau code. Saisissez le code et finalisez l’inscription.

J’ai accidentellement fermé l’onglet où j’ai saisi le code de confirmation

[Connectez-vous](https://miro.com/login/) à l’aide de l’adresse e-mail et du mot de passe que vous avez saisis lors de l’inscription et la [page de confirmation](https://miro.com/email-confirm/) s’ouvrira à nouveau.

>  ️ ✏️ Si vous ne confirmez pas votre adresse e-mail, vous recevrez des rappels au bout de 12 et 24 heures. Si votre adresse e-mail n’est pas confirmée dans les 7 jours, votre **profil sera supprimé**. Vous pourrez enregistrer un nouveau profil en vous servant de la même adresse e-mail.

:::note
Les codes de confirmation peuvent uniquement être envoyés par e-mail.
:::

:::note
Si vous rencontrez toujours des problèmes, [contactez le service d’assistance de Miro](https://miro.com/contact/recover/).
:::
