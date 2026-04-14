---
title: "Miro f\xFCr Jira Cloud"
article_id: 360017572414
translation_id: 7626017826834
locale: de
sidebar_position: 4
created_at: '2022-09-14T08:42:39Z'
updated_at: '2024-10-08T15:15:34Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Visualisiere alles zusammen mit deinem Team – so könnt ihr am Produkt-Backlog mit digitalen Notizen arbeiten und Flussdiagramme, Diagramme und Wireframes erstellen. Du kannst Boards an Jira-Vorgänge anhängen und mit deinem Team in Echtzeit wie bei einem Präsenzmeeting mit Whiteboard zusammenarbeiten.

> **Verfügbar mit:** Starter-, Business- und Enterprise-Preisplan
> Nur Jira Cloud

:::note
Du kannst Miro-Boards auch mit der Atlassian Smart Link-Funktion einbetten.
:::

:::note
Beachte, dass es in Miro zwei Arten von Jira-Integrationen gibt: **Miro für Jira Cloud** (damit kannst du Miro-Boards auf der Jira-Seite einbetten) und **Jira-Karten**. Um mehr über Jira-Karten zu erfahren, besuche [diesen Artikel](https://help.miro.com/hc/articles/360017572434).
:::

## Installationsleitfaden

Der Installationsprozess ist für alle Jira-Add-ons gleich. Melde dich zunächst mit administrativen Rechten bei Jira an und lade das Add-on [hier](https://marketplace.atlassian.com/apps/1215456/miro-for-jira-cloud?tab=overview&hosting=cloud) herunter (die App findest du auch auf dem **Atlassian Marketplace** > **Find new apps** > **Miro for Jira Cloud**): Klicke auf **Get app**und **Get it now**.
Das wars auch schon! Die Installation ist abgeschlossen.

![Miro_for_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134089234_Miro%20for%20Jira.jpg)
*Jira-Benachrichtigung über die erfolgreiche Installation*

Bitte beachte, dass du als Admin während der Einrichtung den Jira-Nutzern keine Miro-Nutzer zuordnen musst. Jeder Nutzer muss sich selbst in Miro innerhalb von Jira autorisieren.

## Verwendung des Add-ons

### Boards an Jira-Vorgänge anhängen

Um ein Board an einen Jira-Vorgang anzuhängen, öffne den Vorgang in Jira. Klicke im Bereich **Miro-Boards** auf **Board hinzufügen**.
![add_Miro_boards_in_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134090642_add%20Miro%20boards%20in%20Jira.jpg)
*Die Schaltfläche für das Add-on erscheint nach der Installation*

:::tip
Wenn du den Bereich „Miro-Boards“ nicht hast, findest du ihn im Kontextmenü des Vorgangs.
:::

![Miro_boards_section.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134091026_Miro%20boards%20section.jpg)
*Hinzufügen des Bereichs „Miro-Boards“ zu einem Jira-Vorgang*

Du siehst ein Auswahltool mit Miro-Boards. Wähle das Board aus, das du hinzufügen möchtest (du kannst im Auswahltool zwischen deinen Teams wechseln). Wenn du nicht für Miro autorisiert bist, musst du dich zuerst anmelden.

Lege die Freigabeeinstellungen des Boards im Dropdown-Menü fest. Du kannst das Board zum Ansehen und Kommentieren freigeben, sodass auch Nutzer, die kein Profil in Miro haben, darauf zugreifen können.

:::note
Für  Nutzer [im Enterprise-Preisplan](https://help.miro.com/hc/articles/360017571534) von Miro folgen deine Zugriffseinstellungen den organisationsweiten Zugriffskontrollen, was bedeuten kann, dass einige Freigabeoptionen eingeschränkt sind. Mehr erfährst du unter [Verwalten der unternehmensweiten Freigaberichtlinien für Integrationen zum Einbetten](https://help.miro.com/hc/articles/4405088016274).
:::

![embed_a_board_in_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134091922_embed%20a%20board%20in%20Jira.jpg)
*Freigabeeinstellungen beim Anhängen eines Boards an einen Jira-Vorgang*

Beachte, dass du nur Boards einbetten kannst, für die du Bearbeitungszugriff hast.

Dein Board ist nun an den ausgewählten Jira-Vorgang angehängt:

![Miro_board_in_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016120705810_Miro%20board%20in%20Jira.jpg)
 *Miro-Boards, die an einen Jira-Vorgang angehängt sind*

### Erstellen neuer Boards von Jira aus

Um ein neues Board direkt von einem Jira-Vorgang aus zu erstellen, klicke auf **Board hinzufügen** und erstelle ein **Neues Board** aus dem Auswahltool.

![create_a_new_board_from_the_picker.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016120706322_create%20a%20new%20board%20from%20the%20picker.jpg)
*Erstellen eines Boards aus der Auswahltool*

### Boards ansehen, kommentieren und bearbeiten

Klicke einfach auf ein angehängtes Board, um es je nach den eingestellten Zugriffsrechten anzuzeigen/zu kommentieren/zu bearbeiten. Das Board-Fenster öffnet sich als Overlay und ermöglicht es dir, so zu arbeiten und zusammenzuarbeiten, als ob du Miro verwenden würdest.

![Miro_embed_in_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016120699410_Miro%20embed%20in%20Jira.jpg)
*Board-Overlay in Jira*

 Du kannst auch auf die Schaltfläche „Quelle“ klicken, um das Board in Miro in einem neuen Tab zu öffnen.

![source_button.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134094738_source%20button.jpg)
*Die Schaltfläche zum Aufrufen der Miro-App*

### Boards entfernen

Um ein Board zu entfernen, klicke einfach auf das Kreuz-Symbol und der Anhang wird sofort aus dem Vorgang entfernt (in Miro ist das Board davon nicht betroffen).

![remove_an_attached_board.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134095634_remove%20an%20attached%20board.jpg)
*Die Option, das angehängte Board zu entfernen*

## Deaktivieren des Add-ons

Um die Integration zu deaktivieren, öffne den **Atlassian Marketplace** > **Manage apps** > öffne die Seite des Add-ons und klicke auf **Uninstall**:

![uninstall_Jira_add-on.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134096274_uninstall%20Jira%20add-on.jpg)
*Die Option zur **Deinstallation** im Bereich der Jira Add-ons*

## Atlassian Smart Link für Miro

Du kannst Miro-Boards in Jira-Vorgänge einbetten, indem du die Atlassian Smart Link-Funktion nutzt. Mit dieser Funktion kannst du ein Board automatisch einbetten, ohne dass du ein Plug-in installieren musst.

:::note
Bitte beachte, dass nur die Nutzer, die Zugriff auf das eingebettete Board auf der Miro-Seite haben, mit der Vorschau arbeiten können, nachdem sie ihre Miro- und Atlassian-Konten verbunden haben. Wenn du die Vorschau für alle Jira-Nutzer verfügbar machen möchtest, kannst du das Jira-Add-on verwenden.
:::

Gehe zu einem Jira-Vorgang und füge einfach einen Board-Link ein oder gib „/link“ ein, um ihn einzufügen. Wenn du die Funktion zum ersten Mal verwendest, wirst du aufgefordert, dein Miro-Team zu verbinden. Klicke auf **Connect, to preview,** autorisiere den Vorgang in Miro und wähle ein Team aus, aus dem du deine Boards einbetten möchtest.

![install_Atllassian_links.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134098834_install%20Atllassian%20links.jpg)
*Auswahl eines Teams zum Einbetten der Boards*

Wenn du den Link eines Miro-Boards in einen Jira-Vorgang einfügst, wird er automatisch in ein Jira-Widget umgewandelt. Wenn du auf den Link klickst, siehst du die Optionen, den Link als Karte oder als Einbettung anzuzeigen.

![display_as_link.gif](../../../../../../docs/integrations-apps/atlassian/images/21016134099346_display%20as%20link.gif)
*Die Optionen zur Anzeige eines Miro-Boards als Link, Karte oder zum Einbetten*

Wenn du dich dafür entscheidest, das Board als Einbettung anzuzeigen, kannst du die Größe der Einbettung durch Ziehen an der Seite ändern.

![changing_embed_size_in_Jira.gif](../../../../../../docs/integrations-apps/atlassian/images/21016120700306_changing%20embed%20size%20in%20Jira.gif)
*Größe der Miro-Einbettung in Jira ändern*

:::warning
Wenn Cookies von Drittanbietern in deinem Browser blockiert sind, kann es unerwartete Probleme bei der Anzeige von eingebetteten Boards geben.
:::

## Häufige Fragen

Kann ich den Abschnitt „Miro-Boards“ in Jira-Vorgängen ausblenden?

Ja, klicke auf die drei Punkte in der oberen rechten Ecke des Bereichs und wähle **Hide Miro boards**.
![hide_Miro_boards.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016120713746_hide%20Miro%20boards.jpg)
*Miro-Boards in Jira ausblenden*

Funktioniert das Add-on in Projekten der nächsten Generation von Jira?

Ja, du kannst deine Boards an Projekte dieser Art anhängen.

Fallen zusätzliche Kosten für das Jira-Add-on an?

Miro für Jira Cloud ist für alle kostenpflichtigen Preispläne ohne zusätzliche Kosten verfügbar (Starter-, Business- und Enterprise-Preispläne).

Wir werden Jira von einer Cloud-Instanz zu einer anderen migrieren. Sind Miro-Boards, die in Jira-Vorgänge eingebettet sind, betroffen?

Es sollte keine Probleme mit eingebetteten Miro-Boards geben, wenn die Inhalte ohne Änderungen verschoben werden.
