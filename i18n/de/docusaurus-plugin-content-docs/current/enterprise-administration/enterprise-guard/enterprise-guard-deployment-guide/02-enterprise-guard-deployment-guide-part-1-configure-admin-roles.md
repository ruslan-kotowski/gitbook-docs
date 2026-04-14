---
title: "Enterprise Guard Einf\xFChrungshandbuch Teil 1: Admin-Rollen konfigurieren"
article_id: 17120595534994
translation_id: 17120595534994
locale: de
sidebar_position: 1
created_at: '2024-02-19T09:19:59Z'
updated_at: '2025-11-25T15:41:04Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Unternehmens-Admins können sich selbst und anderen zusätzliche Admin-Rollen zuweisen, sobald Enterprise Guard aktiviert ist. Daher sollte die Anzahl der Unternehmens-Admins in deinem Unternehmen so gering wie möglich gehalten werden. Überprüfe sorgfältig deine bestehende Admin-Konfiguration und versetze Unternehmens-Admins in andere Rollen (z.B. Team- oder Nutzer-Admin), wenn dies für die Balance zwischen Sicherheit, Compliance und betrieblicher Effizienz angemessen ist.

Obwohl es empfohlen wird, ist eine ganzheitliche Neubewertung deiner Admin-Konfiguration nicht erforderlich, um Enterprise Guard einzusetzen. Mach weiter mit [Teil 2: Setze die Datensicherheit](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md) nach eigenem Ermessen ein.

## Miro Admin Rollen Übersicht

Hier findest du eine Liste der verfügbaren Admin-Rollen in Miro, einschließlich einer Beschreibung der Aufgaben und für wen sie in einer typischen Organisation geeignet sind.

:::note
Hinweise:
- Diese Liste der Rollen und Berechtigungen wird ständig erweitert. Diese Seite wird regelmäßig aktualisiert.
- Um einem Nutzer die Rolle des Datenverwaltungs-Admins oder des Admins für sensible Inhalte zuzuweisen, musst du ein Unternehmens-Admin sein.
:::

|  |  |  |
| --- | --- | --- |
| **Rolle des Admins** | **Zuständigkeiten** | **Empfohlen für** |
| **Unternehmens-Admin** | Verantwortlich für das übergreifende Management und die Delegierung bestimmter Aufgaben an andere Admin-Rollen. Du solltest ein umfassendes Verständnis der betrieblichen Anforderungen und Compliance-Verpflichtungen des Unternehmens haben. | - Leitende IT-Administratoren - AbteilungsleiterInnen - Projektmanager - Teamleiter/innen - Betriebsleiterinnen und Betriebsleiter - Business-Technologie-Manager - Eigentümer des Miro-Produkts |
| **Team-Admins** | Verwalte die teamspezifischen Einstellungen und den Zugriff der Nutzer innerhalb ihrer jeweiligen Teams. Sorgt für die Autonomie des Teams und richtet sich gleichzeitig nach den allgemeinen Richtlinien der Organisation. | - AbteilungsleiterInnen - Projektmanager - Teamleiter/innen - Betriebsleiterinnen und Betriebsleiter |
| **Nutzer-Admins** | Verwalte die Nutzerverwaltung und die Lizenzierung. Ideal für die Verwaltung von Zugriffen und Konten der Mitarbeiter. Verwalte Nutzer effizient, ohne Unternehmens- oder Team-Admins zu überfordern. | - IT-Manager - IT-Administratoren - IT Service Desk |
| **Datenverwaltungs-Admins (Enterprise Guard)** | Verantwortlich für Compliance und Datenverwaltung. Du solltest die rechtlichen und regulatorischen Rahmenbedingungen für die Daten der Organisation kennen, einschließlich der Richtlinien zur Aufbewahrung und Löschung der Daten. | - Chief Compliance Officer (CCO) - Manager für Datenverwaltung - Compliance Manager - Manager für regulatorische Angelegenheiten - Risk Manager - Records Manager - eDiscovery Analyst - Forensik-Analyst |
| **eDiscovery Admins (Enterprise Guard)** | Verwalte die Einstellungen für Legal Hold, um Boards zu erhalten, die für laufende Ermittlungen oder Rechtsfälle relevant sind. Dazu gehört das Erstellen, Ändern und Freigeben von rechtlichen Sperren oder Fällen, um die dauerhafte Löschung von Inhalten zu verhindern und die Compliance mit rechtlichen und behördlichen Verpflichtungen zu gewährleisten. Diese Rolle ist wichtig für Organisationen, die eine strenge Datenaufbewahrung zur Unterstützung von Gerichtsverfahren und Compliance-Vorschriften benötigen. | - Rechtsbeistand - eDiscovery-Spezialisten - Compliance-Beauftragte - Risiko-Manager - Forensik-Analysten - Chief Information Security Officer (CISO) - Datenschutzbeauftragter (DSB) - Datenschutzbeauftragter/Datenschutzmanager |
| **Admins für sensible Inhalte (Enterprise Guard)** | Verantwortlich für Datenschutz und Privatsphäre. Entscheidend für die Klassifizierung, Verwaltung und den Schutz sensibler Informationen im gesamten Unternehmen. Wichtig für den Umgang mit PII, PHI, PCI oder geistigem Eigentum. | - Chief Information Security Officer (CISO) - Datenschutzbeauftragter (DSB) - Datenschutzbeauftragter/Datenschutzmanager - Cybersecurity Analyst - IT Security Consultant |

