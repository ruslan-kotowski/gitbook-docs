---
title: "\xDCberblick \xFCber die Eigenen AGB"
article_id: 27375760557330
translation_id: 27375760557330
locale: de
sidebar_position: 2
created_at: '2025-06-13T08:24:28Z'
updated_at: '2025-11-04T14:10:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Die Funktion für eigene AGB ermöglicht es Admins, einen benutzerdefinierten AGB-Dialog für alle internen Mitglieder ihrer Miro-Organisation anzuzeigen. Dies stellt sicher, dass die Nutzer die Richtlinien und Bedingungen Ihrer Organisation überprüfen und anerkennen, bevor sie Miro nutzen. Nutzen Sie diese Funktion, um die Nutzer über akzeptable Nutzungsrichtlinien für Miro-Funktionen, einschließlich Miro AI, zu informieren. Admins können mehrere Links zu extern gehosteten Richtlinien hinzufügen und die Wiederholung konfigurieren, sodass die Nutzer gemäß den internen Anforderungen erinnert werden. Alle Aktionen im Zusammenhang mit den eigenen AGB werden zur Nachverfolgbarkeit in den Audit-Protokollen protokolliert.

:::note
Eigene AGB sind derzeit nur in der Web-App und in Browsern verfügbar.
:::

## Wichtige Vorteile

- Du zeigst unternehmensweit deine AGB an.
- Präsentiere den Dialog mit den benutzerdefinierten AGB an passenden Nutzungspunkten: nach erfolgreichem Login oder bei Interaktion mit Miro AI.
- Erzwinge die Akzeptanz durch die Nutzer in einem von dir festgelegten zeitlichen Ablauf (Tage, Wochen oder Monate) oder bei Aktualisierungen.
- Verlinke bis zu drei intern oder extern gehostete Richtlinien in deiner bevorzugten Sprache oder deinem bevorzugten Format.
- Behalte die Nachvollziehbarkeit in den Audit-Protokollen bei.

## Geltungsbereich

- Gilt für: Nur interne Nutzer, alle Mitglieder und Admins der Organisation.
- Ausgenommen: Gäste und externe Mitwirkende.
- Auslöser:
  - Erfolgreiche Anmeldung: Wird sofort nach der Anmeldung angezeigt.
  - Miro AI Nutzung: Wird angezeigt, wenn ein Nutzer mit Miro AI interagiert (zum Beispiel beim Umschalten des AI-Layouts, Öffnen des seitlichen Felds oder Starten einer AI-Aktion wie dem KI-Kollege).
- Wiederholung: Vom Admin konfigurierbar in Tagen, Wochen oder Monaten. Jede individuelle AGB hat ihren eigenen Status und ihre eigene Wiederholung. Standard: zwei Wochen.
- Format der Bedingungen: Der Inhalt muss extern gehostet werden. Miro referenziert die Links und speichert nicht den gesamten Text der Richtlinie.
- Links: bis zu drei Richtlinien-Links, jeder mit einem klaren Label.
- Konfiguration: Sie können eine eigene AGB für jeden Trigger (erfolgreiche Anmeldung und Miro AI-Nutzung) konfigurieren. Jede eigene AGB hat ihren eigenen Status und ihre Wiederholungsrate.

## Wer kann dieses Feature nutzen?

Admins müssen die folgenden Enterprise Guard-Berechtigungen haben, um die eigenen AGB anzusehen und zu verwalten:

- **Admin für sensible Inhalte:** hat von vornherein die nötigen Berechtigungen.
- **Benutzerdefinierte Admin-Rollen**, müssen Folgendes beinhalten:
  - Eigene AGB ansehen
  - Eigene AGB verwalten

## So funktioniert's

1. **Bedingungen konfigurieren:** Wählen Sie den Auslöser (erfolgreicher Login oder KI-Nutzung), den Geltungsbereich (interne Mitglieder) und die Wiederholungsrate.
2. **Inhalte hinzufügen:** Geben Sie einen prägnanten Titel, eine kurze Beschreibung und bis zu drei beschriftete Links zu extern gehosteten Richtlinien an.
3. **Prüfen und aktivieren:** Vorschau des Dialogs für Endnutzer anzeigen und die Konfiguration aktivieren.
4. **Durchsetzung:**

- **Erfolgreiche Anmeldung:** Der Dialog kann nicht abgelehnt werden. Nutzer müssen akzeptieren, um fortzufahren oder sich abmelden.
- **AI-Nutzung:** Der Dialog ermöglicht **Weiter** oder **Abbrechen**. Bei "Abbrechen" bleibt der Nutzer angemeldet, jedoch sind die AI-Funktionen deaktiviert.

5. **Protokollierung:** Konfigurationsänderungen und Nutzerannahmen werden in den Audit-Protokollen aufgezeichnet.

### Benutzererfahrung

- **Erfolgreiche Anmeldung**

  - Der Dialog erscheint sofort nach der Anmeldung.
  - Die Nutzer können auf **Weiter** klicken, um zu akzeptieren und fortzufahren, oder auf **Abmelden**.
- **AI-Nutzung**

  - Der Dialog erscheint, wenn der Nutzer mit Miro AI interagiert, zum Beispiel beim Umschalten des AI-Layouts, beim Öffnen des seitlichen Feldes oder beim Starten eines AI-Tools oder -Vorgangs (zum Beispiel KI-Kollege).
  - Nutzer können auf **Weiter** klicken, um zu akzeptieren und AI-Funktionen zu nutzen. Wenn Nutzer auf **Abbrechen** klicken, bleiben sie angemeldet und können alle nicht-AI-Funktionen weiter nutzen.
- Nutzer werden nicht erneut aufgefordert, bis der Wiederholungszeitraum endet oder die Bedingungen aktualisiert werden.

## Akzeptanzverhalten

- **Login-Trigger:** Nutzer müssen den konfigurierten Zeitplan akzeptieren oder sich abmelden. Der Dialog kann nicht umgangen werden.
- **AI-Nutzung Trigger:** Nutzer können akzeptieren, um AI-Funktionen zu aktivieren, oder abbrechen, um die AI-Funktionen deaktiviert zu lassen. Beim Abbruch bleibt der Nutzer angemeldet und kann nicht-AI-Funktionen nutzen.
- **Wiederholung und Versionen:** Nutzer werden nicht erneut aufgefordert, bis die Wiederholungsperiode endet oder eine neue Version veröffentlicht wird, gemäß dem konfigurierten Trigger.

##

###
