---
title: Nutzererfahrung beim Verschieben von Daten zwischen Regionen
article_id: 25075857856658
translation_id: 25075857856658
locale: de
sidebar_position: 4
created_at: '2025-03-04T08:51:38Z'
updated_at: '2025-05-09T08:47:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Verfügbar für: Alle Nutzer Preispläne: Enterprise Plattformen: Browser,
    Desktop, Mobile'
---

Dieser Artikel beschreibt, wie Nutzer während einer Datenmigration zwischen Regionen sowohl bei [automatisierten](../../canvas-25-admin-features/data-residency/05-move-data-between-regions-–-automated-migration.md) Migrationen als auch beim [manuellen Exportieren und Importieren](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md) unterstützt werden.

## Nutzererfahrung während der automatisierten Migration (Beta)

In den folgenden Abschnitten wird beschrieben, was du vor, während und nach einer automatisierten Datenverschiebung zwischen Regionen erwarten kannst.

### Vor der automatisierten Migration

Zwei Wochen vor der Migration erhalten alle Nutzer in deiner Enterprise-Organisation die folgenden Benachrichtigungen:

- **Produktinternes Banner**
  Zeigt das Migrationsdatum und die erwartete Dauer in der lokalen Zeitzone an
- **E-Mail-Adresse-Benachrichtigung**
  Beschreibt die bevorstehende geplante Wartung für alle Nutzer in deiner Enterprise-Organisation

:::note
Wenn du Mitglied mehrerer Miro-Konten bist, bleiben deine anderen Konten während der Migration zugänglich.
:::

### Während der automatisierten Migration

Eine automatisierte Migration führt zu einer Ausfallzeit von circa 8 Stunden.

Während einer automatisierten Migration kannst du nicht auf die Daten deiner Enterprise-Organisation zugreifen, einschließlich Boards, Teams und Einstellungen.

Das Miro-Dashboard zeigt eine Benachrichtigung mit der Information an, dass eine Datenmigration für deine Organisation durchgeführt wird. Während des Migrationsprozesses hast du keinen Zugriff auf Boards, Teams oder Einstellungen deiner Organisation.

:::tip
Wenn du Mitglied mehrerer Organisationen bist, kannst du von deinem Dashboard aus zu einer anderen Organisation wechseln und Miro weiterhin verwenden.
:::

### Nach der automatisierten Migration

Wenn die Migration erfolgreich abgeschlossen ist, erhältst du eine Bestätigungs-E-Mail. Auf deinem Miro-Dashboard wird eine Nachricht angezeigt, die die erfolgreiche Migration bestätigt.

Wenn die Migration nicht erfolgreich ist, erhältst du eine E-Mail. Du kannst Miro weiterhin in der EU-Region verwenden, indem du dich über [miro.com](https://miro.com) anmeldest.

### Board-Umleitungen nach der automatisierten Migration

Alle Boards, die du in deiner vorherigen Region als Lesezeichen markiert hast, werden automatisch an deine neue Region weitergeleitet und verwenden eine aktualisierte URL.

## Nutzererfahrung beim manuellen Exportieren und Importieren

Die Nutzer müssen Board-Backups manuell aus ihrer Quellregion exportieren und ihre Backups in die Zielregion importieren.

**Weitere Informationen:** Siehe [Daten zwischen Regionen verschieben – manuelles Exportieren und Importieren](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md).

## Regionsübergreifende Zusammenarbeit

Nutzer bei Miro sind regional. Um mit Nutzern in Organisationen außerhalb deiner Region zusammenzuarbeiten, musst du ein Nutzerprofil in jeder Region haben.

Wenn du beispielsweise ein Nutzer in der EU-Region bist und mit Nutzern in einer Organisation der AU-Region zusammenarbeiten möchtest, musst du ein separates Nutzerprofil unter [au.miro.com](https://au.miro.com/) erstellen.
