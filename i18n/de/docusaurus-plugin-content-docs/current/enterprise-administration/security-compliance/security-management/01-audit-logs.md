---
title: Audit-Protokolle
article_id: 360017571434
translation_id: 360017571434
locale: de
sidebar_position: 1
created_at: '2019-02-11T10:09:04Z'
updated_at: '2026-03-12T09:21:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Verfügbar für: Enterprise Einrichten durch: Unternehmens-Admins'
---

Audit-Protokolle ermöglichen es Administrationsberechtigten einer Organisation innerhalb von Miro, die Aktivitäten der Nutzer zu verfolgen. Protokolle sind äußerst nützlich, wenn Probleme untersucht oder detaillierte Berichte über wichtige Ereignisse, wie Änderungen in den globalen Sicherheitseinstellungen, Einladungen neuer Nutzer oder das Anlegen neuer Boards, benötigt werden.

:::note
Aktuell werden die Ereignisse ab dem Moment der Erstellung des Enterprise-Abonnements erfasst und standardmäßig 180 Tage lang gespeichert:
a) Wenn du von einem anderen Preisplan auf Enterprise upgraden, werden die Ereignisse ab dem Zeitpunkt des Upgrades protokolliert.
b) Wenn du einige Teams in das Enterprise-Abonnement migrierst, werden deren Daten erst ab dem Moment protokolliert, wenn sie Teil des Abonnements werden.
:::

## Zugriff auf Audit-Protokolle

Um auf die Audit-Protokolle zuzugreifen, gehe wie folgt vor:

1. Gehe zu den **Unternehmenseinstellungen**.
2. Klicke im linken Feld auf **Sicherheit** > **Audit-Protokolle**.
3. Du kannst die Audit-Protokolle nach **Datumsbereich**, **Ausführender**, **Ereigniskategorie** und einem spezifischen **Ereignis** filtern.

Klicke auf die Schaltfläche „Ereignisse ansehen“, um die mit deinen Filterkriterien übereinstimmenden Ereignisse anzuzeigen. Die Zeit wird im **ISO 8601** Format, in der **lokalen** Zeitzone angezeigt. Details zu einem bestimmten Ereignis kannst du sehen, indem du auf die drei Punkte in der Spalte **Details** klickst.

:::note
Nur Ereignisse aus den letzten 90 Tagen sind zur Vorschau verfügbar.
:::

## Audit-Protokolle exportieren

Du kannst Protokolle im **CSV**-Dateiformat exportieren.

Im CSV-Export sind Ereignisdatum und -zeit im ISO 8601-Format in der UTC-Zeitzone angegeben. Es gibt kein Limit für die Anzahl der gleichzeitig zu exportierenden Datensätze; je mehr Daten du exportierst, desto länger dauert es jedoch, die Datei zum Herunterladen vorzubereiten. Beachte auch, dass beliebte Anwendungen zur Tabellenarbeit ihre Grenzen hinsichtlich der Menge an Daten haben, die sie öffnen können.

Um Protokolle zu exportieren, klicke auf die Schaltfläche **Export to CSV**.

Die Leiste mit den Details deiner Exportdatei erscheint unten. Wenn die Datei zum Herunterladen bereit ist, kannst du auf die Schaltfläche Download CSV klicken. Die Datei steht 24 Stunden lang zum Herunterladen bereit.

:::note
Derzeit ist nur eine Exportdatei pro Organisation gleichzeitig verfügbar. Durch Klicken auf die Schaltfläche **Export to CSV** wird die aktuelle Exportdatei ersetzt.
:::

## Zugriff auf Audit-Protokolle über die API

