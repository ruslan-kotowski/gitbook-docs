---
title: Anfragenverwaltung im Enterprise-Preisplan
article_id: 360017237379
translation_id: 360017237379
locale: de
sidebar_position: 9
created_at: '2020-10-27T12:09:40Z'
updated_at: '2026-02-19T11:00:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: access-request-management
availability:
  notes: 'Relevant für: Enterprise-Preisplan Verfügbar für: Unternehmens-Admin'
---

In Miro werden Anfragen für Lizenzen, Team- und Organisationszugriff sowie Single Sign-on (SSO) standardmäßig per E-Mail an Unternehmens-Admins gesendet. Mit der erweiterten Anfragenverwaltung können Unternehmens-Admins den Empfang und die Bearbeitung dieser Anfragen individuell gestalten.

### Art der Anfrage

Die Arten von Anfragen lassen sich in vier Kategorien einteilen:

- Anfragen zum Beitritt zu deiner Organisation
- Anfragen zum Beitritt zu einem Team
- Anfragen zu einer Lizenz
- Anfragen im Zusammenhang mit SSO-Problemen

Erfahre mehr über die verschiedenen Anfrage-Szenarien für den Enterprise-Preisplan.

### Optionen für die Anfragenverwaltung

Unternehmens-Admins haben eine Vielzahl von Optionen für die Anfragenverwaltung, mit denen sie die Prozesse je nach Art der Anfrage anpassen können:

:::note
Die Optionen, alle Unternehmens-Admins oder spezifische Unternehmens-Admins per E-Mail zu erreichen, beinhalten auch Team-Admins.
:::

- E-Mail an alle Unternehmens-Admins senden
- E-Mail an bestimmte Unternehmens-Admins senden
- Ein Service-Desk-Ticket erstellen
- Zu einer individuellen URL umleiten

## Anfragenverwaltung konfigurieren

:::note
Um [Lizenzanfragen direkt in Miro zu verwalten](04-license-requests-on-enterprise-plan.md), wähle entweder **allen Unternehmens-Admins eine E-Mail senden** oder **spezifischen Admins eine E-Mail senden**. Du erhältst alle zukünftigen Lizenzanfragen in deinen Einstellungen für Lizenzanfragen.
:::

### Allen Unternehmens-Admins eine E-Mail senden

Alle Unternehmens-Admins erhalten eine E-Mail-Benachrichtigung, wenn ein Nutzer eine Zugriffsanfrage stellt.

1. Unter **Unternehmens**-Einstellungen gehe zu **Nutzer** > **Zugriffsanfragen** > **Anfragen-Management**.
2. Klicke auf die **Art der Anfrage**, die du verwalten möchtest.
3. Ein Pop-up-Fenster wird geöffnet. Klicke auf das Dropdown-Menü und wähle **Allen Unternehmens-Admins eine E-Mail senden**.

:::note
Die Optionen, allen Unternehmens-Admins oder spezifischen Unternehmens-Admins E-Mails zu senden, beinhalten auch Team-Admins.
:::

### E-Mail an bestimmte Unternehmens-Admins senden

Unternehmens-Admins können bis zu 5 E-Mail-Adressen angeben. Die Anfrage wird nur an die angegebenen E-Mail-Adressen geschickt. Die E-Mail-Adressen müssen nicht von Miro-Nutzenden stammen.

1. Gehe zu den **Unternehmenseinstellungen** > **Benutzer** > **Anfragen** > **Anfragenverwaltung**.
2. Klicke auf die **Art der Anfrage** , die du verwalten möchtest.
3. Es erscheint ein Pop-up-Fenster. Klicke auf das Dropdown-Menü und wähle **Bestimmten Unternehmens-Admins eine E-Mail senden**.
4. Füge bis zu 5 E-Mail-Adressen hinzu. Klicke jedes Mal auf **Hinzufügen**, wenn du eine E-Mail-Adresse in das E-Mail-Feld eingibst.

:::note
Die Optionen, allen Unternehmens-Admins oder bestimmten Unternehmens-Admins eine E-Mail zu senden, schließen Team-Admins ein.
:::

### Ein Service-Desk-Ticket erstellen

Du kannst automatisch ein Service-Desk-Ticket erstellen lassen, wenn ein Nutzer eine Zugriffsanfrage stellt. Diese Funktion wird derzeit für **ServiceNow** und **Jira Service Management** unterstützt.

ServiceNow Jira Service Management

1. Konfiguriere die E-Mail-Einstellungen für ServiceNow. Erstelle einen Katalogeintrag für Miro in ServiceNow. Öffne ServiceNow, gehe zu **System Properties** > **Email Properties** und aktiviere den Empfang eingehender E-Mails

