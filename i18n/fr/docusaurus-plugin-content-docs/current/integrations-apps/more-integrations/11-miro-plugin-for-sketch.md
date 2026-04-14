---
title: Plugin Miro pour Sketch
article_id: 360017731173
translation_id: 360017731173
locale: fr
sidebar_position: 13
created_at: '2019-02-11T10:13:46Z'
updated_at: '2025-02-26T12:15:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Le plugin Miro pour Sketch offre un moyen simple et rapide d’obtenir des images de Sketch directement sur le tableau. Envoyez vos tableaux sur Miro et mettez-les à jour facilement en un clic. Synchronisez toutes vos images à chaque fois que vous apportez une modification sans avoir à les télécharger à nouveau.

### Autoriser le plugin

1. 1. Téléchargez le plugin Sketch depuis GitHub : suivez [ce lien](https://github.com/miroapp/sketch_plugin) > **Code** > **Download ZIP** (Télécharger le ZIP) :

Download_from_Github.jpg

2. 2. Procédez à l’extraction du contenu de l’archive zip > double-cliquez sur le paquet RealtimeBoard.sketchplugin pour installer le plugin.

plugin_installed.jpg
Le plugin Miro pour Sketch est installé

3. 3. Pour l’activer, ouvrez Sketch, allez dans **Plugins >** **Manage plugins** (Gérer les plugins) et cochez la case **Miro by Miro** (Miro par Miro).

Miro_plugin_in_Sketch.jpg
Le plugin Miro est activé dans Sketch

4. 4. Après cela, vous devez vous authentifier avec vos identifiants Miro. Pour ce faire, cliquez sur **Plugins -** **Miro**: **Connectez-vous à Miro, déconnectez-vous de Miro**.

Log_in_to_Miro_in_Sketch.jpg
Connectez-vous à Miro

5. 5. Saisissez votre e-mail et votre mot de passe, ou cliquez sur **Use company credentials (Utiliser les informations d’identification de l’entreprise)** si vous vous connectez via SSO.

Miro_login.jpg
La fenêtre d’authentification pour vous connecter à Miro

### Ajout de tableaux Sketch à Miro

Pour ajouter un tableau d'art Sketch à Miro, allez dans **Plugins**: **Miro -** **Synchroniser tous les artboards avec Miro**.

La fenêtre de dialogue vous donnera la possibilité de choisir entre les tableaux sur lesquels vous avez un rôle d’éditeur via une invitation par e-mail ou via un accès à l’équipe ou au [projet](../../using-miro/sharing-boards/16-projects.md).

> *⚠️ Veuillez noter que les tableaux sur lesquels vous avez un rôle de [visiteur](../../using-miro/sharing-boards/08-collaboration-with-visitors.md) ne seront pas disponibles.*

Sélectionnez un tableau en a) cliquant sur l’une des suggestions de la liste déroulante ou b) en saisissant le nom du tableau. Après cela, cliquez sur l’option appropriée pour ajouter **tous** les tableaux ou les **tableaux sélectionnés**. Cochez la case **Open Miro after sync** si vous souhaitez ouvrir Miro après la synchronisation :

select_a_board.jpg
Sélection d’un tableau pour la synchronisation

Cliquez sur **Sync** (Synchroniser) et les tableaux apparaîtront sur votre tableau Miro.

artiboards_in_Miro.jpg
**Veuillez noter que vous pouvez envoyer des tableaux uniquement sur les tableaux existants sur Miro**

:::warning
Notez que le copier-coller direct des tableaux n’est disponible que dans la version *pour navigateur* de Miro.
:::

### Synchroniser des tableaux Sketch sur Miro

Pour synchroniser les planches d'art qui ont déjà été ajoutées à Miro et ensuite modifiées dans Sketch, allez dans **Plugins -** **Miro**: **Synchronisez tous les plans de travail avec Miro**. Le tableau sur lequel vous avez précédemment synchronisé les tableaux sera automatiquement sélectionné dans la fenêtre de dialogue, il suffit de choisir si vous voulez synchroniser **tous** les tableaux ou seulement les tableaux **sélectionnés**. Cochez la case **Open Miro after sync** si vous souhaitez ouvrir Miro après la synchronisation :