Administratoren können die [Audit-Protokoll-API](https://developers.miro.com/reference/audit-logs) oder unterstützte [SIEM-Integrationen](https://help.miro.com/hc/sections/4404757427090-Security-information-and-event-management-SIEM) nutzen, um programmatisch auf Audit-Protokolldaten zuzugreifen und diese zu sammeln.

## Audit-Protokolle löschen

Administratoren können eine Aufbewahrungsrichtlinie für Audit-Protokolle festlegen. Du kannst zwischen 30, 90, 180 oder 365 Tagen wählen.

:::warning
Gelöschte Audit-Protokolle können nicht wiederhergestellt werden.
:::

:::note
Die unbegrenzte Aufbewahrung für Audit-Protokolle wurde eingestellt.
:::

Um eine Löschfrist festzulegen, gehe wie folgt vor:

1. Gehe zu **Unternehmenseinstellungen**.
2. Klicke im linken Feld auf **Sicherheit** > **Audit-Protokolle**.
3. Unter **Audit-Protokolle**, klicke auf den Tab **Einstellungen**.
4. Wähle eine Option aus der Dropdown-Liste aus. Du wirst aufgefordert, deine Wahl zu bestätigen.

## Ereignisse in Audit-Protokollen

Die Audit-Protokolle enthalten Aufzeichnungen über folgende Ereigniskategorien:

**Verwaltung**

- Änderung des Unternehmensnamens
- Änderung oder Löschung des Unternehmenslogos
- Zugriffsanfrage erstellt
- Zugriffsanfrage abgelehnt
- Nutzeraktivitätskennzahlen in Analysen aktivieren oder deaktivieren
- Aktivierung, Deaktivierung oder Änderung der Single Sign-on (SSO)/SAML-Einstellungen
- Aktivierung, Deaktivierung von SCIM
- Token-Erstellung für SCIM API
- Aktivierung, Deaktivierung der SCIM-Benachrichtigungen
- Aktivierung, Deaktivierung oder Änderung der [Zulassungsliste](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Aktivierung, Deaktivierung der Freigabe für Gäste außerhalb der zugelassenen Domains
- Aktivierung, Deaktivierung der Freigabe [über öffentlichen Link](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Aktivierung, Deaktivierung der Freigabe [über öffentlichen Link zur Bearbeitung](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Vertraulichkeitsschutz für Teams [aktivieren, deaktivieren](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Domainsteuerungseinstellungen [aktivieren, deaktivieren, aktualisieren](../../canvas-25-admin-features/domain-control/01-domain-control.md)
- Deaktivierte Nutzer [blockieren, freigeben](../../user-management/02-block-deactivated-users.md)
- Ändere [die Anfragenverwaltung](../../user-management/09-request-management-on-enterprise-plan.md) (einschließlich der Änderung der ServiceNow E-Mail-Adresse oder der Service-Desk-URL)
- Einrichtung, Löschung eines Teams
- Änderung des Teamnamens
- Änderung, Löschung des Teamlogos
- Ändere die [Team-Einladungseinstellungen](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Ändere die [Team-Discovery](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Aktiviere oder deaktiviere [Gäste für ein Team](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Ändere die [Standard-Boardfreigabeeinstellungen](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Standard-Projektfreigabeeinstellungen ändern
- Installation, Deinstallation einer App
- [Genehmigung, Einschränkung einer App](../../../integrations-apps/integrations-basics/04-how-to-install-apps.md)
- [Miro AI-Moderation](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md)

**Nutzerverwaltung**

- Einladung eines neuen Teammitglieds
- Umwandlung von Mitglied in Gast
- Umwandlung eines Nutzers in ein Vollmitglied
- Beförderung von Benutzer zum Unternehmens-Admin oder Widerruf
- Beförderung von Benutzer zum Team-Admin oder Widerruf
- Löschung von Benutzer aus Team oder aus dem Unternehmen (wenn Benutzer ein Team verlassen, sind sie sowohl handelnd als auch betroffen)
- Einladung zurückziehen
- Deaktivierung, Reaktivierung eines Nutzers
- Beitritt von Benutzer*in zum Team/Unternehmen

**Boards**

- Öffnen eines Boards
- Erstellung, Löschung, Wiederherstellung eines Boards
- Umbenennung eines Boards
- Änderung der Board-Beschreibung
- Änderung des Board-Covers
- Verschieben des Boards in ein anderes Team
- Hinzufügen eines Boards zum Projekt, Entfernen oder Verschieben in ein anderes Projekt
- Änderung des Board-Eigentümers
- Teilen eines Boards mit einem Betrachter/Kommentator/Bearbeiter
- Nutzer aus einem Board entfernen
- Öffentlichen Link für Board aktivieren, deaktivieren, ändern [öffentlicher Link](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Passwort für ein öffentliches Board aktivieren, deaktivieren, ändern [Passwort für ein öffentliches Board](../../../using-miro/sharing-boards/13-password-protection-for-public-boards.md)
- Teilen eines Boards mit dem Unternehmen aktivieren, deaktivieren, ändern [Teilen eines Boards mit dem Unternehmen](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Teilen eines Boards mit einem Team aktivieren, deaktivieren, ändern [Teilen eines Boards mit einem Team](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Ein Board exportieren, eine Datei von einem Board herunterladen.
- Status erstellt
- Status aktualisiert
- Status gelöscht
- Eine Datei hochladen (veraltet, verfügbar im [Inhaltsprotokoll](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md))

Bitte beachte, das Audit-Protokoll **zeichnet keine** Informationen über Änderungen auf Boards auf.

**Vorlagen**

- Öffnen einer Vorlage
- Erstellung, Löschung, Wiederherstellung einer Vorlage
- Umbenennung einer Vorlage
- Änderung von Template-Eigentümer
- Status erstellt
- Status aktualisiert
- Status gelöscht

**Projekte**

- Erstellung, Löschung eines Projekts
- Umbenennung eines Projekts
- Freigabe eines Projekts mit Nutzer, Entfernen eines Projektteilnehmers
- Aktivierung, Deaktivierung der Teamfreigabe für ein Projekt
- Änderung des Projekteigentümers

**Anmeldungen**

- Anmelden
- Anmeldung fehlgeschlagen
- Abmelden
- Profil gesperrt, entsperrt

:::warning
Login-Ereignisse umfassen die Aktivität von [deaktivierten Nutzern](../../user-management/01-deactivated-users.md).
:::

**Profildetails**

- Änderung der Profildetails
- Anfrage zur Änderung der E-Mail-Adresse
- Änderung der E-Mail-Adresse

**Blueprints**

- Blueprint erstellen
- Blueprint löschen
- Blueprint-Abschnitt erstellen
- Blueprint-Abschnitt löschen
- Blueprint-Eigentümer ändern

**Miro AI**

- Miro AI-Funktion nutzen

### Häufige Fragen

Gibt es eine Möglichkeit, Audit-Protokolle automatisch abzurufen?

Ja, du kannst die [Miro App für Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md) konfigurieren, um Miro Protokolle von Splunk aus zuzugreifen.
