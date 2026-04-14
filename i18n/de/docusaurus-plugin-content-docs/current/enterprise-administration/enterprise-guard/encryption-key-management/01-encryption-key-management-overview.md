---
title: "Verwaltung von Verschl\xFCsselungsschl\xFCsseln"
article_id: 14634334255250
translation_id: 14634334255250
locale: de
sidebar_position: 0
created_at: '2023-10-24T14:24:53Z'
updated_at: '2026-02-05T15:17:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: enterprise-key-management
---

Das Add-On Enterprise Guard enthält eine Option für die Verwaltung von Verschlüsselungsschlüsseln. Dieses bietet eine zentrale Kontrolle über die Verschlüsselungsschlüssel, um deine Daten zu schützen. Diese Cloud-basierte Lösung ermöglicht die Überwachung von Aktivitätsprotokollen, die mit Verschlüsselungsschlüsseln verbunden sind, sowie den Entzug des Schlüsselzugriffs auf deine Daten.

Für zusätzliche Kontrolle und Sichtbarkeit darüber, wie Verschlüsselungsschlüssel in Miro verwendet werden, kannst du auch „Bring Your Own Key“ (BYOK) nutzen. Mit BYOK kannst du die Verschlüsselung der Daten deines Unternehmens innerhalb der Miro-Plattform verwalten.

## Erlebe die Vorteile der Verwaltung von Verschlüsselungsschlüsseln

- **Nahtlose Implementierung:** Die Verwaltung von Verschlüsselungsschlüsseln ist 100 % Cloud-basiert und fügt sich daher reibungslos in dein System ein, ohne dass du Hardware installieren oder warten musst.

- **Vollständige Kontrolle über Schlüsslezugriff:** Du hast die absolute Kontrolle über deine Verschlüsselungsschlüssel. Du hast die Möglichkeit, deinen Schlüssel zu widerrufen, wodurch alle verschlüsselten Daten sowohl für Miro als auch für die Nutzer unzugänglich werden.

- **Verbesserte Zugangsübersicht:** Dank der höheren Zugangstransparenz erhältst du Einblicke in wichtige schlüsselbezogene Aktivitäten. Über AWS CloudTrail kannst du Protokolle überwachen und nachverfolgen, um die Verwendung deines Verschlüsselungsschlüssels genau zu verstehen.

![Enterprise Key Management Diagram](images/16422045209490_EKM.png)

## So werden Kundendaten durch die Verwaltung von Verschlüsselungsschlüsseln geschützt

Miro verschlüsselt Produktions- und Backup-Daten im Ruhezustand mit einem kundenspezifischen Verschlüsselungsschlüssel, wobei der Kunde Miro den Zugriff auf den Verschlüsselungsschlüssel gewährt. Dabei wird der Schlüssel im AWS-Konto des Kunden über AWS KMS gehostet. Mit der Verwaltung von Verschlüsselungsschlüsseln erhalten Sie mehr Audit-Transparenz und mehr Zugriffskontrolle über Daten (nutzergenerierte Inhalte) wie Formen, Widgets und hochgeladene Dateien.

## Datenverschlüsselung bei Miro

Die höchste Sicherheit deiner Daten ist für Miro von allergrößter Bedeutung. Wir verschlüsseln prinzipiell die Daten unserer Kunden, sowohl bei der Übertragung als auch im Ruhezustand, unabhängig von ihrem Abo-Preisplan. Wenn du über das Internet auf Miro zugreifst, sind deine Daten durch TLS 1.3-Verschlüsselung und PKI-Zertifikate geschützt, die von Amazon Web Services (AWS) ausgestellt wurden. Wenn deine Daten auf unseren Servern ankommen, werden sie durch eine AES-256-Verschlüsselung im Ruhezustand mit Schlüsseln geschützt, die Miro über den AWS Key Management Service (KMS) verwaltet. [Erfahre mehr über Sicherheit bei Miro.](https://miro.com/trust/security/)

> Hinweis: Du allein bist für die Sicherheit und den Schutz aller Backup-Daten verantwortlich, die du herunterlädst oder auf deine Systeme oder auf die Systeme Dritter überträgst. Du allein bist für den damit verbundenen benutzerdefinierten Verschlüsselungsschlüssel verantwortlich. Wenn du deinen benutzerdefinierten Verschlüsselungsschlüssel verlierst, kann Miro dir nicht dabei helfen, den Zugriff auf die Daten wiederherzustellen. Sobald deine Produktionsdaten oder Backup-Daten übertragen werden oder sich außerhalb der Kontrolle von Miro befinden, kann Miro ihren Schutz nicht mehr garantieren.

## Wie aktiviere ich die Verwaltung von Verschlüsselungsschlüsseln?

Zur Konfiguration und Implementierung der Verwaltung von Verschlüsselungsschlüsseln ist die Unterstützung der internen Teams von Miro erforderlich. Wenn du Hilfe brauchst, wende dich an deinen Miro-Ansprechpartner oder [stelle eine Anfrage an das Miro-Support-Team.](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)

## Glossar

- **Backup-Daten:** Ein Snapshot deiner Inhalte, die im Miro-Dienst erstellt oder an diesen übermittelt wurden und von Miro zur Wiederherstellung und für andere Zwecke gespeichert werden.

- **Benutzerdefinierter Verschlüsselungsschlüssel:**  Ein einmaliger Sicherheitsschlüssel, der von dir eingerichtet und implementiert wird und den Personen benötigen, um auf deine Produktionsdaten und Backup-Daten zuzugreifen.

- **Produktionsdaten:** Alle Daten, auf die du und deine Nutzer während der Nutzung und des täglichen Betriebs der Miro-Dienste zugreifen.
