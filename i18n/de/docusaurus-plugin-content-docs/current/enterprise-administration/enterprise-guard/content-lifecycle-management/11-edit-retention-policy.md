---
title: Aufbewahrungsrichtlinie bearbeiten
article_id: 19205184829330
translation_id: 19205184829330
locale: de
sidebar_position: 11
created_at: '2024-05-28T18:01:39Z'
updated_at: '2025-12-08T16:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Um Aufbewahrungsrichtlinien zu bearbeiten, musst du die [Rolle Datenverwaltungs-Admin](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Um die Rolle Datenverwaltungs-Admin anzufordern, wende dich an deinen Unternehmens-Admin.
:::

Um eine Aufbewahrungsrichtlinie zu bearbeiten, führe die folgenden Schritte aus:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Bereich unter **Enterprise Guard,** auf **Content Lifecycle**.
3. Klicke auf den **Aufbewahrung**-Tab.
4. Auf der Seite **Aufbewahrungsrichtlinien** klicke auf die Aufbewahrungsrichtlinie, die du bearbeiten möchtest.
   Die Seite mit Informationen zur Richtlinie wird angezeigt.
5. Klicke rechts oben auf **Bearbeiten** und bearbeite dann das erforderliche Feld. Die einzelnen Felder und ihre Beschreibungen findest du in der nachstehenden Tabelle.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | **Name**  **(erforderlich)** | Name der Aufbewahrungsrichtlinie.  Maximale Länge: 60 Zeichen. |
   | **Beschreibung**  **(optional)** | Beschreibung dieser Aufbewahrungsrichtlinie.  Maximale Länge: 300 Zeichen. |
   | **Aufbewahrungszeitraum**  **(erforderlich)** | Verhindere, dass Boards für einen bestimmten Zeitraum dauerhaft gelöscht werden, basierend auf einem der folgenden Kriterien: **Letzter Zugriff**, **Letzte Änderung** oder **Erstellt am**. Wähle eine Anzahl, wähle **Monate** oder **Jahre** und dann das Ereignis, von dem die Aufbewahrungsfrist berechnet wird.  Wenn du die Aufbewahrungsfrist in Monaten angibst, muss sie zwischen 1 und 120 Monaten liegen.  Wenn du die Aufbewahrungsfrist in Jahren angibst, muss sie zwischen 1 und 10 Jahren liegen. |
   | **Geltungsbereich**  **(erforderlich)** | Wähle den Geltungsbereich für diese Aufbewahrungsrichtlinie aus. Der Geltungsbereich gibt die Boards an, für die diese Aufbewahrungsrichtlinie gilt. Du kannst den Geltungsbereich einer Aufbewahrungsrichtlinie für alle Boards in einer Organisation oder für bestimmte Board-Klassifizierungsstufen festlegen.  **Aufbewahrungsrichtlinie für alle Boards in der Organisation festlegen** Wenn du den Geltungsbereich der Aufbewahrungsrichtlinie für alle Boards in der Organisation festlegen möchtest, wähle in der **Geltungsbereich**-Liste **Alle Boards in der Organisation** aus.  **Aufbewahrungsrichtlinie für ein oder mehrere Teams in der Organisation festlegen** Wenn du den Geltungsbereich der Aufbewahrungsrichtlinie für ein oder mehrere Teams in der Organisation festlegen möchtest, führe die folgenden Schritte aus:  1. Wähle in der **Reichweite**-Liste **Team** aus. 2. Klicke auf das Eingabefeld für das Team und wähle jedes Team aus, für das du die Aufbewahrungsrichtlinie anwenden möchtest. Ein Häkchen erscheint neben dem Team, das du mit der Aufbewahrungsrichtlinie verbinden möchtest.   ✏️ - Du kannst mehrere Teams für eine Aufbewahrungsrichtlinie auswählen. Jedes Team kann jedoch nur mit einer Aufbewahrungsrichtlinie verknüpft werden. - Du kannst jedes Team, einschließlich gelöschter Teams, als Geltungsbereich bei der Festlegung der Aufbewahrungsrichtlinie auswählen.   - Ein Team, das als Geltungsbereich für eine Aufbewahrungsrichtlinie ausgewählt wurde, kann nicht dauerhaft gelöscht werden, solange es noch im Geltungsbereich ist.  **Setze die Aufbewahrungsrichtlinie für eine Board-Klassifizierungsstufe**  ✏️ Um den Geltungsbereich der Aufbewahrungsrichtlinie auf eine bestimmte Board-Klassifizierungsstufe festzulegen, musst du sicherstellen, dass die „Datenklassifizierung“-Funktion aktiviert ist. Sobald für eine Aufbewahrungsrichtlinie eine Board-Klassifizierungsstufe gilt, kannst du die Datenklassifizierungsfunktion nicht mehr deaktivieren. Weitere Informationen findest du in der Dokumentation zur [Datenklassifizierung](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Wenn du den Geltungsbereich der Aufbewahrungsrichtlinie für eine bestimmte Board-Klassifizierungsstufe festlegen möchtest, gehe wie folgt vor:  1. Wähle in der **Bereich**-Liste die Option **Klassifizierung** aus. 2. Klicke auf die Liste neben der **Klassifizierung**-Liste und wähle dann die Klassifizierungsstufen aus, für die du die Aufbewahrungsrichtlinie anwenden möchtest. Du kannst auch nach den Klassifizierungsstufen suchen und diese dann auswählen.  Ein Häkchen erscheint neben den Klassifizierungsstufen, die mit der Aufbewahrungsrichtlinie verbunden sind.  ✏️ **Notizen:** - Du kannst mehrere Klassifizierungsstufen gleichzeitig auswählen. - Du kannst nicht dieselbe Klassifizierungsstufe für verschiedene Aufbewahrungsrichtlinien festlegen. Wenn eine bestimmte Klassifizierungsstufe bereits mit einer Aufbewahrungsrichtlinie verknüpft ist, erscheint die Klassifizierungsstufe ausgegraut.  - Sobald eine Aufbewahrungsrichtlinie eine Board-Klassifizierungsstufe verwendet, kannst du die Datenklassifizierungsfunktion nicht deaktivieren.  -Sobald eine Klassifizierungsstufe mit einer Aufbewahrungsrichtlinie verknüpft ist, kannst du diese bestimmte Klassifizierungsstufe nicht löschen. - Wenn ein Board sowohl durch "Alle Boards im Geltungsbereich der Organisation" als auch durch eine Aufbewahrungsrichtlinie im Klassifizierungsgeltungsbereich gesteuert wird, gilt die Richtlinie mit der längeren Aufbewahrungsfrist. |
6. Wenn du fertig bist, klicke auf **Weiter**.
   Die Seite **Auswirkungen überprüfen** wird angezeigt.
7. Sieh dir die Auswirkungen der Aufbewahrungsrichtlinie an. Die Seite mit den Auswirkungen enthält die folgenden Informationen:
   - **Zusammenfassung:** Konfiguration der Aufbewahrungsrichtlinie, z. B. der Name der Richtlinie, die Aufbewahrungsfrist und der Geltungsbereich.
   - **Auswirkung der Richtlinie:** Anzahl der Boards, für die diese Richtlinie gilt. Die Aufbewahrungsrichtlinie gilt auch für Boards im Papierkorb, und diese sind in der Berechnung der Auswirkungen enthalten.

   > ✏️ Wenn ein Board sowohl einer zeitbasierten als auch einer klassifizierungsbasierten Aufbewahrungsrichtlinie unterliegt, gilt die Richtlinie mit der längeren Aufbewahrungsfrist.
8. Um die Konfiguration zu speichern und die Aufbewahrungsrichtlinie anzuwenden, klicke auf **Veröffentlichen**.

:::note
Das Erstellen, Aktualisieren oder Löschen einer Richtlinie löst den Aufbewahrungsrichtlinien-Prozess aus, der bis zu 24 Stunden dauern kann. Die Aktualisierung des Namens oder der Beschreibung einer Richtlinie erfolgt jedoch sofort, da diese Aktionen den Aufbewahrungsrichtlinien-Prozess nicht auslösen.
:::
