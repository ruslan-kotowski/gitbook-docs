---
title: "\xDCberwachung des Status der Verwaltung von Verschl\xFCsselungsschl\xFCsseln"
article_id: 31325531757970
translation_id: 31325531757970
locale: de
sidebar_position: 1
created_at: '2025-11-24T17:59:06Z'
updated_at: '2026-02-04T20:46:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: enterprise-key-management
---

Administratoren können den Status ihrer Verschlüsselungsschlüsselverwaltung (EKM) in der Miro Admin-Konsole überwachen und nachverfolgen. Dies sorgt für mehr Transparenz bei der Einführung von Schlüsseln und dem Fortschritt der Verschlüsselung, sodass Sie informiert bleiben, ohne zusätzliche Unterstützung zu benötigen.

## EKM-Status überprüfen

1. Gehen Sie in der Miro Admin-Konsole zu **Enterprise Guard**.
2. Wählen Sie **Verwaltung von Verschlüsselungsschlüsseln**.
3. Überprüfen Sie im Abschnitt **Status** den aktuellen Status und die Nachricht.

## EKM-Status verstehen

Im Abschnitt **Status** sehen Sie, an welchem Punkt im Einrichtungs- und Verschlüsselungsprozess der EKM Sie sich befinden.

| Status | Bedeutung |
| --- | --- |
| **Eigene Schlüssel hinzugefügt** | Miro richtet Verschlüsselung mit deinen eigenen Schlüsseln ein. Sobald die Einrichtung abgeschlossen ist, beginnen deine Schlüssel automatisch mit der Verschlüsselung von Inhalten. |
| **Aktivierung der Schlüssel wird durchgeführt** | Neue Inhalte werden mit deinen eigenen Schlüsseln verschlüsselt. Die Neuverschlüsselung vorhandener Inhalte wird durchgeführt. |
| **Eigene Schlüssel sind aktiv** | Alle Inhalte sind mit deinen eigenen Schlüsseln verschlüsselt. |
| **Wechsel zurück zu Standardschlüsseln wird durchgeführt** | Miro ändert die Verschlüsselung zurück auf Miro’s Standardschlüssel. Deine eigenen Schlüssel werden entfernt. |

## Konfigurierte Schlüssel überprüfen

Im Bereich Schlüssel kannst du die Kennungen der aktuell für die EKM konfigurierten Schlüssel ansehen. Wenn Miro deine benutzerdefinierten Schlüssel verwaltet, siehst du möglicherweise eine Benachrichtigung anstelle einer Schlüssel-ARN.

- **Primärschlüssel**

  Verschlüsselt die Boards, Kommentare und anderen Inhalte deiner Organisation.
- **Schlüssel für Backup-Speicher**

  Verschlüsselt archivierte Versionen und Backups.
- **Schlüssel-ARN**

  Der Schlüsselbezeichner in [AWS KMS](https://aws.amazon.com/kms/). Wenn Miro deine benutzerdefinierten Schlüssel verwaltet, siehst du möglicherweise eine Benachrichtigung anstelle einer Schlüssel-ARN.

(Optional) Um Änderungen an deinen Schlüsseln vorzunehmen (zum Beispiel, wenn du den falschen Schlüssel siehst oder zur Standardverschlüsselung zurückkehren möchtest), wende dich an deinen Customer Success Manager oder an [support@miro.com](mailto:support@miro.com).
