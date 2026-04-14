---
title: So kannst du das Kopieren und Exportieren von Boards und Inhalten erlauben
  oder einschränken
article_id: 360018350399
translation_id: 360018350399
locale: de
sidebar_position: 14
created_at: '2020-12-14T06:10:03Z'
updated_at: '2026-01-22T14:23:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
availability:
  notes: 'Verfügbar für: Teammitglieder, (Setup) Team-Admins, (Setup) Unternehmens-Admins
    Welche Preispläne: Starter, Business, Enterprise, Education Welche Plattformen:
    Browser, Desktop, Mobil'
---

Unternehmens-Admins und Team-Admins können festlegen, ob Teammitglieder und Nicht-Teammitglieder Board-Inhalte kopieren dürfen und die standardmäßige Einstellung zum Kopieren für neue Boards festlegen.

Board-Eigentümer und Board-Miteigentümer können die Kopiereinstellungen für andere Teammitglieder auf einem bestimmten Board festlegen. Wenn Admins es Nicht-Teammitgliedern erlauben, Boards zu kopieren, was Besucher und Gäste einschließt, können Board-Eigentümer und Miteigentümer erlauben, dass Nicht-Teammitglieder kopieren können.

Wenn Admins es Nicht-Teammitgliedern nicht erlauben, Inhalte zu kopieren, wird die Board-Option entfernt, die es Nicht-Teammitgliedern erlaubt, ein Board zu kopieren.

:::note
Bei den Free-Preisplänen ist das Kopieren von Boards standardmäßig aktiviert und kann nicht geändert werden.
:::

## Wie du die Berechtigungen zum Kopieren von Boards in einem Team einstellst

Für ein bestimmtes Team kann ein Unternehmens-Admin oder Team-Admin festlegen, ob Nicht-Teammitglieder Boards und Inhalte kopieren und exportieren dürfen, sowie die Standardberechtigungen für neu erstellte Boards festlegen.

Gehe dazu wie folgt vor:

1. Gehe zur **Admin-Konsole**.
2. Klicke auf **Teams**.
3. Klicke auf die Zeile für **\{Team name\}**.
   Das **\{Team name\}**-Feld öffnet sich.
4. Klicke, um den **Tab** "Einstellungen" zu öffnen.
5. Scrollen Sie zu **Inhaltssicherheit**.
6. Beim **Kopieren von Inhalten** können Sie festlegen, ob nur Teammitglieder oder alle in der Organisation Inhalte kopieren dürfen.
7. Legen Sie die **Standardeinstellung zum Kopieren von Inhalten** fest. Board-Eigentümer können diese Einstellung für einzelne Boards ändern.
   Ihre Einstellungen werden automatisch gespeichert.

:::note
Wenn das Kopieren von Board-Inhalten für Personen außerhalb des Teams nicht gestattet ist, wird die Option für **Alle mit Board-Zugriff** aus den Board-Einstellungen entfernt. Beispielsweise ist es Besuchern und Gästen untersagt, Inhalte zu kopieren.
:::

:::note
Bitte beachten Sie, dass das Kopieren von Bildern zwischen privaten Boards, die mit verschiedenen Teams verbunden sind, nicht möglich ist. Wenden Sie sich an Ihren Miro Unternehmens-Admin, um die Erlaubnis für den Zugriff auf das andere Board zum Kopieren von Bildern zu erhalten.
:::

## So legen Sie die Kopierberechtigungen für ein Board fest

Für ein bestimmtes Board kann der Eigentümer oder Miteigentümer festlegen, wer das Board kopieren kann.

Gehe dazu wie folgt vor:

1. Klicke im oberen rechten Bereich eines Boards, das du besitzt, mitbesitzt oder erstellt hast, auf **Teilen**.
   Das Dialogfeld zum Teilen öffnet sich.