:::tip
Erfahre mehr über die [Rollen der Admins und ihre Berechtigungen](../enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) im Enterprise-Preisplan.
:::

## Detaillierte Enterprise Guard Berechtigungs- und Admin-Rollenmatrix

In der folgenden Tabelle sind die detaillierten Berechtigungen und die Matrix der Admin-Rollen für jede Funktion aufgeführt.

|  |  |  |  |
| --- | --- | --- | --- |
| **Inhaltslebenszyklus-Management** | | |  |
| **Berechtigung** | **Datenverwaltungs-Admin** | **Admin für sensible Inhalte** | **eDiscovery-Admin** |
| Papierkorbeinstellungen aufrufen |  |  |  |
| Papierkorb-Einstellungen bearbeiten |  |  |  |
| Aufbewahrungsrichtlinie hinzufügen |  |  |  |
| Aufbewahrungsrichtlinie bearbeiten |  |  |  |
| Aufbewahrungsrichtlinie löschen |  |  |  |
| Löschungsrichtlinie hinzufügen |  |  |  |
| Löschungsrichtlinie bearbeiten |  |  |  |
| Löschungsrichtlinie löschen |  |  |  |
| **Datenklassifizierung** | | |  |
| **Berechtigung** | **Datenverwaltungs-Admin** | Admin für sensible Inhalte | **eDiscovery-Admin** |
| Datenklassifizierungseinstellungen aufrufen |  |  |  |
| Klassifizierungsstufen bearbeiten |  |  |  |
| Einstellungen für die automatische Klassifizierung bearbeiten |  |  |  |
| Einstellungen für Klassifizierungsvorgaben bearbeiten |  |  |  |
| Standardklassifizierungsstufe bearbeiten |  |  |  |
| **Datenerkennung** | | |  |
| **Berechtigung** | **Datenverwaltungs-Admin** | **Admin für sensible Inhalte** | **eDiscovery-Admin** |
| Datenschutzlabels aufrufen |  |  |  |
| Erkennung datenschutzrelevanter Daten aktivieren/deaktivieren |  |  |  |
| Anzahl der Übereinstimmungen aufrufen – Datenschutzlabels |  |  |  |
| Zensierte Übereinstimmungen aufrufen – Datenschutzlabels |  |  |  |
| Vollständige Übereinstimmungen aufrufen – Datenschutzlabels |  |  |  |
| **eDiscovery** | | |  |
| **Berechtigung** | **Datenverwaltungs-Admin** | **Admin für sensible Inhalte** | **eDiscovery-Admin** |
| Einstellungen für Aufbewahrungsfristen verwalten |  |  |  |
| Einstellungen für Aufbewahrungsfristen anzeigen |  |  |  |

*Tabelle 2: Detaillierte Berechtigungen und Admin Rollen Matrix für jedes Feature*

## Die Umstellung deiner Admin-Konfiguration

### Überprüfe deine aktuelle Admin-Konfiguration

Überprüfe die Liste der Nutzer, die in Miro über Admin-Rechte verfügen, und ihre Zuständigkeiten. Verwende das Admin Configuration Assessment Tool, um eine Zusammenfassung des aktuellen Zustands zu erstellen.

- Filtere die Liste der Nutzer aus dem Abschnitt **Aktive Nutzer** der Unternehmenseinstellungen, um Unternehmens-Admins anzusehen.
- Sieh dir die Liste der Nutzer-Admins, Datenverwaltungs-Admins und Admin für sensible Inhalte in der **Rolle Admin** in den Einstellungen des Unternehmens an.

### Eine neue Admin-Konfiguration mappen

Vergleiche deine aktuelle Admin-Konfiguration mit der obigen Tabelle und den Richtlinien deines Unternehmens. Verwende das Admin Configuration Assessment Tool, um eine neue Konfiguration zu erstellen.

