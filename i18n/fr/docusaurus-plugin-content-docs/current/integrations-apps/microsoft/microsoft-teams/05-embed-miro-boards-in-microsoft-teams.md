---
title: "Int\xE9grer les tableaux Miro dans Microsoft Teams"
article_id: 360017572514
translation_id: 360017572514
locale: fr
sidebar_position: 5
created_at: '2019-02-11T10:13:30Z'
updated_at: '2025-04-24T13:52:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ms-teams
---

Intégrez des tableaux Miro dans des canaux Microsoft Teams et partagez-les de manière fluide avec les membres de l’équipe. Gardez vos tableaux Miro à portée de main et assurez-vous que toute votre équipe est sur la même longueur d’onde.

:::note
Découvrez comment intégrer les tableaux Miro dans Microsoft Teams Meetings : [Miro pour Microsoft Teams Meetings (guide admin)](01-miro-for-microsoft-teams-admin-guide.md), [Miro pour Microsoft Teams Meetings (guide de l’utilisateur)](02-miro-for-microsoft-teams-user-guide.md).
:::

> **Disponible pour :** tous les plans Miro

### Installer le plugin

Vous devez tout d’abord trouver **Miro** dans **Microsoft Teams Store** ou suivez simplement le [lien direct](https://teams.microsoft.com/l/app/8216e453-3db5-48ee-a3d6-5122f505c8a3).

:::warning
Veuillez noter que votre admin client sur Microsoft Teams doit activer l’application Miro dans votre catalogue d’applications tierces pour Teams. Si Miro n’est pas approuvé, il ne sera pas répertorié parmi les applications du Microsoft Teams Store.
:::

Cliquez sur **Add** (Ajouter) pour installer le plugin.

![Miro_plugin_installation.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790725266_Miro%20plugin%20installation.jpg)
*Installation du plugin Miro*

Une fois le plugin Miro installé, le chat apparaîtra et vous pourrez y configurer les notifications Miro. Pour en savoir plus, consultez [ce guide sur les notifications Microsoft Teams](10-miro-notifications-in-microsoft-teams.md).

Toutefois, vous pouvez déjà commencer à intégrer des tableaux Miro dans un canal Microsoft Teams sans configuration supplémentaire.

### Intégrer des tableaux dans les canaux Microsoft Teams

> **Configuré par :** [les propriétaires de tableaux](../../../using-miro/sharing-boards/01-board-access-rights.md) et [les éditeurs de tableaux](../../../using-miro/sharing-boards/01-board-access-rights.md) qui sont membres de l’équipe où se trouve le tableau

Vous pouvez intégrer vos tableaux dans les canaux Microsoft Teams en créant un nouvel onglet. Cliquez sur l’icône plus. Vous verrez alors un sélecteur contenant diverses applications. Trouvez Miro dans la liste des applications et sélectionnez-la. Si vous n’êtes pas autorisé dans Miro dans le même navigateur ou dans l’application de bureau, vous devrez vous connecter. Cliquez sur **Get Started** (Démarrer) et connectez-vous ou [inscrivez-vous sur Miro](../../../getting-started/start-here/02-how-to-register-with-miro.md) (article disponible uniquement en anglais).

![embed_in_MS_teams.gif](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734975122_embed%20in%20MS%20teams.gif)
*Le module qui vous permet d’autoriser votre profil Miro*

Une fois votre autorisation reçue, vous verrez un sélecteur avec des tableaux Miro : le sélecteur vous montrera les tableaux Miro auxquels vous avez accès. Veuillez noter que vous pouvez recevoir votre autorisation dans Miro et dans Microsoft Teams sous différents e-mails.

Sélectionnez un tableau que vous souhaitez ajouter à votre canal Microsoft Teams.

![MS_teams_embed_picker.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734978322_MS%20teams%20embed%20picker.jpg)
*Le sélecteur avec des tableaux Miro*

Notez que seuls les propriétaires et les éditeurs des tableaux qui sont membres de l’équipe peuvent intégrer des tableaux Miro. Si vous choisissez un tableau pour lequel vous n’avez pas le niveau d’accès requis, vous verrez un message d’avertissement.

![unable_to_embed_boards.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790732690_unable%20to%20embed%20boards.jpg)
*Le message d’avertissement indiquant que votre niveau d’accès ne vous permet pas d’intégrer un tableau*

Vous pouvez ensuite définir les autorisations pour le reste des personnes participant à la réunion et donner ou restreindre l’accès au tableau. Vous pouvez choisir parmi ces types de permission :

- **Anyone can edit (Tout le monde peut modifier)** (pas de connexion requise)
- **Anyone can comment** (Tout le monde peut commenter) (pas de connexion requise)
- **Anyone can view** (Tout le monde peut voir) (pas de connexion requise)
- **Private (Privé)**

![sharing_level.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790733586_sharing%20level.jpg)
*Paramètres d’accès pour un tableau intégré*

:::note
✏️ Notez que les paramètres de partage définis pour un tableau dans Miro  peuvent également définir l’accès au tableau dans Microsoft Teams. Si le tableau est partagé publiquement dans Miro, il sera disponible pour tous dans Microsoft Teams, même si vous l’avez intégré en tant que tableau **privé**. Toutefois, si votre tableau est privé sur Miro et que vous l’avez intégré avec des droits Anyone can view/comment/edit (Tout le monde peut voir/commenter/modifier), l’accès au tableau dans Miro ne sera pas affecté. En savoir plus.
:::

:::note
Pour les  utilisateurs du[forfait Enterprise](../../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md) Miro, vos paramètres d’accès suivront les contrôles d’accès à l’échelle de l’organisation, ce qui peut impliquer que certaines options de partage peuvent être restreintes. En savoir plus : [Gérer la politique de partage pour les intégrations embarquées sur un compte Enterprise](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

> **⚠️ L’option [Anyone can comment](../../../plans-billing/miro-plans/09-free-plan.md) (Tout le monde peut commenter) n’est pas prise en charge si vous intégrez un tableau qui se trouve dans une équipe gratuite.**

Une fois le tableau intégré, vous pouvez commencer immédiatement à interagir.

![Miro_embed_in_MS_teams.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734972562_Miro%20embed%20in%20MS%20teams.jpg)
*Tableau intégré dans un canal Microsoft Teams*

> *✏️* Les utilisateurs de Microsoft Teams qui utilisent Miro sur l’application mobile Microsoft Teams peuvent consulter et commenter des tableaux en fonction des autorisations définies. Pour modifier des tableaux, nous vous conseillons vivement d’installer notre [application mobile](../../../getting-started/apps-for-devices/08-mobile-app.md) native pour laquelle nous avons optimisé l’interface utilisateur.

![Miro_in_MS_Team_on_mobile.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734976146_Miro%20in%20MS%20Team%20on%20mobile.jpg)
*Tableau Miro dans Microsoft Teams sur mobile - appuyez sur **Open in the app (Ouvrir dans l’application)** pour installer l’application mobile native Miro*

### Foire aux questions

1. *Chaque membre de l’équipe doit-il disposer d’un profil Miro pour afficher les tableaux intégrés dans Microsoft Teams ?
   - Si vous choisissez **Tout le monde peut voir/commenter/modifier** lors de l’intégration du tableau, même les utilisateurs non inscrits pourront voir/commenter le tableau. Aussi, si le tableau est [partagé publiquement](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#partage-de-tableaux-via-un-lien-public) sur Miro, il sera disponible pour tous dans Microsoft Teams.*
2. *Une fois qu’un tableau est intégré, qui a la possibilité de modifier l’accès au tableau dans MS Teams (par exemple, de "Tout le monde peut voir" à "Privé") ?
   - Personne ne peut modifier l’accès au tableau joint, pas même celui qui l’a joint. Cependant, tout le monde peut cliquer sur **Paramètres** sur l’onglet, puis choisir un autre tableau (ou le même) pour le même onglet et sélectionner un autre niveau d’accès pour le tableau choisi.*
3. *Je possède deux profils Miro, chacun avec un e-mail différent, et je souhaiterais intégrer un tableau Miro à partir de mon deuxième profil Miro. Comment puis-je changer de profil Miro ?
   - Le sélecteur affiche les tableaux de l’utilisateur avec lequel vous êtes autorisé dans Miro dans le même navigateur. Ouvrez Miro dans un autre onglet du navigateur, déconnectez-vous et connectez-vous à votre deuxième profil Miro.
   Si vous utilisez l’application de bureau Microsoft Teams, déconnectez-vous de l’application - cela vous déconnectera également de Miro dans l’application. Ensuite, connectez-vous à l’appli et essayez d’[intégrer un tableau](#h_5af20ae6-78c0-4e6c-ab20-e4968c89c97f). Vous recevrez une invitation à vous connecter à Miro et vous pourrez vous connecter à un autre profil Miro.*
