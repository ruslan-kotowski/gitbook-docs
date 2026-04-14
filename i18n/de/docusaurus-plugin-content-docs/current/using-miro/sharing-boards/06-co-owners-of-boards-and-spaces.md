---
title: Miteigentümer von Boards und Bereichen
article_id: 360021580759
translation_id: 360021580759
locale: de
sidebar_position: 6
created_at: '2021-05-12T07:36:28Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
availability:
  notes: 'Verfügbar für: Board-Eigentümer, Board-Miteigentümer, Space-Eigentümer,
    Space-Miteigentümer, Team-Admins, Unternehmens-Admins Preispläne: Business, Enterprise
    Plattformen: Browser, Desktop, Mobile'
---

Die Rolle des Miteigentümers verbessert die Zusammenarbeit, indem sie es Board-Eigentümern erlaubt, Verantwortlichkeiten für die Vorbereitung und Moderation der Arbeit an einem Board zu delegieren, sei es für Live- oder asynchrone Sitzungen.

Ein Miteigentümer sorgt für einen nahtlosen Arbeitsablauf, selbst wenn der ursprüngliche Board-Eigentümer nicht verfügbar ist, da Miteigentümer nahezu alle Eigentümeraktionen ausführen können, von der Verwaltung der Board-Einstellungen bis zur Kontrolle der Inhaltsansicht. Ein Mitinhaber hilft, die Arbeitslast zu verteilen und bietet eine zuverlässige Unterstützung für das Board-Management.

Um zu erfahren, welche Berechtigungen ein Miteigentümer für ein Board oder einen Bereich hat, siehe Referenz für Miteigentümer.

## Rolle des Miteigentümers für die Organisation aktivieren

Als Unternehmensadministrator befolge diese Schritte:

1. Klicke in deinem Miro-Dashboard rechts oben auf deinen Avatar und auf **Admin-Konsole**.
2. Gehe zu **Sicherheit** > **Freigabe** > **Rollen und Berechtigungen**.
3. Schalte **Miteigentümer-Rolle zulassen** ein.

Admins können jetzt die Rolle des Miteigentümers für ihre Teams aktivieren.

## Aktiviere die Rolle des Miteigentümers für ein Team

Als Unternehmens-Admin oder Team-Admin befolgst du diese Schritte:

1. Klicke auf deinem Miro-Dashboard auf deinen Avatar oben rechts und dann auf **Admin-Konsole** | **Einstellungen**.
2. Gehe zu **Teams**> **\{team name\}** > **Einstellungen**.
3. Unter **Zusammenarbeitseinstellungen** aktiviere **Miteigentümerrolle in Boards und Spaces aktivieren**.

## Miteigentümer zu Boards hinzufügen

Befolge diese Schritte, wenn du Inhaber oder bestehender Mitinhaber eines Boards bist:

1. Von deinem Miro-Dashboard aus, mache einen der folgenden Schritte:
   1. Um ein Board zu bearbeiten, klicke auf die drei Punkte (**...**) und dann auf **Freigeben**.
   2. Öffne ein Board und klicke dann in der oberen rechten Ecke auf **Freigeben**.
2. Gib die E-Mail-Adresse des Nutzers bzw. der Nutzer ein, die du als Mitbesitzer hinzufügen möchtest.
3. Für ihre Zugriffsrechte klicke auf **Ist Mitbesitzer**.
4. (Optional) Füge eine eigene Nachricht hinzu.
5. Klicke auf **Einladungen senden**.

:::note
Du kannst die Rolle des Miteigentümers nur Teammitgliedern zuweisen. Um einen Co-Eigentümer von außerhalb des Teams hinzuzufügen, lade ihn zunächst ein, dem Team beizutreten.
:::

## Miteigentümer zu Spaces hinzufügen

Als Besitzer eines Space oder als bestehender Mitbesitzer, befolge diese Schritte:

1. In deinem Miro-Dashboard mach einen der folgenden Schritte:
   1. Für einen Bereich in der Seitenleiste, klicke auf die drei Punkte (**...**) und dann auf **Teilen**.
   2. Öffne einen Space und klicke dann auf das Etikett oben, das die Anzahl der Mitglieder anzeigt.
2. Klicke auf **Zugriff verwalten**.
3. Für ein Space-Mitglied die Zugriffsrechte auf **Co-Owner** aktualisieren.

> Du kannst die Rolle des Miteigentümers nur Mitgliedern des Bereichs zuweisen. Um einen Miteigentümer von außerhalb des Bereichs hinzuzufügen, lade ihn zunächst ein, dem Bereich beizutreten.