Überlege dir Fragen wie diese:

- Wer braucht die Rolle der Datenverwaltung?
- Wer braucht die Rolle "Sensibler Inhalt"?
- Welche Unternehmens-Admins können zu Nutzer-Admins umgewandelt werden?
- Welche Unternehmens-Admins können in Team-Admins umgewandelt werden?

### Rollen neu zuweisen und Nutzer informieren

In den folgenden Artikeln des Hilfecenters erfährst du, wie du die verschiedenen Rollen zuweisen kannst. Du kannst die mitgelieferten E-Mail-Vorlagen anpassen, um die Nutzer über Übergänge zu informieren.

- [Wie man Unternehmens-Admins und Team-Admins zuweist](../../../administration/user-management/06-how-to-manage-admin-roles.md)
- [Wie man Nutzer-Admins, Datenverwaltungs-Admins und Admins für sensible Inhalte zuweist](../enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)

### zuweisen. die Rolle des Datenverwaltungs-Admins Rolle

:::note
Um einem Nutzer die Rolle des Datenverwaltungs-Admins zuzuweisen, musst du ein Unternehmens-Admin sein.
:::

1. Gehe zu deinen Profileinstellungen.
   - Von einem Board aus: **Hauptmenü > Präferenzen > Profileinstellungen**.- Vom Dashboard aus: Klicke auf deinen Avatar in der oberen rechten Ecke und dann auf **Einstellungen**.
   - Von der URL `https://miro.com/app/settings`: Wähle dein Unternehmen aus der Liste oben links aus.
2. Klicke **unter Nutzerverwaltung auf Admin-Rollen.**
3. Klicke im rechten Bereich auf die **Ellipse (**...) für **Datenverwaltungs-Admin** **und wähle dann** Rolle zuweisen aus.
4. Wähle die Person aus, der du die Rolle „Datenverwaltungs-Admin“ zuweisen möchtest, scrolle bis zum unteren Rand des Fensters und klicke dann auf **Zuweisen**.

### zuweisen. die Rolle Admin für sensible Inhalte Rolle

:::note
Um einem Nutzer die Rolle Admin für sensible Inhalte zuzuweisen, musst du ein Unternehmens-Admin sein.
:::

1. Gehe zu deinen Profileinstellungen.
   - Von einem Board aus: **Hauptmenü > Präferenzen > Profileinstellungen**.- Vom Dashboard aus: Klicke auf deinen Avatar in der oberen rechten Ecke und dann auf **Einstellungen**.
   - Von der URL `https://miro.com/app/settings`: Wähle dein Unternehmen aus der Liste oben links aus.
2. Klicke **unter Nutzerverwaltung auf Admin-Rollen.**
3. OIm rechten Fensterbereich klickst du auf die Ellipse **Admin für sensible Inhalte** **(****...)**und wähle dann **Rolle zuweisen**.
4. Wähle den Nutzer aus, dem du die Rolle Admin für sensible Inhalte zuweisen möchtest, scrolle zum unteren Rand des Fensters und klicke dann auf **zuweisen.**.

### zuweisen. die Rolle eDiscovery Admin Rolle

:::note
Um einem Nutzer die Rolle des eDiscovery-Admins zuzuweisen, musst du ein Unternehmens-Admin sein.
:::

1. Gehe zu deinen Profileinstellungen.
   - Von einem Board aus: **Hauptmenü > Präferenzen > Profileinstellungen**.- Vom Dashboard aus: Klicke auf deinen Avatar in der oberen rechten Ecke und dann auf **Einstellungen**.
   - Von der URL `https://miro.com/app/settings`: Wähle dein Unternehmen aus der Liste oben links aus.
2. Klicke **unter Nutzerverwaltung auf Admin-Rollen.**
3. OIm rechten Bereich klickst du auf die Ellipse **eDiscovery Admin** **(****...)**und wähle dann **Rolle zuweisen**.
4. Wählen Sie den Nutzer aus, dem Sie die Rolle eDiscovery Admin zuweisen möchten, scrollen Sie zum unteren Rand des Fensters und klicken Sie dann auf **zuweisen.**.

### Ressourcen

- [Admin Configuration Assessment Tool](https://docs.google.com/spreadsheets/d/1a0WQc-fBpuVwfnoY8VCx66PjOXS76q7DJ__xDYcp8rk/edit?usp=sharing) (Kopie erstellen)
- [E-Mail Vorlagen | Admin Konfiguration Kommunikation](https://docs.google.com/document/d/18Kw4GNPq7GnAx8R8co5PaZ04peVogfVDgsdKK2MuARM/edit?usp=sharing) (kopieren)
