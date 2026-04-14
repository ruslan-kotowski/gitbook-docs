---
title: OneDrive
article_id: 360017731273
translation_id: 360017731273
locale: fr
sidebar_position: 7
created_at: '2019-02-11T10:14:03Z'
updated_at: '2025-01-13T13:02:45Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-drive-onedrive
---

L’intégration OneDrive vous permet d’enrichir vos tableaux avec des documents Microsoft Office et Office 365 (fichiers Doc, Excel ou PDF, images, présentations PowerPoint, etc.).

> **Disponible sur :** version pour navigateur, [application de bureau](../../getting-started/apps-for-devices/05-desktop-app.md)

### Installer le plugin

Installez le plugin au niveau de l’équipe et connectez votre compte OneDrive à Miro pour commencer à utiliser l’intégration.

Vous pouvez installer le plugin à partir de [Miro](../integrations-basics/04-how-to-install-apps.md): trouvez OneDrive et cliquez sur **Get application.** Sélectionnez ensuite une équipe dans laquelle vous souhaitez installer le plugin et cliquez sur **Installer et autoriser.**

:::warning
Les utilisateurs sans rôle d’administrateur ne peuvent pas installer les applications si cela n’est pas autorisé dans les paramètres des  **Apps & Integrations** (Applications et Intégrations).
:::

install_OneDrive.jpg
Choix de l’équipe lors de l’installation du plugin OneDrive

Vous pouvez également installer l'application à partir d'un tableau. Suivez les étapes suivantes :

1. Dans la barre de création, sélectionnez **Outils, médias et intégrations** **(+).**Le panneau **Outils, médias et intégrations** s'ouvre.
2. Dans l'onglet **Outils**, recherchez et sélectionnez Téléchargements.
   Le menu **Charger** s'ouvre.

![uploads-entry-point.png](../../../../../../docs/integrations-apps/microsoft/images/21537454978706_uploads-entry-point.png)
*L'icône OneDrive de la barre d'outils Création*

Pour connecter votre compte OneDrive à Miro, choisissez OneDrive dans le menu **Upload** (Télécharger). La page de connexion Microsoft s’ouvrira et vous pourrez y autoriser Miro avec votre nom d’utilisateur et votre mot de passe.

Vous pouvez également le faire dans la section [Profile Integrations](https://miro.com/app/account/profile/integrations/) (Intégrations du profil) : trouvez-y **OneDrive** et cliquez sur **Connect** (Se connecter).

connect_OneDrive.jpg
Connexion de OneDrive à Miro

### Ajouter des fichiers

Cliquez sur le bouton **Charger** dans la barre d'outils Création, choisissez **OneDrive**. Sélectionnez les fichiers que vous souhaitez ajouter, puis cliquez sur **Open** (Ouvrir).

Si vous utilisez **OneDrive for Business**, vous pouvez consulter vos documents directement à partir du tableau. Il vous suffit tout simplement de double cliquer sur le document que vous souhaitez afficher. Le document s’ouvre dans une fenêtre contextuelle sur le tableau et vous pouvez le parcourir comme si vous étiez sur votre OneDrive.

Vous pouvez modifier votre document en vous rendant sur votre OneDrive directement depuis le tableau Miro.

file_source_.jpg
Le bouton source permettant d’ouvrir le fichier dans OneDrive

### Mettre à jour des fichiers

Pour mettre à jour un fichier sur un tableau Miro, cliquez sur le bouton correspondant dans le menu contextuel.

update_OneDrive_file.jpg
Mise à jour d’un document OneDrive sur un tableau Miro

Veuillez noter qu’il peut y avoir un retard dans l’affichage des nouvelles données.

### Désactiver le plugin

Si vous souhaitez désinstaller le plugin pour une équipe, ouvrez les paramètres de l’équipe, trouvez OneDrive dans la section **Apps & Integrations** (Applications et intégrations), puis cliquez sur **Uninstall for team** (Désinstaller pour l’équipe).

uninstall_OneDrive.jpg
Désinstallation de OneDrive dans Team settings (Paramètres d’équipe)

Pour déconnecter OneDrive de Miro, ouvrez la section [Profile Integrations](https://miro.com/app/account/profile/integrations/) (Intégrations du profil), trouvez-y **OneDrive** et cliquez sur **Log out** (Se déconnecter) :

log_out_from_OneDrive.jpg
Déconnexion de OneDrive de Miro

### Foire aux questions

1. *Miro permet-il de charger des fichiers partagés ?*
   - Non, ce n'est pas possible. Un dossier Shared (Partagé) n’est pas pris en charge par le sélecteur de fichiers MS One Drive que nous utilisons.
2. *Je reçois le message d’erreur « Please authorize your OneDrive account » (Veuillez autoriser votre compte OneDrive).*  Comment puis-je y remédier ?
   - Veuillez désinstaller le plugin et déconnecter votre compte OneDrive dans les [paramètres du profil.](https://miro.com/app/account/profile/integrations/) Puis, réinstallez et reconnectez l’intégration.
