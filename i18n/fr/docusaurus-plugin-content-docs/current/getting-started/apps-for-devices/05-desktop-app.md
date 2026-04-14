---
title: Application de bureau
article_id: 360017572854
translation_id: 360017572854
locale: fr
sidebar_position: 5
created_at: '2019-02-11T10:15:04Z'
updated_at: '2025-11-25T16:00:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
---

Lancez l’application de bureau Miro en quelques secondes directement depuis votre écran d’accueil et travaillez sur les tableaux sans distraction. L’application prend en charge toutes les fonctionnalités de base de la version pour navigateur.

:::tip
Téléchargez l’application Miro sur [notre site web](https://miro.com/apps/).
:::

## Télécharger l’application de bureau Miro

### Windows

- Windows 64-bit - [téléchargez l’application](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.exe)

:::note
Windows 32-bit est obsolète et n'est plus disponible.
:::

### macOS

- Macs avec puces Apple silicon - [télécharger l'application](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro.dmg)
- Macs avec puces Intel - [télécharger l'application](https://desktop.miro.com/platforms/darwin/Install-Miro.dmg)

Pour déterminer le type de processeur que vous possédez, procédez comme suit :

1. Cliquez sur l’icône Apple dans le coin supérieur gauche de votre Mac.
2. Un menu déroulant s’affiche ainsi à l’écran. Cliquez sur l’option **À propos de ce Mac**.

La fenêtre devrait vous indiquer les informations dont vous avez besoin, y compris le type de processeur (Intel ou Apple silicon).

## Déployer Miro sur plusieurs appareils

Miro propose différentes versions d’installation que les administrateurs informatiques peuvent utiliser pour déployer Miro auprès des utilisateurs sur des milliers de machines. Il y a deux façons de procéder : l’installation par utilisateur ou par machine. Pour chacun d’entre eux, il existe des versions avec et sans mise à jour automatique. La version avec mise à jour automatique signifie que vos utilisateurs obtiendront la version actualisée de l’application dès sa publication. Celle sans mise à jour automatique vous permet de mieux contrôler la version de Miro utilisée par vos employés.

### Pour Windows

#### Déployez Miro dans Program Files

Miro peut également être installé dans le répertoire Program Files, ce qui le rend accessible à tous les utilisateurs d’un appareil, tout en conservant leurs profils distincts. Une installation unique sur une machine permet de réduire l’encombrement du disque dur à grande échelle, tout en mettant Miro à la disposition de tous les utilisateurs de cette machine. Si vous optez pour la version avec mises à jour automatiques, notez que des autorisations administratives sont nécessaires pour installer une mise à jour.

- Windows MSI 64 bits avec mises à jour automatiques - [télécharger l'application](https://desktop.miro.com/platforms/win-nsis/Miro-setup.msi)
- Windows MSI 64 bits sans mises à jour automatiques - [télécharger l'application](https://desktop.miro.com/platforms/win-nsis/Miro-no-updates.msi)

#### Déployer Miro pour un utilisateur particulier

Miro propose différentes versions d’installation que les administrateurs informatiques peuvent utiliser pour déployer Miro pour un seul utilisateur. Cette version peut être mise à jour sans autorisation administrative et ne s’installe que pour le(s) utilisateur(s) choisi(s).

- Windows MSI 64 bits avec mises à jour automatiques - [télécharger l'application](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.msi)
- Windows MSI 64 bits sans mises à jour automatiques - [télécharger l'application](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-no-updates.msi)

### Pour macOS

- Mac Apple silicon sans mises à jour automatiques - [télécharger l'app](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro-no-updates.dmg)
- Mac Intel sans mises à jour automatiques - [télécharger l'app](https://desktop.miro.com/platforms/darwin/Install-Miro-no-updates.dmg)

## Configuration système requise pour l’application

### Pour Windows

|  |  |  |
| --- | --- | --- |
|  | **Minimum** | **Recommandé** |
| **CPU** | 3 GHz (2 cœurs/4 threads) | 2,8 GHz (4 cœurs/8 threads) |
| **RAM** | 8 Go | 16 Go (DDR4) |
| **Système d'exploitation** | Windows 10 ou supérieur pour l’application du Microsoft Store + Microsoft .NET Framework 4.5 (Veuillez noter que la version ARM de Windows n'est pas prise en charge) | Système d’exploitation le plus récent |
| **Réseau** | 8 Mbit/s ou plus rapide | 32 Mbit/s |

### Pour macOS

|  |  |  |
| --- | --- | --- |
|  | **Minimum** | **Recommandé** |
| **CPU** | Intel 64 bits ou Apple M1 |  |
| **Système d’exploitation** | MacOS 12 (Monterey) ou supérieur | Dernière version du système |
| **Réseau** | 8 Mb/s ou plus rapide | 32 Mb/s |

Veuillez noter que l’application aura plusieurs instances s’exécutant sur votre appareil :

- Processus principal
- Processus de fenêtre (rendu de l’interface utilisateur)
- Accélération matérielle
- Gestionnaire d’incident
- + 1 processus par onglet ouvert (car chaque onglet a une vue web)

Par exemple, si vous avez 3 onglets ouverts pendant votre travail, vous verrez 7 instances de Miro.exe. Plus d’informations sur cette architecture peuvent être trouvées [ici](https://www.electronjs.org/docs/glossary#process) et [ici](https://www.chromium.org/developers/design-documents/multi-process-architecture).

## Raccourcis spécifiques à l’application

L’application de bureau dispose de [raccourcis](../../using-miro/working-on-the-board/06-shortcuts-and-hotkeys.md) supplémentaires :

- **Ctrl + R** *(pour Windows)* / **Cmd + R** *(pour Mac)* pour recharger l'onglet
- **Ctrl + W** *(pour Windows)* / **Cmd +W** *(pour Mac)* pour fermer l'onglet
- **Ctrl + Q** *(pour Windows)* / **Cmd + Q** *(pour Mac)* pour quitter l'application
- **Ctrl + Shift + L** *(pour Windows)* / **Cmd + Shift + L** *(pour Mac)* pour copier le lien du tableau
- **Ctrl + ~** *(pour Windows)* **/ Cmd + ~** *(pour Mac)* pour zoomer

## Actions de l’application

Le tableau suivant montre quelles actions disponibles dans l'application de bureau Miro peuvent offrir une expérience différente de celle du navigateur :

| Action | **Applications Windows & Mac depuis** [**Applications Miro**](https://miro.com/apps/) |
| --- | --- |
| Enregistrer en tant qu’image (Petit, moyen, grand) | ✔ |
| Enregistrer en tant qu’image (Vecteur) | ✔ |
| Enregistrer en tant que PDF (Petit) | ✔ |
| Enregistrer au format PDF (vecteur) | ✔ |
| Exporter vers une feuille de calcul (CSV) | ✔ |
| Chat vidéo | ✔ |
| Coller depuis une feuille de calcul | ✔ |
| Plugin pour Confluence | ✔ |

### Actions indisponibles

Les actions suivantes sont indisponibles dans l'application de bureau Miro :

- Les visiteurs ne peuvent pas se connecter.

  > ✏️ Seuls les utilisateurs Miro enregistrés peuvent se connecter à l'application de bureau.
- Pas d'option de copier-coller depuis Sketch
- Pour certaines versions de Jira Server, vous ne pouvez pas modifier les cartes Jira pour des raisons de sécurité.

## Vérification orthographique

Si vous souhaitez désactiver la fonctionnalité de vérification automatique de l’orthographe dans l’application de bureau, procédez comme suit :

- Appuyez sur **Alt** (*pour Windows uniquement*)
- Cliquez sur **View** (Consulter) dans la barre de navigation principale en haut
- Décochez la case **Show Spell Check** (Vérifier l’orthographe)

Notez que l’option de désactivation de la vérification orthographique n’est pas disponible dans l’application téléchargée depuis le Microsoft Store.

## Problèmes éventuels et comment les résoudre

### Comment réinitialiser les données de l’application

Dans de nombreux cas où un problème survient (surtout si vous rencontrez des difficultés avec la procédure de connexion), il peut s’avérer utile de **réinitialiser les données** de l’application, en effaçant la mémoire de l’application.

:::tip
Si le problème persiste après la réinitialisation des données, vous pouvez également supprimer l’application et la réinstaller en [téléchargeant la dernière version](https://miro.com/apps/).
:::

#### Pour Windows

Appuyez sur **Alt > Aide**et choisissez de réinitialiser les données de l’application comme indiqué dans la capture d’écran ci-dessous :

​​
![reset app data on Windows.png](../../../../../../docs/getting-started/apps-for-devices/images/21016134171922_reset%20app%20data%20on%20Windows.png)
*Réinitialisation des données de l'application sur l'application de bureau pour Windows*

Si vous ne trouvez pas le menu, vous utilisez probablement l'application téléchargée depuis le MS Store. Dans ce cas, pour réinitialiser les données de l'application, ouvrez les **Paramètres** Windows > **Applications** > **Applications et fonctionnalités** > trouvez **Miro** dans la liste > **Options avancées** > **Réinitialiser**.

Si cela ne vous aide pas immédiatement, supprimez tous les fichiers de l'application à partir de **C:\Users\username\AppData\Roaming\RealtimeBoard** et **C:\Users\username\AppData\Local\Programs\RealtimeBoard**

> **✏️** Si le dossier **Appdata** est caché, consultez [ici](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) comment le révéler.

#### Pour macOS

Cliquez sur Miro dans le menu supérieur et choisissez **Reset application data** (Réinitialiser les données de l’application) comme indiqué dans la capture d’écran ci-dessous :

![reset app data on Mac.png](../../../../../../docs/getting-started/apps-for-devices/images/21016120799378_reset%20app%20data%20on%20Mac.png)
*Réinitialisation des données de l’application sur Mac*

Après cela, essayez de vous reconnecter à l’application et vérifiez si le problème est résolu.

Si la réinitialisation ne vous aide pas immédiatement, ouvrez une fenêtre de recherche > appuyez sur **Commande + Maj + G** > collez **~/Library/Application Support/RealtimeBoard**et supprimez tous les fichiers de l'application.

Si vous utilisez MDM pour Mac

Si vous rencontrez un problème et que l’application ne se charge pas ou est bloquée dans une boucle, assurez-vous que votre configuration permet à nos mises à jour automatiques de fonctionner. `https://github.com/Squirrel/Squirrel.Mac` doit avoir les autorisations suivantes :

- lecture, écriture et exécution pour le répertoire « Application »,
- lecture et écriture pour « ~/Application Support/Caches/ » afin de pouvoir travailler avec le répertoire « com.electron.realtimeboard.ShipIt » et le répertoire temporaire « private/var/folders ».

Si un problème survient pendant le processus de mise à jour, Squirrel crée « ShipIt_stderr.log » dans « ~/Application Support/Caches/com.electron.realtimeboard.ShipIt ». Vous y trouverez plus d’informations sur le problème.
Veuillez noter que Skype et Slack utilisent un processus de mise à jour similaire et donc, si vous avez déjà configuré MDM pour ces applications, vous pouvez appliquer les mêmes paramètres pour l’application de bureau Miro.

## Foire aux questions

1. *Où puis-je télécharger l'application de bureau ?*
   - Téléchargez-la depuis [notre site web](https://miro.com/apps/).
2. *Comment puis-je supprimer la fenêtre contextuelle pour ouvrir l’application de bureau lorsque je lance Miro dans un navigateur ?*
   - Suivez les étapes de [cet article](../../using-miro/troubleshooting-technical-questions/technical-guidelines/04-how-to-disable-miro-desktop-app-pop-up-in-your-browser.md).
3. *Avez-vous une version de l’application de bureau pour Linux ?*
   - Non, pas pour le moment.
4. *Comment puis-je copier le lien d’un tableau ouvert dans l’application de bureau ?*
   - Vous pouvez ouvrir le menu du tableau **Share** (Partager) et copier le lien du tableau à partir de là. Sinon, vous pouvez cliquer sur **File** (Fichier) dans le coin supérieur droit > **Copy board link** (Copier le lien du tableau). Vous pouvez également utiliser le raccourci **Ctrl + Shift + L** *(pour Windows) /* **Cmd + Shift + L** *(pour Mac).*
5. *Lorsque j’appuie sur **Alt** dans mon application de bureau Windows, le menu n’apparaît pas. Comment puis-je l’afficher ?*
   - Veuillez noter que le menu n'est pas pris en charge dans l'application téléchargée à partir du Microsoft Store. Vous pouvez réinitialiser les données de l'application via les paramètres Windows (**Système > Applications > Applications et fonctionnalités > Rechercher Miro > Options avancées > Réinitialiser**) ou [installer la version originale de l'application](https://miro.com/apps/).
6. *Si je supprime l'application de bureau, mes tableaux seront-ils supprimés ?*
   - Non, votre contenu est lié à votre profil Miro. Vous pouvez y accéder dans un navigateur, [application pour tablette](11-tablet-app.md), [application mobile](08-mobile-app.md) également.
