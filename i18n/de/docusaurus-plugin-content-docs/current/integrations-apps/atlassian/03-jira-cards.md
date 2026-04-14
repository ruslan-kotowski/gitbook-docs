---
title: Jira-Karten
article_id: 360017572434
translation_id: 6634752327058
locale: de
sidebar_position: 5
created_at: '2022-07-15T14:22:34Z'
updated_at: '2025-11-25T15:59:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Pläne: Starter, Business, Education, Enterprise Personen: Alle Nutzer Plattformen:
    Browser, Desktop, Mobil Jira: Jira Cloud, Jira Server (lokal), Jira Data Center'
---

Mit Jira-Karten kannst du Jira-Vorgänge direkt in Miro-Boards bearbeiten. Diese Integration optimiert den Workflow deines Teams, indem sie Jira-Vorgänge in deinen kollaborativen Arbeitsbereich für Retrospektiven, Story Sizing, Backlog-Priorisierung, Story Mapping und andere Teamaktivitäten bringt.

![Jira cards in user story mapping](../../../../../../docs/integrations-apps/atlassian/images/21017348097170_Jira%20cards%20in%20USM.png)

## Jira-Vorgänge in dein Board importieren

Du kannst Jira-Vorgänge auf zwei Arten in dein Board importieren:

1. Kopiere die URL des Jira-Vorgangs und füge sie in das Board ein.
2. Klicke auf das Symbol **Tools, Medien und Integrationen** (**+**) in der Erstellungssymbolleiste, wähle **Jira-Karten** aus, wähle ein oder mehrere Vorgänge aus und klicke auf **Hinzufügen**.

Beim erstmaligen Importieren von Vorgängen musst du dein Jira-Konto verbinden:

1. Klicke im angezeigten Dialogfeld auf **Autorisieren**.
2. Melde dich mit deinen Anmeldeinformationen in deinem Jira-Konto an.
3. Erteile die Berechtigung zur Verbindung zwischen Miro und Jira.

Nach der Autorisierung siehst du im Jira-Karten-Auswähler alle Jira-Vorgänge, auf die du Zugriff hast.

:::note
Nutzern, die ihr Jira-Konto nicht autorisiert haben, wird eine vereinfachte Kartenansicht ohne die Avatare der Zuständigen angezeigt.
:::

## Neue Jira-Vorgänge erstellen

Du kannst Jira-Vorgänge direkt aus Miro auf zwei Arten erstellen.

### Erstellen mit der Jira-App

1. Klicke auf das Symbol **Tools, Media und Integrationen** (**+**) in der Erstellungssymbolleiste
2. Wähle **Jira-Karten** aus.
3. Klicke auf **Vorgang erstellen**.
4. Fülle die erforderlichen Felder aus.
5. Klicke auf **Erstellen**.

### Existierende Elemente in Jira-Vorgänge umwandeln

Du kannst bestehende Notizen oder Karten auf deinem Board in Jira-Vorgänge umwandeln.

1. Wähle bis zu 50 Notizen oder Karten aus.
2. Klicke im Kontextmenü auf **In** > **Jira umwandeln**.
3. Lege die Standardwerte fest (Vorgangstyp, Priorität, Zuweisung usw.).
4. Klicke auf **Umwandeln**.

:::warning
Hinweis:

- Karten in der USM-Aufgabenreihe können nicht in Jira-Vorgänge umgewandelt werden.
- Während der Umwandlung gehen die Tags und das Startdatum von Miro-Karten verloren.
- Informationen zum Bearbeiter müssen nach der Konvertierung erneut festgelegt werden.
:::

## Jira-Vorgänge ansehen und bearbeiten

:::warning
Die Bearbeitung von Jira-Karten wird in der Desktop- oder mobilen App nicht unterstützt.
:::

Du kannst Jira-Karten auf zwei Arten ansehen:

- Seitenansicht
- Zentrierte Ansicht

### Vorgänge in Miro bearbeiten

1. Klicke auf das Symbol **Im seitlichen Feld öffnen** oder **Im mittleren Feld öffnen**.
2. Nimm deine Änderungen vor.
3. Klicke auf **Aktualisieren**, um zu speichern.

### Vorgangsstatus ändern

1. Klicke auf das **Workflow**-Symbol.
2. Wähle den gewünschten **Status** und **Kommentar** aus.
3. Klicke auf **Aktualisieren**, um zu speichern.

### Bearbeiten in Jira

1. Wähle eine Karte aus und klicke auf das **Symbol Quelle**.
2. Bearbeite den Vorgang in Jira im neuen Browser-Tab.
3. Änderungen werden automatisch mit der Miro-Karte synchronisiert.

## Synchronisation zwischen Miro und Jira

|  |  |
| --- | --- |
| **Jira-Instanz-Update vs. Miro-Karten-Update** | **Wann erfolgt das Update?** |
| Update in Jira über OAuth 1.0 und OAuth 2.0 | Miro-Jira-Karte wird sofort über [Webhook](https://help.miro.com/hc/articles/360017731113) aktualisiert. |
| Update in Miro | Die Miro-Jira-Karte wird sofort aktualisiert. Dabei wird gleichzeitig der entsprechende Jira-Vorgang aktualisiert. |

## Anpassen von Jira-Karten

### Kartfarben ändern

1. Wähle eine oder mehrere Jira-Karten aus.
2. Klicke im Kontextmenü auf **Füllfarbe**.
3. Wähle die gewünschte Farbe aus.

### Benutzerdefinierte Felder konfigurieren

1. Klicke auf das Symbol **Tools, Media and Integrations** (**+**) in der Erstellungssymbolleiste
2. Wähle **Jira-Karten** aus.
3. Wähle **Karten konfigurieren** aus.
4. Wähle die Felder aus, die du anzeigen möchtest.
5. Klicke auf **Speichern**.

:::note
Wichtige Hinweise zu Feldern:

- Einstellungen gelten nur für das aktuelle Board.
- Standardfelder (Bearbeiter, Vorgangstyp, Priorität, Status) können nicht entfernt werden.
- Felder werden möglicherweise nicht angezeigt, wenn sie keinen Wert haben oder für den Vorgangstyp nicht verfügbar sind.
- Einige Feldtypen (wie benutzerdefinierte Farb-Felder) werden nicht unterstützt.
:::

## Nach Jira-Vorgängen suchen

Der Jira-Karten-Auswahlbereich zeigt zuerst die zuletzt bearbeiteten Aufgaben an und bietet verschiedene Sortieroptionen:

- Problemtyp
- Priorität
- Schlüssel
- Zusammenfassung
- Bearbeitende Person
- Status

Nutze Schlüsselwörter, um spezifische Vorgänge zu finden oder verwende die **Jira Query Language** (JQL) für komplexe Suchen:

1. Wähle den Schalter **Erweiterte Suche** in der Suchleiste.
2. Gib deine JQL-Abfrage ein.

Die Ergebnisse werden basierend auf deiner Abfrage aktualisiert.

## Verwandte Artikel

- [Jira-Karten Häufige Fragen](https://help.miro.com/hc/articles/360013463739)
- [Jira-Karten einrichten und deinstallieren](https://help.miro.com/hc/articles/360019501754)
- [Webhooks für Jira-Karten einrichten](https://help.miro.com/hc/articles/360017731113)
- [Probleme mit Jira-Karten beheben](https://help.miro.com/hc/articles/360017572654)
