---
title: Azure-Karten
article_id: 360033799934
translation_id: 360033799934
locale: de
sidebar_position: 4
created_at: '2019-08-13T10:01:30Z'
updated_at: '2025-11-25T16:05:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: azure-cards
availability:
  notes: 'Personen: Alle Nutzer Preispläne: Business, Enterprise Plattformen: Browser,
    Desktop, Mobile'
---

Azure-Karten erlauben es dir, Arbeitselemente von Azure Boards (ein Teil der Azure DevOps-Dienste, ehemals VSTS - Cloud-Lösung) in deine Miro-Boards zu importieren. Sie können ein wesentlicher Bestandteil deiner Remote-Retrospektiven, Story Sizing, Backlog-Priorisierung, Story Mapping und anderen Teamaktivitäten werden. Außerdem kannst du sie mit Miro Kanban und User-Story-Mapping-Frameworks verwenden.

Azure-Karten verbessern dein Miro-Erlebnis, indem sie sich direkt in Azure Boards integrieren lassen und ein nahtloses Workflow-Management für verschiedene Teamaktivitäten ermöglichen.

## Wichtige Funktionen

Die Azure Cards-Integration bietet mehrere wichtige Funktionen:

- Importiere Azure-Karten mit der In-App-Auswahl von Azure-Boards für Arbeitselemente. Dies beinhaltet verschiedene Sortieroptionen
- Nach Arbeitselementen von Azure Boards in der In-App-Auswahl suchen
- Automatisierte, leicht lesbare Änderungen der Kartenansicht beim Vergrößern und Verkleinern

:::note
Stelle sicher, dass deine Azure-Karten immer mit Kartenumfragen aktualisiert werden, sodass die Nutzer immer Kartenaktualisierungen erhalten, selbst wenn [Webhooks](../atlassian/14-how-to-set-up-webhooks-for-jira-data-center.md) ausfallen.
:::

## Die Integration Azure-Karten einrichten

Die Einrichtung ist auf zwei Ebenen erforderlich:

1. Die App muss entweder auf Organisationsebene für alle Teams hinzugefügt werden oder auf Teamebene für bestimmte Teams.
2. Sobald die App hinzugefügt wurde, muss die Integration auf persönlicher Ebene verbunden und autorisiert werden, um Azure-Karten zu importieren.

Dieser Prozess erfordert spezifische administrative Berechtigungen sowohl in Miro als auch in Azure DevOps.

:::note
Um Azure-Karten in Miro erfolgreich einzurichten, **müssen der Azure-Admin und der Miro-Admin dasselbe Konto haben**.

Beachte bitte: Das Hinzufügen von Azure-Karten erfordert Miro-Team- oder Unternehmens-Admin-Berechtigungen **und** Projektsammlungsadministrator-Gruppenberechtigungen in Azure Boards. Nach Abschluss der Verbindung können diese Berechtigungen jedoch herabgestuft werden. Die Admins können allerdings nicht entfernt werden und müssen weiterhin auf das Azure-Projekt zugreifen können.
:::

### Azure-Karten für deine Organisation oder dein Team hinzufügen

Unternehmens-Admins von Miro können Azure-Karten für alle Teams hinzufügen, während Team-Admins sie für bestimmte von ihnen verwaltete Teams hinzufügen können. Dieser Schritt macht die Azure-Karten-App zur Verbindung verfügbar.

:::note
Um Azure-Karten auf Teamebene zu verbinden, musst du Team-Admin sein.
:::

