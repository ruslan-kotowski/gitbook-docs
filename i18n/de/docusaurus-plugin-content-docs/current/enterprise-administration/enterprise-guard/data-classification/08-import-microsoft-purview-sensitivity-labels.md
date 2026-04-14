---
title: "Sensibilit\xE4tslabel aus Microsoft Purview importieren"
article_id: 22161930709010
translation_id: 22161930709010
locale: de
sidebar_position: 7
created_at: '2024-10-23T15:05:49Z'
updated_at: '2025-12-01T16:32:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Für Organisationen, die Microsoft Purview nutzen, ist es entscheidend, eine konsistente Datensicherheit und Klassifizierung über mehrere Plattformen hinweg zu gewährleisten. Die Integration von Miro mit Microsoft Purview ermöglicht es Administratoren, Sensibilitätslabels direkt von Microsoft Purview in Miro zu importieren, wodurch das Management von Klassifizierungsschemata auf beiden Plattformen vereinfacht wird.

Durch die Nutzung dieser Integration können Organisationen sicherstellen, dass Inhalte in Miro konsistent mit dem etablierten Microsoft Purview-Framework klassifiziert sind. Dies reduziert nicht nur den betrieblichen Aufwand für die manuelle Neuerstellung oder Aktualisierung von Klassifizierungslabels, sondern stärkt auch die Datensicherheit. Indem Miro's Datenschutzfunktionen mit Microsoft Purview in Einklang gebracht werden, können Admins sensible Informationen im gesamten digitalen Ökosystem ihres Unternehmens sicher verwalten.

## Microsoft Purview-Sensibilitätslabel in Miro importieren

Wenn dein Unternehmen noch keine Datenklassifizierung in Miro eingerichtet hat, kannst du ganz einfach eine Datenklassifizierung in Miro einrichten, indem du vorhandene Sensibilitätslabel direkt aus Microsoft Purview importierst.

Falls du bereits eine Datenklassifizierungskonfiguration hast, kannst du Sensibilitätslabel aus Microsoft Purview importieren und bestehende Klassifikationslabel in Miro übertragen.

## Richte die Datenklassifizierung ein, indem du Sensibilitätslabel von Microsoft Purview importierst

### Voraussetzungen

