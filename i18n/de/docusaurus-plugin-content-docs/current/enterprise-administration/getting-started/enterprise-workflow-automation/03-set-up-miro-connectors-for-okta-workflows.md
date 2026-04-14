---
title: "Einrichten von Miro-Konnektoren f\xFCr Okta-Workflows"
article_id: 8166481458706
translation_id: 8166481458706
locale: de
sidebar_position: 2
created_at: '2022-10-19T06:52:05Z'
updated_at: '2025-02-26T11:59:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: okta-workflows
---

Miro-Konnektoren für Okta-Workflows ermöglichen es dir, sich wiederholende und mehrstufige Admin-Aufgaben in Miro einfach zu automatisieren. Erfahre, wie du die Workflow-Automatisierung einrichten und die Team- und Nutzerverwaltung vereinfachen kannst.

> **Relevant für:** Enterprise-Preisplan

## Miro-Nutzermanagement-Konnektor

Der Nutzermanagement-Konnektor von Miro ermöglicht unseren Enterprise-Kunden mit aktiviertem SCIM, Nutzer zu ihrer Organisation hinzuzufügen und die Lizenzen und den Status der Nutzer zu verwalten.

**Autorisiere deinen Miro-Nutzermanagement-Konnektor:**

Wenn du zum ersten Mal eine Miro-Nutzermanagement-Karte zu einem Flow hinzufügst, wirst du aufgefordert, eine Verbindung für deine Organisation einzurichten.  Siehe Autorisierung/span>.

**Miro-Nutzermanagement-Konnektor-Aktionskarten:**

|  |  |
| --- | --- |
| **Aktion** | **Beschreibung** |
| Nutzer erstellen | Erstellt einen neuen Nutzer. |
| Person lesen | Suche nach einem bestehenden Nutzer in einer Organisation per E-Mail. |
| Upgrade des Nutzerlizenztyps auf Vollmitglied | Aktualisiert eine vorhandene Nutzerressource und ändert ihren Nutzerlizenztyp auf **Vollmitglied**. |
| Aktualisieren des Nutzerstatus | Aktualisiert eine bestehende Nutzerressource und ändert ihren aktiven Status auf den Wert „true“ oder „false“.Der Miro-Nutzermanagement-Konnektor funktioniert mit deinem SCIM-Token.  Das Miro-Nutzermanagement ist nur für Unternehmen mit aktiviertem SSO und SCIM verfügbar. |

## Autorisierung

Du kannst mehrere Verbindungen erstellen und verwalten, indem du die **Verbindungen** Seite erstellen und verwalten.
Das ist nützlich, wenn du planst, mit mehreren Organisationen zusammenzuarbeiten. Jede Verbindung für den Miro-Nutzermanagement/span>-Konnektor kann sich nur auf eine Miro-Organisation beziehen.

