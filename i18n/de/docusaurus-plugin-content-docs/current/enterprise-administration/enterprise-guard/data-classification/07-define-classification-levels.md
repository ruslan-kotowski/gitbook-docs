---
title: Definiere Klassifizierungsstufen
article_id: 16494683650322
translation_id: 16494683650322
locale: de
sidebar_position: 6
created_at: '2024-01-19T18:57:35Z'
updated_at: '2025-11-25T15:40:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Dies ist der erste Schritt der automatischen Klassifizierung und der Konfiguration der Vorgaben. In diesem Schritt des Ablaufs kannst du Klassifizierungsstufen definieren, d.h. neue Klassifizierungsstufen hinzufügen oder die Konfiguration einer Klassifizierungsstufe aktualisieren, z.B. den Namen der Klassifizierung, die Reihenfolge der Sensibilisierung, die Farbe des Abzeichens, den Link zu den Klassifizierungsrichtlinien und mehr. Bei der Festlegung der Klassifizierungsstufen kannst du:

- [Hinzufügen oder Bearbeiten einer Klassifizierungsstufe](07-define-classification-levels.md)
- [Einrichtung der Klassifizierung von Daten durch den Import von Labels aus Microsoft Purview](07-define-classification-levels.md)
- [Aktualisiere die Standard Klassifizierungsstufe für neue Boards](07-define-classification-levels.md)
- [Aktualisiere die Reihenfolge der Empfindlichkeit einer Klassifizierungsstufe](07-define-classification-levels.md)
- [Eine Klassifizierungsstufe entfernen](07-define-classification-levels.md)

## Voraussetzungen

