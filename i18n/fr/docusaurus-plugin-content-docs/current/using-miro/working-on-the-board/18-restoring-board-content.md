---
title: Restaurer le contenu du tableau
article_id: 360019838260
translation_id: 360019838260
locale: fr
sidebar_position: 18
created_at: '2021-02-24T08:56:24Z'
updated_at: '2026-01-06T19:00:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
---

Grâce à la fonctionnalité de restauration du contenu du tableau, vous pouvez être sûr que la suppression accidentelle de contenu n'entrave pas la productivité de votre équipe. Les éditeurs de tableaux peuvent facilement restaurer les objets récemment supprimés de leurs tableaux.

> **Mis en place par : les**éditeurs qui ont été explicitement invités à participer aux tableaux [par e-mail](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) ou qui ont accès au tableau parce qu’ils font partie d’un [projet](../sharing-boards/16-projects.md) ou d’une [équipe](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) dans Miro.
> **Disponible sur** : version navigateur, [application de bureau](../../getting-started/apps-for-devices/05-desktop-app.md), [application pour tablette](../../getting-started/apps-for-devices/11-tablet-app.md)

> **⚠️**La fonctionnalité n’est pas disponible pour les [visiteurs](../sharing-boards/08-collaboration-with-visitors.md).

> Veuillez consulter [ce guide](../managing-boards/12-board-history-versions.md) pour savoir comment restaurer une version du tableau.

### Quel contenu peut être restauré

- Tout contenu supprimé du tableau pendant la session active en cours et 30 minutes après la suppression du contenu si la session est terminée.
- Les 1000 derniers objets supprimés du tableau, si la restauration a lieu plus de 30 minutes après la suppression du contenu.
- Tout contenu supprimé du tableau si les objets ont été sélectionnés et supprimés simultanément pendant une durée indéterminée, jusqu’à ce que les 1000 objets suivants aient été supprimés.

### Comment restaurer le contenu

Pour restaurer les objets supprimés, procédez comme suit :

1. Cliquez sur l’icône **Open sidebar** (Ouvrir la barre latérale) dans le coin inférieur gauche.
2. Dans l’aperçu du tableau ouvert, cliquez sur l’icône **Board history** (Historique du tableau).
3. Cliquez sur l’icône **Restore** (Restaurer) sur n’importe quel objet que vous souhaitez récupérer.  Les objets supprimés réapparaîtront sur le tableau (exactement là où ils se trouvaient avant d’être supprimés) et le tableau zoomera sur cette partie du tableau.

restore_board_content_restore_feature.jpg
Restaurer un objet supprimé

### Restrictions

> **⚠️** Veuillez noter qu’il y aura des cas particuliers dans lesquels :

- le contenu sera restauré dans une autre partie du tableau (par exemple, lorsqu'une [ligne de connexion](../essential-tools/05-connection-lines.md) est restaurée et que le [pense-bête](../essential-tools/14-sticky-notes.md) à laquelle elle était attachée a été repositionné sur le tableau)
- le contenu perdra sa connexion à l'objet auquel il était initialement lié (par exemple, lorsqu'une [carte](../essential-tools/02-cards.md) est supprimée d'un [tableau](../advanced-tools/05-grid.md), puis restaurée, elle sera restaurée dans la même partie du tableau mais ne sera plus attachée au tableau)
- certains contenus ne seront pas restaurés.  Les restrictions actuelles comprennent :

- [les lignes](../essential-tools/05-connection-lines.md) qui étaient connectées à des objets supprimés du tableau plus tard
- le texte d'une cellule du tableau s'il a été supprimé du tableau (si le tableau a été supprimé avec le texte, il sera restauré)
- [la carte de récit utilisateur](../advanced-tools/07-user-story-mapping.md) (à la fois le cadre et les cartes)
- [commentaires](../facilitation-tools/asynchronous-tools/01-comments.md) supprimés séparément

  ![mceclip0.png](../../../../../../docs/using-miro/working-on-the-board/images/21017605949842_mceclip0.png)
  *La bannière que vous obtenez si certains contenus n'ont pas été restaurés*

En règle générale, si des objets ont été supprimés puis restaurés simultanément, tous les liens de cet ensemble seront également restaurés, mais il est possible que les liens vers des objets externes en dehors du tableau ne soient pas restaurés.

Notez que [les doublons de tableau](../managing-boards/03-how-to-duplicate-a-board.md) ne prennent pas en charge l'option de restauration des objets qui ont été supprimés sur le tableau d'origine.

### Foire aux questions

1. *Mon contenu a disparu, mais je ne vois pas l’option de restauration des objets supprimés.*  Que faire ?
   - Veuillez noter que certains contenus ne peuvent pas être restaurés (voir les limitations ci-dessus). Si votre contenu comprenait d'autres types de widgets, veuillez : /span>
   - vous assurer que vous avez ouvert le tableau correct
   - vérifier la liste de vos [modèles personnalisés](../../getting-started/start-here/your-first-board/02-custom-templates.md) avec un nom similaire
   - vérifier la [mini-carte](21-work-smarter-not-harder.md#utiliser-la-minimap) du tableau pour voir s'il y a du contenu dans différentes parties du tableau
   - vous assurer que vous êtes autorisé dans Miro sous l'adresse e-mail correcte si vous avez plusieurs profils Miro.
