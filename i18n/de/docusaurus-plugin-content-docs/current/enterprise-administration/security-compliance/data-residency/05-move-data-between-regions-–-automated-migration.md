---
title: Daten zwischen Regionen verschieben – automatisierte Migration
article_id: 24866660560402
translation_id: 24866660560402
locale: de
sidebar_position: 5
created_at: '2025-02-24T08:47:08Z'
updated_at: '2025-10-29T14:40:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Wer kann es durchführen: Unternehmensadministratoren Welche Preispläne:
    Enterprise Welche Plattformen: Browser, Desktop'
---

:::note
Die automatisierte Migration ist ein kostenpflichtiger Service mit professionellen Dienstleistungen. Für ein Angebot wende dich an deine Miro-Kontaktperson.
:::

In diesem Artikel wird die automatisierte Datenmigration erläutert. Um mehr über andere Optionen zur Verschiebung von Daten zwischen Regionen zu erfahren, siehe [Daten zwischen Regionen verschieben](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Daten, die Teil einer automatisierten Migration zwischen Regionen sind

Die folgende Liste zeigt, welche Daten Teil einer automatisierten Migration zwischen Regionen sind:

- Boards, Board-Inhalte und Board-Freigabe-Einstellungen
- Inhaltshierarchie, einschließlich der Bereiche „Teams“ und „Abschnitte“
- Organisations-, Team- und Board-Einstellungen
- Nutzer, Nutzerprofile und Nutzereinstellungen, einschließlich Gäste
- Audit-Protokolle, Datenklassifizierung und Inhaltssicherheitseinstellungen

## Bereite eine Datenmigration zwischen Regionen vor

Um eine Datenmigration zwischen Regionen vorzubereiten, gehe wie folgt vor:

1. Um sicherzustellen, dass du alle Nutzer in deiner Domain verwalten kannst, bestätige alle Domains, die du besitzt, mit der DNS-Verifizierung.
2. Aktiviere die Domainsteuerungsrichtlinie **Eigene Abos blockieren**, damit Nutzer nicht versehentlich kostenlose Miro-Abos in deiner alten Region erstellen.
3. Führe Teams und/oder Organisationen in einer einzigen Organisation mit einem einzigen Abo zusammen.
4. Überprüfe, welche Integrationen deine Organisation in der neuen Region nutzt und benötigt, und plane dann eine Zeitachse, um jede Integration in deiner neuen Region neu zu konfigurieren.

## Wie eine Datenmigration zwischen Regionen funktioniert und wie lange sie dauert

Eine Migration zwischen Regionen umfasst die folgenden fünf Schritte:

- **Vorbereitung**
  Typischerweise 4-8 Wochen. Der Unternehmens-Admin bereitet mit Unterstützung von Miro die Organisation auf die Migration vor, plant Ausfallzeiten für die Migration und kommuniziert mit den Endnutzern.
- **Migration**
  In der Regel <8 Stunden Ausfallzeit. Die Organisation und ihre Daten werden in die neue Region migriert.

  > ✏️ Das Miro-Team koordiniert mit Ihnen das Datum der Migration. Sollte die Migration aus irgendeinem Grund nicht erfolgreich sein, wird der Zugriff auf Ihre Quellregion wiederhergestellt, und Miro koordiniert mit Ihnen ein neues Migrationsdatum, um die Migration erneut zu versuchen.
- **Verifizierung und Konfiguration**
  Typischerweise 2-3 Wochen. Der Admin muss bestimmte Integrationen, wie SSO, in der neuen Region neu konfigurieren. Admin und Endnutzer bestätigen, dass ihre Boards und Daten wie erwartet in der neuen Region angekommen sind.
- **Schulung**
  Typischerweise 2-3 Wochen. Die Nutzer werden darüber informiert, wo sie auf ihre neue Miro-Organisation zugreifen können.
- **Compliance**
  Innerhalb von 120 Tagen nach dem Migrationsdatum: Miro überprüft, ob die Daten der Organisation aus der Quellregion entfernt wurden.

## Was ist nach einer Datenmigration zwischen Regionen zu tun?

Nach einer Datenmigration zwischen Regionen ist Folgendes zu tun:

- Konfiguriere SSO, falls zutreffend, sofort für die neuen regionalen Subdomains neu. Zum Beispiel: au.miro.com.

  > ✏️ Deine Nutzer können sich nicht in der neuen Region anmelden, bis SSO auf der Seite des Identitätsanbieters neu konfiguriert wurde.
- Konfiguriere SCIM für die neuen regionalen Subdomains neu. Zum Beispiel: au.miro.com.
- Bestätige, dass **Eigene Abos blockieren** in den Domainsteuerungseinstellungen aktiviert ist.
- Überprüfe deine anderen Domainsteuerungseinstellungen.
- Relevante Apps und Integrationen erneut installieren und konfigurieren.

## Automatisierte Datenmigrationen zwischen Regionen – häufige Fragen

**Was ist eine Datenmigration zwischen Regionen?**

Datenmigrationen zwischen Regionen automatisieren die Verschiebung von Kundendaten von einer geografischen Region zur anderen. Bei einer Migration zwischen Regionen werden deine Miro-Kundendaten im Geltungsbereich in der neuen Region gespeichert und verarbeitet

**Wie funktioniert es und wie lange dauert es?**

Siehe Wie eine Datenmigration zwischen Regionen funktioniert und wie lange sie dauert.

**Wer ist berechtigt und wer nicht?**

Um eine automatische Migration zwischen Regionen durchzuführen, musst du Enterprise-Kunde sein. Ein Enterprise-Kunde, der Enterprise Guard und Schlüsselverwaltung verwendet, ist jedoch nicht berechtigt. Für weitere Informationen wende dich an deine Kontaktperson bei Miro.

**Welche Daten sind in einer automatisierten Datenmigration zwischen Regionen enthalten?**

Weitere Infos dazu, welche Daten eine automatische Migration zwischen Regionen umfasst, findest du unter Daten, die in einer automatisierten Migration zwischen Regionen enthalten sind.

**Welche Daten sind nicht Teil einer automatisierten Datenmigration zwischen Regionen?**

Die folgenden Daten sind nicht Teil einer automatisierten Datenmigration zwischen Regionen:

- Apps und Integrationen, einschließlich Single Sign-on (SSO) und SCIM, die für die neue Region neu konfiguriert werden müssen
- Talktracks
- In-App-Benachrichtigungen werden entfernt

**Fallen zusätzliche Kosten an?**

Ja. Eine automatisierte Migration zwischen Regionen ist ein kostenpflichtiger Vorgang mit Miro Services. Für weitere Informationen wende dich an deine Kontaktperson bei Miro.

**Wie stellt Miro sicher, dass die Daten meiner Organisation aus der Quellregion entfernt werden?**

Um deine Daten nach einer Migration zwischen Regionen aus der Quellregion zu entfernen, geht Miro folgendermaßen vor:

- Die Daten bleiben 30 Tage lang in der Quellregion, sodass ein zuverlässiges Backup verfügbar ist, falls es ein Problem bei der Migration gibt.
- Nach 30 Tagen beginnt Miro mit dem Löschen deiner Daten aus der Quellregion.
- Nach maximal 120 Tagen nach dem ersten Migrationsdatum hat Miro alle Daten aus der Quellregion gelöscht.

**Was sehen Nutzer während einer Migration zwischen Regionen?**

Weitere Informationen zur Nutzererfahrung während einer Migration findest du unter [Nutzererfahrung beim Verschieben von Daten zwischen Regionen](../../canvas-25-admin-features/data-residency/04-user-experience-while-moving-data-between-regions.md).

**Was passiert, wenn die Migration nicht erfolgreich ist?**

Wenn die Migration aus irgendeinem Grund nicht erfolgreich ist, stellt Miro den Zugang zu deiner Quellregion wieder her und koordiniert ein neues Datum, um die Migration zu wiederholen.
