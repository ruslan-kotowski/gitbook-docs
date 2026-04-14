---
title: Daten zwischen Regionen verschieben – manuelles Exportieren und Importieren
article_id: 24778387087122
translation_id: 24778387087122
locale: de
sidebar_position: 6
created_at: '2025-02-20T09:07:00Z'
updated_at: '2025-11-25T15:49:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Verfügbar für: Board-Eigentümer, Board-Miteigentümer, Content-Admins, Unternehmens-Admins
    Preispläne: Enterprise Plattformen: Browser, Desktop'
---

In diesem Artikel wird das manuelle Exportieren und Importieren zum Verschieben von Daten zwischen Regionen beschrieben. Weitere Informationen zu deinen Optionen zum Verschieben von Daten zwischen Regionen, einschließlich der automatisierten Migration, erfährst du unter [Daten zwischen Regionen verschieben](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Bereite den manuellen Export und Import in eine neue Region vor.

Als Unternehmens-Admin helfen dir die folgenden Best Practices, dich auf eine manuelle Migration in eine neue Region vorzubereiten:

- Um eine neue Organisation in deiner Zielregion zu initiieren, wende dich an deinen dedizierten Miro-Kontakt.
- Um sicherzustellen, dass du alle Nutzer in deiner Domain verwalten kannst, bestätige alle Domains, die du besitzt, mit der DNS-Verifizierung.
- Aktiviere die Domainsteuerungsrichtlinie **Eigene Abos blockieren**, damit Nutzer nicht versehentlich kostenlose Miro-Abos in deiner alten Region erstellen.
- Teams und/oder Organisationen können mit einem einzigen Abo in einer einzigen Organisation zusammengeführt werden.
- Du kannst überprüfen, welche Integrationen deine Organisation in der neuen Region nutzt und benötigt, und dann einen Plan erstellen, um jede Integration in deiner neuen Region neu zu konfigurieren.
- Überprüfe alle Einstellungen, die deine Organisation derzeit verwendet, und plane dann, wann du jede Einstellung, die du in deiner neuen Region benötigst, neu konfigurierst.

## Daten manuell in eine neue Region exportieren und importieren

Miro richtet eine neue Enterprise-Organisation in der Zielregion ein. Die Nutzer müssen ihre Boards als Board-Backups aus der Quellregion exportieren und dann ihr Backup in die Zielregion importieren.

**Weitere Informationen:** Siehe [So kannst du Board-Backups speichern](../../../using-miro/import-and-export/export/05-how-to-save-board-backup.md).

Nur Nutzer mit den folgenden Berechtigungen können Inhalte manuell exportieren und importieren:

- Board-Eigentümer
- Board-Miteigentümer
- Unternehmens-Admin
- Content-Admin

:::note
Alle Board-Freigaben gehen verloren. Die Nutzer müssen ihre Freigabeberechtigungen wiederherstellen, nachdem sie ihr Backup in die Zielregion hochgeladen haben.
:::

Um mit dem manuellen Importieren von Inhalten zu beginnen, können sich die Nutzer bei ihrer neuen regionalen URL anmelden, und zwar bei einer der folgenden:

- (Australien) [au.miro.com](https://au.miro.com/)
- (USA) [us.miro.com](https://us.miro.com/)

:::note
Bevor du dich als Nutzer zum ersten Mal anmeldest, überprüfe, ob deine Organisation Single Sign-on (SSO) verwendet. Wenn du SSO verwendest, warte, bis dein Unternehmens-Admin die SSO-Einstellungen für deine neue Region neu konfiguriert hat.
:::

## Was nach einem manuellen Export und Import zu tun ist

Nach einer Datenmigration zwischen Regionen ist Folgendes zu tun:

- Konfiguriere SSO, falls zutreffend, sofort für die neuen regionalen Subdomains neu. Zum Beispiel: au.miro.com.
  > ✏️ Deine Nutzer können sich nicht in der neuen Region anmelden, bis SSO auf der Seite des Identitätsanbieters neu konfiguriert wurde.
- Konfiguriere SCIM für die neuen regionalen Subdomains neu. Zum Beispiel: au.miro.com.
- Bestätige, dass Eigene A**bos blockieren in den** Einstellungen für die Domainsteuerung aktiviert ist.
- Du kannst alle anderen Organisations-, Domainsteuerungs- und Teameinstellungen validieren.
- Du kannst jede Enterprise-App und -Integration erneut installieren und konfigurieren, z. B. SIEM, SAM, eDiscovery, Smarsh und Okta.
- Lade Nutzer zur Organisation in der neuen Region ein.

## Manuelles Exportieren und Importieren von Daten in eine neue Region – FAQ

**Wie funktioniert eine manuelle Migration in eine neue Region?**

Die Admins richten die Organisation und alle ihre Teams, Teameinstellungen und Nutzer effektiv erneut ein. Außerdem können die Endnutzer Board-Backups manuell aus der alten Organisation herunterladen und in die neue Organisation hochladen.

**Wer ist berechtigt und wer nicht?**

Enterprise-Kunden können ihre Daten in eine andere Region verschieben. Für weitere Informationen wende dich an deine Kontaktperson bei Miro.

**Welche Daten sind Teil einer manuellen Migration?**

Nur Boards, die von Nutzern verschoben wurden. Weitere Informationen findest du unter Daten manuell in eine neue Region exportieren und importieren.

**Fallen zusätzliche Kosten an?**

Nein. Miro kann eine neue Organisation in Australien oder den USA gemäß dem Enterprise-Standardvertrag bereitstellen.

**Wie lange dauert eine manuelle Verschiebung?**

Die Dauer einer manuellen Migration hängt davon ab, wie viel Zeit die Nutzer benötigen, um ihre gespeicherten Boards als Backup zu exportieren und ihre Backup-Inhalte in die Zielregion zu importieren.

**Wie stellt Miro sicher, dass die Daten meiner Organisation aus der Quellregion entfernt werden?**

Benachrichtige den Miro-Support, nachdem du den manuellen Export und Import in deine neue Region abgeschlossen hast (einschließlich der Neukonfiguration) und wenn alle Nutzer ihre Backups in die Zielregion importiert haben. Der Miro-Support löscht dann deine Organisation und alle Daten aus der Quellregion.