2. [Erstelle eine eingehende E-Mail-Aktion](https://docs.servicenow.com/bundle/tokyo-servicenow-platform/page/administer/notification/task/t_CreatingAnInboundEmailAction.html). Im Feld **From**
Gib im Feld **Von** unter der Zeile **Nur E-Mails von diesem Absender lösen diese eingehende Aktion aus** die E-Mail-Adresse [notification@miro.com](mailto:notification@miro.com) ein.

Stelle die [Feldwerte aus dem E-Mail-Inhalt ein](https://docs.servicenow.com/bundle/rome-servicenow-platform/page/administer/notification/reference/r_SetFieldValsFromTheEmailBody.html), um zusätzliche Einstellungen zu konfigurieren und den Prozess der Umwandlung einer Miro-E-Mail in ein ServiceNow-Ticket einzurichten. Beispielsweise kannst du einer bestimmten Person ein neu erstelltes Ticket zuweisen.

Gehe zu Miro, öffne **Company** Einstellungen > **Benutzer** > **Anfragen** > **Anfragenverwaltung**, und wähle **Ticket in ServiceNow erstellen**. Gib im E-Mail-Feld deine ServiceNow-E-Mail-Adresse ein.

1. Konfiguriere die E-Mail-Einstellungen für Jira Service Management. Wähle in deinem Serviceprojekt **Projekteinstellungen** > **E-Mail-Anfragen** aus. [Wähle deinen E-Mail-Dienstanbieter und folge den Anweisungen, um Miro zu verknüpfen](https://support.atlassian.com/jira-service-management-cloud/docs/receive-requests-from-an-email-address/).

2. Gehe zu Miro, öffne **Unternehmen** Einstellungen > **Nutzerverwaltung** > **Zugriffsanfragen** > **Anfragenverwaltung** und wähle **Ein Ticket in Jira Service Management erstellen**. Gib im E-Mail-Feld deine Jira Service Management E-Mail-Adresse ein.

### Zu einer individuellen URL umleiten

Die anfragende Person wird für die nächsten Schritte an eine URL deiner Wahl weitergeleitet.

1. Unter **Unternehmen**-Einstellungen gehe zu **Nutzer** > **Access Requests** > **Anfragenverwaltung**.
2. Klicke auf den **Anfragetyp**, den du verwalten möchtest.
3. Ein Pop-up-Fenster wird geöffnet. Klicke auf das Dropdown-Menü und wähle **Zu einer individuellen URL umleiten**.
4. Gib den Weiterleitungslink im Feld **individuelle URL** ein.

## Anfrage-Szenarien

Die folgenden Szenarien zeigen, wie verschiedene Anfragen in Miro ausgelöst werden. Überprüfe die Szenarien, um zu entscheiden, wie du die einzelnen Arten von Anfragen verwalten möchtest.

|  |  |
| --- | --- |
| **Anfragen auf Beitritt zu deinem Unternehmen** | - Wenn ein neuer Nutzer sich einem Team anschließen möchte, das ein unternehmensverwaltetes Abo mit [Domainsteuerung](../canvas-25-admin-features/domain-control/01-domain-control.md) ist (sofern Domainsteuerung nicht eingestellt ist, um neue Nutzer zu erfassen). |
| **Lizenzanfragen** | - Wenn ein [Free Restricted Nutzer](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) eine Standard- oder Voll- (Legacy) Lizenz anfragt. - Wenn ein Mitglied für einen Nutzer mit einer kostenlosen eingeschränkten Lizenz eine Standard- oder Voll-Lizenz (Legacy) anfordert, es sei denn, Mitgliedern ist es in den [Einstellungen für Einladungen](03-invitation-settings-on-enterprise-plan.md) erlaubt, neue Nutzer zum Abo einzuladen. - Wenn ein Nutzer mit einer Standard- oder Voll-Lizenz (Legacy) eine erweiterte Lizenz anfordert. - Wenn ein Mitglied versucht, einen Nutzer mit einer kostenlosen eingeschränkten Lizenz einzuladen oder ihm Bearbeitungszugriff zu geben. |
| **Anfragen auf Beitritt zu einem Team** | - Wenn ein Nutzer, der kein Admin ist, versucht, ein Board mit einem Nutzer zu teilen, der *kein* Mitglied des Teams ist, Gästeinladungen in den [Einladungseinstellungen](03-invitation-settings-on-enterprise-plan.md) deaktiviert sind und nur Admins neue Mitglieder zum Team einladen können. - Wenn ein Mitglied, das keine neuen Mitglieder einladen darf, versucht, einem Nutzer, der nicht Mitglied des Teams ist, eine Eigentümer- oder [Miteigentümer](../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md)-Rolle für ein bestimmtes Board zuzuweisen. - Wenn ein Enterprise-Nutzer beantragt, einem Team beizutreten, das für Nutzer in seiner Organisation [sichtbar](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) ist. - Wenn ein[Gast](../../using-miro/sharing-boards/07-collaboration-with-guests.md) zu bestimmten Boards in einem Team eingeladen wurde und dem Team beitreten möchte |
| **Anfragen im Zusammenhang mit SSO-Problemen** | - Wenn ein Nutzer keinen Zugriff auf Miro im Identitätsanbieter hat und Probleme bei der Anmeldung über SSO hat. |

## Häufig gestellte Fragen

**Warum erhalte ich immer noch E-Mails, obwohl ich meine Einstellungen so konfiguriert habe, dass Tickets erstellt werden?**

Wenn Team-Admins in den [Einladungseinstellungen](03-invitation-settings-on-enterprise-plan.md) neue Nutzer in ein Team einladen dürfen, erhalten sie Einladungsanfragen zu diesem Team per E-Mail, auch wenn die Einstellungen zur Anfragenverwaltung anders gesetzt sind. Unternehmens-Admins, die auch Team-Admins sind, werden diese E-Mails ebenfalls noch erhalten.

**Wie erfahren Team-Admins, ob es Anfragen gibt, ihrem Team beizutreten?**

Wenn sie Nutzer in ihre Teams einladen dürfen, erhalten Team-Admins unabhängig von den Einstellungen für die Anfragenverwaltung eine E-Mail.
