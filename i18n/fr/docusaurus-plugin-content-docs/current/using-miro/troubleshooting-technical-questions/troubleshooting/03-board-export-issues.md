---
title: "Probl\xE8mes d\u2019exportation de tableau"
article_id: 360020567820
translation_id: 360020567820
locale: fr
sidebar_position: 3
created_at: '2021-03-18T12:15:46Z'
updated_at: '2025-11-05T13:45:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Vous pouvez [exporter votre tableau Miro](../../import-and-export/export/03-how-to-export-your-board.md) en tant qu'image, PDF ou fichier CSV. Si vous rencontrez des problèmes pour exporter votre tableau Miro, explorez les solutions possibles ci-dessous.

## Je ne peux pas exporter le tableau

**Le bouton d’exportation est manquant sur mon tableau**

Le bouton d’exportation se trouve sous le menu **trois points** (**...**), puis sous le sous-menu **Tableau**.

Aucune option d’exportation dans le [menu du tableau](../../../getting-started/start-here/your-first-board/05-toolbars.md) :

1. Vérifiez que le propriétaire/copropriétaire du tableau a autorisé les utilisateurs à exporter le tableau dans les paramètres de contenu du tableau.

   Pour connaître le nom du propriétaire du tableau, cliquez sur le nom du tableau dans le coin supérieur gauche pour ouvrir la carte d’informations du tableau. Si vous n’avez pas les droits nécessaires pour voir ces informations, vous pouvez vérifier le nom de l’utilisateur qui vous a invité au tableau dans l’e-mail d’invitation.

   Contactez le propriétaire du tableau et demandez-lui d’activer cette option pour vous dans la **fenêtre** > **Paramètres de partage** > **Autorisations**. Le propriétaire/copropriétaire doit sélectionner quelle catégorie d'utilisateurs peut [copier le contenu du tableau](../../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).
   ![.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044218642_.gif.png)
   *Configuration de qui peut copier le tableau*