- Stelle sicher, dass du die notwendigen Rollen oder Berechtigungen hast, um mit Sensibilitätslabels in Microsoft Purview zu arbeiten.
- Du musst die Details der Board-Klassifizierungsstufen kennen, die du basierend auf deinen Sicherheits- und Governance-Anforderungen konfigurieren möchtest.
- Du musst die [Admin-Rolle für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Um die Admin-Rolle für sensible Inhalte zu beantragen, wende dich an deinen Unternehmens-Admin.

:::note
Hinweise:
- Laut Microsoft-Dokumentation können Aktualisierungen von Sensibilitätslabels in Microsoft Purview bis zu 24 Stunden dauern, um in allen Apps und Diensten repliziert zu werden. Bitte erlaube genügend Zeit, damit die Änderungen wirksam werden, bevor du die Sensibilitätslabels importierst. Falls die von dir vorgenommenen Änderungen in MS Purview nach 24 Stunden nicht repliziert wurden, kontaktiere bitte das Microsoft Purview Support-Team.
- Du kannst bis zu 50 Sensibilitätslabels von Microsoft Purview in Miro importieren.
- Wenn du bereits eine bestehende Datenklassifizierungskonfiguration hast, kannst du Sensibilitätslabels aus Microsoft Purview importieren und bestehende Klassifikationslabels in Miro übertragen. Weitere Informationen findest du unter [Import von Sensibilitätslabels aus Microsoft Purview in eine bestehende Datenklassifizierungskonfiguration in Miro](08-import-microsoft-purview-sensitivity-labels.md).
:::

Um Sensibilitätslabels aus Microsoft Purview zu importieren und die Datenklassifizierung in Miro einzurichten, führe die folgenden Schritte aus:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Bereich unter **Enterprise Guard** auf **Datenklassifizierung**.
3. Klicke auf der **Klassifizierungsseite** am unteren Ende des Bildschirms auf **Erste Schritte**.
4. Klicke im Feld **Import aus Microsoft Purview** auf **Anmelden**.
5. Auf der Seite **Microsoft-Anmeldung**, die in einem neuen Tab erscheint, gib deine Microsoft-Anmeldeinformationen ein und melde dich an. Sobald du bei deinem Microsoft-Konto angemeldet bist, wird der Tab automatisch geschlossen.
6. Auf der Seite **Klassifizierung**, in der Box **Import von Microsoft Purview**, klicke auf **Importieren**.
   Die Seite **Klassifizierung aus Microsoft Purview importieren** erscheint.
7. Wähle die Microsoft Purview Sensibilitätslabel aus, die du als Klassifizierungsstufen in Miro verwenden möchtest, und klicke dann auf **Weiter**.

   > ✏️ Laut der Dokumentation von Microsoft können Aktualisierungen von Sensibilitätslabeln in Microsoft Purview bis zu 24 Stunden benötigen, um in allen Apps und Diensten übernommen zu werden. Bitte gewährleiste genügend Zeit für Änderungen und importiere dann die Sensibilitätslabel. Wenn die Aktualisierungen, die du in Microsoft Purview vorgenommen hast, nach 24 Stunden nicht übernommen sind, wende dich bitte an den Microsoft Purview Support.
8. Auf der Seite **Klassifizierungsstufen definieren** kannst du die Klassifizierungsstufen bearbeiten, um die Standardklassifizierungsstufe zuzuweisen oder einen Link zu den Richtlinien hinzuzufügen. Die einzelnen Felder und ihre Beschreibungen findest du in der nachstehenden Tabelle.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | **Link zu den Richtlinien** | URL, die weitere Informationen über Richtlinien oder Anweisungen bereitstellt, die für diese Klassifizierungsstufe gelten. Dies könnte eine Seite sein, die Nutzern in deiner Organisation mehr Informationen über Klassifizierungsstufen für Boards bietet und wie man mit ihnen arbeitet. Du musst die URL in folgendem Format angeben: `http://www.example.com`  Wenn der Nutzer auf das **Mehr erfahren**-Symbol (Fragezeichensymbol) neben dem Klassifizierungsabzeichen des Boards klickt, wird diese URL in einem neuen Browser-Tab geladen. |
   | **Als Standardstufe für neue Boards verwenden** | Wähle dieses Kästchen, um diese Klassifizierungsstufe als Standardklassifizierung für alle neuen Boards festzulegen. |
   | **Vorschau** | Zeigt eine Vorschau des Board-Klassifizierungsabzeichens mit seiner Beschreibung und dem "Mehr erfahren"-Symbol. Die Vorschau zeigt genau, wie das Klassifizierungsabzeichen für Nutzer auf einem Board erscheint. |
9. Um die Klassifizierungsstufe zu speichern, klicke auf **Fertig**.
10. Klicke auf **Weiter**. Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, nachdem du auf der Seite [**Einfluss überprüfen**](https://help.miro.com/hc/articles/16494764223378) auf **Veröffentlichen** geklickt hast.

    Du kannst dann mit einem der folgenden nächsten Schritte fortfahren:

    - [Automatische Klassifizierung festlegen](09-define-auto-classification.md). Dies ist optional. Wenn du die automatische Klassifizierung zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
    - [Vorgaben definieren](05-define-guardrails.md). Sie ist optional. Wenn du die Vorgaben später festlegen möchtest, klicke auf **Weiter**.
    - [Auswirkung überprüfen](https://help.miro.com/hc/articles/16494764223378). Dies ist der letzte Schritt des Workflows und er ist obligatorisch.

## Importiere Sensibilitätslabels von Microsoft Purview in bestehende Datenklassifizierungskonfiguration in Miro

### **Voraussetzungen**

- Stelle sicher, dass du die notwendigen Rollen oder Berechtigungen hast, um mit Sensibilitätslabels in Microsoft Purview zu arbeiten.
- Du musst die Details der Boards-Klassifizierungsstufen kennen, die du basierend auf deinen Sicherheits- und Governance-Anforderungen konfigurieren möchtest.
- Du musst die [Admin-Rolle für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Um die Admin-Rolle für sensible Inhalte zu beantragen, wende dich an deinen Unternehmens-Admin.

:::note
Anmerkungen:
- Laut Microsoft-Dokumentation können Aktualisierungen von Sensibilitätslabels in Microsoft Purview bis zu 24 Stunden dauern, um in allen Apps und Diensten repliziert zu werden. Bitte lasse genügend Zeit für die Änderungen und importiere dann die Sensibilitätslabels. Wenn die in MS Purview vorgenommenen Aktualisierungen nach 24 Stunden nicht repliziert werden, wende dich bitte an das Microsoft Purview Support-Team.
- Du kannst bis zu 50 Sensibilitätslabels von Microsoft Purview in Miro importieren.
- Du kannst keine Klassifizierungsstufen übertragen, die in Aufbewahrungsrichtlinien verwendet werden. Du musst sicherstellen, dass die Klassifizierungsstufen nicht in Aufbewahrungsrichtlinien verwendet werden, bevor du fortfährst. Weitere Informationen findest du unter [Aufbewahrungsrichtlinie bearbeiten](../content-lifecycle-management/11-edit-retention-policy.md).
:::

Um Sensibilitätslabels aus Microsoft Purview zu importieren und auf vorhandene Klassifizierungslabels in Miro abzubilden, führe folgende Schritte aus:

1. Gehe zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Bereich unter **Enterprise Guard** auf **Datenschutzklassifizierung**.
3. Klicke auf der Seite **Klassifizierung** oben auf dem Bildschirm auf **Importieren**.
4. Wenn du bereits bei Microsoft angemeldet bist, überspringe diesen Schritt und fahre mit dem nächsten fort.
   Wenn du nicht bei Microsoft angemeldet bist, klicke auf **Anmelden**. Auf der **Microsoft Anmeldeseite**, die in einem neuen Tab erscheint, gib deine Microsoft-Anmeldeinformationen ein und melde dich an. Sobald du bei deinem Microsoft-Konto angemeldet bist, wird der Tab automatisch geschlossen.
5. Klicke im **Import aus Microsoft Purview** Feld auf **Importieren** neben Sensibilitätslabels nach Miro importieren. Die Seite **Klassifizierung aus Microsoft Purview importieren** erscheint.
6. Auf der Seite **Import Levels** wähle das Kontrollkästchen für die Microsoft Purview-Sensibilitätslabel aus, die du als Klassifizierungsstufen in Miro verwenden möchtest, und klicke dann auf **Weiter**. Die Seite **Transfer existing levels** erscheint.

   > ✏️ Laut Microsoft-Dokumentation können Aktualisierungen von Sensibilitätslabeln in Microsoft Purview bis zu 24 Stunden benötigen, um auf alle Apps und Dienste repliziert zu werden. Bitte gib genügend Zeit für die Umsetzung der Änderungen und importiere dann die Sensibilitätslabel. Wenn die von dir vorgenommenen Aktualisierungen in MS Purview nach 24 Stunden nicht repliziert wurden, wende dich bitte an das Microsoft Purview Support-Team.
7. Um sicherzustellen, dass Inhalte korrekt klassifiziert werden, musst du die vorhandenen Miro-Klassifizierungsstufen auf die neu importierten Sensibilitätslabels von Microsoft Purview übertragen. Die auf der linken Seite aufgelisteten Stufen sind die vorhandenen Miro-Klassifizierungsstufen, und die im Dropdown-Menü auf der rechten Seite aufgelisteten sind die importierten Microsoft Purview Sensibilitätslabels. Wenn du fertig bist, klicke auf **Weiter**.
8. Auf der Seite **Klassifizierungsstufen definieren** kannst du die Klassifizierungsstufen bearbeiten, um die Standardklassifizierungsstufe zuzuweisen oder einen Link zu den Richtlinien hinzuzufügen. Die einzelnen Felder und ihre Beschreibungen findest du in der nachstehenden Tabelle.

   |  |  |
   | --- | --- |
   | **Feld** | **Beschreibung** |
   | **Link zu den Richtlinien** | URL, die weitere Informationen zu Richtlinien oder Anweisungen für diese Klassifizierungsstufe enthält. Dies könnte eine Seite sein, die Nutzern in deiner Organisation mehr über die Klassifizierungsstufen für Boards und deren Handhabung vermittelt. Du musst die URL im folgenden Format angeben: `http://www.example.com`  Wenn der Nutzer auf das Symbol **Mehr erfahren** (Fragezeichensymbol) neben dem Klassifizierungsabzeichen klickt, wird diese URL in einem neuen Browser-Tab geladen. |
   | **Als Standardstufe für neue Boards verwenden** | Aktiviere dieses Kästchen, um diese Klassifizierungsstufe als Standardklassifizierung für alle neuen Boards festzulegen. |
   | **Vorschau** | Zeigt eine Vorschau des Klassifizierungsabzeichens mit seiner Beschreibung und dem Symbol „Mehr erfahren“ an. Die Vorschau zeigt genau, wie das Klassifizierungsabzeichen für Nutzer auf einem Board erscheint. |

   Um die Konfiguration der Klassifizierungsstufe zu speichern, klicke auf **Fertig**.
9. Klicke auf **Weiter**. Deine Konfiguration wird gespeichert, aber sie tritt erst in Kraft, nachdem du auf der Seite [**Auswirkungen überprüfen**](https://help.miro.com/hc/articles/16494764223378) auf **Veröffentlichen** clickst.

   Du kannst dann mit einem der folgenden nächsten Schritte fortfahren:

   - [Automatische Klassifizierung definieren](09-define-auto-classification.md). Diese ist optional. Wenn du die automatische Klassifizierung zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
   - [Vorgaben definieren](05-define-guardrails.md). Diese ist optional. Wenn du später Vorgaben definieren möchtest, klicke auf **Weiter**.
   - [Auswirkungen überprüfen](https://help.miro.com/hc/articles/16494764223378). Dies ist der letzte Schritt des Workflows und ist obligatorisch.

## Verbindung zu Microsoft Purview trennen

Wenn du mit Purview verbunden bist, kannst du keine Klassifikationsnamen hinzufügen oder bearbeiten, Klassifizierungsstufen aktualisieren und so weiter. Um diese Aktionen auszuführen, musst du die Verbindung zu Microsoft Purview trennen. Du kannst keine Updates von Microsoft Purview in Miro importieren, nachdem du die Verbindung zu Purview getrennt hast.

Um die Verbindung zu Microsoft Purview zu trennen, führe folgende Schritte aus:

1. Wechsle zu deinen [Miro-Einstellungen](https://miro.com/app/settings).
2. Klicke im linken Bereich unter **Enterprise Guard** auf **Datenschutzklassifizierung**.
3. Klicke auf der Seite **Klassifizierung** oben auf dem Bildschirm auf die Schaltfläche **Letzter Import** und danach auf **Verbindung zu Purview trennen**.
