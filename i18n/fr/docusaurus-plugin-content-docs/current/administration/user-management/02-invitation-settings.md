---
title: Paramètres d’invitation
article_id: 360022258119
translation_id: 360022258119
locale: fr
sidebar_position: 3
created_at: '2021-06-03T10:01:33Z'
updated_at: '2025-06-02T11:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
availability:
  notes: 'Qui peut le faire: Les admins d''équipe (Free, Starter, Education), les
    admins d''entreprise (Business, Enterprise), les admins d''équipe'
---

Les admins peuvent configurer les autorisations relatives aux invitations au sein d'une équipe et restreindre la capacité des utilisateurs non-admins à [inviter de nouveaux membres](01-invite-users.md) et à modifier la taille de l'abonnement.

Accédez à la console d'administration en cliquant sur votre avatar de profil dans le coin supérieur droit, puis sur **Console d'administration**.

Dans l’onglet **Sécurité** > **Autorisations**, défiler vers le bas jusqu’aux **Paramètres d’invitation**. La présentation des paramètres diffère selon les différents plans Miro.

Sur les plans Free, Starter et Education, vous pouvez également activer ou désactiver le lien d'invitation d'équipe qui permet aux utilisateurs de rejoindre votre équipe en suivant un lien spécial qui peut être copié dans les modaux de partage et d'invitation des tableaux. [En savoir plus](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

![invitation-settings.png](../../../../../../docs/administration/user-management/images/25007070132626_invitation-settings.png)
*Paramètres d’invitation sur le plan Starter*

Sur les plans Starter et Education, seuls les membres peuvent modifier les tableaux. Ainsi, si un utilisateur qui n’est pas autorisé à inviter des membres tente de partager un tableau avec un éditeur qui n’est pas membre de l’équipe, la fenêtre contextuelle s’affichera.

## Paramètres d’invitation pour Business et Enterprise

Sur les forfaits Business et Enterprise, les admins d'entreprise peuvent en plus autoriser ou interdire les [invités](../../using-miro/sharing-boards/07-collaboration-with-guests.md).

![inv-settings-invitation.png](../../../../../../docs/administration/user-management/images/21855329470994_inv-settings-invitation.png)
*Paramètres d’invitation du forfait Enterprise*

Les admins d'entreprise des plans Business et Enterprise [Company Admins](../get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md) peuvent configurer les paramètres d'invitation pour chaque équipe au sein de l'abonnement.

Suivez les étapes suivantes :

1. Accédez à la **console d'administration**.
   Depuis votre tableau de bord Miro, cliquez sur votre avatar dans le coin supérieur droit et sélectionnez **Console d'administration**.
2. Cliquez sur **Teams**.
3. Sous **Nom de l'équipe**, sélectionnez une équipe.
   Le panneau des paramètres de l'équipe s'ouvre.
4. Cliquez sur **Paramètres**.
5. Sous **Invitation**, sélectionnez qui peut inviter des utilisateurs à rejoindre cette équipe.
   > ⚠️ (Business) Vos licences augmentent automatiquement lorsqu’un nouvel utilisateur est ajouté. Si vous autorisez quelqu'un à inviter de nouveaux utilisateurs, alors n'importe qui peut entraîner l'ajout de nouvelles licences à votre abonnement.
6. Sélectionnez **Autoriser** ou **Ne pas autoriser** pour les invités.
7. Dans le coin supérieur droit, cliquez sur le **X** pour fermer le panneau des paramètres de l'équipe.
   Vos paramètres sont enregistrés.

Si les utilisateurs ne sont pas autorisés à inviter de nouveaux membres, ils ne verront pas l'option sur leurs tableaux de bord. Une fenêtre contextuelle est affichée pour les utilisateurs des plans Business si les invités ne sont pas autorisés.

Pour en savoir plus sur les paramètres d'invitation du forfait Enterprise, consultez [cet article](../../enterprise-administration/user-management/03-invitation-settings-on-enterprise-plan.md).