2. Assurez-vous que votre navigateur, votre forfait et votre appareil prennent en charge l’export. Vous pouvez vérifier la disponibilité ci-dessous. Si votre navigateur, votre forfait ou votre appareil ne prend pas en charge l’option d’exportation, nous vous recommandons de passer à un autre navigateur ou appareil ou de [changer de forfait](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

   |  |  |  |  |  |  |
   | --- | --- | --- | --- | --- | --- |
   |  | Forfait Free | | Forfaits Starter, Business, Enterprise, Education | | Exporter au format CSV (tous les forfaits) |
   |  | Basse résolution | Haute résolution sans filigrane | Basse résolution | Haute résolution sans filigrane |
   | Google Chrome | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Safari | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Firefox | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Opera | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Edge < 79 | ✘ | ✘ | ✘ | ✔ | ✘ |
   | [Application de bureau](../../../getting-started/apps-for-devices/05-desktop-app.md) | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Tablette | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Mobile | ✘ | ✘ | ✘ | ✘ | ✘ |

**Pour les exports de mauvaise qualité**

Pour résoudre ce problème, fermez les onglets du navigateur et les onglets en arrière-plan. Vous pouvez également essayer de changer de navigateur.

Pour des exports de haute qualité, faites ce qui suit :

- Masquez les cadres que vous ne souhaitez pas exporter. Le contenu des cadres masqués n'est pas exporté.
- Divisez le tableau en tableaux plus petits pour l'exportation.

**Conseils généraux**

- Mettez tout ce que vous voulez exporter dans des cadres, seuls les widgets à l'intérieur des cadres étant exportés.
- Évitez le PDF dans le PDF. Si vous avez un PDF sur un tableau que vous souhaitez exporter au format PDF, remplacez le PDF sur le tableau par des images de basse qualité.
- Convertissez les images haute résolution en JPEG ou réduisez leur taille avec un outil externe.
- Consultez la page d'état de Miro pour les incidents pertinents.
- Divisez le tableau en cadres et exportez chaque cadre séparément. Les fichiers PDF distincts peuvent ensuite être fusionnés à l'aide d'un outil externe.
- Fractionnez les grands tableaux en tableaux plus petits et utilisez les [espaces](../../spaces/01-spaces.md) pour vous aider à rester organisé et à grouper les tableaux qui vont ensemble.

**« Désolé, quelque chose s’est mal passé lors de la génération du document PDF »**

Essayez de diviser le tableau en cadres et d'exporter les cadres séparément, car le problème pourrait être lié à la taille du tableau.

Si cela ne fonctionne pas, vérifiez [les journaux de la console de votre navigateur](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md). Si les journaux contiennent le message suivant :

```
ERR_CONNECTION_ABORTED
```

*où :*

L'exportation est bloquée par un logiciel de sécurité sur votre appareil ou un pare-feu sur votre réseau.

Vous ou votre administrateur système devez configurer les paramètres de votre programme antivirus et/ou votre pare-feu pour permettre à Miro d'effectuer la procédure d’exportation.

En cas de doute, [contactez le service d’assistance Miro](../../tools/troubleshooting/06-contacting-miro-support.md).

**Rien ne se passe lorsque j'essaie d'exporter un tableau en PDF, et Miro n'affiche aucune erreur**

Ce problème connu se produit principalement dans le navigateur Safari, lorsque les fenêtres contextuelles sont désactivées. Pour résoudre le problème sur Safari, [suivez ces étapes](https://support.apple.com/en-gb/guide/safari/sfri40696/mac). Assurez-vous d'activer les fenêtres contextuelles pour miro.com, ou pour tous les sites web. Revenez à Miro et réessayez d'exporter votre tableau.

Pour Chrome, [suivez ces étapes](https://support.google.com/chrome/answer/95472?hl=en&co=GENIE.Platform%3DDesktop).

## J’ai des problèmes avec les fichiers exportés (PDFs, images, CSVs)

**Les images/PDF sont flous sur le document exporté**

Si les images ou les PDF téléchargés sont flous sur votre fichier enregistré :

1. Réglez le zoom du tableau à 100 % et laissez les images/PDF s’afficher avant d’exporter le tableau
2. L’image/PDF téléchargée est peut-être trop complexe ou trop grande pour être exportée. Pour réduire la taille du fichier, convertissez l’image/PDF au format PNG et replacez-la sur le tableau. Ensuite, exportez à nouveau le tableau

Le forfait Free ne permet l’exportation qu’en basse qualité. Si vous devez exporter votre tableau en haute qualité, nous vous recommandons de [le déplacer vers une équipe payante](../../managing-boards/04-how-to-move-a-board.md) ou de [changer de forfait](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

**L’ordre des pages n’est pas le même que celui des cadres sur le tableau**

L’ordre des cadres exportés au format PDF est le même que dans le panneau des cadres. Pour modifier l’ordre des cadres :

1. Ouvrez l’aperçu du tableau dans le coin inférieur gauche.
2. Faites glisser les cadres pour modifier leur position dans la liste. Vous pouvez également utiliser [Magic organize](../../essential-tools/07-frames.md) pour organiser rapidement vos cadres dans l'ordre dans lequel ils sont placés sur le tableau
   ![move_frames.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057584914_move%20frames.gif)
   *Modifier l'ordre des cadres*

**Le fichier exporté est coupé**

Si vous **exportez votre tableau sous forme d’image**, veillez à inclure tout le contenu que vous souhaitez exporter dans la zone exportée sélectionnée.

![save_as_image.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057583890_save%20as%20image.gif)
*Exporter un tableau sous forme d’image*

Si vous **exportez votre tableau au format PDF**, veillez à créer un cadre qui comprendra tout le contenu que vous souhaitez exporter. Puis [exportez le cadre](../../import-and-export/export/03-how-to-export-your-board.md).

**Le fichier PDF exporté ne contient pas de noms de cadre**

Lorsque vous exportez votre tableau sous forme de fichier PDF, les titres des cadres ne sont pas inclus dans l’exportation. Vous pouvez remplacer les titres des cadres en utilisant la [fonctionnalité de texte](../../essential-tools/16-text.md) et apposer le texte sur les cadres. Les titres apparaîtront sur votre PDF.

**Les données d'un fichier CSV exporté ne sont pas structurées**

À l’heure actuelle, l’exportation CSV ne conserve pas la structure des tableaux ni les relations. Cependant, si vous exportez des [tables](../../advanced-tools/05-grid.md) sous forme de fichier CSV, la structure est enregistrée.

Si vous avez besoin d'exporter une [carte mentale](../../advanced-tools/03-mind-map.md) sous forme de fichier avec des données intelligentes, utilisez le [téléchargeur de cartes mentales](https://miro.com/marketplace/mindmapdownloader/?backUrl=%2Fmarketplace%2F).

**Les polices du tableau diffèrent des polices du fichier exporté**

La fonctionnalité d’exportation de Miro utilise les polices installées dans le système d’exploitation de votre appareil. Si la police n’est pas présente dans votre système d’exploitation, une police similaire de votre système sera utilisée à la place. Si vous avez besoin de la même police que sur votre tableau Miro, choisissez une police différente sur le tableau ou installez la police nécessaire sur votre appareil.

## Je ne trouve pas le fichier exporté

**Je ne trouve pas le fichier exporté sur mon appareil**

**Si vous utilisez Miro dans un navigateur**

Les fichiers seront stockés dans le dossier par défaut qui contient les téléchargements du navigateur. Vous pouvez vérifier les options de téléchargement dans les paramètres du navigateur.

**Si vous utilisez l’application de bureau ou l’application pour tablette Miro**

Vérifiez le dossier Téléchargements de votre appareil. Vous pouvez également rechercher vos fichiers en utilisant le nom du tableau.

**Miro crée un nouveau dossier chaque fois que j’exporte un tableau**

> **En rapport avec** : [application de bureau Windows](../../../getting-started/apps-for-devices/05-desktop-app.md)

Il est possible que le chemin ait été enregistré dans les paramètres de l’application Miro. Pour supprimer le chemin :

1. Supprimez l’application de bureau Miro
2. En bas à gauche de Windows (barre de recherche), tapez **%AppData%** et ouvrez le dossier **Local,** puis supprimez le dossier **RealTimeBoard**
3. Ouvrez à nouveau **%AppData%** parcourir jusqu’au dossier **Roaming,** et supprimez le dossier **RealTimeBoard**

Réinstallez la dernière [application Miro](https://miro.com/apps/).

Si aucune des solutions ne fonctionne, [contactez le service d’assistance Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
