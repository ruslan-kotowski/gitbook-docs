---
title: "L\xF6schungsrichtlinie hinzuf\xFCgen"
article_id: 19551031552018
translation_id: 19551031552018
locale: de
sidebar_position: 17
created_at: '2024-06-14T19:49:31Z'
updated_at: '2025-12-08T16:13:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Um Löschungsrichtlinien hinzuzufügen, musst du die [Rolle des Datenverwaltungs-Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) besitzen. Um die Rolle des Datenverwaltungs-Admins zu beantragen, wende dich an deinen Unternehmens-Admin.
:::

Um eine Löschungsrichtlinie hinzuzufügen, führe die folgenden Schritte aus:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Bereich unter **Enterprise Guard** auf **Content Lifecycle**.
3. Klicke auf den **Tab Löschung**.
   Die Seite **Löschungsrichtlinien** wird angezeigt.
4. Klicke auf **Löschungsrichtlinie hinzufügen**.
5. Füge für jedes Feld die entsprechenden Informationen hinzu bzw. wähle sie aus. Die einzelnen Felder und ihre Beschreibungen findest du in der nachstehenden Tabelle.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | **Name**  **(erforderlich)** | Name der Löschungsrichtlinie.  Maximale Länge: 60 Zeichen. |
   | **Beschreibung**  **(optional)** | Beschreibung dieser Löschungsrichtlinie.  Maximale Länge: 300 Zeichen. |
   | **Löschungszeitraum**  **(erforderlich)** | Gib an, wann Boards automatisch in den Papierkorb verschoben werden sollen. Wähle eine Zahl, wähle **Monate** oder **Jahre** und entscheide dann, ob der Zeitraum ab dem Datum der **letzten Änderung** oder **letzten Nutzung** des Boards berechnet wird.  Wenn du den Löschungszeitraum in Monaten angibst, musst du einen Löschungszeitraum zwischen 1 und 120 Monaten auswählen.  Wenn du den Löschungszeitraum in Jahren angibst, musst du einen Löschungszeitraum zwischen 1 und 10 Jahren auswählen.  Zum Beispiel, wenn du möchtest, dass Boards in den Papierkorb verschoben werden, wenn sie ein Jahr lang nicht geändert wurden, kannst du 1 Jahr auswählen und **Zuletzt geändert** wählen. |
   | **Geltungsbereich**  **(erforderlich)** | Wähle den Geltungsbereich für diese Löschungsrichtlinie aus. Der Geltungsbereich gibt die Boards an, für die diese Löschungsrichtlinie gilt. Du kannst den Geltungsbereich einer Löschungsrichtlinie für alle Boards in einer Organisation oder für bestimmte Board-Klassifizierungsstufen festlegen.  **Lege die Löschungsrichtlinie für alle Boards in der Organisation fest** Wenn du den Geltungsbereich der Löschungsrichtlinie für alle Boards in der Organisation festlegen möchtest, wähle in der **Geltungsbereich**-Liste **Alle Boards in der Organisation** aus.  **Löschrichtlinie für ein oder mehrere Teams in der Organisation festlegen** Wenn du den Geltungsbereich der Löschrichtlinie für ein oder mehrere Teams in der Organisation festlegen möchtest, führe die folgenden Schritte aus:  1. Wähle in der **Bereich**-Liste **Team** aus. 2. Klicke in das Feld **Team eingeben** und wähle jedes Team aus, für das du die Löschrichtlinie anwenden möchtest. Ein Häkchen erscheint neben dem Team, das du mit der Löschrichtlinie verknüpfen möchtest.   ✏️ - Du kannst mehrere Teams für eine Löschungsrichtlinie auswählen. Allerdings kann ein Team jeweils nur mit einer Löschungsrichtlinie verknüpft sein.  - Du kannst jedes Team, einschließlich gelöschter Teams, als Geltungsbereich festlegen, wenn du die Löschungsrichtlinie einstellst.   - Ein Team, das als Geltungsbereich für eine Löschungsrichtlinie ausgewählt ist, kann nicht dauerhaft gelöscht werden, bis es aus dem Geltungsbereich entfernt wird.  **Lege die Löschrichtlinie für eine Board-Klassifizierungsstufe fest**  ✏️ Um den Geltungsbereich der Löschungsrichtlinie auf eine bestimmte Board-Klassifizierungsstufe festzulegen, musst du sicherstellen, dass die Datenklassifizierungsfunktion aktiviert ist. Sobald eine Löschungsrichtlinie eine Board-Klassifizierungsstufe verwendet, kannst du die Datenklassifizierungsfunktion nicht deaktivieren. Weitere Informationen findest du in der Dokumentation zur [Datenklassifizierung](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Wenn du den Geltungsbereich der Löschungsrichtlinie für eine bestimmte Board-Klassifizierungsstufe festlegen möchtest, führe folgende Schritte aus:  1. Wähle in der **Umfang**-Liste die Option **Klassifizierung** aus. 2. Klicke auf die Liste neben der **Klassifizierung**-Liste und wähle dann die Klassifizierungsstufen aus, für die du die Löschungsrichtlinie anwenden möchtest. Du kannst auch nach den Klassifizierungsstufen suchen und dann die Klassifizierungsstufen auswählen.  Neben den Klassifizierungsstufen, die du für die Löschungsrichtlinie ausgewählt hast, wird ein Häkchen angezeigt.  ✏️ **Hinweise:** - Du kannst mehrere Klassifizierungsstufen gleichzeitig auswählen. - Du kannst nicht dieselbe Klassifizierungsstufe für verschiedene Löschungsrichtlinien festlegen. Wenn eine bestimmte Klassifizierungsstufe bereits einer Löschungsrichtlinie zugeordnet ist, wird die Klassifizierungsstufe ausgegraut.  - Sobald eine Löschungsrichtlinie eine Board-Klassifizierungsstufe verwendet, kannst du die Datenklassifizierungsfunktion nicht deaktivieren.  -Sobald eine Klassifizierungsstufe mit einer Löschungsrichtlinie verknüpft ist, kannst du diese bestimmte Klassifizierungsstufe nicht löschen. - Wenn ein Board sowohl allen Boards im Organisationsbereich als auch den Löschungsrichtlinien im Klassifizierungsbereich unterliegt, gilt die Richtlinie mit der längeren Löschungsfrist. |
6. Klicke auf **Weiter**.
   Die **Impact-Überprüfungsseite** wird angezeigt.
7. Sieh dir die Auswirkungen der Löschungsrichtlinie an. Die Seite mit den Auswirkungen enthält die folgenden Informationen:
   - **Zusammenfassung:** Konfiguration der Löschungsrichtlinie, u. a. Name der Richtlinie, Löschungszeitraum und Geltungsbereich.
   - **Auswirkung der Richtlinie:** Anzahl der Boards, für die diese Richtlinie gilt.
8. Um die Konfiguration zu speichern und die Löschungsrichtlinie anzuwenden, klicke auf **Veröffentlichen**.
   Das **Dialogfeld „Löschungsbenachrichtigungen einschalten“** erscheint.
9. **Löschungsbenachrichtigungen** ermöglichen es Nutzern, Vorab-Hinweise zu erhalten, bevor ein Board aufgrund von Inaktivität automatisch in den Papierkorb verschoben wird. Diese Benachrichtigungen helfen Nutzern, Maßnahmen zu ergreifen, wenn sie ihre Inhalte behalten möchten.

   Wenn du Löschungsbenachrichtigungen aktivieren möchtest:

   a. Klicke auf **Benachrichtigen**.

   b. Konfiguriere, wie viele Tage im Voraus die Benachrichtigung gesendet werden soll – ein beliebiger Wert zwischen **1 und 30 Tagen**.

   Falls durch das Aktivieren von Benachrichtigungen **einige Boards sofort in den Papierkorb verschoben werden** würden (weil sie bereits die Schwelle überschritten haben), wirst du gefragt, ob Nutzer über diese spezifischen Boards benachrichtigt werden sollen. Du kannst wählen:

   - **Ja** – um die Eigentümer und Miteigentümer der Boards zu benachrichtigen, auch wenn die Boards sofort in den Papierkorb verschoben werden.

   - **Nein** – um die Boards ohne Benachrichtigung über diese Sofortmaßnahme zu verschieben.

   Einmal aktiviert, werden Nutzer mit Boards im Geltungsbereich einer Löschungsrichtlinie mit aktivierten Benachrichtigungen:

   - Während des konfigurierten Prüfzeitraums eine Benachrichtigung in ihrem Miro **Feed** erhalten.

   - In der Lage sein, das Board direkt aus der Benachrichtigung zu öffnen.

   - Ein **Banner** auf dem Board sehen, das vor der bevorstehenden automatischen Verschiebung in den Papierkorb warnt, mit der Option **Board behalten**, wenn sie es behalten möchten.

:::note
Mit dem Erstellen, Aktualisieren oder Löschen einer Richtlinie löst du den Prozess der Löschungsrichtlinien aus, der bis zu 24 Stunden dauern kann. Die Aktualisierung des Namens oder der Beschreibung einer Richtlinie erfolgt jedoch sofort, da diese Aktionen keinen Löschungsrichtlinienprozess auslösen.
:::

#