- Du musst die Details der Klassifizierungsstufen des Boards kennen, die du auf der Grundlage deiner Sicherheits- und Governance-Anforderungen konfigurieren möchtest.
- Du musst die [Rolle Admin für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Wenn du die Rolle des Admin für sensible Inhalte anfragen möchtest, wende dich an deinen Unternehmens-Admin.

## Hinzufügen oder Bearbeiten einer Klassifizierungsstufe

Du kannst eine Klassifizierungsstufe hinzufügen oder bearbeiten, indem du wie folgt vorgehst:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Fensterbereich unter **Enterprise Guard** auf **Datenklassifizierung**.
3. Wenn du die Klassifizierungsstufen zum ersten Mal festlegst, klicke unten auf dem Bildschirm auf **Klassifizierung einrichten** .
   Wenn du die Klassifizierungsstufen bearbeiten möchtest, klicke oben rechts auf **Klassifizierungsstufen bearbeiten**.
4. Auf der Seite **Klassifizierungsstufen definieren**:
   Um eine Klassifizierungsstufe hinzuzufügen, klicke auf **Stufe hinzufügen**.
   Um eine Klassifizierungsstufe zu bearbeiten, klicke auf **Klassifizierungsstufen bearbeiten**.
5. Füge die Klassifizierungsstufe entsprechend deinen Anforderungen hinzu oder bearbeite sie. In der folgenden Tabelle sind die einzelnen Felder und ihre Beschreibung aufgeführt.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | **Level** | Gibt die Board-Sensibilitätsreihenfolge für diese Klassifizierungsstufe an.  Derzeit gibt die Sensibilitätsstufe **1** die **am wenigsten sensible** Klassifizierungsstufe an.  Klicke auf die Pfeile nach oben oder unten, um die Reihenfolge der Boards für diese Klassifizierungsstufe festzulegen. |
   | **Name** | Name der Klassifizierungsstufe.  Wenn Nutzer ein Board ansehen, das zu dieser Klassifizierungsstufe gehört, erscheint dieser Name auf dem Abzeichen für die Klassifizierung des Boards neben dem Namen des Boards.  Abbildung 1 zeigt ein Beispiel, bei dem der Name der Klassifizierung des Boards **INTERNAL** lautet.  sample_board_internal.png Abbildung 1: Beispiel, bei dem der Name der Klassifizierung des Boards " **INTERN"** lautet |
   | **Beschreibung** | Beschreibung dieser Klassifizierungsstufe.  Wenn Nutzer ein Board ansehen, das zu dieser Klassifizierungsstufe gehört, und sie auf das Abzeichen für die Klassifizierung des Boards klicken, wird die Beschreibung der Klassifizierungsstufe angezeigt.  Wir empfehlen, dass du eine aussagekräftige Beschreibung hinzufügst, die deine Nutzer über die Empfindlichkeit dieses Boards und die empfohlenen Vorsichtsmaßnahmen oder Aktionen informiert.  Abbildung 2 zeigt ein Beispiel für die **Beschreibung**, die für die Klassifizierungsstufe INTERN hinzugefügt wurde.   sample_internal_description.png Abbildung 2: Beispiel für die **Beschreibung**, die für die Klassifizierungsstufe INTERN hinzugefügt wurde |
   | **Farbe des Abzeichens** | Hintergrundfarbe für das Abzeichen zur Klassifizierung des Boards.  Abbildung 3 zeigt ein Beispiel, in dem die Klassifizierungsstufe INTERNAL des Boards mit einem **gelben** Abzeichen gekennzeichnet ist.  sample_board_internal.png Abbildung 3: Beispiel, bei dem die Klassifizierungsstufe des Boards INTERN mit einem **gelben** Abzeichen gekennzeichnet ist |
   | **Link zu den Leitlinien** | URL, die weitere Informationen über Richtlinien oder Anweisungen enthält, die für diese Klassifizierungsstufe gelten. Dies könnte eine Seite sein, die den Nutzern in deiner Organisation mehr Informationen über die Klassifizierungsstufen deines Boards und die Arbeit mit ihnen bietet. Du musst die URL im folgenden Format angeben: `http://www.example.com`  Wenn der Nutzer auf das Symbol " **Mehr erfahren"** (Fragezeichen) neben dem Abzeichen für die Klassifizierung des Boards klickt, wird diese URL in einem neuen Tab des Browsers geladen. |
   | **Als Standardstufe für neue Boards verwenden** | Aktiviere dieses Kästchen, um diese Klassifizierungsstufe als Standardklassifizierung für alle neuen Boards festzulegen. |
   | **Vorschau** | Zeigt eine Vorschau des Abzeichens für die Klassifizierung des Boards mit seiner Beschreibung und dem Symbol "Mehr erfahren" an. Die Vorschau zeigt genau, wie das Abzeichen zur Klassifizierung für Nutzer auf einem Board aussieht. |

   Um die Konfiguration der Klassifizierungsstufe zu speichern, klicke auf " **Fertig"**.
6. Klicke auf **Weiter**. Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, wenn du auf der Seite **Veröffentlichen** [**Auswirkungen überprüfen**](https://help.miro.com/hc/articles/16494764223378) Seite klickst.

   Du kannst dann mit einem der folgenden nächsten Schritte fortfahren:

   - [Definiere die automatische Klassifizierung](09-define-auto-classification.md). Dies ist optional. Wenn du die automatische Klassifizierung zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Definiere Vorgaben](05-define-guardrails.md). Dies ist optional. Wenn du die Vorgaben zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Überprüfung der Auswirkungen](https://help.miro.com/hc/articles/16494764223378). Dies ist der letzte Schritt des Workflows und er ist obligatorisch.

## Einrichtung der Klassifizierung von Daten durch den Import von Labels aus Microsoft Purview

### Voraussetzungen

- Vergewissere dich, dass du die erforderlichen Rollen oder Berechtigungen hast, um mit Sensitivitäts-Labels in Microsoft Purview zu arbeiten.
- Du musst die Details der Klassifizierungsstufen des Boards kennen, die du auf der Grundlage deiner Sicherheits- und Governance-Anforderungen konfigurieren möchtest.
- Du musst die [Rolle Admin für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Wenn du die Rolle des Admin für sensible Inhalte anfragen möchtest, wende dich an deinen Unternehmens-Admin.

:::note
Anmerkungen:
- Laut Microsofts Dokumentation kann es bis zu 24 Stunden dauern, bis Aktualisierungen von Sensitivitätslabels in Microsoft Purview auf alle Apps und Dienste übertragen werden. Bitte lass dir genügend Zeit für die Änderungen und importiere dann die Sensitivitätslabels. Wenn die Aktualisierungen, die du in MS Purview vorgenommen hast, nach 24 Stunden nicht repliziert wurden, wende dich bitte an das Microsoft Purview Support Team.
- Du kannst bis zu 50 Sensitivitäts-Labels aus Microsoft Purview in Miro importieren.
- Wenn du bereits über eine Konfiguration zur Klassifizierung von Daten verfügst, kannst du Sensitivitäts-Labels aus Microsoft Purview importieren und bestehende Klassifizierungs-Labels in Miro übertragen. Weitere Informationen findest du unter [Importieren von Sensitivitäts-Labels aus Microsoft Purview in die bestehende Konfiguration der Datenklassifizierung in Miro](08-import-microsoft-purview-sensitivity-labels.md).
:::

Um sensible Labels aus Microsoft Purview zu importieren und die Datenklassifizierung in Miro einzurichten, gehe wie folgt vor:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Fensterbereich unter **Enterprise Guard** auf **Datenklassifizierung**.
3. Klicke auf der Seite **Klassifizierung** am unteren Rand des Bildschirms auf **Los geht's**.
4. Klicke im Feld **Aus Microsoft Purview importieren** auf **Anmelden**.
5. Gib auf der **Microsoft Anmeldeseite**, die in einem neuen Tab erscheint, deine Microsoft Anmeldeinformationen ein und melde dich an. Sobald du in deinem Microsoft Konto angemeldet bist, wird der Tab automatisch geschlossen,
6. Klicke auf der Seite **Klassifizierung** im Feld **Import aus Microsoft Purview** auf **Importieren**.
   Die Seite **Klassifizierung aus Microsoft Purview importieren** wird angezeigt.
7. Aktiviere das Kontrollkästchen für die Microsoft Purview Sensitivity Labels, die du als Klassifizierungsstufen in Miro verwenden möchtest, und klicke dann auf **Weiter**.
   > ✏️ Laut Microsofts Dokumentation kann es bis zu 24 Stunden dauern, bis Aktualisierungen von Sensitivitätslabels in Microsoft Purview auf alle Apps und Dienste übertragen werden. Bitte lass dir genügend Zeit für die Änderungen und importiere dann die Sensitivitätslabels. Wenn die Aktualisierungen, die du in MS Purview vorgenommen hast, nach 24 Stunden nicht repliziert wurden, wende dich bitte an das Microsoft Purview Support Team.
8. Auf der Seite **Klassifizierungsstufen definieren** kannst du die Klassifizierungsstufen bearbeiten, um die Standardklassifizierungsstufe zuzuweisen oder einen Link zu den Richtlinien hinzuzufügen. In der folgenden Tabelle sind die einzelnen Felder und ihre Beschreibung aufgeführt.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | **Link zu den Leitlinien** | URL, die weitere Informationen über Richtlinien oder Anweisungen enthält, die für diese Klassifizierungsstufe gelten. Dies könnte eine Seite sein, die den Nutzern in deiner Organisation mehr Informationen über die Klassifizierungsstufen deines Boards und die Arbeit mit ihnen bietet. Du musst die URL im folgenden Format angeben: `http://www.example.com`  Wenn der Nutzer auf das Symbol " **Mehr erfahren"** (Fragezeichen) neben dem Abzeichen für die Klassifizierung des Boards klickt, wird diese URL in einem neuen Tab des Browsers geladen. |
   | **Als Standardstufe für neue Boards verwenden** | Aktiviere dieses Kästchen, um diese Klassifizierungsstufe als Standardklassifizierung für alle neuen Boards festzulegen. |
   | **Vorschau** | Zeigt eine Vorschau des Abzeichens für die Klassifizierung des Boards mit seiner Beschreibung und dem Symbol "Mehr erfahren" an. Die Vorschau zeigt genau, wie das Abzeichen zur Klassifizierung für Nutzer auf einem Board aussieht. |

   Um die Konfiguration der Klassifizierungsstufe zu speichern, klicke auf " **Fertig"**.
9. Klicke auf **Weiter**. Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, wenn du auf der Seite **Veröffentlichen** [**Auswirkungen überprüfen**](https://help.miro.com/hc/articles/16494764223378) Seite klickst.

   Du kannst dann mit einem der folgenden nächsten Schritte fortfahren:

   - [Definiere die automatische Klassifizierung](09-define-auto-classification.md). Dies ist optional. Wenn du die automatische Klassifizierung zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Definiere Vorgaben](05-define-guardrails.md). Dies ist optional. Wenn du die Vorgaben zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Überprüfung der Auswirkungen](https://help.miro.com/hc/articles/16494764223378). Dies ist der letzte Schritt des Workflows und er ist obligatorisch.

## Aktualisiere die Standard Klassifizierungsstufe für neue Boards

Du kannst die standardmäßige Klassifizierungsstufe mit den folgenden Schritten aktualisieren:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Fensterbereich unter **Enterprise Guard** auf **Datenklassifizierung**.
3. Klicke auf **Klassifizierungsstufen bearbeiten** oben rechts im Bildschirm.
4. Klicke auf der Seite **Klassifizierungsstufen definieren** auf **Klassifizierungsstufen bearbeiten**.
5. Klicke auf das Symbol **Bearbeiten** (![Screenshot 2024-01-22 um 23.20.18.png](images/16548150428050_Screenshot%202024-01-22%20at%2023.20.18.png)) für die Stufe, die du als Standardklassifizierungsstufe festlegen möchtest.
6. Aktiviere das Kästchen **Als Standardstufe für neue Boards verwenden**.
7. Klicke auf **Fertig**.
   Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, wenn du auf der Seite **Veröffentlichen** [**Auswirkungen überprüfen**](https://help.miro.com/hc/articles/16494764223378) Seite klickst.
8. Klicke auf **Weiter**. Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, wenn du auf der Seite **Veröffentlichen** [**Auswirkungen überprüfen**](https://help.miro.com/hc/articles/16494764223378) Seite klickst.

   Du kannst dann mit einem der folgenden nächsten Schritte fortfahren:

   - [Definiere die automatische Klassifizierung](09-define-auto-classification.md). Dies ist optional. Wenn du die automatische Klassifizierung zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Definiere Vorgaben](05-define-guardrails.md). Dies ist optional. Wenn du die Vorgaben zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Überprüfung der Auswirkungen](https://help.miro.com/hc/articles/16494764223378). Dies ist der letzte Schritt des Workflows und er ist obligatorisch.

## Aktualisiere die Reihenfolge der Empfindlichkeit einer Klassifizierungsstufe

Du kannst die Sensibilitätsreihenfolge einer Klassifizierungsstufe aktualisieren, indem du wie folgt vorgehst:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Fensterbereich unter **Enterprise Guard** auf **Datenklassifizierung**.
3. Klicke auf **Klassifizierungsstufen bearbeiten** oben rechts im Bildschirm.
4. Klicke auf der Seite **Klassifizierungsstufen definieren** auf **Klassifizierungsstufen bearbeiten**.
5. Die Klassifizierungsstufen erscheinen in der Reihenfolge ihrer aktuellen Sensibilität. Klicke auf die Auf- oder Abwärtspfeile für die Klassifizierungsstufen, für die du die Sensibilitätsreihenfolge aktualisieren möchtest.

   > ✏️ Derzeit gibt die Sensibilitätsstufe **1** die **am wenigsten sensible** Klassifizierungsstufe an.

   Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, wenn du auf der Seite **Veröffentlichen** **[Auswirkungen überprüfen](https://help.miro.com/hc/articles/16494764223378)** Seite klickst.
6. Klicke auf **Weiter**. Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, wenn du auf der Seite **Veröffentlichen** [**Auswirkungen überprüfen**](https://help.miro.com/hc/articles/16494764223378) Seite klickst.

   Du kannst dann mit einem der folgenden nächsten Schritte fortfahren:

   - [Definiere die automatische Klassifizierung](09-define-auto-classification.md). Dies ist optional. Wenn du die automatische Klassifizierung zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Definiere Vorgaben](05-define-guardrails.md). Dies ist optional. Wenn du die Vorgaben zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Überprüfung der Auswirkungen](https://help.miro.com/hc/articles/16494764223378). Dies ist der letzte Schritt des Workflows und er ist obligatorisch.

## Eine Klassifizierungsstufe entfernen

:::note
Du kannst eine Klassifizierungsstufe nicht entfernen, wenn sie mit einer [Richtlinie zur Aufbewahrung](https://help.miro.com/hc/sections/19180529348754) verknüpft ist.
:::

Du kannst eine Klassifizierungsstufe mit den folgenden Schritten entfernen:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Fensterbereich unter **Enterprise Guard** auf **Datenklassifizierung**.
3. Klicke auf **Klassifizierungsstufen bearbeiten** oben rechts im Bildschirm.
4. Klicke auf der Seite **Klassifizierungsstufen definieren** auf **Klassifizierungsstufen bearbeiten**.
5. Klicke auf das Symbol zum Löschen der Klassifizierungsstufe, die du entfernen möchtest.
6. Wenn die Klassifizierungsstufe, die du löschen möchtest, bereits auf 1 oder mehrere Boards angewendet wurde, erscheint ein Benachrichtigungsfenster, das dich über die Anzahl der Boards informiert, auf die die Klassifizierungsstufe angewendet wurde.
   Wähle die neue Klassifizierungsstufe, die du für die betroffenen Boards anwenden möchtest.
7. Klicke auf **Fertig**.
   Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, wenn du auf der Seite **Veröffentlichen** [**Auswirkungen überprüfen**](https://help.miro.com/hc/articles/16494764223378) Seite klickst.
8. Klicke auf **Weiter**. Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, wenn du auf der Seite **Veröffentlichen** [**Auswirkungen überprüfen**](https://help.miro.com/hc/articles/16494764223378) Seite klickst.

   Du kannst dann mit einem der folgenden nächsten Schritte fortfahren:

   - [Definiere die automatische Klassifizierung](09-define-auto-classification.md). Dies ist optional. Wenn du die automatische Klassifizierung zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Definiere Vorgaben](05-define-guardrails.md). Dies ist optional. Wenn du die Vorgaben zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Überprüfung der Auswirkungen](https://help.miro.com/hc/articles/16494764223378). Dies ist der letzte Schritt des Workflows und er ist obligatorisch.
