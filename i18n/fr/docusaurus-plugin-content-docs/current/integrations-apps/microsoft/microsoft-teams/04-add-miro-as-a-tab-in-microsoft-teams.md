---
title: Ajouter Miro en tant qu'onglet dans Microsoft Teams
article_id: 4411292563602
translation_id: 4411292563602
locale: fr
sidebar_position: 4
created_at: '2021-12-01T04:50:21Z'
updated_at: '2025-11-25T16:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
availability:
  notes: 'Disponible pour: Free, Starter, Business, Education, Enterprise plans, et
    tous les plans Microsoft 365.'
---

Les utilisateurs peuvent ajouter des tableaux Miro aux réunions, canaux et événements de calendrier de Microsoft Teams pour collaborer de manière transparente et partager l'accès avec d'autres membres de l'équipe.
Dans cet article, vous apprendrez à utiliser Miro à l'intérieur :

- Microsoft Teams Meetings
- Événements du calendrier Microsoft Teams
- Chaînes et équipes Microsoft Teams

## Ajouter Miro dans les réunions Microsoft Teams

- Les utilisateurs qui rejoignent une réunion dans MS Teams via un mobile ou une tablette ne peuvent consulter qu’un tableau Miro joint et ne peuvent pas le modifier ou le commenter
- Tout utilisateur de Microsoft Teams ayant autorisé l'application Miro peut ajouter Miro à la réunion. Les utilisateurs de Teams qui ont un profil Miro peuvent partager un tableau à l’étape centrale
- ⚠️ Microsoft ne prend pas en charge l’utilisation des applications au sein d’une réunion Teams par des utilisateurs invités. Les utilisateurs doivent se connecter dans Teams afin de pouvoir utiliser les applications qui s’y trouvent (Miro compris).

1. Cliquez sur le menu déroulant **Plus d'actions.**
2. Sélectionnez **+Ajouter une application.**
3. Recherchez Miro et cliquez sur l’icône de Miro.
4. Ici, vous devrez vous inscrire à Miro ou vous connecter à votre profil Miro.
5. Sélectionnez le tableau que vous souhaitez partager ou choisissez de créer un nouveau tableau Miro vierge.
6. Définissez les autorisations pour le reste des participants à la réunion et donnez ou restreignez l'accès au tableau. Vous pouvez choisir parmi ces types de permission :

