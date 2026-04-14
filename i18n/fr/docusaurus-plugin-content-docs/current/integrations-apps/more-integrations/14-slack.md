---
title: Slack
article_id: 360017572494
translation_id: 360017572494
locale: fr
sidebar_position: 15
created_at: '2019-02-11T10:13:25Z'
updated_at: '2025-02-26T12:10:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
---

Recevez des notifications Slack pour les nouveaux commentaires et les nouvelles mentions sur vos tableaux ainsi que les autres modifications liées à votre profil, partagez facilement vos tableaux Miro depuis Slack et déployez automatiquement les liens des tableaux. Lisez cet article pour découvrir comment connecter votre Slack à Miro et accéder à toutes les fonctionnalités intéressantes.

:::note
En cliquant sur un lien vers un tableau Miro depuis un canal Slack, les utilisateurs de Slack peuvent recevoir une suggestion les invitant à s’inscrire facilement sur Miro.  La fonctionnalité est actuellement en version bêta et est gérée par Slack. Il n’est pas nécessaire que notre application soit installée dans l’espace de travail Slack.
Les administrateurs d’espace de travail ont la possibilité de désactiver complètement la fonctionnalité Se connecter avec Slack dans les paramètres de l’espace de travail Slack (App Management Settings (Paramètres de gestion des applications) > Sign in with Slack Settings (Se connecter avec les paramètres Slack)). /span> Les organisations Enterprise Grid ainsi que leurs espaces de travail sont exclues du lancement pendant la bêta.
:::

:::note
Pour obtenir de l’aide sur l’application Slack, envoyez un e-mail à [slack_integration_support@miro.com](mailto:slack_integration_support@miro.com) ou consultez l’article [Comment contacter le service d’assistance de Miro ?](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).
:::

## Activer l’application

L’intégration de l’application Slack est configurée par un utilisateur pour son propre profil. Pour activer l’intégration, ouvrez les [détails du profil](../../using-miro/managing-your-profile/01-profile-settings.md) de votre compte Miro.