Um SCIM zu aktivieren und ein neues Token zu erhalten oder ein vorhandenes Token zu kopieren, folgen Sie den Anweisungen unter [Wie aktiviere ich SCIM?](https://developers.miro.com/docs/how-to-enable-scim).
Erstellen einer neuen Verbindung von einer Aktionskarte:

1. Klicke auf **Neue Verbindung**.
2. Gib einen **Verbindungsnamen ein**.  Wir empfehlen einen Namen, der die Organisation repräsentiert.
3. Aktiviere die SCIM-Bereitstellung auf der [Enterprise-Integrationsseite von Miro, indem du den](https://developers.miro.com/docs/how-to-enable-scim) Anweisungen folgst.
   1. Kopiere die **Basis-URL** aus Miro füge sie in das Feld **Basis-URL** in der Verbindung ein.
   2. Kopiere das **Api-Token** aus Miro und füge es in der Verbindung in das Feld **Zugriffs-Token**ein.
4. Klicke auf **Erstellen**.  Damit speicherst du deine Verbindung und gelangst zu deinem Flow zurück.

### Nutzer erstellen

Erstellt einen Nutzer in der Organisation.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Nutzerdetails** |  |  |  |
| E-Mail-Adresse | Die E-Mail-Adresse des Nutzers. | String | WAHR |
| Aktiv | Der Status des Nutzers.   - **Wahr**: der Nutzer ist aktiv. - **Falsch**: Die Person ist inaktiv.    Wenn nicht angegeben, lautet die Standardeinstellung **falsch**. | Dropdown | FALSCH |
| Nutzerlizenztyp | Der Lizenztyp des Nutzers.   - **Volllizenz** - **Free**    Wenn nicht angegeben, wird die Nutzerlizenz gemäß der internen Miro-Logik festgelegt, die vom Preisplan der Organisation abhängt. | Dropdown | FALSCH |
| Rolle | Die Rolle des Nutzers in der Organisation.   - **Organisationsmitglied**: Reguläres Mitglied ohne Administratorrechte. - **Organisations-Administrator**: Nutzer mit unternehmensweiten Administratorrechten.    Wenn nicht angegeben, lautet die Standardeinstellung **Organisationsmitglied**. | Dropdown | FALSCH |
| **Name** |  |  |  |
| Familienname | Der Familienname oder Nachname der Person. | String | FALSCH |
| Vorname | Der Vorname des Nutzers. | String | FALSCH |
| Anzeigename | Der Name, der in Miro angezeigt wird. | String | FALSCH |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Nutzer** |  |  |
| ID des Nutzer | Die ID des neuen Nutzers. | String |

### Person lesen

Suche nach einem bestehenden Nutzer in einer Organisation per E-Mail.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Abfrage** |  |  |  |
| E-Mail-Adresse | Die E-Mail-Adresse des zu suchenden Nutzers | String | WAHR |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Nutzer** |  |  |
| ID des Nutzers | Die ID des Nutzer. | Nummer |
| Nutzerlizenztyp | Der Lizenztyp des Nutzers. | Nummer |
| Aktiv | Der Status des Nutzers.  - **Wahr**: der Nutzer ist aktiv. - **Falsch**: Die Person ist inaktiv. | Nummer |
| **Name** |  |  |
| Name des Nutzers | Die E-Mail-Adresse des Nutzers. | Nummer |
| Familienname | Der Familienname oder Nachname der Person. | Nummer |
| Vorname | Der Vorname des Nutzers. | Nummer |
| Anzeigename | Der in Miro angezeigte Name. | Nummer |

### Upgrade des Nutzerlizenztyps auf Vollmitglied

Aktualisiert eine vorhandene Nutzerressource und ändert ihren Nutzertyp (Lizenz) auf **Vollmitglied**.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| Nutzer |  |  |  |
| ID des Nutzers | Die ID des Nutzers. | String | WAHR |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Antwort** |  |  |
| Statuscode | HTTP-Status der Anfrage.  Codes, die eine erfolgreiche Lizenzaktualisierung anzeigen:   - 200, OK    Codes, die eine nicht erfolgreiche Lizenzaktualisierung anzeigen:   - 400, 400: Fehlerhafte Anfrage - 401, 401: Nicht autorisiert - 403, 403: Verboten - 404, nicht gefunden - 409, 409: Konflikt - 429, 429: Zu viele Anfragen | Nummer |

### Aktualisieren des Nutzerstatus

Aktualisiert eine vorhandene Nutzerressource und ändert ihren **aktiven Status** in den Wert „wahr“ oder „falsch“.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| Nutzer |  |  |  |
| ID des Nutzers | Die ID des Nutzers. | String | WAHR |
| Aktiv | Der neue Status des Nutzers.  - **Wahr**: der Nutzer ist aktiv. - **Falsch**: Die Person ist inaktiv. | Dropdown | WAHR |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Antwort** |  |  |
| Statuscode | HTTP-Status der Anfrage.  Codes, die eine erfolgreiche, aktive Statusaktualisierung anzeigen:   - 200, OK    Codes, die eine nicht erfolgreiche, aktive Statusaktualisierung anzeigen:   - 400, 400: Fehlerhafte Anfrage - 401, 401: Nicht autorisiert - 403, 403: Verboten - 404, nicht gefunden - 409, 409: Konflikt - 429, 429: Zu viele Anfragen | Nummer |

## Miro-Admin-Konnektor

Der Miro-Administrations-Konnektor ermöglicht Enterprise-Kunden, Teams zu erstellen und ihre Teameinstellungen und -mitglieder zu verwalten.

**Autorisieren deines Miro-Administrations-Konnektors**:

Wenn du zum ersten Mal eine Miro-Karte zu einem Flow hinzufügst, wirst du aufgefordert, eine Verbindung für deine Organisation einzurichten.  Siehe Autorisierung/span>.

**Miro-Administrations-Konnektor-****Aktionskarten**:

|  |  |
| --- | --- |
| **Aktion** | **Beschreibung** |
| Team erstellen | Erstellt in einer bestehenden Organisation ein neues Team. |
| Teams suchen | Suche nach bestehenden Teams in einer Organisation.  Die ersten zehn übereinstimmenden Datensätze werden aus dem Ergebnissatz ausgewählt. |
| Mitglied zum Team hinzufügen | Fügt einem bestehenden Team ein neues Mitglied hinzu. |
| Teammitgliedsrolle aktualisieren | Aktualisiert eine Teammitgliedsrolle in einem bestehenden Team. |
| Teameinstellungen abrufen | Ruft die Teameinstellungen eines bestehenden Teams ab. |
| Einstellungen der Team-Freigaberichtlinien aktualisieren | Aktualisiert die Einstellungen für die Freigaberichtlinien eines bestehenden Teams. |
| Team-Einladungseinstellungen aktualisieren | Aktualisiert die Einstellungen für die Einladungsrichtlinie eines bestehenden Teams. |
| Team-Zusammenarbeitseinstellungen aktualisieren | Aktualisiert die Einstellungen für die Zusammenarbeitsrichtlinien eines bestehenden Teams. |
| Einstellungen zum Finden von Teams aktualisieren | Aktualisiert die Einstellungen für die Richtlinie zum Finden eines bestehenden Teams. |
| Einstellungen für die Berechtigungsstufe zum Kopieren innerhalb eines Teams aktualisieren | Aktualisiert die Einstellungen für die Kopierzugriffsrichtlinie eines bestehenden Teams. |
| Löschung der Nutzersitzung (Beta) | Löscht alle Sitzungen für eine bestimmte E-Mail-Adresse. |

## Autorisierung

Der Miro-Administrations-Konnektor arbeitet mit dem OAuth-API-Token.  Der Miro-Administrations-Konnektor ist nur für Kundinnen und Kunden mit Enterprises-Preisplan verfügbar. Zum Erstellen einer neuen Verbindung, müssen Nutzer die erforderlichen Berechtigungen haben, um Apps mit den unten aufgeführten unterstützten Bereichen zu installieren.

Du kannst mehrere Verbindungen erstellen und verwalten, indem du die **Verbindungen** Seite erstellen und verwalten.
Das ist nützlich, wenn du planst, mit mehreren Organisationen zusammenzuarbeiten. Jede Verbindung für den Miro-Administrations-Konnektor kann nur auf eine Miro-Organisation zeigen.

Erstellen einer neuen Verbindung von einer Aktionskarte:

1. Klicke auf **Neue Verbindung**.
2. Gib einen **Verbindungsnamen ein**.  Wir empfehlen einen Namen, der die Organisation repräsentiert.
3. Hole dir die **Organisations-ID** und das **Zugriffs-Token** von der Enterprise-Integrationsseite von Miro gemäß den [Anweisungen](02-miro-connector-for-okta-workflows.md).
4. Klicke auf **Erstellen**.  Damit speicherst du deine Verbindung und gelangst zu deinem Flow zurück.

Unterstützte Bereiche:

- organizations:teams:write
- organizations:teams:read

### Team erstellen

Erstellt ein Team in einer bestehenden Organisation.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| = Team |  |  |  |
| Teamname | Der Name des Teams. | String | WAHR |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Antwort** |  |  |
| Team-ID | Die ID des neuen Teams. | String |

### Teams suchen

Suche nach bestehenden Teams in einer Organisation.  Die ersten zehn übereinstimmenden Datensätze werden aus dem Ergebnissatz ausgewählt.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Abfrage** |  |  |  |
| Teamname | Wörter, die mit dem Teamnamen übereinstimmen.  Jedes Team, dessen Name genau diese Wörter enthält, werden als Ergebnissatz zurückgegeben. Teams mit Namen, die vollständig mit der Abfrage übereinstimmen, werden im Ergebnis ganz oben stehen. | String | FALSCH |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Antwort** |  |  |
| **Teams** | Liste mit zehn ersten Teams gefunden. Jedes Team hat die folgenden Felder. | Liste |
| Team-ID | Die ID des Teams | String |
| Name | Name des Teams | String |

### Mitglied zum Team hinzufügen

Fügt einem bestehenden Team ein neues Mitglied hinzu.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Team** |  |  |  |
| Team-ID | Die ID des Teams. | String | WAHR |
| Mitglied |  |  |  |
| Nutzer-E-Mail-Adresse | Die E-Mail-Adresse des Nutzers, den du in das Team aufnehmen möchtest. | String | WAHR |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Antwort** |  |  |
| Mitglieds-ID | Die ID des neuen Teammitglieds. | String |

### Teammitgliedsrolle aktualisieren

Aktualisiert eine Teammitgliedsrolle in einem bestehenden Team.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Team** |  |  |  |
| Team-ID | Die ID des Teams. | String | WAHR |
| Mitglied |  |  |  |
| Mitglieds-ID | Die ID des Teammitglieds. | String | WAHR |
| Rolle | Die neue Rolle des Mitglieds im Team.  - **Mitglied**: reguläres Mitglied. - **Admin**: Mitglied mit Adminrechten im Team. - **Gast des Teams**: Gast mit begrenzten Rechten. | Dropdown | WAHR |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Antwort** |  |  |
| Mitglieds-ID | Die ID des Teammitglieds. | String |
| Rolle | Die neue Rolle, die dem Teammitglied zugewiesen ist.  - **Mitglied**: reguläres Mitglied. - **Admin**: Mitglied mit Administratorrechten im Team. - **team_guest**: Gast mit begrenzten Rechten. | String |

### Teameinstellungen abrufen

Ruft die Teameinstellungen eines bestehenden Teams ab.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| = Team |  |  |  |
| Team-ID | Die ID des Teams. | String | WAHR |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| Team-Einladungseinstellungen |  |  |
| Wer einladen kann | - **Nur Unternehmens-Admins**: Nur Unternehmens-Admins können Mitwirkende einladen. - **Admins**: Unternehmens-Admins und Team-Admins können Teammitglieder einladen. - **all_members**: Alle Teammitglieder können Mitwirkende einladen. | String |
| Externe Nutzer einladen | - **allowed**: Mitwirkende erlauben, die keine Teammitglieder sind. - **Not_allowed**: Keine Mitwirkenden erlauben, die nicht Teammitglieder sind. | String |
| **Team-Zusammenarbeitseinstellungen** |  |  |
| Miteigentümerrolle | - **Aktiviert**: Rolle des Miteigentümers in Boards und Projekten aktivieren. - **disabled**: Miteigentümerrolle in Boards und Projekten deaktivieren. | String |
| **Einstellungen für die Berechtigungsstufe zum Kopieren innerhalb eines Teams** |  |  |
| Kopierberechtigungsstufe | - **anyone**: Alle mit Zugriff auf das Board können vorhandene Board-Inhalte auf neu erstellte Boards kopieren. WARNUNG: Diese Option ist nur verfügbar, wenn **Zugriffsebene kopieren Beschränkung** eingestellt ist auf **jeder**. - **team_members**: Teammitglieder können vorhandene Board-Inhalte in neu erstellte Boards kopieren. - **Team-Editoren**: Teammitglieder mit Bearbeitungsrechten können vorhandene Board-Inhalte in neu erstellte Boards kopieren. - **Board-Eigentümer**: Nur Board-Eigentümer können vorhandene Board-Inhalte in neu erstellte Boards kopieren. | String |
| Kopierberechtigungsstufe – Einschränkungen | - **Jeder**: Teammitgliedern und Nutzer außerhalb des Teams kann die Berechtigung zum Kopieren von Board-Inhalten erteilt werden. - **team_members**: Die Berechtigung zum Kopieren von Board-Inhalten kann nur Teammitgliedern erteilt werden. | String |
| Einstellungen zum Finden von Teams |  |  |
| Finden | - **Verborgen**: Nur eingeladene Nutzer können das Team sehen und darauf zugreifen. - **Anfrage**: Mitglieder der Organisation können das Team finden und den Beitritt zum Team mit Admin-Genehmigung beantragen. - **join**: Mitglieder der Organisation können das Team finden und ihm beitreten. | String |
| **Einstellungen der Team-Freigaberichtlinien** |  |  |
| Standard-Board-Zugriff | - **Privat**: Nur Board-Eigentümer können auf Boards zugreifen. - **view**: Alle im Team können sich Boards ansehen. - **comment**:Alle im Team können Kommentare auf Boards hinzufügen. - **edit**: Alle im Team können Boards bearbeiten. | String |
| Standard-Organisationszugriff | - **Privat**: Nur Board-Eigentümer können auf Boards zugreifen. - **view**: Alle in der Organisation können sich Boards ansehen. - **comment**: Alle in der Organisation können Kommentare auf Boards hinzufügen. - **edit**: Alle in der Organisation können Boards bearbeiten. | String |
| Freigabe in der Organisation | - - **Erlaubt**: Freigabe auf Organisationsebene erlauben. - **Erlaubt mit Bearbeitungsrechten**: Freigabe mit Bearbeitungsrechten auf Organisationsebene erlauben. - **Nicht erlaubt**: Freigabe auf Organisationsebene nicht erlauben. | String |
| Freigabe im Team | - - **allowed**: Freigabe auf Teamebene erlauben. - **Erlaubt mit Bearbeitungsrechten**: Freigabe mit Bearbeitungsrechten auf Teamebene erlauben. - **not_allowed**: Freigabe auf Teamebene nicht erlauben. | String |
| Freigabe über öffentlichen Link | - **allowed**:**Freigabe über öffentlichen Link erlauben.** - **allowed_with_editing**:Freigabe mit Bearbeitungsrechten über öffentlichen Link erlauben. - **not_allowed**:Freigabe über öffentlichen Link nicht erlauben. | String |
| Board zum Team verschieben | - **allowed**: Boards zu einem anderen Team verschieben erlauben. - **not_allowed**: Boards zu einem anderen Team verschieben nicht erlauben. | String |

### Einstellungen der Team-Freigaberichtlinien aktualisieren

Aktualisiert die Einstellungen für die Freigaberichtlinien eines bestehenden Teams.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Team** |  |  |  |
| Team-ID | Die ID des Teams. | String | WAHR |
| Standard-Board-Zugriff | - **Privat**: Nur Board-Eigentümer können auf Boards zugreifen. - **Lesen**: Alle im Team können sich Boards ansehen. - **Kommentieren**: Alle im Team können Kommentare auf Boards hinzufügen. - **Bearbeiten**: Alle im Team können Boards bearbeiten. | Dropdown | FALSCH |
| Standard-Organisations-Zugriff | - **Privat**: Nur Board-Eigentümer können auf Boards zugreifen. - **Lesen**: Alle im Team können sich Boards ansehen. - **Kommentieren**: Alle im Team können Kommentare auf Boards hinzufügen. - **Bearbeiten**: Alle im Team können Boards bearbeiten. | Dropdown | FALSCH |
| Freigabe über öffentlichen Link | - **allowed**:Freigabe über öffentlichen Link erlauben. - **allowed_with_editing**:Freigabe mit Bearbeitungsrechten über öffentlichen Link erlauben. - **Nicht erlaubt**: Freigabe über öffentlichen Link nicht erlauben. | Dropdown | FALSCH |
| Freigabe im Team | - **allowed**: Freigabe auf Teamebene erlauben. - **Erlaubt mit Bearbeitungsrechten**: Freigabe mit Bearbeitungsrechten auf Teamebene erlauben. - **not_allowed**: Freigabe auf Teamebene nicht erlauben. | Dropdown | FALSCH |
| Freigabe in der Organisation | - **Erlaubt**: Freigabe auf Organisationsebene erlauben. - **Erlaubt mit Bearbeitungsrechten**: Freigabe mit Bearbeitungsrechten auf Organisationsebene erlauben. - **Nicht erlaubt**: Freigabe auf Organisationsebene nicht erlauben. | Dropdown | FALSCH |
| Board zum Team verschieben | - **Erlaubt** Boards in ein anderes Team verschieben erlauben. - **Nicht erlaubt** Boards in ein anderes Team verschieben nicht erlauben. | Dropdown | FALSCH |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Einstellungen der Team-Freigaberichtlinien** |  |  |
| Standard-Board-Zugriff | - **Privat**: Nur Board-Eigentümer können auf Boards zugreifen. - **view**: Alle im Team können sich Boards ansehen. - **comment**:Alle im Team können Kommentare auf Boards hinzufügen. - **edit**: Alle im Team können Boards bearbeiten. | String |
| Standard-Organisations-Zugriff | - **Privat**: Nur Board-Eigentümer können auf Boards zugreifen. - **view**: Alle in der Organisation können sich Boards ansehen. - **comment**: Alle in der Organisation können Kommentare auf Boards hinzufügen. - **edit**: Alle in der Organisation können Boards bearbeiten. | String |
| Freigabe in der Organisation | - - **Erlaubt**: Freigabe auf Organisationsebene erlauben. - **Erlaubt mit Bearbeitungsrechten**: Freigabe mit Bearbeitungsrechten auf Organisationsebene erlauben. - **Nicht erlaubt**: Freigabe auf Organisationsebene nicht erlauben. | String |
| Freigabe im Team | - - **allowed**: Freigabe auf Teamebene erlauben. - **allowed_with_editing**: Freigabe mit Bearbeitungsrechten auf Teamebene erlauben. - **not_allowed**: Freigabe auf Teamebene nicht erlauben. | String |
| Freigabe über öffentlichen Link | - - **allowed**:Freigabe über öffentlichen Link erlauben. - **allowed_with_editing**:Freigabe mit Bearbeitungsrechten über öffentlichen Link erlauben. - **not_allowed**:Freigabe über öffentlichen Link nicht erlauben. | String |
| Board zum Team verschieben | - **allowed**: Boards zu einem anderen Team verschieben erlauben. - **not_allowed**: Boards zu einem anderen Team verschieben nicht erlauben. | String |

### Team-Einladungseinstellungen aktualisieren

Aktualisiert die Einstellungen für die Einladungsrichtlinie eines bestehenden Teams.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Team** |  |  |  |
| Team-ID | Die ID des Teams. | String | WAHR |
| Externe Nutzer einladen | - **Erlaubt**: Mitwirkende erlauben, die nicht Mitglieder des Teams sind. - **Nicht erlaubt** Keine Mitwirkenden erlauben, die nicht Mitglieder des Teams sind. | Dropdown | FALSCH |
| Wer einladen kann | - **Nur Unternehmens-Admins**: Nur Unternehmens-Admins können Mitwirkende einladen. - **Admins**: Unternehmens-Admins und Team-Admins können Teammitglieder einladen. - **Alle Mitglieder**: Alle Teammitglieder können Mitwirkende einladen. | Dropdown | FALSCH |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Team-Einladungseinstellungen** |  |  |
| Externe Nutzer einladen | - **allowed**: Mitwirkende erlauben, die keine Teammitglieder sind. - **Not_allowed**: Keine Mitwirkenden erlauben, die nicht Teammitglieder sind. | String |
| Wer einladen kann | - **Nur Unternehmens-Admins**: Nur Unternehmens-Admins können Mitwirkende einladen. - **Admins**: Unternehmens-Admins und Team-Admins können Teammitglieder einladen. - **all_members**: Alle Teammitglieder können Mitwirkende einladen. | String |

### Einstellungen für die Berechtigungsstufe zum Kopieren innerhalb eines Teams aktualisieren

Aktualisiert die Einstellungen für die Kopierzugriffsrichtlinie eines bestehenden Teams.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Team** |  |  |  |
| Team-ID | Die ID des Teams. | String | WAHR |
| Kopierberechtigungsstufe – Einschränkungen | - **anyone**: Alle mit Zugriff auf das Board können vorhandene Board-Inhalte auf neu erstellte Boards kopieren. - **Teammitglieder**: Teammitglieder können vorhandene Board-Inhalte in neu erstellte Boards kopieren. - **Team-Bearbeiteren**: Teammitglieder mit Bearbeitungsrechten können bestehende Board-Inhalte in neu erstellte Boards kopieren. - **Board-Eigentümer**: Nur Board-Eigentümer können vorhandene Board-Inhalte in neu erstellte Boards kopieren. | Dropdown | FALSCH |
| Kopierberechtigungsstufe – Einschränkungen | - **Jeder**: Teammitgliedern und Nutzer außerhalb des Teams kann die Berechtigung zum Kopieren von Board-Inhalten erteilt werden. - **Teammitglieder**: Nur Teammitgliedern kann die Berechtigung zum Kopieren von Board-Inhalten erteilt werden. | Dropdown | FALSCH |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Einstellungen für die Berechtigungsstufe zum Kopieren innerhalb eines Teams** |  |  |
| Kopierberechtigungsstufe | - **anyone**: Alle mit Zugriff auf das Board können vorhandene Board-Inhalte auf neu erstellte Boards kopieren. - **team_members**: Teammitglieder können vorhandene Board-Inhalte in neu erstellte Boards kopieren. - **Team-Editoren**: Teammitglieder mit Bearbeitungsrechten können vorhandene Board-Inhalte in neu erstellte Boards kopieren. - **Board-Eigentümer**: Nur Board-Eigentümer können vorhandene Board-Inhalte in neu erstellte Boards kopieren. | String |
| Kopierberechtigungsstufe – Einschränkungen | - **Jeder**: Teammitgliedern und Nutzer außerhalb des Teams kann die Berechtigung zum Kopieren von Board-Inhalten erteilt werden. - **team_members**: Die Berechtigung zum Kopieren von Board-Inhalten kann nur Teammitgliedern erteilt werden. | String |

### Team-Zusammenarbeitseinstellungen aktualisieren

Aktualisiert die Einstellungen für die Zusammenarbeitsrichtlinien eines bestehenden Teams.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Team** |  |  |  |
| Team-ID | Die ID des Teams. | String | WAHR |
| Rolle des Miteigentümers | - **Aktiviert**: Rolle des Miteigentümers in Boards und Projekten aktivieren. - **Deaktiviert**: Miteigentümerrolle in Boards und Projekten deaktivieren. | Dropdown | FALSCH |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Team-Zusammenarbeitseinstellungen** |  |  |
| Miteigentümerrolle | - **Aktiviert**: Rolle des Miteigentümers in Boards und Projekten aktivieren. - **disabled**: Miteigentümerrolle in Boards und Projekten deaktivieren. | String |

### Einstellungen zum Finden von Teams aktualisieren

Aktualisiert die Einstellungen für die Richtlinie zum Finden eines bestehenden Teams.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Team** |  |  |  |
| Team-ID | Die ID des Teams. | String | WAHR |
| Finden | - **Verborgen**: Nur eingeladene Nutzer können das Team sehen und darauf zugreifen. - **Anfrage**: Mitglieder der Organisation können das Team finden und den Beitritt zum Team mit Admin-Genehmigung beantragen. - **Beitreten**: Mitglieder der Organisation können das Team finden und ihm beitreten. | Dropdown | FALSCH |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Einstellungen zum Finden von Teams** |  |  |
| Finden | - **Verborgen**: Nur eingeladene Nutzer können das Team sehen und darauf zugreifen. - **Anfrage**: Mitglieder der Organisation können das Team finden und den Beitritt zum Team mit Admin-Genehmigung beantragen. - **join**: Mitglieder der Organisation können das Team finden und ihm beitreten. | String |

### Löschung der Nutzersitzung

Löscht alle Sitzungen für eine bestimmte E-Mail-Adresse.

Eingabe

|  |  |  |  |
| --- | --- | --- | --- |
| **Feld** | **Definition** | **Typ** | **Erforderlich** |
| **Nutzerdetails** |  |  |  |
| E-Mail-Adresse | Die E-Mail-Adresse der Person, deren Sitzungen gelöscht werden sollen. | String | WAHR |

Ausgabe

|  |  |  |
| --- | --- | --- |
| **Feld** | **Definition** | **Typ** |
| **Antwort** |  |  |
| Statuscode | HTTP-Status der Anfrage.  Codes, die eine erfolgreiche Aktualisierung der Nutzersitzung anzeigen:   - 200, 200: Nutzersitzung gelöscht    Codes, die eine fehlgeschlagene Aktualisierung der Nutzersitzung anzeigen:   - 400, 400: Fehlerhafte Anfrage - 401, 401: Nicht autorisiert - 403, 403: Verboten - 404, nicht gefunden - 409, 409: Konflikt - 429, 429: Zu viele Anfragen | Nummer |