1. Gehe zu deinen **Profileinstellungen** (klicke auf das Dreistrich-Menü im Hauptmenü und wähle **Profileinstellungen** aus, oder klicke im Dashboard oben rechts auf deinen Avatar und wähle **Einstellungen** aus).
2. Klicke auf **Apps** und navigiere dann zum Tab **Apps hinzufügen** auf der rechten Seite.
3. Gib „Azure-Karten“ ein und wähle es aus der Dropdown-Liste aus. Klicke auf **Hinzufügen**.
4. Wähle im nächsten Dialogfeld entweder **Alle Teams** oder **In bestimmten Teams** aus (wähle dein Team aus, falls erforderlich) und klicke dann auf **Nächster Schritt**.
5. Klicke im Bildschirm „Azure-Karten überprüfen und hinzufügen“ auf **Hinzufügen**. Die App wird zu deinem Unternehmen oder deinem Team hinzugefügt.
6. Gehe zum **Apps verwalten** Tab, suche nach Azure-Karten und klicke auf **Genehmigen**. Die App wird jetzt auf Unternehmens- oder Teamebene genehmigt.
7. Als Nächstes verbindest du deine Azure-Organisation mit Miro. Gehe im Apps-Panel zu **Apps verwalten.**
8. Suche in deiner Apps-Liste nach „Azure-Karten“ und klicke auf **Einstellungen.**
9. Füge im Einstellungsfeld für Azure-Karten die URL deiner **Azure-Instanz** hinzu und klicke auf **Verbinden**. Gib deine Microsoft Azure-Anmeldeinformationen ein.
10. Klicke im Autorisierungsdialogfeld auf **Akzeptieren**, um die Verbindung von Azure mit Miro abzuschließen.

### Benutzerdefinierte Azure-Karten-Einstellungen für bestimmte Teams anwenden

Wenn du für bestimmte Teams andere Einstellungen als die globale Unternehmensebene benötigst, können Team-Admins dies im Bereich **Team-Apps & Integrationen** konfigurieren.

1. Klicke in deinen Profileinstellungen auf **Teams**.
2. Klicke auf das Team, für das du die benutzerdefinierten Einstellungen festlegen möchtest.
3. Klicke im Teams-Panel auf **Apps & Integrationen**.
4. Suche nach **Azure-Karten** und klicke darauf.
5. Wähle im Bereich „App-Einstellungen“ die Option **Benutzerdefinierte Einstellungen anwenden** aus dem Dropdown-Menü auf der rechten Seite und verbinde dann das Azure-Konto, für das du benutzerdefinierte Einstellungen möchtest.
6. Autorisiere Miro in Azure DevOps mit deinem Microsoft-Konto: Klicke auf **Verbinden** neben „Microsoft-Konto“ und melde dich bei deinem Microsoft-Konto an, damit Miro es nutzen kann.
7. Gib deine **Azure-Organisations-URL** ein (du kannst dies von Azure DevOps kopieren) und klicke auf **Verbinden.** Miro akzeptiert entweder die personalisierte URL deiner Instanz oder die allgemeine `https://dev.azure.com/` Adresse, die mit dem Namen deiner Instanz endet.
   ![Animation, die zeigt, wie benutzerdefinierte Azure-Cards-Einstellungen für ein bestimmtes Team angewendet werden.](../../../../../../docs/integrations-apps/microsoft/images/21017013136658_azure_cards_custom_team_settings.gif)
   *Benutzerdefinierte Einstellungen für Azure-Karten zu bestimmten Teams hinzufügen*

### Verbinde dein persönliches Azure-Konto, um Azure-Karten zu verwenden.

Nachdem ein Miro-Admin die App installiert und genehmigt hat, muss jedes Teammitglied, das Azure-Karten verwenden möchte, die Verbindung zu seinem Azure-Konto persönlich autorisieren. Dies personalisiert den Karten-Picker und ermöglicht das Importieren aller Azure-Arbeitsitems, auf die der Nutzer zugreifen kann.

Das Symbol für Azure-Karten befindet sich in der Erstellungssymbolleiste. Wenn das Symbol nicht da ist, musst du möglicherweise danach suchen:

1. Wähle dazu in der Erstellungsleiste die Option **Tools, Medien und Integrationen** (**+**) aus.
   Das **Feld „Tools, Medien und Integrationen“** wird geöffnet.
2. Suche auf dem **Tools**-Tab nach Azure Cards und wähle sie aus.

Um dein Konto zu verbinden:

