---
title: Comment supprimer votre profil
article_id: 360017571354
translation_id: 360017571354
locale: fr
sidebar_position: 7
created_at: '2019-02-11T10:08:54Z'
updated_at: '2026-01-07T13:30:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
availability:
  notes: 'Créé par: propriétaire du profil'
---

La suppression de votre profil de Miro entraînera la suppression de vos informations dans notre système. Veuillez noter qu’un profilet une équipe sont deux choses différentes.

- Votre profil représente les données liées à votre inscription et à votre adresse e-mail.
- Une équipe est un espace que vous partagez avec d’autres membres de l’équipe et où les membres peuvent créer du contenu et stocker leurs tableaux.

Un même profil peut être associé à plusieurs équipes. Si vous souhaitez supprimer une équipe, découvrez comment procéder [ici](../../administration/team-management/06-delete-and-restore-teams.md).
:::warning
La suppression d’un profil **ne peut** pas être annulée.
:::

:::warning
Notez que la suppression du profil n’annule pas vos abonnements actifs. Pour arrêter les renouvellements, veuillez [annuler votre abonnement dans les paramètres](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md).
:::

### Comment supprimer votre profil

1. Rendez-vous sur vos [paramètres de profil](https://miro.com/app/settings/user-profile/).

2. Faites défiler la page jusqu’en bas et choisissez **Supprimer mon profil.**

![Supprimer le profil.png](../../../../../../docs/using-miro/managing-your-profile/images/21017429126546_Delete%20profile.png)
*Suppression de votre profil*

3. À ce stade, nous vous conseillons d’effectuer des [sauvegardes](../import-and-export/export/05-how-to-save-board-backup.md) ou d’[exporter](../import-and-export/export/03-how-to-export-your-board.md) vos tableaux avant de les supprimer.

![profil_suppression_modal.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017429125778_profile%20removal%20modal.jpg)*Message de confirmation de la suppression du profil*

4. Peu après, vous recevrez un e-mail contenant un lien de confirmation. Cliquez sur le lien pour terminer. Veuillez noter que votre profil Miro doit être actif dans le navigateur lorsque vous cliquez sur **Supprimer le profil** pour terminer la suppression du profil avec succès.

![Profil_suppression_email.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017416055186_Profile%20deletion%20email.jpg)
*E-mail de confirmation de la suppression du profil*

### Que se passe-t-il avec votre contenu après la suppression du profil ?

Dès que vous supprimez votre profil, vos tableaux sont supprimés.

Si vous êtes le seul admin de votre équipe, le contenu sera *entièrement* supprimé. Les droits d’admins seront accordés au membre invité en premier dans l’ordre chronologique.

S’il y a d’autres Admins dans l’équipe dont vous êtes membre, le contenu sera supprimé et réaffecté à l’un des Admins - cela signifie que l’admin pourra [restaurer vos tableaux dans les 90 jours](../managing-boards/08-how-to-restore-a-deleted-board.md) (les utilisateurs payants les trouveront dans la Corbeille, les utilisateurs gratuits pourront les restaurer via le lien du tableau).

### Foire aux questions

1. *Puis-je supprimer mon profil si je me connecte à Miro avec l’[authentification unique (SSO)](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)?*
   - Oui, vous le pouvez. Toutefois, si votre organisation utilise [SCIM](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md), votre profil sera immédiatement recréé tant que votre e-mail est fourni à Miro via SCIM.
2. *Comment puis-je modifier mon adresse e-mail liée au profil Miro ?*
   - Utilisez ce guide : [Comment changer votre e-mail](04-how-to-change-your-email.md).
3. *Je ne reçois pas l’e-mail contenant le lien de confirmation. Que faire ?*
   - Veuillez suivre les étapes suivantes :

- Ouvrez vosdossiers **Spam, Promotions,** **Junk, Réseaux sociaux** et **Notifications** et vérifiez si votre e-mail de confirmation Miro ne s’y trouve pas
- Vérifiez si votre boîte de réception est pleine pour vous assurer que vous n’avez pas atteint la limite de mémoire de votre boîte de réception d’e-mails. S’il est plein, il se peut que vous deviez supprimer certains e-mails existants pour en recevoir de nouveaux. Après avoir supprimé les e-mails, demandez à nouveau la suppression du profil.
- Il se peut qu’un pare-feu empêche l’e-mail d’atteindre votre boîte de réception. Veuillez contacter votre *administrateur système* et demandez-lui d’autoriser nos domaines et sous-domaines : [Miro.com](http://miro.com/)*, *.[Miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) et [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). [Voici un article](../tools/troubleshooting/02-allowlist-miro-mailers.md) avec plus d’informations sur les expéditeurs que vous devez autoriser.
- Si aucune de ces solutions n’est utile, [signalez le problème au service d’assistance Miro](../tools/troubleshooting/06-contacting-miro-support.md)
