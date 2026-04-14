---
title: "L\xF6schungsszenarien im \xDCberblick"
article_id: 19596032332434
translation_id: 19596032332434
locale: de
sidebar_position: 6
created_at: '2024-06-17T17:24:29Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

## Automatisches Verschieben von Boards in den Papierkorb

Boards werden am angegebenen Löschungsdatum automatisch in den Papierkorb verschoben. Wenn keine aktive Aufbewahrungsrichtlinie auf das Board zutrifft, gilt die Papierkorbrichtlinie für die endgültige Löschung.
![disposition1.png](images/19599506827666_disposition1.png)

Nehmen wir als Beispiel ein Projekt-Board, das am 1. Juli 2025 gemäß der Löschungsrichtlinie in den Papierkorb verschoben werden soll und auf das keine Aufbewahrungsrichtlinie zutrifft. Das Board wird am 1. Juli 2025 automatisch in den Papierkorb verschoben und am 29. September 2025 gemäß der 90-Tage-Richtlinie dauerhaft gelöscht.

:::note
Eine aktive Aufbewahrungsrichtlinie ersetzt die Papierkorbrichtlinie. Daher wird das Datum für die dauerhafte Löschung des Boards von der geltenden Aufbewahrungsrichtlinie bestimmt.
:::

Wenn Löschungsbenachrichtigungen für die Richtlinie aktiviert sind, erhalten Nutzer eine Benachrichtigung gemäß der konfigurierten Anzahl von Tagen im Voraus, bevor das Board gemäß dem Zeitplan in den Papierkorb verschoben wird.

Die Benachrichtigung erscheint im Miro-Feed und verlinkt direkt zum Board. Ein Banner wird auch oben auf dem Board angezeigt, das den Nutzer vor der bevorstehenden Papierkorbaktion warnt. Board Eigentümer und Miteigentümer haben die Möglichkeit, das Board zu behalten.

## Von Nutzern initiiertes Löschen von Boards

Wenn ein Board-Eigentümer ein Board in den Papierkorb verschiebt, hat die Löschungsrichtlinie keinen Einfluss mehr auf den Lebenszyklus des Boards. Wenn für das Board keine aktiven Aufbewahrungsrichtlinien gelten, gilt für das dauerhafte Löschen die Papierkorbrichtlinie.

![disposition2.png](images/19599506828946_disposition2.png)

Ein weiteres Beispiel wäre ein Board, das als Betriebsplan am 13. Oktober 2024 gelöscht werden soll. Wenn der Board-Eigentümer das Board bereits am 15. Mai 2024 in den Papierkorb verschiebt und keine aktiven Aufbewahrungsrichtlinien für das Board vorliegen, gilt in diesem Fall die Papierkorbrichtlinie. Das Board wird am 13. August 2024 gemäß der 90-Tage-Papierkorbrichtlinie dauerhaft gelöscht.

:::note
Wenn eine aktive Aufbewahrungsrichtlinie für das Board gilt, setzt diese die Papierkorbrichtlinie außer Kraft und es gilt stattdessen das Datum für die dauerhafte Löschung gemäß der Aufbewahrungsrichtlinie.
:::

## Vom Nutzer initiierte Board-Wiederherstellung

Wenn ein Nutzer ein Board aus dem Papierkorb wiederherstellt, werden alle relevanten Löschungsrichtlinien automatisch wiederhergestellt. So wird sichergestellt, dass das Board seinen Lebenszyklus wieder aufnimmt und alle ursprünglichen Richtlinieneinstellungen wiederhergestellt werden.

![disposition3.png](images/19599490625298_disposition3.png)

Zum Beispiel könnte ein Nutzer am 20. Juni 2024 ein Marketingstrategie-Board aus dem Papierkorb wiederherstellen, für das zuvor eine 1-Jahres-Löschungsrichtlinie galt. Diese Richtlinie würde dann bei der Wiederherstellung automatisch wiederhergestellt. Das neue Löschungsdatum des Boards würde ab dem Wiederherstellungsdatum neu berechnet. Als aktualisiertes Löschungsdatum gälte dann der 20. Juni 2025 oder das Datum ein Jahr nach dem Tag, an dem dieses Board zuletzt nach der Wiederherstellung geändert wurde.

## Benachrichtigungen zur Löschung

Löschungsbenachrichtigungen informieren Nutzer im Voraus, wenn ein Board aufgrund von Inaktivität, basierend auf einer aktiven Löschungsrichtlinie, automatisch in den Papierkorb verschoben wird.

- Admins können Benachrichtigungen aktivieren, wenn sie eine Richtlinie veröffentlichen.
- Der Benachrichtigungszeitpunkt ist von 1 bis 30 Tagen vor dem geplanten Verschiebedatum konfigurierbar.
- Benachrichtigungen werden gemäß der konfigurierten Anzahl von Tagen gesendet, an denen die Benachrichtigung zur Löschung vor dem Datum des Papierkorbs gesendet werden muss.

Wenn ein Board in die Prüfungsphase eintritt:

- Eine Benachrichtigung erscheint im Benachrichtigungs-Feed des Nutzers.
- Beim Anklicken öffnet sich das Board mit einem oberen Banner, das vor der bevorstehenden Verschiebung in den Papierkorb warnt.
- Nutzer können das Board behalten, um es zu bewahren, was den Löschungs-Timer zurücksetzt.

Dieser Benachrichtigungsmechanismus gilt für alle Szenarien, in denen:

- Eine Löschungsrichtlinie mit Benachrichtigungen ist aktiv.
- Das Board tritt in seine Prüfungsphase ein (gemäß der konfigurierten Anzahl von Tagen vor dem Löschdatum).

