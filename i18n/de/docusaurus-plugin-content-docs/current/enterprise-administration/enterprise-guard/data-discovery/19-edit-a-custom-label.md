---
title: Ein benutzerdefiniertes Label bearbeiten
article_id: 21690361870354
translation_id: 21690361870354
locale: de
sidebar_position: 18
created_at: '2024-09-30T13:43:27Z'
updated_at: '2026-03-04T23:02:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

:::note
Wir empfehlen, Labels nur zu bearbeiten, bevor du sie mit einer Klassifizierungsstufe verbindest.
:::

Bearbeite Labels, um Bedingungen wie Suchbegriffe oder Widgets zu aktualisieren, die du identifizieren und auf Miro-Boards finden möchtest. Um ein Label zu bearbeiten, führe die folgenden Schritte aus:

:::note
Um benutzerdefinierte Labels zu bearbeiten, musst du die [Rolle des Admins für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Um die Rolle des Admins für sensible Inhalte zu beantragen, wende dich an deinen Unternehmens-Admin.
:::

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Bereich unter **Enterprise Guard** auf **Datenerkennung**.
3. Klicke auf der **Übersicht** der **Datenerkennung**-Seite auf die Ellipse (drei Punkte) in der Zeile des Labels, das du bearbeiten möchtest, und klicke dann auf **Label bearbeiten**.
4. Auf der Seite **Benutzerdefiniertes Label bearbeiten** bearbeite die Details des Labels.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | **Labelname** | **Maximale Länge:** 80 Zeichen  Beschreibender Name für das benutzerdefinierte Label. Du kannst einen unternehmensinternen Projektnamen verwenden, da dieses Label nicht in den Protokollen angezeigt wird.  **Hinweis:** Der Labelname ist in Audit-Protokollen nicht sichtbar. Wenn du die mit diesem Label verbundenen Audit-Protokolle suchen/anzeigen möchtest, kannst du die Label-ID verwenden. |
   | **Kurzname** | **Maximale Länge:** 10 Zeichen, alphanumerisch  Kurzversion des Labelnamens. Der Kurzname wird in der Datenerkennung und der Inhaltssuche zur Bezugnahme auf dieses benutzerdefinierte Label verwendet. **Note:** Der Kurzname ist in Audit-Protokollen nicht sichtbar. Wenn du die mit diesem Label verbundenen Audit-Protokolle suchen/anzeigen möchtest, kannst du die Label-ID verwenden. |
   | **Beschreibung** | **Maximale Länge:** 500 Zeichen  Beschreibung der Informationen, die dieses Label ermittelt. Diese Informationen sind für andere Admins nützlich. |
   | **Bedingungen** | Füge Suchbegriffe und Widget-Typen hinzu, die du erkennen möchtest und denen dieses Label hinzugefügt werden soll, wenn sie auf einem Miro-Board erkannt werden. Du musst mindestens eine Bedingung hinzufügen.  Wenn du nur Suchbegriffe hinzufügst und kein Widget-Kästchen aktivierst, erkennt die Datenerkennung alle Boards, die genaue Übereinstimmungen mit den Schlüsselwörtern enthalten, die du für alle unterstützten Widgets angegeben hast. Die aktuelle Version unterstützt die folgenden Board-Elemente zur Schlüsselworterkennung: Notiz, Karte, Jira-Karte, Codeblock, Kommentar, Rahmen, Tabelle, Verbindungslinie/Linie, Form, Textblock, Kanban-Board, User Story Map.  Du kannst auch auswählen, dass nur Codeblocks, Jira-Karten, Azure-Karten oder Prototyping-Screens erkannt werden sollen, ohne Suchbegriffe hinzuzufügen. Die Datenerkennung erkennt dann alle Boards, die diese Widgets enthalten.  Wenn du sowohl Suchbegriffe als auch Widgets als Bedingungen hinzufügst, erkennt die Datenerkennung das Board nur, wenn sowohl die Schlüsselwort- als auch die Widget-Kriterien erfüllt sind. So kannst du die Suche verfeinern und Boards mit benutzerdefinierten Labels präziser anvisieren.  **Beispiele:**  - Wenn du die Board-Erkennung eingrenzen möchtest, um speziell produktentwicklungsbezogene Boards zu erkennen, aber keine marketingbezogenen Boards, und wenn das Board außerdem den Projektnamen *Enterprise* *Guard* enthalten muss und du nur die Boards finden möchtest, die auch eine Jira-Karte enthalten (da es sich um eine Produktentwicklung handelt), dann konfiguriere dieses Label so, dass es das Schlüsselwort *Enterprise* *Guard* enthält und aktiviere das Kästchen für die Jira-Karte. Die Datenerkennung findet dann Boards, die das Schlüsselwort Enterprise Guard und eine Jira-Karte enthalten. Die Datenerkennung findet auch Boards, die Jira-Karten mit dem Schlüsselwort Enterprise Guard im Titel oder in der Beschreibung enthalten. Wenn ein Board nur das Schlüsselwort *Enterprise* *Guard* enthält, aber keine Jira-Karte, wird das Board nicht erkannt, da es nicht beide angegebenen Bedingungen erfüllt.  - Wenn du alle Boards mit dem Wort *Enterprise* *Guard* für alle unterstützten Widget-Typen erkennen möchtest, unabhängig davon, welche Widget-Typen das Board enthält, dann füge im Abschnitt **Suchbegriffe hinzufügen** den Suchbegriff **Enterprise** **Guard** hinzu. Du brauchst für dieses Beispiel keinen Widget-Typen hinzuzufügen.  - Wenn du alle Boards mit Jira-Karten unabhängig von bestimmten Inhalten erkennen möchtest, aktiviere im Abschnitt **Widget-Typ hinzufügen** das Kästchen für die **Jira-Karte**. Du brauchst für dieses Beispiel keinen Suchbegriff hinzuzufügen.    **So fügst du einen Suchbegriff hinzu:**  1. Klicke auf **Suchbegriffe hinzufügen**.  2. Gib Suchbegriffe ein oder kopiere sie und trenne sie dabei mit Kommas. **Hinweise:**  - Suchbegriffe unterstützen alphanumerische und Unicode-Zeichen.  - Du kannst bis zu 100 Suchbegriffe oder Phrasen hinzufügen. - Die Datenerkennung erkennt genaue Übereinstimmungen für die eingegebenen Suchbegriffe und achtet dabei nicht auf Groß- und Kleinschreibung. - Die aktuelle Version unterstützt die folgenden Board-Elemente bei der Erkennung von Suchbegriffen: Notiz, Karte, Jira-Karte, Codeblock, Rahmen, Tabelle, Konnektor/Linie, Form, Textblock, Kanban-Board, User Story Map. Merkzettel und Kommentare werden derzeit bei der Datenerkennung nicht gescannt. Wir arbeiten daran, bei künftigen Versionen mit Funktionserweiterungen die Merkzettel und Kommentare einzubeziehen.  **Beispiel:** Um Boards mit den Suchbegriffen *vertraulich* oder *intern* zu identifizieren und zu kennzeichnen, füge die folgenden Suchbegriffe hinzu: *vertraulich, intern* (setze dabei zwischen den Suchbegriffen ein Komma). Die Datenerkennung findet dann alle Boards, die einen dieser Suchbegriffe enthalten.  **So fügst du einen Widget-Typ hinzu:**  1. Klicke auf **Widget-Typ hinzufügen**.  2. Wähle das Kästchen für den Widget-Typ aus, den du auf Miro-Boards erkennen möchtest.  **Beispiel:** Wenn du Boards, die eine Jira-Karte enthalten, erkennen und mit Labels kennzeichnen möchtest, wähle das Kästchen für die **Jira-Karte** aus. |
5. Klicke auf **Weiter**.
6. Überprüfe die Details des benutzerdefinierten Labels.

   Wenn du die Details des benutzerdefinierten Labels aktualisieren möchtest, klicke auf die **Zurück** Schaltfläche.

   Wenn die Details des benutzerdefinierten Labels korrekt sind, klicke auf die **Benutzerdefiniertes Label aktualisieren** Schaltfläche.

   Sobald du das benutzerdefinierte Label aktualisiert hast, startet der Scan automatisch. Die Ergebnisse, die mit den ausgewählten Bedingungen übereinstimmen, sind nach ein paar Minuten oder Stunden verfügbar, je nachdem, wie viele Miro-Boards deine Organisation hat.
