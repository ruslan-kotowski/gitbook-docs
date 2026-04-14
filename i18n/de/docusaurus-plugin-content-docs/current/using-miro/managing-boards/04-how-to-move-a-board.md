---
title: So verschiebst du ein Board
article_id: 360017730093
translation_id: 4436273204882
locale: de
sidebar_position: 4
created_at: '2022-02-21T04:03:23Z'
updated_at: '2026-03-27T16:09:59Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
availability:
  roles: board_owner
  notes: 'Relevant for: All plans'
backstage_link:
  entity_kind: capability
  entity_id: move-board-to-space
---

> **Verfügbar für:** Board-Eigentümer
> **Relevant für:** Alle Preispläne

Jeder Miro-Nutzer kann Mitglied mehrerer Teams sein. Dein Miro-Profil ist deine E-Mail-Adresse. Du kannst ein Miro-Board von einem Team in ein anderes verschieben oder dein Miro-Board auf ein anderes Profil übertragen.

:::note
In den Enterprise-Preisplänen können Miteigentümer und Content-Admins Boards mithilfe der [REST-API von Miro](https://developers.miro.com/reference/update-board) verschieben, was sich absichtlich von der Miro-Oberfläche unterscheidet, wo nur Eigentümer ihre Boards verschieben können.
:::

:::note
Unternehmens-Admins im Enterprise-Preisplan können die Möglichkeit für alle Nicht-Admin-Nutzer und Board-Eigentümer [einschränken, Boards zu einem Team hinzuzufügen oder daraus zu entfernen](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).
:::

## Typische Szenarien

Hier findest du ein paar typische Beispiele für das Verschieben von Boards. In einem Abschnitt dieses Artikels erklären wir, wie es funktioniert:

- Du hast **zwei Miro-Profile** (mit Miro verbundene E-Mail-Adressen) und möchtest Boards von einem Profil in das andere verschieben.
  *Führe die in* [*diesem Abschnitt*](04-how-to-move-a-board.md) *beschriebenen Schritte aus. Verwende dazu den **Free-Preisplan**-Tab.*
- Du hast **von einem Free-Preisplan auf einen kostenpflichtigen Preisplan upgegradet** und möchtest Boards in den kostenpflichtigen Preisplan verschieben.
  *Führe die in* [*diesem Abschnitt*](04-how-to-move-a-board.md) *beschriebenen Schritte aus. Verwende dazu den **Free-Preisplan**-Tab.*
- Du möchtest **Boards zwischen zwei kostenpflichtigen Teams verschieben**.
  *Folge den Schritten in* [*diesem Abschnitt*](04-how-to-move-a-board.md) *unter dem Tab **Kostenpflichtige, Education Preispläne**.*

## Boards zwischen Teams verschieben

:::warning
Wenn du ein Board in ein anderes Team verschiebst, geht der [Verlauf](12-board-history-versions.md) verloren. Wenn du den Verlauf behalten möchtest, empfehlen wir stattdessen, den [Board-Inhalt zu kopieren](../working-on-the-board/09-copy-as-text-or-as-an-image.md).
:::

Um ein Board zwischen Teams zu verschieben, musst du:

- Board-Eigentümer sein
- ein Mitglied von beiden Teams sein

Es gibt zwei Möglichkeiten, ein Board in ein anderes Team zu verschieben: über das Dashboard oder direkt innerhalb eines Boards.

### So verschiebst du ein Board direkt innerhalb des Boards

1. Öffne dein Board und klicke auf das Symbol mit den drei Punkten (**...**) rechts neben dem Namen deines Boards (obere linke Ecke).
2. Navigiere zu **Board > Verschieben in > Anderes Team![moving-board-three-dots.png](../../../../../../docs/using-miro/managing-boards/images/21537437708306_moving-board-three-dots.png)**

### So verschiebst du Boards vom Dashboard aus

1. Auf deinem Dashboard siehst du alle Boards in einem Team.
2. Fahre mit dem Zeiger über die Karte des Boards, das du verschieben möchtest.
3. Klicke auf die drei Punkte und dann auf **Ins Team verschieben**.
   Ein Dialogfeld öffnet sich.
4. Wähle die Organisation, zu der du das Board verschieben möchtest.
5. Wähle ein Team in dieser Organisation.
6. Klicke auf **Verschieben**.

### Wie man ein Board in einen anderen Bereich verschiebt

1. Öffne dein Board und klicke auf das Symbol mit den drei Punkten (**...**) direkt rechts neben dem Namen deines Boards (linke obere Ecke)
2. Navigiere zu **Board > Verschieben in > Anderen Bereich.** Außerdem kannst du die Teammitglieder darüber informieren, dass das Board in einen anderen Bereich verschoben wurde.![moving-boards-spaces.png](../../../../../../docs/using-miro/managing-boards/images/21537453797394_moving-boards-spaces.png)*Ein Board in einen anderen Bereich verschieben*

### Nutzer hat keinen Zugriff mehr

Wenn Board-Mitwirkende nicht Teil des Teams sind, in das das Board verschoben wird, siehst du eine Nachricht mit „Zugriff verweigert“.

Es gibt zwei Möglichkeiten, zu sehen, welche E-Mail-Adressen von Nutzern nach dem Verschieben den Zugriff auf das Board verlieren. Bei weniger als 10 Nutzern kannst du die E-Mail-Liste aufrufen, indem du auf **Nutzer-E-Mails anzeigen** in der **Nachricht „Zugriff verweigert“** klickst. Wenn es mehr als 10 sind, kannst du die E-Mail-Liste über einen Link herunterladen.

Um sicherzustellen, dass alle Mitwirkenden weiterhin Zugang zum Board haben, kannst du [Mitglieder zum neuen Team einladen](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md), bevor du das Board verschiebst.

Du kannst auch **„Trotzdem verschieben“** wählen und die Mitwirkenden dem Board erneut hinzufügen, nachdem es verschoben wurde.

![warning when moving a board.png](../../../../../../docs/using-miro/managing-boards/images/16759524012690_warning%20when%20moving%20a%20board.png)
*Nachricht „Zugriff verweigert“, wenn ein Board von einem Team in ein anderes verschoben wird*

**Wenn du ein Board in ein Free-Team verschiebst**, wird es mit allen Teammitgliedern geteilt.

![private boards are not available in free teams.png](../../../../../../docs/using-miro/managing-boards/images/16759539790738_private%20boards%20are%20not%20available%20in%20free%20teams.png)
*Privat-Boards sind in freien Teams nicht verfügbar*

## Boards zwischen Profilen verschieben

Dein Profil in Miro ist die E-Mail-Adresse, mit der du dich registriert hast. Wenn du dich mit zwei verschiedenen E-Mail-Adressen registriert hast, hast du zwei Profile. Du kannst ein Board von einem Profil auf ein anderes übertragen.

### So verschiebst du Boards zwischen Profilen

Kostenpflichtige, Education-Pläne Free-Plan

Wenn sich das Board in einem kostenpflichtigen oder Education-Team befindet und du es in ein anderes kostenpflichtiges oder Education-Team verschieben möchtest, speichere einfach das Board-Backup und lade es in das jeweilige Team hoch.

1. Öffne dein Dashboard.
2. Fahre mit dem Zeiger über die Karte des Boards, das du verschieben möchtest.
3. Klicke auf die drei Punkte.
4. Klicke auf **Board-Backup herunterladen**.
5. Die .rtb-Datei wird auf deinem Gerät gespeichert.

   ![board-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136352530_board-backup.png)
6. Melde dich bei deinem zweiten Miro-Profil an.
7. Wechsle zu dem Team, in das du das Board verschieben möchtest.
8. Klicke auf **+ Neu erstellen** > **Importieren** > **Backup importieren**.
9. Der Datei-Picker öffnet sich.
10. Wähle die .rtb-Backup-Datei, die du zuvor gespeichert hast, und klicke auf **Öffnen**. Das Board wird dann in deinem Dashboard verfügbar sein.

    ![board-import-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136353682_board-import-backup.png)

Wenn dein Board sich in einem kostenlosen Team befindet oder du dein Board in ein Free-Team verschieben möchtest, führe die folgenden Schritte aus:

1. Melde dich bei deinem ersten Miro-Profil an.
2. Gib das Board für dein zweites Profil frei. Klicke auf **Teilen**.
   ![free-sharing-board.png](../../../../../../docs/using-miro/managing-boards/images/23122136354066_free-sharing-board.png)
3. Gib die E-Mail-Adresse für Profil #2 ein > klicke auf **Einladungen senden**.

   ![free-sharing-board-dialog.png](../../../../../../docs/using-miro/managing-boards/images/23122136354706_free-sharing-board-dialog.png)
4. Übertrage das Eigentum des Boards von Profil Nr. 1 zu Profil Nr. 2. Klicke auf die **Schaltfläche „Teilen“** > **Teilen-Einstellungen** > wähle Profil Nr. 2 > wähle im Dropdown-Menü **Eigentümer** aus.
5. Melde dich in Miro unter Profil Nr. 2 an. Dort siehst du nun das Board.
6. Verschiebe das Board in ein anderes Team.

:::warning
Wenn dein zweites Profil den Free-Preisplan verwendet und du dein kostenloses Profil zu einem kostenpflichtigen Profil einlädst, belegst du in deinem kostenpflichtigen Preisplan eine Lizenz. Wenn dadurch die Anzahl der Lizenzen in deinem Preisplan überschritten wird, wird dir möglicherweise eine zusätzliche Lizenz in Rechnung gestellt.
:::

## Häufig gestellte Fragen

**Warum sehe ich die Option, in ein Team zu verschieben, nicht auf meinem Board-Menü?**

Nur Board-Eigentümer, die Mitglieder mehrerer Teams sind, können Boards zwischen ihnen verschieben. Wenn du nicht der Board-Eigentümer bist, kannst du [das Board duplizieren](03-how-to-duplicate-a-board.md) (sofern dies in den [Inhaltseinstellungen des Boards](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md) erlaubt ist) und die Kopie des Boards verschieben.

Die Option zum Verschieben von Boards kann bei Enterprise-Preisplänen auch von Unternehmens-Admins eingeschränkt werden.

**Wie kann ich die Eigentümerschaft meines Boards an einen anderen Nutzer übertragen?**

Erfahre, wie du die [Eigentümerschaft des Boards an einen anderen Mitwirkenden übertragen](05-how-to-transfer-board-ownership.md) kannst.

**Ändert sich der Board-Link, wenn ich das Board in ein anderes Team verschiebe?**

Nein, die Board-URL ändert sich nicht.

**Kann ich ein Vorlagen-Board in das Team eines anderen Nutzers verschieben?**

Ja, du kannst entweder den Nutzer bitten, dich in sein Team einzuladen, und dann das Board verschieben, oder [das Board freigeben](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) und es ihnen erlauben, dein Board in den [Board-Inhaltseinstellungen](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md) zu [duplizieren](03-how-to-duplicate-a-board.md).

**Kann ich Bereiche zwischen Teams verschieben?**

Nein, du kannst nur separate Boards verschieben.

**Kann ich mehrere Boards auf einmal verschieben?**

Nein, das wird momentan nicht unterstützt.

**Wenn ich versuche, mein Board zu verschieben, passiert nichts oder es erscheint eine Fehlermeldung – was kann ich tun?**

Bitte versuche, das Board in einem anderen Browser oder im Inkognito-Modus zu verschieben. Du kannst auch versuchen, zu einem anderen Netzwerk oder Gerät zu wechseln.

Eine weitere Option ist, das [Board zu duplizieren](03-how-to-duplicate-a-board.md) und die Kopie zu verschieben. Wenn das nicht hilft, [berichte den Vorgang dem Miro Support](../tools/troubleshooting/06-contacting-miro-support.md).