### Szenario 1: Boards, die einer Löschungsrichtlinie entsprechen

Diese Boards fallen unter eine Richtlinie und werden nach dem festgelegten Zeitraum der Inaktivität in den Papierkorb verschoben.

Wenn Löschungsbenachrichtigungen für die Richtlinie aktiviert sind, wird eine Benachrichtigung gemäß der konfigurierten Anzahl von Tagen gesendet, an denen die Benachrichtigung zur Löschung vor dem geplanten Verschiebungsdatum des Boards in den Papierkorb gesendet werden muss. Das Board wird auch ein Banner anzeigen, das es den Nutzern ermöglicht, es zu überprüfen oder zu behalten.

### Szenario 2: Boards mit einem Klassifizierungslabel, das nach der letzten Bearbeitung des Boards hinzugefügt wurde.

Diese Boards werden nachträglich in den Geltungsbereich aufgenommen und folgen weiterhin derselben Löschungszeitachse basierend auf ihrem letzten Änderungsdatum.

Falls Benachrichtigungen zur Löschung aktiviert sind, erhalten die Nutzer eine Benachrichtigung gemäß der konfigurierten Anzahl von Tagen, wann die Löschungsbenachrichtigung im Voraus vor dem geplanten Verschieben in den Papierkorb gesendet werden muss, selbst wenn das Label nach der letzten Bearbeitung angewendet wurde.

### Szenario 3: Boards mit einem Klassifizierungslabel, das entfernt wurde, bevor die Richtlinie veröffentlicht wurde.

Diese Boards fallen nicht mehr unter die Richtlinie und sind von der Löschungsbewertung ausgeschlossen.

Da sie aus dem Geltungsbereich herausfallen, werden keine Benachrichtigungen zur Löschung gesendet.

### Szenario 4: Kürzlich geänderte Boards, die noch nicht im Löschungsschwellenwert liegen.

Diese Boards wurden kürzlich bearbeitet und sind noch nicht zur Löschung berechtigt.

Eine Benachrichtigung wird nur gesendet, wenn das Board in die Inspektionsperiode eintritt – das heißt, gemäß der konfigurierten Anzahl von Tagen, wann die Löschungsbenachrichtigung im Voraus vor dem Löschungsdatum gesendet werden muss. Bis dahin wird keine Benachrichtigung ausgelöst.

### Szenario 5: Boards, die nach Eintritt in den Inspektionszeitraum geändert wurden

Sobald ein Board in den Inspektionszeitraum eintritt, wird sein Löschdatum festgelegt. Das bedeutet, dass das Board, sofern der Eigentümer nicht ausdrücklich entscheidet, es zu behalten, am geplanten Datum automatisch in den Papierkorb verschoben wird.

Das Ändern oder der Zugriff auf das Board während des Inspektionszeitraums beeinflusst den Löschungszeitplan nicht. Die folgenden Aktionen ändern das Löschungsergebnis nicht: das Bearbeiten oder Ansehen des Boards, das Ändern seines Klassifizierungslabels oder Teams, oder sogar das Löschen der zugehörigen Richtlinie.

Wenn Löschungsbenachrichtigungen aktiviert sind, wird eine Benachrichtigung gemäß der konfigurierten Anzahl von Tagen gesendet, bevor das Löschungsdatum erreicht wird. Das Board zeigt dann ein Banner an, das dem Nutzer erlaubt, es zu überprüfen oder zu behalten.

### Szenario 6: Boards, die bereits gelöscht oder manuell in den Papierkorb verschoben wurden.

Diese Boards sind bereits aus dem Arbeitsbereich entfernt und werden nicht mehr durch Löschungsrichtlinien verwaltet.

Für Boards, die sich bereits im Papierkorb befinden oder dauerhaft gelöscht wurden, werden keine Löschungsbenachrichtigungen gesendet.

### Szenario 7: Boards unter mehreren Richtlinien

Boards können gleichzeitig unter mehr als eine aktive Löschungsrichtlinie fallen, insbesondere wenn mehrere Richtlinien dasselbe Klassifizierungslabel oder Team anvisieren.

Wenn mehr als eine Richtlinie mit aktivierten Benachrichtigungen auf ein Board angewendet wird, erhält der Nutzer nur eine Benachrichtigung, sobald das Board in den Inspektionszeitraum eintritt. Die Benachrichtigung basiert auf der Richtlinie mit dem frühesten angesetzten Löschungsdatum und wird gemäß der konfigurierten Anzahl von Tagen gesendet, bevor die Löschungsbenachrichtigung an diesem Datum erfolgen muss.

## Szenario 8: Boards befinden sich bereits im Prüfstatus und die Löschungsrichtlinie wird anschließend gelöscht

Wenn ein Board bereits den Prüfzeitraum erreicht hat und Löschungsbenachrichtigungen versandt wurden (falls aktiviert), ist das geplante Löschungsdatum festgelegt. Auch wenn die zugehörige Löschungsrichtlinie später gelöscht oder geändert wird, wird das Board am ursprünglichen Löschungsdatum automatisch in den Papierkorb verschoben – es sei denn, der Board-Eigentümer entscheidet sich, es zu behalten.

Im Gegensatz dazu wird das Board als außerhalb des Geltungsbereichs betrachtet und nicht in den Papierkorb verschoben, wenn die Richtlinie gelöscht wird, bevor das Board den Prüfzeitraum erreicht hat.
Dies stellt sicher, dass die Löschungsaktion konsistent und vorhersagbar bleibt, sobald die Nutzer benachrichtigt wurden, unabhängig von danach vorgenommenen Richtlinienänderungen.