- **Tout le monde peut modifier** (aucune connexion à Miro n'est requise).
- **Tout le monde peut commenter** (pas de connexion requise, non pris en charge pour les tableaux situés dans une équipe Free).
- Anyone can view (Tout le monde peut voir) (pas de connexion requise)
- **Privé** (seules les personnes ayant déjà eu accès au tableau peuvent collaborer)

"**Tout le monde peut modifier, commenter ou afficher**" permet à toute personne de votre locataire Microsoft Teams d'accéder au tableau. Cela comprend :

- D’autres utilisateurs Miro qui ne font pas partie de votre organisation.
- Des utilisateurs qui ne possèdent pas de profil Miro.
- Des utilisateurs au sein de votre organisation qui ne sont pas connectés à leur compte Miro.

:::note
Les paramètres de partage définis pour un tableau dans Miro peuvent également définir l'accès au tableau dans Microsoft Teams. Si le tableau est partagé publiquement dans Miro, il sera disponible pour tout le monde dans Microsoft Teams, même si vous avez épinglé le tableau comme étant [privé](../../../using-miro/sharing-boards/15-make-a-miro-board-private.md). Toutefois, si votre tableau est privé du côté Miro et que vous l'avez épinglé avec la mention Tout le monde peut voir/commenter/modifier, l'accès au tableau du côté Miro ne sera pas affecté. [En savoir plus](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).
:::

:::note
Pour les utilisateurs de comptes Enterprise, vos paramètres d’accès correspondront aux contrôles d’accès à l’échelle de l’organisation. Le partage de liens publics pour les liens doit être activé par les admin d'**entreprise** dans **Paramètres de l'entreprise** > **Sécurité.** Pour en savoir plus, consultez la section [Gestion de la politique de partage de l'Enterprise pour les intégrations](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

Si vous devez modifier les droits d’accès d’un tableau intégré, supprimez l’onglet et ajoutez-le à nouveau avec un niveau d’accès différent.

Vous pouvez désormais accéder au tableau Miro à tout moment pendant la réunion dans l'onglet spécifique. Si vous créez plusieurs tableaux, il y aura un seul onglet pour chaque tableau.

Si vous cliquez sur Miro, l’onglet de Miro apparaîtra à droite du tableau que vous avez joint à cette réunion.

Vous pouvez sélectionner le bouton Share-to-Stage (Partager sur la scène) afin d’envoyer le tableau à toutes les personnes participantes et ainsi collaborer ensemble en simultané. Vous pouvez cesser le partage du tableau à tout moment en cliquant sur le bouton Stop presenting (Arrêter de présenter) situé en haut.

## Épingler des tableaux aux événements du calendrier Microsoft Teams

:::note
Le calendrier Outlook n'est pas encore pris en charge.
:::

- ⚠️ Les événements du calendrier de Teams doivent être enregistrés et doivent au moins compter une personne participante pour qu’un tableau Miro puisse être joint à la réunion.
- ⚠️ [Il n’existe pas de moyen de supprimer un tableau Miro d’une invitation à une réunion dans Teams (voir](https://support.microsoft.com/en-gb/office/remove-a-tab-in-microsoft-teams-c18c875c-0738-40ec-a228-61d7eb27f745#:~:text=In%20one%2Don%2Done%20and,the%20tab%20and%20select%20Remove.) l’article de référence de Microsoft). Les utilisateurs doivent supprimer l’invitation et en créer une nouvelle sans un tableau.

1. Premièrement, planifiez une nouvelle réunion dans le calendrier de Microsoft Teams.  Assurez-vous de nommer la réunion et d’y inviter des personnes.
2. Cliquez sur **Envoyer** pour partager l'invitation.
3. **Une fois la réunion enregistrée, cliquez à nouveau sur la réunion et cliquez sur** Edit (Modifier) pour pouvoir y joindre un tableau Miro.
4. Vous pourrez épingler Miro en tant qu'onglet en utilisant le signe plus en haut de l'écran**(+).**
5. Sur l'écran suivant, vous serez prompt à ajouter l'application Miro. Recherchez Miro dans la barre de recherche ou sélectionnez Miro si vous le voyez déjà.
6. Sélectionnez **Ajouter** pour ajouter Miro.
7. Il vous sera demandé de vous connecter à votre profil Miro dans Teams.
8. Une fois votre profil Miro connecté, vous devrez sélectionner le tableau que vous souhaitez ajouter à la réunion. Vous pouvez rechercher et sélectionner un tableau existant ou créer un tableau vierge.
9. Dans cette section, vous pouvez également définir les autorisations dont bénéficieront les autres personnes participant à la réunion et leur donner accès ou restreindre leur accès au tableau. Puis s**choisissez Save pour pouvoir joindre le tableau Miro sélectionné à la réunion Teams. Vous pouvez choisir parmi ces types de permission :**

- **Anyone can edit (Tout le monde peut modifier)** (pas de connexion requise)
- **Anyone can comment (Tout le monde peut commenter)** (pas de connexion requise)
- **Anyone can view (Tout le monde peut consulter)** (pas de connexion requise)
- **Private (Privé)**

## Épinglez des tableaux dans les canaux et les chats de Microsoft Teams.

> **Rôle requis :** [Les propriétaires](../../../using-miro/sharing-boards/01-board-access-rights.md) et [éditeurs de tableaux](../../../using-miro/sharing-boards/01-board-access-rights.md) qui sont membres de l'équipe où se trouve le tableau.

Vous pouvez épingler des tableaux aux chaînes Microsoft Teams en créant un nouvel onglet.

1. Cliquez sur l’icône plus.
2. Un sélecteur s'ouvre avec différentes applications.
3. Trouvez Miro dans la liste des applications et sélectionnez-la.
4. Si vous n’êtes pas autorisé dans Miro dans le même navigateur ou dans l’application de bureau, vous devrez vous connecter. Cliquez sur **Get Started** (Démarrer) et connectez-vous ou [inscrivez-vous sur Miro](../../../getting-started/start-here/02-how-to-register-with-miro.md) (article disponible uniquement en anglais).
5. Une fois votre autorisation reçue, vous verrez un sélecteur avec des tableaux Miro : le sélecteur vous montrera les tableaux Miro auxquels vous avez accès. Veuillez noter que vous pouvez recevoir votre autorisation dans Miro et dans Microsoft Teams sous différents e-mails.
6. Sélectionnez un tableau que vous souhaitez ajouter à votre canal Microsoft Teams. Si vous choisissez un tableau pour lequel vous n’avez pas le niveau d’accès requis, vous verrez un message d’avertissement.
7. Définissez les autorisations pour le reste des participants à la réunion et donnez ou restreignez l'accès au tableau. Vous pouvez choisir parmi ces types de permission :

   - **Anyone can edit (Tout le monde peut modifier)** (pas de connexion requise)
   - **Anyone can comment** (Tout le monde peut commenter) (pas de connexion requise)
   - **Anyone can view** (Tout le monde peut voir) (pas de connexion requise)
   - **Private (Privé)**
   > ✏️ Les utilisateurs de Microsoft Teams qui utilisent Miro sur l’application mobile Microsoft Teams peuvent consulter et commenter des tableaux en fonction des autorisations définies. Pour modifier des tableaux, nous vous conseillons vivement d’installer notre [application mobile](../../../getting-started/apps-for-devices/08-mobile-app.md) native pour laquelle nous avons optimisé l’interface utilisateur.

   ## Foire aux questions

Chaque membre de l’équipe doit-il disposer d’un profil Miro pour afficher les tableaux intégrés dans Microsoft Teams ?

- Si vous choisissez **Tout le monde peut voir/commenter/modifier** lors de l’intégration du tableau, même les utilisateurs non inscrits pourront voir/commenter le tableau. Aussi, si le tableau est partagé publiquement sur Miro, il sera disponible pour tous dans Microsoft Teams.

Une fois qu’un tableau est intégré, qui a la possibilité de modifier l’accès au tableau dans MS Teams (par exemple, de "Tout le monde peut voir" à "Privé") ?

- Personne ne peut modifier l’accès au tableau joint, pas même celui qui l’a joint. Cependant, tout le monde peut cliquer sur **Paramètres** sur l’onglet, puis choisir un autre tableau (ou le même) pour le même onglet et sélectionner un autre niveau d’accès pour le tableau choisi.

Je possède deux profils Miro, chacun avec un e-mail différent, et je souhaiterais intégrer un tableau Miro à partir de mon deuxième profil Miro. Comment puis-je changer de profil Miro ?

- Le sélecteur affiche les tableaux de l’utilisateur avec lequel vous êtes autorisé dans Miro dans le même navigateur. Ouvrez Miro dans un autre onglet du navigateur, déconnectez-vous et connectez-vous à votre deuxième profil Miro.

Si vous utilisez l’application de bureau Microsoft Teams, déconnectez-vous de l’application - cela vous déconnectera également de Miro dans l’application. Ensuite, connectez-vous à l’appli et essayez d’[intégrer un tableau](05-embed-miro-boards-in-microsoft-teams.md). Vous recevrez une invitation à vous connecter à Miro et vous pourrez vous connecter à un autre profil Miro.
