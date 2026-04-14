---
title: "L\xF6schungsrichtlinie bearbeiten"
article_id: 19551033354002
translation_id: 19551033354002
locale: de
sidebar_position: 18
created_at: '2024-06-14T19:50:51Z'
updated_at: '2025-12-08T16:14:46Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Um Löschungsrichtlinien zu bearbeiten, musst du die [Rolle des Datenverwaltungs-Admins](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Um die Rolle des Datenverwaltungs-Admins zu beantragen, wende dich an deinen Unternehmens-Admin.
:::

Um eine Löschungsrichtlinie zu bearbeiten, führe die folgenden Schritte aus:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Bereich unter **Enterprise Guard** auf **Content Lifecycle**.
3. Klicke auf den **Löschungs**-Tab.
   Die Seite **Löschungsrichtlinien** wird angezeigt.
4. Klicke auf der Seite **Löschungsrichtlinien** auf die Löschungsrichtlinie, die du bearbeiten möchtest.
   Die Seite mit Informationen zur Richtlinie wird angezeigt.
5. Klicke rechts oben auf **Bearbeiten** und bearbeite dann die erforderlichen Felder. Die einzelnen Felder und ihre Beschreibungen findest du in der nachstehenden Tabelle.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | **Name**  **(erforderlich)** | Name der Löschungsrichtlinie.  Maximale Länge: 60 Zeichen. |
   | **Beschreibung**  **(optional)** | Beschreibung dieser Löschungsrichtlinie.  Maximale Länge: 300 Zeichen. |
   | **Löschungszeitraum**  **(erforderlich)** | Gib an, wann Boards automatisch in den Papierkorb verschoben werden sollen. Wähle eine Zahl, dann **Monate** oder **Jahre** und entscheide, ob der Zeitraum ab dem **letzten Änderungsdatum** des Boards oder ab dem **letzten Zugriffsdatum** berechnet wird.  Wenn du den Löschungszeitraum in Monaten angibst, musst du einen Zeitraum zwischen 1 und 120 Monaten auswählen.  Wenn du den Löschungszeitraum in Jahren angibst, musst du einen Zeitraum zwischen 1 und 10 Jahren wählen.  Wenn du Boards nach einem Jahr ohne Bearbeitung in den Papierkorb verschieben möchtest, kannst du 1 Jahr auswählen und **Zuletzt bearbeitet** wählen. |
   | **Geltungsbereich**  **(erforderlich)** | Wähle den Geltungsbereich für diese Löschungsrichtlinie. Der Umfang zeigt die Boards an, für die diese Löschungsrichtlinie gilt. Du kannst den Geltungsbereich einer Löschungsrichtlinie für alle Boards in einer Organisation oder für bestimmte Board-Klassifizierungsstufen festlegen.  **Löschungsrichtlinie für alle Boards in der Organisation festlegen** Wenn du den Geltungsbereich der Löschungsrichtlinie für alle Boards in der Organisation festlegen möchtest, wähle in der Liste **Geltungsbereich** **Alle Boards in der Organisation** aus.  **Lege die Löschrichtlinie für ein oder mehrere Teams in der Organisation fest** Wenn du den Geltungsbereich der Löschrichtlinie für ein oder mehrere Teams in der Organisation festlegen möchtest, führe die folgenden Schritte aus:  1. Wähle in der **Bereichsliste** **Team** aus. 2. Klicke auf das **Team eingeben**-Feld und wähle jedes Team aus, für das du die Löschungsrichtlinie anwenden möchtest. Ein Häkchen erscheint neben dem Team, das du ausgewählt hast, um es mit der Löschungsrichtlinie zu verknüpfen.   ✏️ - Du kannst mehrere Teams für eine Löschung-Richtlinie auswählen. Allerdings kann ein bestimmtes Team immer nur mit einer Löschung-Richtlinie verknüpft sein.  - Du kannst jedes Team, einschließlich gelöschter Teams, als Geltungsbereich beim Festlegen der Löschung-Richtlinie auswählen.   - Ein Team, das als Geltungsbereich für eine Löschung-Richtlinie ausgewählt wurde, kann nicht dauerhaft gelöscht werden, bis das Team aus dem Geltungsbereich entfernt wurde.  **Festlegen der Löschrichtlinie für eine Board-Klassifizierungsstufe**  ✏️ Um den Geltungsbereich der Löschungsrichtlinie auf eine bestimmte Board-Klassifizierungsstufe festzulegen, musst du sicherstellen, dass die Datenklassifizierungsfunktion aktiviert ist. Sobald eine Löschungsrichtlinie eine Board-Klassifizierungsstufe verwendet, kannst du die Datenklassifizierungsfunktion nicht deaktivieren. Weitere Informationen findest du in der Dokumentation zur [Datenklassifizierung](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Wenn du den Geltungsbereich der Löschungsrichtlinie für eine bestimmte Board-Klassifizierungsstufe festlegen möchtest, führe folgende Schritte aus:  1. Wähle in der **Liste** **Klassifizierung** aus. 2. Klicke auf die Liste neben der **Klassifizierung** und wähle dann die Klassifizierungsstufen aus, für die du die Löschungsrichtlinie anwenden möchtest. Du kannst auch nach den Klassifizierungsstufen suchen und diese dann auswählen.  Neben den Klassifizierungsstufen, die du für die Löschungsrichtlinie ausgewählt hast, erscheint ein Häkchen.  ✏️ **Hinweise:** - Du kannst mehrere Klassifizierungsstufen gleichzeitig auswählen. - Du kannst nicht dieselbe Klassifizierungsstufe für verschiedene Löschungsrichtlinien festlegen. Wenn eine bestimmte Klassifizierungsstufe bereits einer Löschungsrichtlinie zugeordnet ist, wird die Klassifizierungsstufe ausgegraut. - Sobald eine Löschungsrichtlinie eine Board-Klassifizierungsstufe verwendet, kannst du die Datenklassifizierungsfunktion nicht deaktivieren. - Sobald eine Klassifizierungsstufe mit einer Löschungsrichtlinie verknüpft ist, kannst du diese bestimmte Klassifizierungsstufe nicht löschen. - Wenn ein Board sowohl den Löschungsrichtlinien für alle Boards im Organisationsbereich als auch den Klassifizierungsbereichsrichtlinien unterliegt, gilt die Richtlinie mit der längeren Löschungsfrist. |
6. Klicke auf **Weiter**.
   Die **Seite "Auswirkung überprüfen"** erscheint.
7. Sieh dir die Auswirkungen der Löschungsrichtlinie an. Die Seite mit den Auswirkungen enthält die folgenden Informationen:
   - **Zusammenfassung:** Konfiguration der Löschungsrichtlinie, u.a. Name der Richtlinie, Löschungszeitraum und Geltungsbereich.
   - **Auswirkung der Richtlinie:** Anzahl der Boards, für die diese Richtlinie gilt.
8. Um die Konfiguration zu speichern und die Löschungsrichtlinie anzuwenden, klicke auf **Veröffentlichen**.
   Wenn du keine Löschungsmitteilungen aktiviert hast, erscheint das **Dialogfeld Löschungsmitteilung aktivieren**.
9. **Löschungsbenachrichtigungen** ermöglichen es Nutzern, Vorwarnungen zu erhalten, bevor ein Board aufgrund von Inaktivität automatisch in den Papierkorb verschoben wird. Diese Benachrichtigungen helfen Nutzern, Maßnahmen zu ergreifen, wenn sie ihre Inhalte behalten möchten.

   Wenn du Löschungsbenachrichtigungen aktivieren möchtest:

   a. Klicke auf **Benachrichtigen**.

   b. Konfiguriere, wie viele Tage im Voraus die Benachrichtigung gesendet werden soll – jeder Wert zwischen **1 und 30 Tagen**.

   Wenn das Aktivieren der Benachrichtigungen dazu führt, dass **einige Boards sofort in den Papierkorb verschoben werden** (da sie bereits die Schwelle überschritten haben), wirst du gefragt, ob du die Nutzer über diese spezifischen Boards benachrichtigen möchtest. Du hast folgende Auswahlmöglichkeiten:

   - **Ja** – um die Eigentümer und Miteigentümer der Boards zu benachrichtigen, auch wenn das Board sofort in den Papierkorb verschoben wird.

   - **Nein** – um die Boards zu verschieben, ohne eine Benachrichtigung über diese sofortige Aktion zu senden.

   Sobald sie aktiviert sind, werden Nutzer mit Boards im Geltungsbereich jeder Löschrichtlinie, bei der Benachrichtigungen aktiviert sind:

   - Eine Benachrichtigung in ihrem Miro **Feed** während des konfigurierten Inspektionsfensters erhalten.

   - Direkt aus der Benachrichtigung auf das Board zugreifen können.

   - Sie sehen ein **Banner** auf dem Board, das vor dem bevorstehenden automatischen Verschieben in den Papierkorb warnt, mit der Option **Board behalten**, wenn sie es behalten möchten.

:::note
Mit dem Erstellen, Aktualisieren oder Löschen einer Richtlinie löst du den Prozess der Löschungsrichtlinien aus. Dieser Vorgang kann bis zu 24 Stunden in Anspruch nehmen. Die Aktualisierung des Namens oder der Beschreibung einer Richtlinie erfolgt jedoch sofort, denn dies löst keinen Prozess der Löschungsrichtlinien aus.
:::

#
