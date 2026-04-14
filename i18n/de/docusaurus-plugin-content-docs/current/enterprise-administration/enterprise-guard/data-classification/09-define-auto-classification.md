---
title: Automatische Klassifizierung definieren
article_id: 16494707596050
translation_id: 16494707596050
locale: de
sidebar_position: 9
created_at: '2024-01-19T19:01:08Z'
updated_at: '2025-11-25T15:40:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Um dich beim Schutz deiner sensiblen Inhalte zu unterstützen, gibt es im Enterprise Guard die automatische Klassifizierung. Dabei handelt es sich um einen automatisierten Datenklassifizierungsprozess, der Miro-Boards nach der Stufe ihrer sensiblen Inhalte kategorisiert. Die automatische Klassifizierung stellt einen wesentlichen Fortschritt bei der Verwaltung und dem Schutz deiner sensiblen Daten dar, denn die Automatisierung dieses Prozesses hilft deiner Organisation, ein höheres Maß an Datensicherheit zu gewährleisten, die regulatorischen Anforderungen einzuhalten und die Sicherheit besser zu verwalten. Der Übergang von der manuellen zur automatischen Klassifizierung ist ein strategischer Schritt in Richtung eines genaueren, sichereren und effizienteren Frameworks für die Datensicherheit.

Weitere Informationen zur automatischen Klassifizierung und Beispielszenarien findest du unter [Übersicht über die automatische Klassifizierung](03-auto-classification-overview-and-scenarios.md).

## Automatische Klassifizierung definieren

Dies ist der zweite Schritt der automatischen Klassifizierung und der Konfiguration der Vorgaben. In diesem Schritt des Ablaufs konfigurierst du das Label für die automatische Klassifizierung, das für jede Klassifizierungsstufe gilt. Die Klassifizierung der Boards wird automatisch auf alle neuen Boards und bestehenden Boards angewendet, die den festgelegten Kriterien entsprechen. Dies geschieht, nachdem du die Auswirkungen überprüft und beschlossen hast, Aktualisierungen zu veröffentlichen.

## Voraussetzungen

- [Du musst die Datenerkennung aktivieren](../data-discovery/13-activate-privacy-related-data-discovery.md).
- Du musst den ersten Schritt des Ablaufs der automatischen Klassifizierung und der Vorgaben  abschließen , [1: die Klassifizierungsstufen definieren](07-define-classification-levels.md)/a>
- Du musst wissen, welche Sensibilitäts-Labels du jeder Klassifizierungsstufe auf der Grundlage deiner Sicherheits- und Governance-Anforderungen zuweisen willst.
- Du musst die [Rolle Admin für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Die Rolle des Admins für sensible Inhalte kannst du bei deinem Unternehmens-Admin anfordern.

## Zuweisen von Sensitivitäts-Labels für die automatische Klassifizierung

Um einer Klassifizierungsstufe Labels zuzuweisen, gehe wie folgt vor:

1. Klicke auf der Seite **Automatische Klassifizierung definieren** auf das Symbol **Bearbeiten** der Klassifizierungsstufe, für die du die Labels für die Empfindlichkeit zuweisen möchtest. Wenn du zum Beispiel die Sensibilitätslabels für die automatische Klassifizierung der Klassifizierungsstufe **VERTRAULICH** zuweisen möchtest, klicke auf das Symbol Bearbeiten in der Zeile der Klassifizierungsstufe **VERTRAULICH**.
2. Aktiviere das Kästchen für jedes Label, das du dieser Klassifizierungsstufe zuordnen möchtest. Wenn du z. B. alle Boards, die sensible Daten im Zusammenhang mit der GDPR enthalten, automatisch klassifizieren möchtest, aktiviere das Kästchen **GDPR General Data Protection Regulation**. Du kannst jedem Klassifizierungs-Label ein oder mehrere Sensitivitäts-Labels zuweisen.
3. Klicke auf Fertig.
   Die Klassifizierung der Boards wird automatisch auf alle neuen Boards und bestehenden Boards angewendet, die den festgelegten Kriterien entsprechen. Dies geschieht, nachdem du die Auswirkungen überprüft und beschlossen hast, Aktualisierungen zu veröffentlichen.
4. Wenn du mit der Zuweisung von Labels für die verschiedenen Klassifizierungsstufen fertig bist, fahre fort mit [Konfiguration der automatischen Klassifizierung abschließen](09-define-auto-classification.md).

## Vollständige Konfiguration der automatischen Klassifizierung

Wenn du die Zuweisung von Labels für die automatische Klassifizierung abgeschlossen hast, klicke auf **Weiter**. Deine Konfiguration wird gespeichert, aber sie wird erst wirksam, wenn du auf der Seite **Veröffentlichen** [**Auswirkungen überprüfen**](https://help.miro.com/hc/articles/16494764223378) Seite klickst.

Du kannst dann mit einem der folgenden nächsten Schritte fortfahren:

- Vorgaben definieren Dies ist optional. Wenn du die Vorgaben zu einem späteren Zeitpunkt festlegen möchtest, klicke auf **Weiter**.
- Auswirkungen überprüfen Dies ist der letzte Schritt des Workflows und er ist obligatorisch.
