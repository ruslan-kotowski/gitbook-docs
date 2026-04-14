---
title: Vorgaben definieren
article_id: 16494716849810
translation_id: 16494716849810
locale: de
sidebar_position: 4
created_at: '2024-01-19T19:01:45Z'
updated_at: '2025-11-25T15:40:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Die Definition von Vorgaben ist der dritte Schritt im Ablauf der Konfiguration der automatischen Klassifizierung und der Vorgaben. In diesem Schritt des Prozesses wirst du die Vorgaben konfigurieren, die die Einschränkungen für jede Klassifizierungsstufe festlegen, wie zum Beispiel das Blockieren der öffentlichen Freigabe, das Blockieren der Freigabe mit Teams, das Blockieren der Freigabe mit der Organisation oder das Blockieren der Inhaltsreplikation. Du kannst beispielsweise Vorgaben einrichten, um die öffentliche Freigabe zu blockieren, die Freigabe mit Teams zu verhindern, die Freigabe innerhalb der Organisation zu unterbinden und die Replikation von Inhalten für Nutzer von Boards zu blockieren, die als VERTRAULICH klassifiziert sind.

### Voraussetzungen

- Du musst den ersten und zweiten Schritt des automatischen Klassifizierungs- und Vorgabenflusses abschließen, [1: Definiere Klassifizierungsstufen](07-define-classification-levels.md) und [2: Automatische Klassifizierung definieren](07-define-classification-levels.md).
- Du musst die Vorgaben kennen, die du basierend auf deinen Sicherheits- und Governance-Anforderungen jeder Klassifizierungsstufe zuweisen möchtest.
- Du musst die [Rolle des Admins für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Um die Admin-Rolle für sensible Inhalte zu beantragen, wende dich an deinen Unternehmens-Admin.

Admins haben zwei Möglichkeiten, um intelligente Hilfslinien in ihrer Organisation einzuführen:
**Standardmodus:** Standardmäßig wirken sich Vorgaben nicht auf die derzeit aktiven Freigabeoptionen von Boards aus, damit die laufende Zusammenarbeit nicht gestört wird, auch nicht, wenn die Boards während der automatischen Klassifizierung neu klassifiziert werden.

- **Strikter Modus:** Wenn die Umschaltfläche „Vorgaben im strikten Modus anwenden“ aktiviert ist, setzen die Vorgaben alle aktiven Freigabeoptionen außer Kraft. Dies bietet Admins die strengsten Kontrollstufen, kann jedoch auch dazu führen, dass einige Nutzer den Zugriff auf das Board sofort verlieren.

![guardrails.png](images/26201281436306_guardrails.png)

## Vorgaben zuweisen

Um Guardrails einer Klassifizierungsstufe zuzuweisen, führe die folgenden Schritte aus:

1. Auf der Seite **Schutzmaßnahmen definieren** klicke auf das **Bearbeiten**-Symbol der Klassifizierungsstufe, für die du die Schutzmaßnahmen zuweisen möchtest. Wenn du zum Beispiel Leitplanken für die Klassifizierungsstufe VERTRAULICH zuweisen möchtest, klicke auf das Symbol "Bearbeiten" in der Zeile der Klassifizierungsstufe VERTRAULICH.
2. Aktiviere das Kästchen für jede Schutzmaßnahmen-Kennzeichnung, die du dieser Klassifizierungsstufe zuweisen möchtest. Wenn du beispielsweise das öffentliche Teilen, das Teilen mit Teams, das Teilen mit der Organisation, die Vervielfältigung von Inhalten für die Nutzer von Boards, die als VERTRAULICH eingestuft sind, das Teilen außerhalb der erlaubten Domains und die Nutzung von Miro AI blockieren möchtest, wähle die folgenden Kontrollkästchen aus:
   - **Inhaltsreplikation blockieren**- **Nutzung von Miro AI blockieren (Beta)**
   - **Öffentliche Freigabe blockieren**
   - **Freigabe für Teams blockieren**
   - **Freigabe für die Organisation blockieren**
   **- Freigabe außerhalb zugelassener Domains blockieren (Beta)**
   Nachdem du dieses Kontrollkästchen ausgewählt hast, musst du die Domains, die du zulassen möchtest, eingeben und aus der Liste der in der Organisation erlaubten Domains auswählen oder eine neue Domain in das Feld eingeben und auf + **Hinzufügen** klicken.
   Für mehr Informationen zu jedem Inhalts- und Freigabe-Leitplanke, siehe [Überblick und Szenarien der intelligenten Leitplanken](01-intelligent-guardrails-overview.md).
3. Standardmäßig wirken sich Vorgaben nicht auf die aktiven Freigabeoptionen auf Boards aus, um die laufende Zusammenarbeit nicht zu stören, auch wenn Boards während der automatischen Klassifizierung neu klassifiziert werden.

   Wenn du Vorgaben anwenden und alle aktiven Freigabeoptionen außer Kraft setzen möchtest, aktiviere den Schalter **Vorgaben im strikten Modus anwenden**. Dies kann dazu führen, dass Nutzer den Zugriff auf Boards verlieren. Dies bietet den Admins die strengsten Kontrollstufen, kann aber auch dazu führen, dass einige Nutzer den Zugriff auf das Board sofort verlieren.
   ![schutzplanken.png](images/26201281436306_guardrails.png)
4. Klicke auf **Fertig**.
   Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, nachdem du auf der Seite [**Auswirkungen überprüfen**](06-review-impact.md) auf **Veröffentlichen** klickst.
5. Wenn du mit der Definition von Vorgaben für verschiedene Klassifizierungsstufen fertig bist, fahre fort mit der [Abschlusskonfiguration der Vorgaben](05-define-guardrails.md).

## Vorgaben-Konfiguration abschließen

Nachdem du die Vorgaben für verschiedene Klassifizierungsstufen zugewiesen hast, klicke auf **Weiter**. Deine Konfiguration wurde gespeichert, wird jedoch erst wirksam, nachdem du **Veröffentlichen** auf der [Auswirkungen überprüfen](06-review-impact.md)-Seite angeklickt hast.