1. Klicke in der Symbolleiste auf das Azure-Karten-Symbol. Ein Popup wird dich auffordern, zu **autorisieren**.
2. Klicke auf die Schaltfläche **Autorisieren** und dann auf **Weiter**. Du wirst zu den Teameinstellungen > Apps & Integrationen weitergeleitet.
3. Verwende die App-Einstellungen, um dein Microsoft-Konto mit Miro zu verbinden und die Azure-Instanz anzugeben, die du verwenden möchtest. Diese URL kann von Azure DevOps kopiert werden; Miro akzeptiert entweder die personalisierte URL deiner Instanz oder die allgemeine `https://dev.azure.com/` Adresse, die mit dem Namen deiner Instanz endet.
   ![Azure-Organisations-URL in den Miro-App-Einstellungen angeben.](../../../../../../docs/integrations-apps/microsoft/images/21017013107730_org%20URL.jpg)

:::note
Bitte beachte, dass nur Team-Admins die anfängliche Konfiguration auf Team- oder Unternehmensebene einrichten können. Wenn du die Schaltfläche **Verbinden** für die Azure-Organisations-URL während der Administrator-Einrichtung nicht siehst, stelle bitte sicher, dass du [Team-Admin-Rechte für das Team](../../administration/user-management/06-how-to-manage-admin-roles.md) hast.
:::

## Azure-Arbeitselemente in ein Miro-Board importieren

Sobald die Azure Cards-App konfiguriert und dein persönliches Konto verbunden ist, kannst du Azure-Arbeitsaufgaben in jedes Miro-Board importieren, das mit dem verbundenen Team verknüpft ist. Es gibt zwei Hauptmethoden, um dies zu tun:

- Kopiere die URL des Azure-Arbeitselements und füge sie direkt auf das Miro-Board ein. Der Artikel wird automatisch in eine Azure-Karte umgewandelt.
- Verwende den Azure-Karten-Picker: Klicke auf das **Azure-Karten**-Symbol in der Symbolleiste, um die Auswahl zu öffnen.

  ![Azure Cards picker interface in Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017013109010_Azure%20cards%20picker.jpg)*Auswahlfeld von Azure-Karten*

  Der Picker unterstützt die Suche in allen Feldern, sodass du eine Karte anhand ihres Titels, Typs, Zustands usw. finden kannst. Du kannst auch die umfassende [Stichwortsuche](https://docs.microsoft.com/azure/devops/project/search/get-started-search?view=azure-devops#start-your-search-with-a-keyword) verwenden, die von Microsoft unterstützt wird.

  ![Animation showing search functionality within the Azure Cards picker.](../../../../../../docs/integrations-apps/microsoft/images/21017013114002_Azure%20Cards%20picker.gif)*Azure-Karten im Picker suchen*

  Du kannst die Karten nach Projekt, zugewiesener Person, Typ, Bereich und Zustand filtern, was dir eine erweiterte Filterung von Azure-Arbeitselementen direkt in Miro ermöglicht.

  ![Filtering options within the Azure Cards picker.](../../../../../../docs/integrations-apps/microsoft/images/21017013116306_filter.jpg)*Azure-Karten im Picker filtern*

  Um zum ursprünglichen Azure-Arbeitsobjekt zu navigieren, wähle eine Karte auf dem Board aus und klicke auf die **Quelle**-Schaltfläche im Kontextmenü.

  ![Source button on an Azure Card linking to the item in Azure DevOps.](../../../../../../docs/integrations-apps/microsoft/images/21017042632338_card%20spurce.jpg)*Die Quellenschaltfläche der Karte*

  Azure-Karten können als eigenständige Board-Widgets oder als Komponenten von interaktiven [Kanban](../../using-miro/advanced-tools/02-columns-formerly-kanban.md)- und [User-Story-Map](../../using-miro/advanced-tools/07-user-story-mapping.md)-Frameworks verwendet werden. Du kannst Azure-Karten zu diesen Frameworks hinzufügen, indem du sie dort hineinziehst.

  ![Animation showing Azure Cards being used within a Miro Kanban board.](../../../../../../docs/integrations-apps/microsoft/images/21017042632850_Azure%20cards%20and%20kanban.gif)*Mit Azure-Karten in Kanban arbeiten*

## Azure-Karten direkt in Miro erstellen und bearbeiten

Die Zwei-Wege-Integration zwischen Miro und Azure DevOps ermöglicht es Teams, neue Azure-Arbeitsgegenstände zu erstellen und bestehende direkt von einem Miro-Board aus zu bearbeiten. Du kannst auch bereits vorhandene Miro-Karten und Haftnotizen in Azure-Karten umwandeln.

### Eine neue Azure-Karte erstellen

So erstellst du ein neues Azure-Arbeitselement aus Miro:

1. Wähle in der Erstellungssymbolleiste **Azure-Karten** aus und wähle **Arbeitselement erstellen** in der oberen rechten Ecke der Auswahl aus.
2. Fülle die Felder der Karte aus, wähle ein Projekt, einen Elementtyp, einen Zugewiesenen und klicke auf **Erstellen**. Das neue Element wird sowohl in deinem Azure DevOps-Verzeichnis als auch auf deinem Miro-Board erstellt.

![Animation showing the process of creating a new Azure Card from Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017042635282_create%20an%20Azure%20Card.gif)*Eine Azure-Karte in Miro erstellen*

### Wandle Miro-Karten oder Notizzettel in Azure-Karten um.

So wandelst du eine bestehende Miro-Karte oder einen Haftnotiz in eine Azure-Karte um:

1. Wähle die Notiz oder Karte auf dem Board aus.
2. Klicke auf die Option zum Umwandeln (in der Regel ein Azure DevOps-Symbol oder "In Azure-Arbeitselement umwandeln") im Kontextmenü des Objekts.
3. Lege die Kartenparameter (wie Projekt, Elementtyp) im Dialog fest und klicke auf **Umwandeln**. Der Text auf der Notiz/der Karte wird in den Kartentitel umgewandelt.

> **💡** Spare Zeit, indem du Notizen oder Miro-Karten massenhaft in Azure-Karten umwandelst. Klicke und ziehe, um alle Objekte auszuwählen, die du umwandeln möchtest, und wähle im Kontextmenü die Option **In Azure-Arbeitselemente umwandeln**.

![Converting a Miro sticky note into an Azure Card.](../../../../../../docs/integrations-apps/microsoft/images/21017013125650_convert%20a%20sticky%20into%20an%20Azure%20Card.jpg)*Eine Notiz in eine Azure-Karte umwandeln*

### Azure-Karte bearbeiten

Durch die Option, Azure-Karten in Miro zu bearbeiten, entfällt der Aufwand, zwischen den Tools zu wechseln. So bearbeitest du eine Karte:

1. Klicke auf die Azure-Karte auf deinem Miro-Board.
2. Klicke auf das **Stiftsymbol (bearbeiten)** im Kontextmenü der Karte. Ein Pop-up-Fenster wird geöffnet, in dem du die Felder des Elements bearbeiten kannst.
3. Klicke auf **Aktualisieren**, um die Änderungen zu speichern. Die Änderungen werden sich auch in Azure DevOps widerspiegeln.

![Editing an Azure Card's details directly within Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017042639890_edit%20an%20Azure%20card.jpg)*Die Option, eine Azure-Karte in Miro zu bearbeiten*

### Die Farbe der Azure-Karte ändern

Um das Erscheinungsbild deiner Azure-Karten auf dem Board anzupassen:

Um die Füllfarbe einer Karte zu ändern, klicke auf die Karte(n) und wähle **Füllfarbe** im Kontextmenü aus. Wenn du die Karte(n) duplizierst, haben alle nachfolgenden Kopien die gleiche Füllfarbe.

## Deinstallation der Integration Azure-Karten

Wenn du die Azure-Karten-Integration nicht mehr benötigst, kannst du sie deinstallieren. Die Deinstallation auf Teamebene erfordert Team-Admin-Berechtigungen.

1. Gehe zu **Teameinstellungen > Apps & Integrationen > Azure-Karten**.
2. Scrolle nach unten und klicke auf **Für das Team deinstallieren.**
3. Um Azure-Karten nur für dein persönliches Konto zu deinstallieren, klicke auf **Für mich deinstallieren.**

![Options to uninstall Azure Cards for the team or for an individual user.](../../../../../../docs/integrations-apps/microsoft/images/21017042628370_uninstall%20Azure%20cards.jpg)*Die App für das gesamte Team oder nur für dich deinstallieren*

## Unterstützte Azure-Kartenfelder

Die folgenden Felder werden für Azure-Karten in Miro unterstützt:

- Titel
- Projekt
- Typ
- Status
- Beschreibung (Bearbeiten wird nicht unterstützt)
- Übergeordnetes WI
- Bearbeiter
- Priorität
- Story Points
- Bereich
- Iteration
- Akzeptanzkriterien

Benutzerdefinierte Felder werden nicht unterstützt.

## Fehlerbehebung für Azure Cards

Wenn du Probleme mit der Azure-Karten-Integration hast, konsultiere die häufigen Probleme und Lösungen unten.

Die URL ist ungültig

Die URL, die du verwendet hast, ist nicht korrekt. Bitte überprüfe die Rechtschreibung und Formatierung. Die Adresse der Azure-Organisation muss beispielsweise mit einem Schrägstrich enden.

Die URL der Azure-Organisation kann nicht erreicht werden.

Die eingegebene URL existiert nicht. Bitte gib die vorhandene URL ein oder überprüfe die Schreibweise. Probiere außerdem Folgendes aus:

- Vergewissere dich, dass deine Organisation die Autorisierung von Dritten akzeptiert: in **Organisationseinstellungen > Richtlinien (Sicherheit)** **>** „Zugriff von Drittanbieteranwendungen über OAuth“ ist aktiviert.
- Deine Azure-Organisation ist in einem privaten Netzwerk/deine Unternehmens-Firewall blockiert externe Netzwerkverbindungen. Bitte nimm die notwendigen Änderungen an deiner Firewall und VPN-Konfiguration vor, indem du unsere Domains zu deiner Zulassungsliste hinzufügst: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com, realtimeboard.com*, *.realtimeboard.com, *static.miro-apps.com-Domains. Wenn du einen Proxy verwendest, konfiguriere bitte einen Reverse-Proxy, um uns Zugriff zu gewähren. Gib im**Azure DevOps URL**-Feld in den Einstellungen die Adresse ein, auf die wir zugreifen können (die Adresse kann von der tatsächlichen Adresse deiner eingeschränkten Azure DevOps abweichen). Du kannst auch den Timeout-Wert auf deinem Proxyserver verlängern.
- Alle Anfragen für die Integration laufen über einen Amazon Load Balancer, sodass die Bereitstellung spezifischer Netzwerkinformationen von Miro nicht möglich ist.

Das Abo für Service Hook konnte nicht erstellt werden

Die Person, die derzeit bei Azure angemeldet ist, hat nicht die erforderlichen Berechtigungen. Der Azure-Nutzer, in dessen Namen die Azure-Instanz mit Miro verknüpft wird, muss Zugriff auf diese REST-API-Methoden haben:

- [*Abo für Service Hook erstellen*](https://docs.microsoft.com/rest/api/azure/devops/hooks/subscriptions/create?view=azure-devops-rest-6.0) ("*vso.serviceendpoint_manage"* [Umfang](https://docs.microsoft.com/azure/devops/integrate/get-started/authentication/oauth?view=azure-devops#scopes) erforderlich)
- [*Metadaten über Projekte erhalten (diese Informationen werden verwendet, um Arbeitselemente in Abo-Events korrekt anzugeben)*](https://docs.microsoft.com/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-6.0)
- *Die folgenden Methoden müssen auch für alle Nutzer zugänglich sein, die die Integration verwenden.*
  - [*Elemente abrufen*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/get%20work%20item?view=azure-devops-rest-6.0)
  - [*Elemente auflisten*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/list?view=azure-devops-rest-6.0)
  - [*Elementtypen abrufen*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/get?view=azure-devops-rest-6.0)
  - [*Elementtypen auflisten*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/list?view=azure-devops-rest-6.0)

Der Nutzer **username@microsoft.com** hat keinen Zugriff auf ein Projekt in der angegebenen Azure-Organisations-URL.

Du kannst auf keine Projekte, die in der Azure-Organisation verwendet werden, zugreifen. Um Karten zu importieren, solltest du in den Azure-Boards auf sie zugreifen können. Bitte wende dich an die Person im Besitz der Azure-Organisation und bitte sie, dich zur Azure-Organisation einzuladen. [Dieser Artikel](https://docs.microsoft.com/azure/devops/organizations/security/look-up-organization-owner?view=azure-devops) kann dir helfen, den Namen des Organisationseigentümers herauszufinden.

Das Abo für den Service Hook konnte nicht erstellt werden: Der Nutzer **username@microsoft.com** ist kein Eigentümer der Organisation. Bitte den Eigentümer deiner Organisation, diesen Schritt zu konfigurieren.

Du solltest sowohl im Besitz der Azure-Organisation als auch Unternehmens-Admin von Miro sein, um Azure-Karten in Miro einzurichten.

Die Autorisierung ist abgelaufen. Bitte verknüpfe die Integration in den Einstellungen deines Teams erneut.

Die Azure-Autorisierung ist abgelaufen. Bitte verbinde die Integration auf persönlicher Ebene erneut, wie im Abschnitt "Verbinde dein persönliches Azure-Konto, um Azure-Karten zu verwenden" oben beschrieben.

Die Karte, mit der du arbeitest, zeigt ein unerwartetes Verhalten.

- Dies kann passieren, wenn die Karte nicht von der Azure-Organisation synchronisiert wurde. Zum Beispiel, wenn du die Karte von einem anderen Board kopiert hast oder an einem Board arbeitest, das zwischen Teams verschoben wurde. Um das Problem zu lösen, füge bitte das Azure-Element erneut zum Board hinzu.

Die Anzahl der zurückgegebenen Arbeitselemente überschreitet die Größengrenze von 200. Ändere die Abfrage, um weniger Elemente zurückzugeben.

Wenn du diese Fehlermeldung erhältst, bedeutet das, dass du zu viele Aufgaben ausgewählt hast, um diese dem Board als Karten hinzuzufügen. Bitte beschränke die Anzahl der Aufgaben mithilfe der Suchleiste. Momentan werden beim Öffnen des Pickers keine Filter angewendet und alle Aufgaben der letzten drei Monate werden angezeigt. Jedes Mal, wenn der Picker mehr als 200 Aufgaben anzuzeigen versucht, erhältst du die Fehlermeldung.

Ich erhalte den **Verbinden**-Button nicht, wenn ich versuche, meine Azure-Organisation über die Miro-Einstellungen mit Miro zu verbinden.

Stelle sicher, dass du Team-Admin-Rechte hast. Gehe zum Tab **Aktive Nutzer** in deinen Teameinstellungen und [mach dich zum Team-Admin](../../administration/user-management/06-how-to-manage-admin-roles.md), falls nötig. Dies gilt für die Ersteinrichtung der Verbindung zur Azure-Organisation durch einen Administrator.

:::note
Wenn du weitere Probleme hast, wende dich bitte an den [Miro-Support](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).
:::

## Azure Cards Häufig gestellte Fragen

Hier sind Antworten auf einige häufig gestellte Fragen zur Integration von Azure-Karten.

Welche IPs sollten für Azure-Karten zugelassen werden?

Damit die Azure-Karten-Integration korrekt funktioniert, insbesondere in eingeschränkten Netzwerkumgebungen, musst du möglicherweise die folgenden IP-Adressen auf die Zulassungsliste setzen:

- 18.203.61.162
- 54.220.74.201
- 54.216.81.236
- 54.73.153.141
- 52.215.228.26
- 52.16.47.17
- 54.217.180.21

Was passiert mit den vorhandenen Azure-Karten, wenn du die Verknüpfung trennst und die App „Azure-Karten“ deinstallierst?

Die Karten bleiben auf den Miro-Boards ohne Datenverlust erhalten, aber sie werden nicht mehr mit Azure synchronisiert und die Schaltfläche "Quelle" verschwindet.