2. Klicke unten rechts auf **Freigabeeinstellungen**.
3. Für **Wer kann Board-Inhalte kopieren** wähle eine Option aus.

   > ✏️ Wenn dein Unternehmens-Admin oder Team-Admin die Option **Jeder mit Board-Zugriff** deaktiviert, ist die Option nicht verfügbar.
4. Klicke auf **Fertig**.
   Deine Änderungen werden automatisch gespeichert und gelten für alle, die Zugriff auf das Board haben.

## Optionen zum Kopieren des Boards je nach Nutzertyp

Angenommen, **Jeder mit Zugriff auf das Board** kann Inhalte kopieren, zeigt die folgende Tabelle die Berechtigungen pro Nutzertyp.

|  | Board als Vorlage speichern | Board-Inhalte kopieren | Exportieren | Duplizieren | Dateien vom Board herunterladen |
| --- | --- | --- | --- | --- | --- |
| Teammitglieder | ✔ | ✔ | ✔ | ✔ | ✔ |
| Gäste | ✘ | ✔ | ✔ | ✔ | ✔ |
| Besucher mit einem Miro-Konto | ✘ | ✔ | ✔ | ✔ | ✔ |
| Besucher ohne Miro-Konto | ✘ | (Mit Bearbeitungsrechten) ✔ | ✘ | ✘ | ✔ |

:::note
(Enterprise) Wenn [das Verschieben von Boards zwischen Teams nicht erlaubt ist](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md), ist die Option zum Duplizieren eines Boards nicht verfügbar.
:::

:::note
Hinweis: Einige Optionen sind für bestimmte Nutzerkategorien nicht verfügbar, selbst wenn der Board-Eigentümer allen mit dem Link erlaubt, die Board-Inhalte zu kopieren
:::

## FAQ

*Warum kann ich keine Inhalte auf einem Miro-Board kopieren und einfügen?*

Der Board-Eigentümer oder Miteigentümer erlaubt das Kopieren möglicherweise nicht für deine Rolle. Du kannst deine Rolle in der Zusammenarbeitsleiste oben rechts auf einem Miro-Board ansehen. Kontaktiere den Board-Eigentümer oder Miteigentümer, um Kopierberechtigungen für deine Rolle anzufragen.

Stelle auch sicher, dass du bei Miro angemeldet bist. Wenn deine Rolle Kopierberechtigungen hat und du angemeldet bist, melde dich an und öffne das Board in einem anderen Browser und versuche zu kopieren.

*Warum steht die Option **Jeder mit Zugriff auf das Board** nicht zur Verfügung?*

Ihr(e) Unternehmens-Admin(s) oder Team-Admin(s) haben diese Option deaktiviert. Wenn Sie ein Unternehmens-Admin oder Team-Admin sind, lesen Sie Wie man Kopierberechtigungen für ein Team-Board festlegt.

*Wie kann ich Besuchern erlauben, Dateien herunterzuladen, während ich ihre Fähigkeit einschränke, das Board zu kopieren oder duplizieren?*

Erstelle ein separates Board nur mit den Dateien, und aktiviere das Kopieren der Board-Inhalte für alle mit dem Board-Link. Teile den Board-Link mit den Besuchern.

Alternativ kannst du das neue Board mit den Dateien, und Kopieren aktiviert für alle mit dem Link, in das ursprüngliche Board einbetten. Für mehr Informationen zum Einbetten, [Miro-Board einbetten](../import-and-export/export/02-embed-a-miro-board.md).

*Warum kann ich im Menü **Teilen** die Option **Berechtigungen** nicht finden?*

(Kostenpflichtig) Nur der Board-Eigentümer und der Miteigentümer können Inhaltsberechtigungen festlegen. (Free) Inhaltsberechtigungen können nicht von ihrem Standardstatus abweichen, der das Kopieren für alle Nutzer ermöglicht.

*Kann ich festlegen, wer Inhalte auf mein Board hochladen kann?*

Jeder mit **Bearbeitungsrechten** kann Inhalte auf dein Board hochladen.
