---
title: "Aufbewahrungsrichtlinie hinzuf\xFCgen"
article_id: 19205113739282
translation_id: 19205113739282
locale: de
sidebar_position: 10
created_at: '2024-05-28T18:00:55Z'
updated_at: '2025-12-08T16:05:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Um Aufbewahrungsrichtlinien hinzuzufügen, musst du die [Rolle des Datenverwaltungs-Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Um die Rolle des Datenverwaltungs-Admins zu beantragen, wende dich an deinen Unternehmens-Admin.
:::

Um eine Aufbewahrungsrichtlinie hinzuzufügen, gehe wie folgt vor:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Bereich unter **Enterprise Guard** auf **Content Lifecycle**.
3. Klicke auf den **Aufbewahrung**-Tab.
   Die Seite für **Aufbewahrungsrichtlinien** erscheint.
4. Klicke auf **Aufbewahrungsrichtlinie hinzufügen**.
   Die Seite **Kriterien definieren** erscheint.
5. Füge die entsprechenden Informationen für jedes Feld hinzu oder wähle sie aus. Die einzelnen Felder und ihre Beschreibungen findest du in der nachstehenden Tabelle.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | **Name**  **(erforderlich)** | Name der Aufbewahrungsrichtlinie.  Maximale Länge: 60 Zeichen. |
   | **Beschreibung**  **(optional)** | Beschreibung dieser Aufbewahrungsrichtlinie.  Maximale Länge: 300 Zeichen. |
   | **Aufbewahrungsfrist**  **(erforderlich)** | Verhindere, dass Boards dauerhaft gelöscht werden, indem du für einen bestimmten Zeitraum anhand eines der folgenden Kriterien auswählst: **Letzter Zugriff**, **Zuletzt geändert** oder **Erstellungsdatum**. Wähle eine Zahl, entscheide dich für **Monate** oder **Jahre** und gib dann an, von welchem Ereignis die Aufbewahrungsfrist berechnet wird.  Wenn du die Aufbewahrungsfrist in Monaten angeben möchtest, muss diese zwischen 1 und 120 Monaten liegen.  Wenn du die Aufbewahrungsfrist in Jahren angeben möchtest, muss diese zwischen 1 und 10 Jahren liegen. |
   | **Geltungsbereich**  **(erforderlich)** | Wähle den Geltungsbereich für diese Aufbewahrungsrichtlinie aus. Der Geltungsbereich gibt die Boards an, für die diese Aufbewahrungsrichtlinie gilt. Du kannst den Geltungsbereich einer Aufbewahrungsrichtlinie für alle Boards in einer Organisation oder für bestimmte Klassifizierungsstufen von Boards festlegen.  **Gesetz die Aufbewahrungsrichtlinie für alle Boards in der Organisation** Wenn du den Geltungsbereich der Aufbewahrungsrichtlinie für alle Boards in der Organisation festlegen möchtest, wähle in der **Geltungsbereich**-Liste **Alle Boards in der Organisation** aus.  **Setze die Aufbewahrungsrichtlinie für ein oder mehrere Teams in der Organisation** Falls du den Geltungsbereich der Aufbewahrungsrichtlinie für ein oder mehrere Teams in der Organisation festlegen willst, führe folgende Schritte aus:  1. Wähle in der **Scope**-Liste die Option **Team** aus. 2. Klicke auf das Feld „Team eingeben“ und wähle jedes Team aus, für das du die Aufbewahrungsregel anwenden möchtest. Ein Häkchen erscheint neben dem Team, das du mit der Aufbewahrungsregel verknüpfen möchtest.   ✏️ - Du kannst mehrere Teams für eine Aufbewahrungsrichtlinie auswählen. Allerdings kann ein bestimmtes Team jeweils nur mit einer Aufbewahrungsrichtlinie verbunden werden.  - Du kannst jedes Team, einschließlich gelöschter Teams, als Geltungsbereich beim Festlegen der Aufbewahrungsrichtlinie auswählen.   - Ein Team, das als Geltungsbereich für eine Aufbewahrungsrichtlinie ausgewählt wurde, kann nicht dauerhaft gelöscht werden, bis das Team aus dem Geltungsbereich entfernt wurde.  **Festlegen der Aufbewahrungsrichtlinie für eine Board-Klassifizierungsstufe**  ✏️ Um den Geltungsbereich der Aufbewahrungsrichtlinie für eine bestimmte Board-Klassifizierungsstufe festzulegen, musst du sicherstellen, dass die Datenklassifizierungsfunktion aktiviert ist. Sobald eine Aufbewahrungsrichtlinie eine Board-Klassifizierungsstufe verwendet, kannst du die Datenklassifizierungsfunktion nicht deaktivieren. Weitere Informationen findest du in der Dokumentation zur [Datenklassifizierung](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Wenn du den Geltungsbereich der Aufbewahrungsrichtlinie für eine bestimmte Board-Klassifizierungsstufe festlegen möchtest, gehe wie folgt vor:  1. Wähle in der **Bereich**-Liste **Klassifizierung** aus. 2. Klicke auf die Liste neben der **Klassifizierung**-Liste und wähle dann die Klassifizierungsstufen aus, auf die du die Aufbewahrungsrichtlinie anwenden möchtest. Du kannst auch nach den Klassifizierungsstufen suchen und dann die gewünschten auswählen.  Neben den Klassifizierungsstufen, die du mit der Aufbewahrungsrichtlinie verknüpfen möchtest, wird ein Häkchen angezeigt.  ✏️ **Hinweise:** - Du kannst mehrere Klassifizierungsstufen gleichzeitig auswählen. - Du kannst nicht dieselbe Klassifizierungsstufe für verschiedene Aufbewahrungsrichtlinien festlegen. Wenn eine bestimmte Klassifizierungsstufe bereits mit einer Aufbewahrungsrichtlinie verknüpft ist, erscheint die Klassifizierungsstufe ausgegraut.  - Sobald eine Aufbewahrungsrichtlinie eine Board-Klassifizierungsstufe verwendet, kannst du die Datenklassifizierungsfunktion nicht deaktivieren.  - Sobald eine Klassifizierungsstufe mit einer Aufbewahrungsrichtlinie verknüpft ist, kannst du diese Klassifizierungsstufe nicht mehr löschen. - Wenn für ein Board sowohl die Richtlinien zur Aufbewahrung für alle Boards im Geltungsbereich der Organisation als auch für den Geltungsbereich der Klassifizierung gelten, ist die Richtlinie mit der längeren Aufbewahrungsfrist anwendbar. |
6. Klicke auf **Weiter**.
   Die Seite **Auswirkung überprüfen** wird angezeigt.
7. Sieh dir die Auswirkungen der Aufbewahrungsrichtlinie an. Die Seite mit den Auswirkungen enthält die folgenden Informationen:
   - **Zusammenfassung:** Konfiguration der Aufbewahrungsrichtlinie, z. B. der Name der Richtlinie, die Aufbewahrungsfrist und der Geltungsbereich.
   - **Auswirkung der Richtlinie:** Anzahl der Boards, für die diese Richtlinie gilt. Die Aufbewahrungsrichtlinie gilt auch für Boards im Papierkorb, und diese sind in der Berechnung der Auswirkungen enthalten.

   > ✏️ Wenn ein Board sowohl einer zeitbasierten als auch einer klassifizierungsbasierten Aufbewahrungsrichtlinie unterliegt, gilt die Richtlinie mit der längeren Aufbewahrungsfrist.
8. Um die Konfiguration zu speichern und die Aufbewahrungsrichtlinie anzuwenden, klicke auf **Veröffentlichen**.

:::note
Das Erstellen, Aktualisieren oder Löschen einer Richtlinie löst den Aufbewahrungsrichtlinien-Prozess aus. Dieser Vorgang kann bis zu 24 Stunden in Anspruch nehmen. Die Aktualisierung des Namens oder der Beschreibung einer Richtlinie erfolgt jedoch sofort, da diese Aktionen den Prozess der Aufbewahrungsrichtlinien nicht auslösen.
:::

#
