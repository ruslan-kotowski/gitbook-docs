---
title: "Erstelle Labels und Suchbegriffe f\xFCr benutzerdefinierte, gesch\xE4ftskritische\
  \ Informationen"
article_id: 21626517022610
translation_id: 21626517022610
locale: de
sidebar_position: 11
created_at: '2024-09-26T21:36:45Z'
updated_at: '2026-03-04T22:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Du kannst Labels erstellen, um Dinge wie Suchbegriffe oder Widgets zu definieren, die du auf deinen Miro-Boards identifizieren und finden möchtest. Du kannst bis zu 100 benutzerdefinierte geschäftskritische Labels erstellen. Gehe wie folgt vor, um ein Label zu erstellen:

:::note
Um benutzerdefinierte Labels zu erstellen, musst du die [Rolle des Admins für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Die Rolle des Admins für sensible Inhalte kannst du bei deinem Unternehmens-Admin anfordern.
:::

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Bereich unter **Enterprise Guard** auf **Datenerkennung**.
3. Auf der Seite **Datenerkennung** klicke auf den Tab **Konfiguration**.
4. Im Abschnitt **Benutzerdefiniert geschäftskritisch** klicke auf die Schaltfläche **Erstellen**.
5. Auf der Seite **Eigenes Label definieren** kannst du die Label-Details hinzufügen.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | **Labelname** | **Maximale Länge:** 80 Zeichen  Beschreibender Name für das benutzerdefinierte Label. Du kannst einen unternehmensinternen Projektnamen verwenden, da dieses Label nicht in den Protokollen angezeigt wird.  **Hinweis:** Der Labelname ist in den Audit-Protokollen nicht sichtbar. Wenn du die mit diesem Label verbundenen Audit-Protokolle suchen/anzeigen möchtest, kannst du die Label-ID verwenden. |
   | **Kurzname** | **Maximale Länge:** 10 Zeichen, alphanumerisch  Kurzversion des Labelnamens. Der Kurzname wird verwendet, um in der Datenerkennung, der Inhaltssuche und der Datenklassifizierung auf dieses bestimmte Label zu verweisen. **Hinweis:** Der Kurzname ist in Audit-Protokollen nicht sichtbar. Wenn du die mit diesem Label verbundenen Audit-Protokolle suchen/anzeigen möchtest, kannst du die Label-ID verwenden. |
   | **Beschreibung** | **Maximale Länge:** 500 Zeichen  Beschreibung der Informationen, die dieses Label ermittelt. Diese Informationen sind für andere Admins nützlich. |
   | **Bedingungen** | Füge Schlüsselwörter und Widget-Typen hinzu, die du erkennen möchtest und denen dieses Label bei Erkennung auf einem Miro-Board hinzugefügt werden soll. Du musst mindestens eine Bedingung hinzufügen.  Wenn du nur Schlüsselwörter hinzufügst und kein Widget-Kästchen aktivierst, erkennt die Datenerkennung alle Boards, die genaue Übereinstimmungen mit den von dir angegebenen Schlüsselwörtern für alle unterstützten Widgets enthalten. Die aktuelle Version unterstützt die folgenden Board-Elemente für die Schlüsselworterkennung: Notiz, Karte, Jira-Karte, Codeblock, Kommentare, Rahmen, Tabelle, Verbindungslinie/Linie, Form, Textblock, Kanban-Board, User Story Map.  Du kannst auch auswählen, dass nur Codeblocks, Jira-Karten, Azure-Karten oder Prototyping-Bildschirme erkannt werden sollen, ohne Schlüsselwörter hinzuzufügen. Die Datenerkennung erkennt dann alle Boards, die diese Widgets enthalten.  Wenn du sowohl Suchbegriffe als auch Widgets als Bedingungen hinzufügst, erkennt die Datenerkennung das Board nur, wenn sowohl die Schlüsselwort- als auch die Widget-Kriterien erfüllt sind. So kannst du die Suche verfeinern und Boards mit benutzerdefinierten Labels präziser anvisieren.  **Beispiele:**  - Wenn du die Board-Erkennung eingrenzen möchtest, damit speziell produktentwicklungsbezogene Boards erkannt werden, aber keine marketingbezogenen Boards, und wenn das Board außerdem den Projektnamen *Enterprise* *Guard* enthalten muss und du nur die Boards finden möchtest, die auch eine Jira-Karte enthalten (da es sich um eine Produktentwicklung handelt), dann konfiguriere dieses Label so, dass es den Suchbegriff *Enterprise* *Guard* enthält und aktiviere das Kästchen für die Jira-Karte. Die Datenerkennung findet dann Boards, die den Suchbegriff Enterprise Guard und eine Jira-Karte enthalten. Die Datenerkennung findet auch Boards, die Jira-Karten mit dem Suchbegriff Enterprise Guard im Titel oder in der Beschreibung enthalten. Wenn ein Board nur den Suchbegriff *Enterprise* *Guard* enthält, aber keine Jira-Karte, wird das Board nicht erkannt, da es nicht beide angegebenen Bedingungen erfüllt.  - Wenn du alle Boards mit dem Wort *Enterprise* *Guard* für alle unterstützten Widget-Typen erkennen möchtest, und zwar unabhängig davon, welche Widget-Typen das Board enthält, dann füge im Abschnitt **Suchbegriffe hinzufügen** den Suchbegriff **Enterprise** **Guard** hinzu. Du brauchst für dieses Beispiel keinen Widget-Typen hinzuzufügen.  - Wenn du alle Boards mit Jira-Karten unabhängig von bestimmten Inhalten erkennen möchtest, aktiviere im Abschnitt **Widget-Typ hinzufügen** das Kästchen für die **Jira-Karte**. Du brauchst für dieses Beispiel keinen Suchbegriff hinzuzufügen.    **So fügst du einen Suchbegriff hinzu:**  1. Klicke auf **Suchbegriffe hinzufügen**.  2. Gib Suchbegriffe über die Tastatur ein oder kopiere sie und trenne sie dabei mit Kommas. **Hinweise:**  - Suchbegriffe unterstützen alphanumerische und Unicode-Zeichen. - Du kannst bis zu 100 Suchbegriffe oder Phrasen hinzufügen. - Alle führenden und nachfolgenden Leerzeichen werden in Suchbegriffen ignoriert. - Die Datenerkennung erkennt genaue Übereinstimmungen für die eingegebenen Suchbegriffe, ohne auf Groß- und Kleinschreibung zu achten. - Wenn du vor einem Suchbegriff ein Leerzeichen hinzufügst, findet die Datenerkennung exakte Übereinstimmungen, die auch ein Leerzeichen vor dem Suchbegriff haben. - Die aktuelle Version unterstützt die folgenden Board-Elemente bei der Erkennung von Suchbegriffen: Notiz, Karte, Jira-Karte, Codeblock, Rahmen, Tabelle, Konnektor/Linie, Form, Textblock, Kanban-Board, User Story Map. Merkzettel und Kommentare werden derzeit bei Scans der Datenerkennung nicht einbezogen. Wir arbeiten daran, bei künftigen Versionen mit Funktionserweiterungen Merkzettel und Kommentare einzubeziehen.  **Beispiel:** Um Boards mit den Suchbegriffen *vertraulich* oder *intern* zu identifizieren und zu kennzeichnen, füge die folgenden Suchbegriffe hinzu: *vertraulich, intern* (setze dabei zwischen den Suchbegriffen ein Komma). Die Datenerkennung findet dann alle Boards, die einen dieser Suchbegriffe enthalten.  **So fügst du einen Widget-Typ hinzu:**  1. Klicke auf **Widget-Typ hinzufügen**.  2. Wähle das Kästchen für den Widget-Typ aus, den du auf Miro-Boards erkennen möchtest.  **Beispiel:** Wenn du Boards, die eine Jira-Karte enthalten, erkennen und mit Labels kennzeichnen möchtest, aktiviere das Kästchen für die **Jira-Karte**. |
6. Klicke auf **Weiter**.
7. Überprüfe die Details des benutzerdefinierten Labels.

   Wenn du die Details zum eigenen Label bearbeiten möchtest, klicke auf die **Zurück**-Schaltfläche.

   Wenn die Details zum eigenen Label korrekt sind, klicke auf die **Eigenes Label erstellen**-Schaltfläche.

   Sobald du das Label erstellt hast, startet der erste Scan automatisch. Die Ergebnisse, die mit den ausgewählten Bedingungen übereinstimmen, sind nach ein paar Minuten oder Stunden verfügbar, je nachdem, wie viele Miro-Boards deine Organisation hat.