syncing_boards.jpg
Synchronisation des tableaux avec Miro

### Désactiver le plugin

Pour arrêter la synchronisation de Sketch et Miro allez dans **Plugins >** **Manage plugins** (Gérer les plugins) et décochez la case **Miro by Miro** (Miro par Miro).

disable_Miro_sync.jpg
Le plugin Miro est désactivé dans Sketch

### Problèmes éventuels et comment les résoudre

|  |  |  |
| --- | --- | --- |
| **Message d’erreur ou problème** | **Causes éventuelles** | **Solution** |
| 1. Une erreur s’est produite. There was an error during syncing. Please retry. » (Une erreur est survenue. Une erreur est survenue lors de la synchronisation. Veuillez réessayer.) | 1. 1. Vous utilisez une version obsolète de Sketch./span>  2. 2. Votre tableau Sketch est énorme (il y a une très grande image dans le tableau Sketch). | 1. 1. Mettez le plugin Sketch à jour vers sa version la plus récente.  2. 2. Vérifiez la taille de l’image et diminuez-la si nécessaire. |
| 2. Erreur de connexion Something went wrong. » (Erreur de connexion. Une erreur est survenue.) | 1. 1. Le plugin n’est pas en mesure de se connecter à l’API de Miro.  2. 2. Le taux est limité par l’API de Miro.  3. 3. Il y a d’autres problèmes éventuels avec le réseau. | Déconnectez-vous et reconnectez-vous à votre profil Miro dans Sketch et essayez de synchroniser le tableau à nouveau. |
| 3. There was an error during syncing. Please retry. » (Une erreur est survenue. Une erreur est survenue lors de la synchronisation. Veuillez réessayer.) | Le problème peut être causé par des modifications apportées aux paramètres de votre réseau. | Enregistrez les journaux de la console et [envoyez un rapport de bogue au service d’assistance de Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md). |
| 4. 4. Le plugin Sketch se fige et fonctionne de manière inattendue lorsqu’il tente de synchroniser plusieurs tableaux avec Miro. | Cela se produit lorsque vous avez un énorme tableau Miro et que vous essayez de synchroniser plusieurs tableaux via le plugin Sketch. | Créez un nouveau tableau Miro dans Miro et synchronisez un seul tableau à la fois avec celui-ci. |
| 5. 5. Les tableaux ne s’affichent pas dans les résultats de la recherche dans Sketch | Cela se produit lorsqu’un tableau a été déplacé vers un autre [projet](../../using-miro/sharing-boards/16-projects.md) dans Miro ou si vous n’avez pas de licence dans le projet où se trouve le tableau. | 1. 1. Vérifiez si le tableau qui n’apparaît pas dans la liste de synchronisation dans Sketch a été déplacé vers un autre projet Miro.  2. 2. Vérifiez si vous avez une licence dans un projet où se trouve un tableau. |
| 6. 6. Sketch ne remplace pas les tableaux existants sur un tableau Miro - ils sont dupliqués sur le schéma et non remplacés | Cela se produit lorsqu’un tableau synchronisé avec Sketch a été [déplacé](../../using-miro/managing-boards/04-how-to-move-a-board.md) [vers une autre équipe Miro](../../using-miro/managing-boards/04-how-to-move-a-board.md).  Dans ce cas, les images seront dupliquées lors de la première synchronisation. Par la suite, elles seront remplacées. | Supprimez les tableaux précédents du tableau Miro. Les doublons seront à nouveau remplacés. |

#### Comment enregistrer les journaux de Sketch pour le service d’assistance de Miro

1. Ouvrez la recherche Spotlight (cliquez sur l’icône de loupe dans le coin supérieur droit de l’écran) > /span>[Console](https://www.howtogeek.com/356942/how-to-view-the-system-log-on-a-mac/) :

spotlight_search.jpg
Recherche Spotlight

2. 2. Saisissez **sketch-rtb-error** dans le champ de recherche de la console et recherchez avec les filtres By message (Par message) ou Any (N’importe lequel) :

search_in_Sketch.jpg
Recherche dans la console

3. 3. Cliquez sur la ligne contenant le message dans la partie inférieure de la console, faites une capture d’écran et partagez-la avec nous.

error_message.jpg
Message d’erreur de la console