> Ein Bereichs-Miteigentümer hat Bearbeitungsrechte für alle Inhalte innerhalb des Bereichs.

## Miteigentümer-Referenz

### Berechtigungen für Board-Miteigentümer

Zusätzlich zu allen Bearbeitungsberechtigungen hat ein Miteigentümer eines Boards die folgenden Berechtigungen:

- **Board-Inhaltseinstellungen und Einstellungen für Zusammenarbeits-Tools verwalten**
  Steuern Sie, wer Board-Inhalte kopieren kann und verwalten Sie Tools wie den Timer, Abstimmungen, Videochat, Bildschirmfreigabe und Aufmerksamkeitssteuerung.
- **Rahmen ausblenden und einblenden**
  Steuere die Sichtbarkeit von Rahmeninhalten während Präsentationen oder Workshops.
- **Geschützte Sperre hinzufügen**
  Verhindere die versehentliche Verschiebung oder Löschung von Inhalten während der Zusammenarbeit.
- **Board-Passwort hinzufügen**
  Öffentliche Boards sichern, indem für den Zugriff ein Kennwort erforderlich ist.
- **Ein Board-Backup herunterladen**
  Archivierte Kopien von Boards erstellen. Miteigentümer können ebenfalls Boards aus Backups wiederherstellen.
- **Miteigentümer hinzufügen**
  Anderen Benutzern Co-Owner-Status zuweisen.
- **Board-Details ändern**
  Cover ändern und das Board umbenennen
- **Teile das Board**
  Zugriffsrechte für das Team und andere Nutzer auf dem Board ändern
- **Erweiterte Berechtigungen zur Freigabe des Boards konfigurieren**
  Gib an, ob das Board außerhalb des Teams oder der Organisation geteilt werden kann

:::note
In Enterprise-Preisplänen können Board-Miteigentümer und Inhalts-Admins Boards über die [Miro REST API](https://developers.miro.com/reference/update-board) verschieben, was sich bewusst von der Miro UI-Erfahrung unterscheidet, bei der nur Eigentümer ihre Boards verschieben können.
:::

Ein Board-Mitbesitzer kann die folgenden Aktionen nicht ausführen:

- Das Board löschen
- Verschiebe das Board in ein anderes Team
- Ändere den Board-Eigentümer

### Co-Eigentümerberechtigungen für Spaces

Zusätzlich zu allen Bearbeitungsberechtigungen hat ein Miteigentümer eines Bereichs die folgenden Berechtigungen:

- Bereich umbenennen
- Teile den Bereich
- Zugriffsrechte für das Team und andere Nutzer im Space ändern
- Miteigentümer zum Space hinzufügen

Ein Space-Miteigentümer kann die folgenden Aktionen nicht durchführen:

- Den Bereich löschen
- Bereichseigentümer ändern

## Häufig gestellte Fragen

**Ich habe nicht die Möglichkeit, einen Miteigentümer zu bestimmen. Warum?**

Die Co-Owner-Funktion ist in den Business- und Enterprise-Preisplänen verfügbar. Dein Unternehmens-Admin muss diese Funktion in den Team- oder Unternehmenseinstellungen aktivieren. Nur vorhandene Teammitglieder können zu Miteigentümern befördert werden. Stelle sicher, dass der Nutzer per E-Mail zum Board eingeladen wurde, bevor du versuchst, die Rolle des Miteigentümers zuzuweisen.

**Ich bin ein Admin mit aktivierten Berechtigungen für die Verwaltung von Inhalten. Warum kann ich keine Board-Miteigentümer hinzufügen?**

Admins mit Berechtigungen für die Verwaltung von Inhalten (CAP) müssen sich zuerst als Eigentümer zu dem spezifischen Board hinzufügen. Sobald sie Eigentümer eines Boards sind, können sie Miteigentümer bestimmen.

**Soll ich zusätzlich für Miteigentümer zahlen, die zu meinen Boards eingeladen werden?**

Nur bestehende Teammitglieder können als Miteigentümer benannt werden. Wenn der Benutzer, den du als Mitinhaber hinzufügen möchtest, noch nicht zu deinem Team gehört, musst du ihn zuerst in das Team einladen. Dies kann je nach deinem Plan und aktueller Benutzeranzahl den Kauf eines zusätzlichen Sitzplatzes erfordern. Nachdem sie ein Teammitglied sind, kannst du ihnen die Rolle des Miteigentümers zuweisen.
