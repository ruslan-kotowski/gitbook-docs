---
title: Zapier
article_id: 360025942994
translation_id: 360025942994
locale: de
sidebar_position: 18
created_at: '2019-07-04T17:26:16Z'
updated_at: '2025-02-26T12:10:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Mit Zapier kannst du deine Lieblings-Apps mit Miro verknüpfen und so die Liste der Möglichkeiten zur Automatisierung deiner täglichen Aufgaben erweitern. Verschiebe automatisch Informationen zwischen deinen Apps und Boards, damit du dich auf deine wesentlichen Aufgaben konzentrieren kannst.

> **Verfügbar mit:** Free-, Starter-, Business- und Enterprise-Preispläne

## Erstellen eines Zaps in Miro

Um Miro über Zapier mit anderen Apps zu verbinden, brauchst du ein Zapier-Konto.

Klicke auf dem [Dashboard in Zapier](https://zapier.com/app/dashboard) auf die entsprechende Schaltfläche, um einen Zap zu erstellen.

Create_Zap.jpg
Schaltfläche „Create Zap“ (Zap erstellen)

Zapier schafft mit **Triggern** (Auslösern) und **Actions** (Aktionen) einen automatisierten Workflow zwischen Apps.

:::warning
Miro fungiert in Zapier ausschließlich als **Action**.
:::

**Trigger**

Ein Trigger ist ein Event (Ereignis) in einer App, das den Zap startet. Sobald du einen Zap eingerichtet hast, überwacht Zapier die App für dieses Event. Im Beispiel „Save new events in Google Calendar to Miro card widgets“ (Neue Ereignisse in Google Calendar in Miro-Karten-Widgets speichern) wird der Zap nur dann ausgelöst, wenn ein neues Ereignis im Google Calendar erstellt wird.

new_event_trigger.jpg
Einrichten eines Trigger-Events in Zap

**Aktion**

Eine Aktion ist ein Event, das den Zap vollendet. Im vorherigen Beispiel „Save new events in Google Calendar to Miro card widgets“ verhalten sich neue Miro-Karten wie eine Action.

:::warning
Miro funktioniert im Moment nur als Action in Zapier.
:::

Finde Miro und wähle dort eine der drei Aktionen: Board kopieren, Board erstellen, Karten-Widget erstellen.

creating_a_Zap_with_Miro_as_an_action.gif
Deinen eigenen Zap mit Miro als Action erstellen

### Die Action „Copy Board“

Es handelt sich um eine Action, die dazu dient, eine Kopie eines bestimmten Boards zu erstellen. Du musst ein Team auswählen, in dem die Board-Kopie erstellt werden soll.

install_Zapier.jpg
Ein Miro-Team auswählen

Wähle im nächsten Schritt die folgenden Parameter aus:

- Original Board – Wähle ein Board aus dem Team aus, um eine Kopie davon zu erstellen. Du kannst das Board anhand seines Namens oder seiner ID finden *(*z. B. *o9J_rxLXasqA).* Wenn du ein Board nicht in der Liste findest, versuche bitte, die Daten neu zu laden und schaue dann noch einmal nach.
- Title: Gib einen Titelnamen für die Board-Kopie ein. Wenn du das Feld leer lässt, wird das Board mit dem Namen **Untitled** erstellt.
- Description: Gib Text für die Beschreibung des Boards ein.
- Team Access: Du kannst zwischen den Zugriffsarten **Private** (privat), **View** (anzeigen), **Comment** (kommentieren) und **Edit** (bearbeiten) für das Team auf das Board auswählen.
- Access Via Link: Erstelle Regeln bezüglich der Freigabe dieses Boards mit einem Link. Du kannst die Zugriffsgruppen als **Private** (Privat), **View** (Ansehen) und **Comment** (Kommentieren) festlegen.

set_up_action.jpg
/em>Action-Event „Copy Board“ (Board kopieren) einrichten /font>

### Die Action „Create Board“

Diese Action erstellt ein Board mit einem bestimmten Titel, einer bestimmten Beschreibung und bestimmten Zugriffseinstellungen.

- Title: Gib einen Titelnamen für das neue Board ein. Wenn du das Feld leer lässt, wird das Board mit dem Namen **Untitled** erstellt.
- Description: Gib Text für die Beschreibung des Boards ein.
- Team Access: Du kannst zwischen den Zugriffsarten **Private** (Privat), **View**, (Ansehen) **Comment** (Kommentieren) und **Edit** (Bearbeiten) für dein Team wählen.
- Access Via Link: Erstelle Regeln bezüglich der Freigabe dieses Boards mit einem Link. Du kannst den Zugriff über einen öffentlichen Link auf **Private**, **View** oder **Comment** festlegen.

create_board_action.jpg
Action-Event „Create Board“ (Board erstellen) einrichten

### Die Action „Create Card Widget“

Mit dieser Aktion kannst du Informationen (z. B. Slack-Nachrichten) als [Karten](../../using-miro/essential-tools/02-cards.md)-Widget direkt in einen bestimmten [Rahmen](../../using-miro/essential-tools/07-frames.md) auf einem Miro-Board mit benutzerdefinierten Regeln übertragen.

- Board: Wähle ein Board aus dem Team, das du verwenden möchtest. Du kannst das Board anhand seines Namens oder seiner ID finden *(*z. B. *o9J_rxLXasqA).* Wenn du ein Board nicht in der Liste findest, versuche bitte, die Daten neu zu laden und schaue dann noch einmal nach.
- Frame: Wähle einen Rahmen aus dem von dir ausgewählten Board aus. Du kannst den Rahmen anhand seines Namens suchen. Falls du ihn nicht findest, versuche bitte, die Daten neu zu laden und schaue dann noch einmal nach.
- Card Title: Gib einen Titel für deine Karte ein.
- Card Title Link: Hier kannst du einen Link aus der verknüpften App einfügen (du kannst z. B. eine Karte mit einem Link zu einer neu erstellten Aufgabe in Asana erstellen).
- Card Description: Erstelle eine Beschreibung für deine Karte.
- Card Due Date: Lege ein Fälligkeitsdatum für die Karte fest.
- Card Border Color: Wähle eine benutzerdefinierte Farbe für die Kartenränder aus (z. B. wird die Kartenfarbe durch **#ff0000** in diesem Feld auf rot gesetzt).

create_card_action.jpg
Action-Event „Create card“ (Karte erstellen) einrichten

## Deaktivieren der Zapier-Integration

Um die Zapier-Integration aus deinem Miro-Team zu entfernen, öffne die [Team-Einstellungen](../../administration/get-started-as-a-miro-admin/06-manage-starter-and-education-plan.md)**> Apps & Integrationen > Zapier**und klicke auf **Deinstallieren***.*

uninstall_Zapier.jpg
Deinstallationsoptionen für Zapier

## Häufige Fragen

1. *Brauche ich ein Zapier-Konto für Unternehmen, um es mit Miro zu nutzen?*
   - Nein, das ist nicht erforderlich. Die Miro-Integration kann mit jedem Zapier-Plan erstellt werden.
2. *Wo werden meine Zapier-Daten gespeichert?*
   - Dies ist eine offizielle, von Miro gewartete Integration und alle Datenspeicherungspraktiken in Miro gelten auch hier.
3. *Muss ich Team-Admin in Miro sein, um die Zapier-Integration einzurichten?*
   - Das hängt von den Admin-Einstellungen in Miro und in Zapier ab. Standardmäßig können auch Teammitglieder, die keine Administratoren sind, die Integration einrichten.
4. *Werden die Karten (Trello, Asana, etc.) mit den in Miro-Boards importierten Karten synchronisiert?*
   - Nein, Zapier bietet derzeit keine Synchronisierung an. Wenn du zum Beispiel deine Trello-Karte von „doing“ auf „done“ verschiebst, wird das nicht in Miro angezeigt.
5. *Ich kann Gmail nicht über Zapier mit Miro verknüpfen.*  Warum?
   - Bitte prüfe deine E-Mail. Im Moment können Personen mit einem Gmail-Konto, das auf *@gmail.com* oder *@googlemail.com* endet, Gmail nicht mit Miro verknüpfen, da Zapier Gmail-Informationen nur an eine begrenzte Anzahl von Apps senden kann.
