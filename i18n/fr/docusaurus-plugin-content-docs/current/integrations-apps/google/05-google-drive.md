---
title: Google Drive
article_id: 360017731253
translation_id: 360017731253
locale: fr
sidebar_position: 6
created_at: '2019-02-11T10:14:01Z'
updated_at: '2025-01-13T14:51:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-drive-onedrive
---

**Google Drive** vous permet de stocker des fichiers en ligne en toute sécurité, d’y accéder de n’importe où et de collaborer avec d’autres personnes. Avec l’intégration de Google Drive, nous vous permettons de vous concentrer plus facilement sur vos tâches et de suivre vos documents directement sur le tableau.

![Google_Drive_sur_le_menu_de_chargement.jpg](../../../../../../docs/integrations-apps/google/images/21016121222546_Google%20Drive%20on%20the%20Upload%20menu.jpg)

> **Configuration par :** chaque utilisateur séparément (les admins peuvent restreindre l’installation de l’application par des utilisateurs non admins)
> **Disponible sur :** version navigateur, [application de bureau](../../getting-started/apps-for-devices/05-desktop-app.md) (fonctionnalité complète et édition de fichiers) ; [application tablette](../../getting-started/apps-for-devices/11-tablet-app.md), [application mobile](../../getting-started/apps-for-devices/08-mobile-app.md) (fonctionnalité limitée, l’édition n’est pas prise en charge).

### Activation de Google Drive

Pour commencer à ajouter des fichiers depuis Google Drive, vous devez installer le plug-in et connecter votre Google Drive à Miro.

