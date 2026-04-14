---
title: "Comment r\xE9soudre et signaler un bug"
article_id: 360017731413
translation_id: 360017731413
locale: fr
sidebar_position: 7
created_at: '2019-02-11T10:14:28Z'
updated_at: '2025-11-25T16:03:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Si vous rencontrez des problèmes de performance ou que vous ne pouvez pas utiliser Miro, découvrez comment signaler le bug au service d’assistance de Miro.

## Avant de signaler un bug

1. Consultez la [page d’état de Miro](https://status.miro.com/) afin de prendre connaissance d’éventuelles dégradations des performances.
2. Vérifiez si le problème se reproduit en [navigation](https://support.google.com/chrome/answer/95464) **privée** et sur un **autre navigateur**.
3. [Désactivez les extensions du navigateur](https://support.box.com/hc/articles/360044196613-How-To-Disable-Plugins-Add-Ons-Extensions-In-Multiple-Browsers). Parfois, elles entrent en conflit avec les processus Miro (par exemple, Grammarly avec les widgets de texte).
4. Si vous travaillez sur l’application de bureau, [effacez les données de l’application.](../../../getting-started/apps-for-devices/05-desktop-app.md)
5. Si vous rencontrez des problèmes de performance sur un tableau spécifique, essayez de le [dupliquer](../../managing-boards/03-how-to-duplicate-a-board.md) afin de voir si le problème persiste sur la copie.
6. Consultez nos guides de dépannage :

- [Problèmes de performance et de chargement des tableaux](../../tools/troubleshooting/04-board-performance-and-loading-issues.md)
- [Je ne peux pas me connecter](../../tools/troubleshooting/09-i-can't-log-in.md)
- [Je ne peux pas accéder à un tableau Miro ou le modifier](../../tools/troubleshooting/08-i-can't-access-or-edit-a-miro-board.md)
- [Problèmes d’exportation de tableau](../../tools/troubleshooting/03-board-export-issues.md)
- [J’ai perdu mon tableau ou mon contenu](../../tools/troubleshooting/11-i-lost-my-board-or-content.md)
- Autres guides

## Comment soumettre un bug

Fournissez autant de détails que possible. Cela nous aidera à comprendre rapidement votre problème afin de mieux vous aider.

1. Incluez une description du problème et envoyez des captures d’écran, des fichiers GIF ou une [courte vidéo](https://chrome.google.com/webstore/detail/openvid-screen-recorder-c/liecbddmkiiihnedobmlmillhodjkdmb).  En outre :

- Si le problème se produit sur un tableau spécifique : [partagez ce tableau](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) avec [support@help.miro.com](mailto:support@help.miro.com) avec, si possible, des droits de modification.
- Si le problème est lié à un fichier spécifique téléchargé : envoyez-nous le fichier.

2. Spécifiez votre appareil, votre système d’exploitation et la version du navigateur.
3. Fournissez les journaux de la console de votre navigateur et les journaux du réseau ou ceux de l’application de bureau.

### Comment enregistrer les journaux de la console

**Comment enregistrer les journaux de la console du navigateur**

1. Lors que vous êtes sur un tableau Miro, **cliquez sur la barre d’adresse** de votre navigateur (suivez cette étape si le problème se reproduit sur l’un des tableaux et non pas sur la page des paramètres ou le tableau de bord). mceclip1.png
2. Appuyez sur **F12** ou **fn + F12** pour ouvrir les outils de développement du navigateur.
3. Choisissez **l’onglet Network (Réseau), cochez la case** **Preserve logs** (Conserver le journal).
4. Rechargez la page.
5. Essayez de reproduire le problème.
6. Cliquez sur la flèche de téléchargement **Export** pour exporter les registres HAR du réseau.
   network_console_logs.jpg
7. Passez à l’onglet Console, faites un clic droit sur les enregistrements et choisissez **Save as** (Enregistrer sous).save_console_logs.jpg
8. Envoyez-nous les *fichiers  .log *et .*har.*  Si la taille du fichier ne permet pas de le joindre à votre ticket, téléchargez le fichier sur n’importe quel stockage cloud et envoyez-nous le lien (autorisez toute personne ayant le lien à télécharger les fichiers).

**Comment enregistrer les journaux de l’application de bureau sur Mac**

Si vous rencontrez un bug sur l’application de bureau sur Mac, envoyez-nous les enregistrements de journal.

1. Sur l’application de bureau, cliquez sur **Help** (Aide) dans le coin supérieur gauche.  Sélectionnez Open developer tools for tabs (Ouvrir les outils de développement pour les onglets). /span>​​​​​​​
   open_developer_tools_for_tabs.jpg
2. ​Passez à l'onglet **Network**.​​​ Cochez la case **Conserver les journaux**
3. Ouvrez le tableau que vous souhaitez dépanner (passez cette étape si vous ne pouvez pas accéder aux tableaux).
4. Rechargez la page à l’aide du **raccourci** Ctrl + R.
5. Reproduisez le problème.
6. Cliquez sur la flèche de téléchargement Export pour exporter les registres HAR du réseau.
   preserve_logs.jpg
7. Passez à l’onglet Console, faites un clic droit sur les enregistrements et choisissez **Save as** (Enregistrer sous).save_as_.jpg
8. Cliquez à  nouveau sur **Aide** > choisissez **Ouvrir les outils de développement** et répétez les étapes 2 à 7. Cela permettrait de collecter un autre type de journal qui nous fournirait un ensemble différent de données, afin d'étudier le problème plus en détail pour vous.
9. Envoyez-nous les fichiers  .log et .har.  Si la taille du fichier ne permet pas de le joindre à votre ticket, téléchargez le fichier sur n’importe quel stockage cloud et envoyez-nous le lien (autorisez toute personne ayant le lien à télécharger les fichiers).

**Comment enregistrer les journaux de l’application de bureau sur Windows**

Si vous rencontrez un bug sur l’application de bureau sur Windows, envoyez-nous les enregistrements de journal.

1. Dans l'application de bureau, appuyez sur la touche **Alt** > cliquez sur **Aide** > **Ouvrez les outils de développement pour les onglets![open_developer_tools_for_tabs_on_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264830994_open%20developer%20tools%20for%20tabs%20on%20Windows.jpg)**
2. ​Passez à l'onglet **Network**.​​​ Cochez la case **Conserver les journaux**
3. Ouvrez le tableau que vous souhaitez dépanner (passez cette étape si vous ne pouvez pas accéder aux tableaux).
4. Appuyez sur **Ctrl + R** pour recharger la page.
5. Reproduisez le problème.
6. Cliquez sur l’icône de téléchargement pour exporter les journaux HAR du réseau.
   preserve_logs.jpg
7. Passez à l’onglet Console, faites un clic droit sur les enregistrements et choisissez **Save as** (Enregistrer sous).
   save_as_.jpg
8. Ouvrez  à nouveau l'**aide** > choisissez **Ouvrir les outils de développement** et répétez les étapes 2 à 7. Cela permettrait de collecter un autre type de journal qui nous fournirait un ensemble différent de données, afin d'étudier le problème plus en détail pour vous.
9. Envoyez-nous les fichiers  .log et .har.  Si la taille du fichier ne permet pas de le joindre à votre ticket, téléchargez le fichier sur n’importe quel stockage cloud et envoyez-nous le lien (autorisez toute personne ayant le lien à télécharger les fichiers).

### Comment collecter un rapport de navigation

Lorsque vous signalez des problèmes de chargement ou de performance, le fait de partager des informations étendues sur la version du navigateur aide l'assistance Miro à diagnostiquer le problème. Vous pouvez trouver ces informations en saisissant une commande spécifique dans la **barre d'adresse de** votre navigateur. Vous trouverez ci-dessous comment accéder à ces informations dans différents navigateurs.

- **Chrome**: chrome://version
- **Microsoft Edge**: edge://version
- **Firefox**: about:support (ou about:version dans certaines versions)
- **Opera**: opera://about
- **Navigateur Yandex**: browser://version

> **✏️** Voir [Comment contacter le service d’assistance de Miro ?](../../tools/troubleshooting/06-contacting-miro-support.md)
