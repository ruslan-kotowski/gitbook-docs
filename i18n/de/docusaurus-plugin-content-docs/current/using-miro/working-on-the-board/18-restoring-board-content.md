---
title: Wiederherstellung von Board-Inhalten
article_id: 360019838260
translation_id: 360019838260
locale: de
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

Mit der Funktion zur Wiederherstellung von Whiteboard-Inhalten kannst du sicher sein, dass versehentliches Löschen von Inhalten die Produktivität deines Teams nicht beeinträchtigt. Board-Bearbeitende können Objekte leicht wiederherstellen, die kürzlich von deinen Boards gelöscht wurden.

> **Einrichtung durch:** Bearbeiter, die explizit [per E-Mail](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) zu Boards eingeladen wurden  oder Zugriff auf das Board haben, weil sie Teil eines [Projekts](../sharing-boards/16-projects.md) oder [Teams](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) in Miro sind
> **Verfügbar mit:** Browser-Version, [Desktop-App](../../getting-started/apps-for-devices/05-desktop-app.md), [Tablet-App](../../getting-started/apps-for-devices/11-tablet-app.md)

> **⚠️** Die Funktion ist für [Besucher](../sharing-boards/08-collaboration-with-visitors.md) nicht verfügbar.

>   Sieh dir [diese Anleitung](../managing-boards/12-board-history-versions.md) an, um zu erfahren, wie du eine Whiteboard-Version wiederherstellst.

### Welche Inhalte können wiederhergestellt werden

- Alle Inhalte, die während deiner aktuellen aktiven Sitzung aus dem Whiteboard gelöscht wurden, und 30 Minuten nach dem Löschen des Inhalts, falls die Sitzung vorbei ist
- Die letzten 1000 Objekte, die vom Board gelöscht wurden – wenn die Wiederherstellung mehr als 30 Minuten nach dem Löschen des Inhalts erfolgt
- Alle Inhalte, die vom Board gelöscht wurden, wenn die Objekte für einen unbestimmten Zeitraum gleichzeitig ausgewählt und gelöscht wurden – bis die nächsten 1000 Objekte gelöscht werden

### Wie du Inhalte wiederherstellst

Um gelöschte Objekte wiederherzustellen, gehe wie folgt vor:

1. Klicke auf das Symbol **Seitenleiste öffnen** in der unteren linken Ecke.
2. Klicke in der geöffneten Whiteboard Übersicht auf das Symbol **Whiteboard-Verlauf**.
3. Klicke auf das Symbol **Wiederherstellen** auf jedem Objekt, das du wiederherstellen möchtest.  Die gelöschten Objekte erscheinen auf dem Whiteboard (genau dort, wo sie waren, bevor sie gelöscht wurden), und das Whiteboard wird auf diesen Teil des Whiteboards vergrößert.

restore_board_content_restore_feature.jpg
*Wiederherstellen eines gelöschten Objekts*

### Einschränkungen

> **⚠️** Bitte beachte, dass Sonderfälle auftreten können, wenn:

- der Inhalt an einer anderen Stelle des Whiteboards wiederhergestellt wird (z. B. wenn eine [Verbindungslinie](../essential-tools/05-connection-lines.md) wiederhergestellt wird und der [Notizzettel](../essential-tools/14-sticky-notes.md), an der sie befestigt war, auf dem Whiteboard neu positioniert wurde)
- der Inhalt seine Verbindung zu dem Objekt verliert, mit dem er ursprünglich verbunden war (z. B. wenn eine [Karte](../essential-tools/02-cards.md) aus einer [Tabelle](../advanced-tools/05-grid.md) gelöscht und dann wiederhergestellt wird – sie wird an derselben Stelle des Whiteboards wiederhergestellt, ist aber nicht mehr mit der Tabelle verbunden)
- bestimmte Inhalte werden nicht wiederhergestellt.  Zu den aktuellen Einschränkungen gehören:

- [Zeilen](../essential-tools/05-connection-lines.md), die mit Objekten verbunden waren, die später aus dem Whiteboard gelöscht wurden
- Text aus einer Tabellenzelle, wenn er aus der Tabelle entfernt wurde (wenn die Tabelle zusammen mit dem Text gelöscht wurde, wird sie wiederhergestellt)
- [User-Story-Map](../advanced-tools/07-user-story-mapping.md) (sowohl das Framework als auch die Karten)
- [Kommentare](../facilitation-tools/asynchronous-tools/01-comments.md) separat gelöscht

  ![mceclip0.png](../../../../../../docs/using-miro/working-on-the-board/images/21017605949842_mceclip0.png)
  *Das Banner, das du erhältst, wenn einige Inhalte nicht wiederhergestellt wurden*

Wenn Objekte gelöscht und dann gleichzeitig wiederhergestellt wurden, werden alle Links innerhalb dieser Charge auch wiederhergestellt, aber es besteht die Möglichkeit, dass Links zu externen Objekten außerhalb des Boards nicht wiederhergestellt werden.

Beachte, das [Whiteboard-Duplikate](../managing-boards/03-how-to-duplicate-a-board.md) die Option, Objekte wiederherzustellen, die auf dem ursprünglichen Whiteboard gelöscht wurden, nicht unterstützen.

### Häufige Fragen

1. *Mein Inhalte sind verschwunden, aber ich sehe nicht die Option, gelöschte Objekte wiederherzustellen.*  Was muss ich tun?
   - Bitte beachte, dass bestimmte Inhalte nicht wiederhergestellt werden können (siehe die Einschränkungen oben). Wenn dein Inhalt andere Arten von Widgets enthält: /span>
   - stelle sicher, dass du das richtige Board geöffnet hast
   - überprüfe die Liste deiner [benutzerdefinierten Templates](../../getting-started/start-here/your-first-board/02-custom-templates.md) mit einem ähnlichen Namen
   - prüfe die Board-[Mini-Karte](21-work-smarter-not-harder.md#minimap-verwenden) um zu sehen, ob Inhalte in verschiedenen Teilen des Boards enthalten sind
   - stelle sicher, dass du bei Miro unter der richtigen E-Mail-Adresse autorisiert bist, wenn du mehrere Miro-Profile hast.
