---
title: "\xDCberblick \xFCber intelligente Vorgaben"
article_id: 14375998880018
translation_id: 14375998880018
locale: de
sidebar_position: 0
created_at: '2023-10-12T12:35:03Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Miro-Board-Elemente können Daten zum Datenschutz und zur Regulierung enthalten (wie PII, PHI, PCI) oder vertrauliche, geschäftskritische Inhalte (wie Finanzinformationen, HR-Informationen, geistiges Eigentum, Geschäftsgeheimnisse). Nach der Datenerkennung und Autoklassifizierung müssen Organisationen proaktive Kontrollen umsetzen, die entscheidend sind, um anhaltenden Datenschutz, Sicherheit und Compliance mit relevanten Vorschriften zu gewährleisten.

- Mit Vorgaben kannst du jetzt proaktive Kontrollen automatisch durchsetzen, wie zum Beispiel:
  Automatisches Einschränken der Freigabemöglichkeiten auf verschiedenen Ebenen (öffentlich, Team, Organisation) basierend auf dem Inhalt des Boards und der Klassifizierungsstufe.
- Einschränkung der Inhaltsreplikation.
- Verhindern der Nutzung von Miro AI, um KI-gestützte Interaktionen mit sensiblen oder klassifizierten Daten zu blockieren.

Diese proaktiven Kontrollen gewährleisten dauerhaften Datenschutz und Compliance, ohne den Geschäftsbetrieb zu behindern.

Admins haben zwei Möglichkeiten, um intelligente Vorgaben in ihrer Organisation einzuführen:
- **Standardmodus:** Im Standardmodus beeinflussen die Vorgaben die aktiven Freigabeoptionen auf Boards nicht, um die laufende Zusammenarbeit nicht zu stören, auch nicht, wenn die Boards während der automatischen Klassifizierung neu klassifiziert werden.

- **Strikter Modus:** Wenn der Umschalter **Vorgaben im strikten Modus anwenden** aktiviert ist, setzen die Vorgaben alle aktiven Freigabeoptionen außer Kraft. Dies bietet Admins die strengsten Kontrollmöglichkeiten, kann jedoch dazu führen, dass einige Nutzer sofort den Zugang zum Board verlieren.

Stell dir ein Szenario vor, in dem du die Vorgaben so konfiguriert hast, dass Nutzern von Boards, die als VERTRAULICH klassifiziert sind, nicht erlaubt ist, das Board öffentlich, mit Teams oder innerhalb der Organisation freizugeben oder Inhalte zu replizieren. Jemand in deiner Organisation hat ein neues Board namens Finanzplan erstellt, einige Umsatzzahlen hinzugefügt und die Klassifizierungsstufe *VERTRAULICH* für dieses Board festgelegt. Die Vorgaben werden automatisch angewandt und alle Nutzer können das Board nicht freigeben, und alle außer dem Eigentümer des Boards können keine Inhalte replizieren (Abbildung 2).

Weitere Informationen zu den einzelnen Vorgaben, deren Beschreibungen und betroffene Nutzer findest du in der [Vorgaben-Referenzdokumentation](02-guardrails-reference.md).