Installez l’application depuis le [Marketplace de Miro](https://miro.com/marketplace/google-drive/?backUrl=%2Fmarketplace%2F). Après avoir cliqué sur " **Obtenir l’application"**, il vous sera proposé de choisir une équipe pour laquelle installer le plugin.![install_Google_Drive.jpg](../../../../../../docs/integrations-apps/google/images/21016134562450_install%20Google%20Drive.jpg)*Choix d’une équipe lors de l’installation du plugin Google Drive*

Vous pouvez également installer le plug-in à partir d’un tableau. Dans la barre de création, sélectionnez **Outils, médias et intégrations****(+).** Un panneau s'ouvre. Dans l'onglet **Outils**, recherchez Google Drive. Sélectionnez **Charger**, puis **Google Drive**.

![Google_Drive_sur_la_barre_d’outils.jpg](../../../../../../docs/integrations-apps/google/images/21016121227026_Google%20Drive%20on%20the%20toolbar.jpg)

Ensuite, connectez Google Drive à Miro. Vous pouvez le faire facilement de deux façons différentes.

1.  Dans les paramètres de votre profil. Dans la barre du tableau, sélectionnez l'icône hamburger. La barre latérale s'ouvre. Sélectionnez votre avatar, puis sélectionnez **Paramètres**. Les paramètres de votre profil s'ouvrent dans une nouvelle fenêtre. Sélectionnez l'onglet **Intégrations** . Pour **Google Drive**, sélectionnez **Connecter**.

![connecter_Google_Drive.jpg](../../../../../../docs/integrations-apps/google/images/21016121228306_connect%20Google%20Drive.jpg)*Google Drive sur la page Intégrations*

2. Connectez votre profil Miro à Google Drive à partir du tableau en cliquant sur **Google Drive** dans le menu **Charger de** la barre d’outils :

![Google_Drive_sur_le_menu_de_chargement.jpg](../../../../../../docs/integrations-apps/google/images/21016121222546_Google%20Drive%20on%20the%20Upload%20menu.jpg)*L’icône Google Drive dans la barre d’outils*

Confirmez l’autorisation pour le compte Google requis et **autorisez** l’application à accéder à vos fichiers :

![permissions.jpg](../../../../../../docs/integrations-apps/google/images/21016121229586_permissions.jpg)
*Autorisations de Google Drive*

Veuillez noter qu’il s’agit des autorisations standard de pour Google Drive.

- **Consulter et télécharger tous vos fichiers Google Drive** - pour un sélecteur de fichiers Google Drive sur un tableau. Cela vous permet d’importer des documents de Google Drive vers Miro.

- **Afficher, modifier, créer et supprimer uniquement les fichiers Google Drive spécifiques que vous utilisez avec cette application** - afin de pouvoir enregistrer un tableau Miro sur Google Drive.

L’application Google Drive ne gère que les fichiers que nous créons sur le Drive (liens vers les tableaux, etc).  Miro n’a pas la possibilité de gérer le contenu de votre Google Drive. Pour implémenter l’intégration, nous utilisons **Google Drive API v3**. Dans cette API, les champs d’application sont regroupés de manière à ce que les autorisations d’accès en écriture ne puissent pas être demandées séparément des autorisations d’accès complet au disque. Si vous souhaitez jeter un coup d’œil, consultez les autorisations dans l’article de Google, [Champs d’application pour les API Google](https://developers.google.com/identity/protocols/googlescopes).

Si vous avez besoin de changer le compte Google connecté à Miro, allez dans **Paramètres du profil** > **Intégrations**, cliquez sur **Se déconnecter** à côté de **Google Drive** et connectez-vous à un autre compte.

![Google_Drive_logout_in_settings.jpg](../../../../../../docs/integrations-apps/google/images/21016121230610_Google%20Drive%20log%20out%20in%20settings.jpg)*Connexion à Google Drive dans les paramètres du profil*

### Ajouter des fichiers à partir de Google Drive et des Drive partagés

> **Disponible sur :** version pour navigateur, [application de bureau](../../getting-started/apps-for-devices/05-desktop-app.md), [application pour tablette](../../getting-started/apps-for-devices/11-tablet-app.md), [application mobile](../../getting-started/apps-for-devices/08-mobile-app.md) (fonctionnalité limitée)

:::warning
Toute personne ayant accès à un tableau Miro peut extraire ses tableaux importés, même s’ils sont restreints du côté de Google. Pour protéger vos tableaux, il est important d’éviter de partager le tableau avec des personnes qui ne devraient pas avoir accès aux documents.
:::

Pour ajouter un fichier depuis Google Drive :

1. Collez l’URL du document directement sur le tableau (notez que coller une URL dans une [forme](../../using-miro/essential-tools/11-shapes.md) ou un [pense-bête](../../using-miro/essential-tools/14-sticky-notes.md) n’intégrera pas votre document au tableau, mais ajoutera le lien sous forme de texte simple). Lorsque vous copiez un lien vers une feuille de calcul spécifique à partir des feuilles de calcul Google et que vous le collez dans le tableau Miro, la feuille de calcul collée démarre toujours à partir de la première page dans Miro.

   ou :
2. Cliquez sur le bouton **Charger** dans la barre d’outils (illustré dans la capture d’écran ci-dessus) et choisissez **Google Drive**. Vous verrez alors le menu du sélecteur. Sélectionnez tous les documents que vous souhaitez ajouter et cliquez sur **Sélectionner**. Vous pouvez également vous aider de la barre de recherche pour trouver des documents sur votre Google Drive.

:::tip
Pour ajouter un document Google Drive sur un tableau dans l’[application mobile](../../getting-started/apps-for-devices/08-mobile-app.md), collez l’URL du document via le menu Charger.
:::

![select_a_file_in_Google_Drive.gif](../../../../../../docs/integrations-apps/google/images/21016121231122_select%20a%20file%20in%20Google%20Drive.gif)*Sélection d’un document dans Google Drive*

Ajoutez des documents à partir de **Drive partagés** : passez sur l’onglet concerné et choisissez des fichiers.

![team_drive.jpg](../../../../../../docs/integrations-apps/google/images/21016134572434_team%20drive.jpg)*Équipe Drive dans le sélecteur Google Drive*

### Modifier des documents Google

> **Disponible sur :** version pour navigateur, [application de bureau](../../getting-started/apps-for-devices/05-desktop-app.md)

Vous pouvez intégrer des documents Google Docs, Google Sheets et Google Slides directement sur le tableau, les déplacer et les redimensionner et également changer les pages des documents.

Cliquez sur le document et vous verrez un menu contextuel avec les options permettant de changer de page, d’**épingler** une page, d’**extraire** des pages, de **modifier** le contenu, de **recharger**, de **mettre à jour** ou d’accéder à la **source**.

Pour modifier le document, cliquez sur l’icône du stylo dans le menu contextuel ou double-cliquez sur le document. Le document s’ouvre dans une fenêtre contextuelle et vous pouvez le modifier comme s’il se trouvait dans votre Google Drive. Cliquez sur **Fermer** ou sur la zone grise pour terminer la modification. Toutes les modifications sont automatiquement enregistrées et visibles sur le tableau et dans Google Docs.

![google_drive_edit_docs.gif](../../../../../../docs/integrations-apps/google/images/21016121248274_google_drive_edit_docs.gif)*Modification d’un document Google intégré*

Si vous préférez, vous pouvez également cliquer sur le bouton **source** et le document s’ouvrira pour être modifié dans l’onglet suivant.

Si vous avez apporté des modifications directement à partir de votre Google Drive (en particulier lorsque vous travaillez hors ligne), actualisez l’intégration sur le tableau à l’aide du bouton **Mettre à jour** dans le menu contextuel. Les fichiers Google Drive intégrés ne sont pas mis à jour automatiquement sur les tableaux Miro (sauf si le fichier est modifié à partir de Miro).

![bouton_mise_à_jour.jpg](../../../../../../docs/integrations-apps/google/images/21016121232274_update%20button.jpg)*Bouton de mise à jour*

### Gérer les droits d’accès

Notez que les droits d’accès dans Google Drive et dans Miro sont définis *séparément*. Cela signifie que pour permettre à quelqu’un de modifier un document Google sur le tableau, vous devez partager le document avec cette personne dans Google Drive en lui octroyant des droits de *modification* et en l’[invitant en tant qu’*éditeur* sur le tableau](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

Si vous autorisez quelqu’un à modifier le document dans Google, mais que vous l’invitez sur le tableau avec uniquement [le droit de consulter et de commenter](../../using-miro/sharing-boards/01-board-access-rights.md), cette personne ne pourra pas activer le mode de modification du document. Inversement, si vous invitez une personne sur le tableau en tant qu’éditeur mais que vous ne partagez pas le document avec elle dans Google Drive, Google ne lui permettra pas de le modifier.

Assurez-vous que vous et les membres de votre équipe disposez du niveau d’accès requis pour une collaboration réussie.

### Enregistrer votre tableau sur Google Drive

> **Configuré par :** les propriétaires du tableau

Dans la barre du tableau, sélectionnez les trois points verticaux. Le menu **principal** s'ouvre. Sélectionnez **Tableau** > **Exporter** > **Enregistrer sur Google Drive**.

Dans Google Drive, vous pouvez désormais cliquer sur le tableau enregistré et il s’ouvrira dans un onglet de navigateur distinct. Si vous supprimez le tableau de Google Drive, il sera toujours disponible dans Miro. Toutefois, si vous supprimez le tableau dans Miro, vous ne pourrez plus y accéder à partir de Google Drive.

:::warning
Si vous n’êtes pas le propriétaire du tableau, le message d’erreur ci-dessous apparaîtra.
:::

![Google_Drive_error.jpg](../../../../../../docs/integrations-apps/google/images/21016121236882_Google%20Drive%20error.jpg)*Message d’erreur concernant les droits d’enregistrement insuffisants*

### Désinstallation du plugin

Pour désinstaller le plugin pour une équipe, cherchez-le dans la section **Applications et intégrations** des paramètres de l’équipe et cliquez sur **Désinstaller pour l’équipe**.

![uninstall_Google_Drive_app.jpg](../../../../../../docs/integrations-apps/google/images/21016134575122_uninstall%20Google%20Drive%20app.jpg)*Désinstallation de Google Drive pour une équipe*

Pour déconnecter Miro de Google Drive, ouvrez la page **Intégrations** dans Paramètres du profil et cliquez sur **Se déconnecter** près de l’icône Google Drive.

![Google_Drive_logout_in_settings.jpg](../../../../../../docs/integrations-apps/google/images/21016121230610_Google%20Drive%20log%20out%20in%20settings.jpg)*Déconnexion de Google Drive de Miro*

### Fonctionnalités non disponibles pour les fichiers Google Drive intégrés

**Général**

- Page de démarrage de Google Drive
- Déplacement des fichiers entre les dossiers
- Partage
- Aide à la recherche

**Présentations Google**

- Mode de présentation

### Problèmes éventuels et comment les résoudre

**Erreur « Impossible de charger »**

Si vous obtenez le message d’erreur **Sorry, il semble que vous n’ayez pas le droit de charger ce fichier ou que le fichier ait été supprimé. Veuillez vérifier le droit d’accès et réessayer** lorsque vous essayez de charger un fichier Google Drive sur un tableau Miro, demandez à votre administrateur Google d’autoriser les utilisateurs à accéder à Google Drive avec l’API Drive SDK :

1. Connectez-vous à la [console d’administration Google.](https://admin.google.com/)
2. Cliquez sur **Accueil > Applications > Google Workspace**. Assurez-vous que **Drive et Docs** sont **activés pour tous.**
3. Cliquez sur **Drive et Docs > Fonctionnalités et applications**. Dans la section **Drive SDK**, assurez-vous que l’option **Autoriser les utilisateurs à accéder à Google Drive avec l’API Drive SDK** est **activée**.

![unable_to_upload.png](../../../../../../docs/integrations-apps/google/images/21016134575634_unable%20to%20upload.png)
*Message d’avertissement "Impossible de charger".*

**Problème d’autorisation**

Si vous ne pouvez pas connecter votre Google Drive à Miro, veillez à donner à Miro l’accès à l’**affichage et au téléchargement de tous vos fichiers Google Drive** et à l’**affichage, la modification, la création et la suppression uniquement des fichiers Google Drive spécifiques que vous utilisez avec cette application** lors de la connexion de votre Google Drive. Pour cela, allez dans les [paramètres de votre profil Miro](../../using-miro/managing-your-profile/01-profile-settings.md) > **Intégrations**, supprimez la connexion avec Google Drive, puis réinstaurez-la.

![Permissions.png](../../../../../../docs/integrations-apps/google/images/21016121246994_Permissions.png)
*Accès de Miro au compte Google Drive*

### Foire aux questions

1. *Puis-je ouvrir un fichier incorporé dans Google Drive ?*
   - Oui, sélectionnez le document et cliquez sur le bouton **source** dans le menu contextuel.
2. *Puis-je coller le contenu des tableaux Miro dans un fichier Google Drive ?*
   - Vous pouvez [copier le contenu du tableau sous forme de texte ou d’image](../../using-miro/working-on-the-board/09-copy-as-text-or-as-an-image.md) et le coller dans un fichier Google Drive.
