---
title: Miro pour Google Meet
article_id: 6251039904530
translation_id: 6251039904530
locale: fr
sidebar_position: 10
created_at: '2022-06-24T07:22:19Z'
updated_at: '2025-11-25T16:08:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-meet
---

Rendez vos réunions encore plus attrayantes et interactives avec Miro dans Google Meet.  COnsultez et ouvrez n’importe lequel de vos tableaux Miro, voire créez-en un nouveau, et collaborez avec n’importe qui, même sans profil Miro. Enregistrez votre travail pour y revenir plus tard et accédez-y à tout moment.

Les intégrations Google Meet font maintenant partie du module complémentaire Google Workspace, ce qui signifie que les utilisateurs qui ont déjà le module complémentaire Miro auront toujours accès à Google Meet.  Les utilisateurs qui n’ont pas installé le module complémentaire Miro en auront besoin pour accéder au module complémentaire Google Meet.

En savoir plus sur [comment installer le module complémentaire Miro pour Google Workspace](07-miro-for-google-workspace.md).

## Points importants à noter

- Il n’est pas nécessaire d’être l’organisateur ou l’organisatrice de la réunion pour ouvrir un tableau Miro dans Google Meet : toute personne participant à la réunion peut ouvrir des tableaux Miro.
- Les utilisateurs sans profil Miro ou ceux qui ne se sont pas encore connectés pourront toujours voir et participer sur le tableau Miro en tant qu’[invités](../../using-miro/sharing-boards/07-collaboration-with-guests.md) sans créer de profil, tant que les autorisations appropriées ont été définies sur le tableau.
- Si vous créez un tableau Miro sans profil, il vous sera d’abord demandé de fournir votre adresse e-mail à Miro. Vous recevrez ensuite sous 24 heures et par e-mail des informations pour enregistrer votre travail et créer un profil Miro.
- Les admins ont la possibilité d’empêcher certaines équipes ou certains utilisateurs individuels de l’entreprise d’utiliser Miro avec Meet. [En savoir plus](https://support.google.com/a/answer/6089179?hl=en).

:::warning
Miro dans Google Meet n’est pas pris en charge en mode Incognito ou Compagnon dans Chrome et n’est pris en charge que sur les navigateurs Chrome et Edge.
:::

## Comment configurer Miro pour Google Meet

1. Commencez une réunion Google Meet.
2. Pour ouvrir Miro, cliquez sur l'onglet **Activités.**

   activities.jpg
   *Activités dans Google Meet*
3. Sélectionnez Miro dans la liste des applications.

   ![Miro_platform_in_Google_Meet.jpg](../../../../../../docs/integrations-apps/google/images/21016033814290_Miro%20platform%20in%20Google%20Meet.jpg)*Complément Miro dans Google Meet*
4. Ici, vous aurez la possibilité de vous connecter à votre profil Miro ou de commencer un tableau sans profil.
   Si vous créez un tableau Miro sans profil, vous recevrez par e-mail les informations nécessaires pour sauvegarder votre travail et créer un profil Miro dans les 24 heures.

   Pour enregistrer un nouveau profil Miro, choisissez de vous connecter, puis cliquez sur **S'inscrire dans** le coin supérieur droit de la fenêtre de connexion.

   sign_in_or_create_a_board.jpg
   *Option de connexion pour les nouveaux utilisateurs de Miro*
5. Une fois que vous avez ouvert une session, vous verrez tous vos tableaux.  Sélectionnez le tableau que vous souhaitez utiliser pendant la réunion. Vous ne pouvez sélectionner que les tableaux que vous êtes autorisé à modifier. ![google_meet_board_picker.png](../../../../../../docs/integrations-apps/google/images/21016020380562_google_meet_board_picker.png)
   L’outil de sélection de tableaux dans Miro pour Google Meet/span>
6. Sélectionnez le niveau d’accès au tableau approprié pour toutes les personnes présentes à la réunion et cliquez sur **Intégrer le tableau**.  Vous pouvez choisir entre quatre options : autoriser l’accès avec droit de consulter/commenter/modifier ou laisser le tableau privé et disponible pour les utilisateurs Miro connectés qui y ont accès du côté de Miro.
   > ⚠️ L’option **Tout le monde peut commenter** n’est pas prise en charge si vous intégrez un tableau se trouvant dans une [équipe gratuite](../../plans-billing/miro-plans/09-free-plan.md).

   > ✏️ Si vous sélectionnez Privé dans ce flux alors que le tableau est [public sur Miro](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#partage-de-tableaux-via-un-lien-public), il sera également public par défaut dans Google Meet.  Toutefois, le niveau d’accès que vous avez défini dans Google Meet pour le tableau intégré n’affecte pas les paramètres de partage du tableau dans Miro.  [En savoir plus](../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

   > ✏️ Pour les  utilisateurs du[forfait Enterprise](../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md) Miro, vos paramètres d’accès suivront les contrôles d’accès à l’échelle de l’organisation, ce qui peut impliquer que certaines options de partage peuvent être restreintes. En savoir plus : Gestion de la politique de partage de l’entreprise pour les intégrations embarquées[.](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)

   ![google_meet_board_access_settings.png](../../../../../../docs/integrations-apps/google/images/21016020382098_google_meet_board_access_settings.png)*Paramètres d'accès au tableau dans Google Meet*
7. Cliquez sur **Démarrer une activité** pour partager le tableau Miro avec toutes les personnes participant à la réunion.  La réunion s’ouvrira au centre. Un message de confirmation s'affiche avec tous les utilisateurs que vous avez invités à travailler sur le tableau.

   ![google_meet_starting_collaboration.png](../../../../../../docs/integrations-apps/google/images/21016020384018_google_meet_starting_collaboration.png)*Démarrer une activité sur un tableau Miro dans Google Meet.*Les participants à la réunion recevront une notification contextuelle leur demandant de rejoindre le tableau pour collaborer.

   Google_Meet_Miro_collaboration.jpg

Voici comment Miro pour Google Meet recherche les présentateurs et les participants :

![google_meet_presenter_view.png](../../../../../../docs/integrations-apps/google/images/21016033821458_google_meet_presenter_view.png)*Vue du présentateur dans Miro pour Google Meet*

![google_meet_attendee_view.png](../../../../../../docs/integrations-apps/google/images/21016033817746_google_meet_attendee_view.png)*Vue des participants dans Miro pour Google Meet*

## Mettre fin à l’activité dans Google Meet

Si vous avez terminé de travailler dans le tableau Miro, vous pouvez mettre fin à l’activité et rester sur l’appel Google Meet.

1. Cliquez sur **Mettre fin à l’activité**.
2. Une nouvelle fenêtre contextuelle s’ouvrira vous demandant de confirmer. Cliquez sur **Continuer** pour mettre fin à l’activité et revenir à votre appel.  Cela mettra fin à la collaboration Miro, mais vous pouvez toujours commencer une nouvelle collaboration ou sélectionner un autre tableau en cliquant sur l’icône Activités dans le coin inférieur droit de Meet.

   ![google_meet_end_activity.gif](../../../../../../docs/integrations-apps/google/images/21016033824146_google_meet_end_activity.gif)*Fin de la collaboration sur un tableau Miro dans Google Meet*

En savoir plus sur [Miro pour Google Meet](https://support.google.com/meet/answer/12312774).