getting_to_profile_settings.jpg
[Accès à la section Profile settings (Paramètres du profil) à partir du tableau de bord Miro](https://miro.com/app/dashboard/)

Allez sur l’onglet **Intégrations**, trouvez **Miro Feed (Slack App)** et cliquez sur Se connecter :

connect_Slack.jpg
Connexion à l’application Slack

Une autre option consiste à l’activer directement depuis l’[onglet Notifications](https://miro.com/app/account/profile/notifications/) :

connect_Slack_from_notifications.jpg
Activation de l’application Slack sur la page de notification

Cela vous redirigera vers la page d’autorisation dans Slack. Veuillez entrer vos identifiants et vous connecter à Slack.

authorize_Slack.jpg
Permettre à Miro d’accéder à l’espace de travail

## Configurer les notifications

Personnalisez le flux que vous recevez en choisissant les événements pour lesquels vous souhaitez recevoir des notifications.

Vous pouvez suivre les événements suivants :

- Les personnes que vous avez invitées s’inscrivent.
- Quelqu’un demande l’accès à une équipe ou à un tableau.
- Vous recevez une invitation à un projet.
- Un tableau a été partagé avec vous.
- Un nouveau commentaire a été publié sur votre tableau ou votre commentaire sur un tableau a reçu une réponse.
- Quelqu’un vous @mentionne dans un commentaire ou une réponse.

Ouvrez la [page Notifications](https://miro.com/app/account/profile/notifications/) et configurez vos préférences :

notification_settings.jpg
Paramètres des notifications

N’oubliez pas que dans certains cas, une notification ne vous sera envoyée *que si la personne à l’origine de cette notification* décide de l’envoyer.

## Réagir aux notifications dans Slack

Lorsque quelqu’un demande l’accès à votre tableau, vous pouvez le lui accorder dans Slack. Choisissez l’option et cliquez sur le bouton :

react_in_Slack.jpg
Accorder l’accès à un tableau dans le canal Slack

## Déployer des liens de tableau

La dernière version de l’application Slack de Miro déploie des liens vers les tableaux Miro en y ajoutant les noms, les descriptions et les vignettes des tableaux.

unfurl_a_board_link.jpg
*/span>Nom, description et vignette du tableau dans le canal Slack*

Réinstallez votre intégration Slack pour accéder à la fonctionnalité : sur Miro, rendez-vous sur **Paramètres du profil > **Intégrations****, puis cliquez sur **Se déconnecter** à coté de Miro Feed (Slack App).  Ensuite, cliquez sur Se connecter et Réautoriser.

:::note
Afin de réautoriser, vous devrez peut-être obtenir l’approbation de l’administrateur de l’espace de travail de Slack.
:::

Pour définir une vignette de tableau, accédez à votre tableau Miro et ouvrez la carte d’informations du tableau en cliquant sur le titre dans le coin supérieur gauche de votre tableau. Dans la fenêtre contextuelle, cliquez sur l’image dans le coin supérieur gauche, puis chargez une image à partir de votre appareil ou sélectionnez une section du tableau. La vignette apparaîtra alors dans Slack lorsque vous partagerez le lien du tableau.

change_board_thumbnail.gif
Définition de la vignette d’un tableau

## Partager un tableau à partir de Slack

Lorsque vous publiez un lien de tableau dans Slack, vous verrez une notification indiquant les utilisateurs qui n’ont pas accès au tableau. Vous pouvez facilement les inviter à consulter le tableau directement via Slack.  N’hésitez pas à [rendre le tableau public](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) pour que toute personne ayant le lien puisse le consulter/commenter.

share_from_Slack.jpg
/span>Partager d’un tableau Miro depuis Slack/em>

>  Si l’option n’est pas disponible pour vous, veuillez réinstaller l’application dans les paramètres ou demander à votre administrateur de mettre à jour le plug-in dans Slack Marketplace.

## Créer un tableau à partir de Slack

Vous pouvez utiliser le raccourci Miro pour créer un tableau à partir de Slack.  Recherchez dans Miro et choisissez **Créer un tableau**

Miro_shortcut.jpg
Créer un tableau à partir de Slack

Saisissez un titre pour le tableau, sélectionnez une équipe Miro et ajoutez un court message à envoyer avec le lien vers le tableau nouvellement créé dans Slack.

create_board_modal.jpg
/span>Définition des paramètres d’un nouveau tableau dans Slack

Une fois le tableau créé, le message sera envoyé au canal/à la conversation avec le lien du tableau.

new_board_message.jpg
Un message sera publié après la création d’un nouveau tableau à partir de Slack

Si certains membres du canal n’ont pas accès au tableau nouvellement créé, vous recevrez une suggestion vous invitant à [partager le tableau avec eux depuis Slack](#h_007785b5-df52-43e2-9eb0-ccb53b795955).

## Désactiver l’application

Pour désactiver l’intégration, rendez-vous sur **Profile settings > Integrations** (Paramètres du profil > Intégrations), puis cliquez sur **Log out** (Se déconnecter) :

Slack_log_out.jpg
Désactivation du flux Miro

Pour supprimer complètement l’application de Slack, ouvrez les paramètres du canal **Miro** dans Slack et cliquez sur **Configuration**.

Miro_Slack_configuration.jpg
Configuration de l’application Miro pour Slack

La page des paramètres de l’application Miro s’ouvrira. Faites défiler vers le bas, cherchez votre nom dans la liste des utilisateurs autorisés et cliquez sur **Revoke** (Révoquer).

revoke_access.jpg
Suppression de l’accès de Miro à Slack

Les admins de l’espace de travail verront également l’option permettant de supprimer l’application de *l’ensemble* de l’espace de travail.

remove_app.jpg
Suppression de l’application de Slack

## Foire aux questions et problèmes possibles

*1. Si un utilisateur ajoute Miro à Slack, Miro pourra-t-il lire ses canaux Slack ?*
- Non, Miro se contentera de view basic information about public channels in the workspace. Cela signifie que Miro pourra lire la liste des noms des canaux et ne pourra pas lire les messages des canaux.

2. *Je reçois le message "Something went wrong" lorsque j'essaie de connecter le flux Miro pour Slack.*
- Veuillez vérifier si votre navigateur autorise les fenêtres publicitaires intempestives provenant du domaine Miro.com. Il peut y avoir une page supplémentaire demandant des autorisations d’application./span>

3. 3. *Je ne reçois pas de notifications Miro-Slack et la réinstallation de l’application Miro dans Slack n’aide pas.*  Comment puis-je y remédier ?
- Veuillez essayer de reconnecter Miro et Slack du côté de Miro**(Paramètres du profil > [Intégrations](https://miro.com/app/account/profile/integrations/)**).
