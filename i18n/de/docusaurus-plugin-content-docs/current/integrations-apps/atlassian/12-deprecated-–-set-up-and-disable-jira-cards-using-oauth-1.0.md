---
title: Veraltet – Jira-Karten einrichten und deaktivieren (OAuth 1.0)
article_id: 360019501754
translation_id: 7316324517010
locale: de
sidebar_position: 14
created_at: '2022-08-25T09:57:07Z'
updated_at: '2025-11-25T16:03:50Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Erhältlich für: Jira Cloud, Jira Server (On-Premise) und Datacenter (auch
    LDAP-geschützt) Einrichtung durch: Team-Admin bei Miro & System-Admin bei Jira
    mit administrativen Projektberechtigungen'
---

:::note
Die folgende OAuth1.0-Authentifizierungsmethode wird ab dem 31. Juli 2025 in Miro nicht mehr unterstützt. OAuth1.0 ist ein [veraltetes Authentifizierungsprotokoll in Jira](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively.) und sollte nicht verwendet werden. Diese Änderung ist Teil einer umfassenderen Umstellung auf OAuth2.0, die in Übereinstimmung mit den bewährten Sicherheitspraktiken empfohlen wird. Nutzern wird empfohlen, zu OAuth2.0 zu migrieren, um den Support und die Kompatibilität mit den Diensten von Miro sicherzustellen.
:::

## Konfiguration von Miro in Jira

:::warning
Sollten technische Probleme auftreten, lies bitte unseren Artikel über [Mögliche Probleme und wie du sie beheben kannst](https://help.miro.com/hc/articles/360017572654).
:::

:::tip
Erfahre mehr über Jira-Karten in den Artikeln [FAQ zu Jira-Karten](https://help.miro.com/hc/articles/360013463739) und [Wie du WebHooks für Jira-Karten einrichtest](https://help.miro.com/hc/articles/360017731113).
:::

Einrichtung der Jira-Cloud Jira-Server und -Datencenter

:::note
Bitte beachte, dassJira-Menüs je nach verwendeter Jira-Version unterschiedlich sein können, der allgemeine Ablauf sollte jedoch derselbe sein. Die folgenden Anweisungen findest du auch im [Atlassian-Support](https://confluence.atlassian.com/adminjiraserver071/using-applinks-to-link-to-other-applications-802592232.html).
:::

### Schritt 1: Anwendungslink

Erstelle zunächst einen Anwendungslink und konfiguriere ihn.

1. Gehe zu **Jira-Einstellungen** > **Produkte** > **Integrationen** > **Anwendungslinks** > **Link erstellen:
   ![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)***Beachte, dass die Jira-Oberfläche je nach Version unterschiedlich sein kann*
2. Wähle **Direkter Anwendungslink** und gib `https://miro.com/` im Feld **Anwendungs-URL** ein.
   Wichtig: Du musst die URL genau in diesem Format eingeben. Klicke auf **Weiter**.
   ![mceclip2.png](../../../../../../docs/integrations-apps/atlassian/images/21017004818066_mceclip2.png)
    *Den Link erstellen*
3. Klicke im nächsten Menü einfach erneut auf **Weiter**.
4. Im Menü **Link überprüfen** überprüfe, ob die URL immer noch genau `https://miro.com/` ist, und gib den **App-Namen** nach deiner Wahl ein. Scrolle nach unten und aktiviere unten das Kontrollkästchen **Eingehenden Link erstellen**. *Überspringe die übrigen Felder* und klicke auf **Weiter**.
   ![mceclip3.png](../../../../../../docs/integrations-apps/atlassian/images/21017004819346_mceclip3.png)  *Nur das Feld Anwendungsname muss ausgefüllt werden*
5. Hier siehst du die Felder für die Miro-Werte. Um die Werte zu erhalten, melde dich bei Miro an.
   - Für die Integration auf Teamebene geh zu **[Teameinstellungen](https://help.miro.com/hc/articles/360021841280)** > **Apps & Integrationen** > **Jira-Karten.**
   - Für eine Integration auf Organisationsebene gehe zu [**Unternehmenseinstellungen**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **Apps** > **Apps verwalten** > **Jira-Karten** > **Einstellungen**.
     > Falls du keine Jira-Karten in deiner Apps-Liste hast, scrolle zum oberen Abschnitt, klicke auf **Apps installieren** und fahre mit der Installation der App aus dem Miro Marketplace fort. Sobald du die Jira-Karten in der Liste siehst, klicke darauf, um sie zu öffnen.


     Die Plugin-Registerkarte wird geöffnet und du siehst **Schritt 1**, um die erforderlichen Werte zu erhalten:

     ![Jira_Cards_values.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017515668626_Jira Cards values.jpg)*Jira-Karten-Werte*
     Kopiere die Werte und füge sie zum Atlassian **Review Link**-Menü hinzu.
6. Du siehst einen Moment lang die Verarbeitungsmeldung:
   ![mceclip4.png](../../../../../../docs/integrations-apps/atlassian/images/21017528655634_mceclip4.png)
    *Der letzte Schritt der Link-Erstellung*

Damit sind alle Schritte, die auf der Seite von Atlassian durchgeführt werden müssen, abgeschlossen. Der Link erscheint in der Liste deiner App-Links.

### Schritt 2: Verbindung

Gehe zurück zu deinen Jira-Karteneinstellungen in Miro und wähle eine der beiden Optionen aus: Erstelle einen Webhook manuell oder automatisch. Wenn du es manuell auswählst, deaktiviere die Option. Weitere Informationen findest du in [diesem Artikel](https://help.miro.com/hc/articles/360017731113). Wir empfehlen dringend, den automatischen Webhook zu verwenden, damit du ihn bei großen Updates des Plugins nicht zurücksetzen musst.

Zum Schluss gib deine Jira-URL ein und klicke auf **Verbinden:**

![step_2.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017528650898_step%202.jpg)*Jira-Karten verbinden*

Um die Jira-URL zu erhalten, kopiere die Base-URL deiner Jira-Instanz. Wir akzeptieren folgende Formate:

`https://your-server.example.com/`
[https://your-server.example.com/
https://IPadresse/](https://your-server.example.com/)[https://your-ip-address/](https://your-server.example.com/)

Falls deine Jira-URL nicht akzeptiert wird, lies bitte [diesen Artikel.](https://help.miro.com/hc/articles/360017572654) Bitte stelle außerdem sicher, dass Miro ausreichend Zugriff auf dein Jira-Konto hat, um die [Verbindung herstellen zu können.](https://help.miro.com/hc/articles/360017572694)

Jetzt hast du deine Jira-Instanz mit deinem Miro-Team verbunden.

:::warning
Während Atlassian den Support für Jira Server ab Februar 2024 einstellt, wird Miro die Integration der Jira-Karten für Jira Server auf absehbare Zeit weiterhin unterstützen.
:::

1. Gehe zu `https://your-jira-server/plugins/servlet/applinks/listApplicationLinks`[.](https://your-jira-server/plugins/servlet/applinks/listApplicationLinks) Wenn „Anwendungslinks“ nicht ausgewählt ist, klicke ihn an. ![jira_server_create_application_links.png](../../../../../../docs/integrations-apps/atlassian/images/21017515683858_jira_server_create_application_links.png)*Anwendungslinks des Jira-Servers*
2. Klicke auf **Link erstellen**. Wähle „Atlassian-Produkt“ aus und gib die **Anwendungs-URL** „https://miro.com“ ein. Klicke auf **Weiter**. ![jira_server_create_link.png](../../../../../../docs/integrations-apps/atlassian/images/21017528656274_jira_server_create_link.png)*Konfiguration der Anwendungs-URL*
3. Du wirst zum Dialogfeld „Link-Anwendungen“ weitergeleitet. Gib einen **Anwendungsnamen** ein (z. B. Miro Jira-Karte) und wähle "Generische Anwendung" als **Anwendungstyp** aus.
   Unter „Du erstellst einen Link von:“ solltest du nun die URL deiner Jira-App sehen und unter „Zu dieser App:“ sollte `https://miro.com` angezeigt werden. Klicke auf **Weiter**.![jira_server_link_applications.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017528658834_jira_server_link_applications.jpg)*Informationen zu Link-Anwendungen konfigurieren*
4. Die Link-Konfiguration wird verarbeitet. Wenn der Prozess abgeschlossen ist, siehst du deinen neuen Link im Bereich „App-Links“ des Jira-Servers. ![jira_server_application_links_created.png](../../../../../../docs/integrations-apps/atlassian/images/21017515685522_jira_server_application_links_created.png)*Deine konfigurierte App auf dem Jira-Server*
5. Als Nächstes musst du die Details deiner App konfigurieren. Klicke auf das Bleistiftsymbol deiner App, um die App-Details zu bearbeiten.
6. Klicke im Dialogfeld "Konfigurieren" auf die Option **Eingehende Authentifizierung**. Gib den **API-Schlüssel, den API-Namen, den Public Key** und optional eine Beschreibung ein.
   - Für die Integration auf Teamebene sind diese Informationen unter [**Teameinstellungen**](https://help.miro.com/hc/articles/360021841280) > **Apps & Integrationen** > **Jira-Karten** verfügbar.
   - Für Integrationen auf Organisationsebene sind diese Informationen unter [**Company settings**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **Apps** > **Apps verwalten** > **Jira-Karten** > **Einstellungen** verfügbar.
     ![jira_server_config_oauth.png](../../../../../../docs/integrations-apps/atlassian/images/21017528687506_jira_server_config_oauth.png)*Konfiguration der im Jira-Server eingehenden Authentifizierungsinformationen*
     ![jira_webhooks_jira_server_config.png](../../../../../../docs/integrations-apps/atlassian/images/21017515686418_jira_webhooks_jira_server_config.png)*Informationen zu den Links der in Miro verwendeten Jira-Anwendung*
7. Scrolle bis zum Ende der Optionen für die „Eingehende Authentifizierung“ und klicke auf **Speichern**. Dein Verifizierungsstatus sollte nun bestätigt sein, und dieser Jira-Server kann ab sofort innerhalb von Miro für die Verwendung mit Jira-Karten genutzt werden. Bitte achte darauf, dass auf der Miro-Seite „Jira Server“ und „OAuth 1.0“ ausgewählt sind.![jira_server_welcome_to_jira.png](../../../../../../docs/integrations-apps/atlassian/images/21017515690258_jira_server_welcome_to_jira.png)

### Autorisierung von Nutzern

Nachdem die Integration verbunden ist, muss jede Person ihr persönliches Jira-Profil verbinden, um die richtigen Berechtigungen einzurichten – das stellt sicher, dass der Zugriff jedes Nutzers auf der Miro-Seite *genau der gleiche ist wie bei deiner Jira-Instanz*. Wenn Endnutzer versuchen, eine Jira-Karte zum ersten Mal zu importieren oder zu bearbeiten, werden sie aufgefordert, sich mit ihren individuellen Anmeldeinformationen bei Jira anzumelden.

Nachdem das erledigt ist, können die Nutzer Aufgaben als Karten auf dem Whiteboard hinzufügen. Alle Änderungen, die in Jira vorgenommen wurden, werden auch in den Jira-Karten auf dem Board angezeigt.

:::note
Wenn ein Nutzer keine Jira-Anmeldeinformationen hat, aber Zugriff auf das Board, auf dem die Karte hinzugefügt wurde, sieht er den Titel der Karte, den Vorgangstyp, die Priorität, die zugewiesene Person und alle Attribute, die auf der Jira-Karte konfiguriert sind, um angezeigt zu werden. Allerdings können sie die Karte nicht erweitern, um weitere Attribute zu sehen und sie zu bearbeiten, es sei denn, dies wurde autorisiert. Wenn die Nutzer ihre Jira-Anmeldeinformationen nicht verbinden, wird der Avatar der zugewiesenen Person nicht angezeigt und das allgemeine Aussehen der Karte wird anders sein.
:::

### Verwenden einer Jira-Instanz für mehrere Miro-Teams

Du kannst Karten auf Teamebene oder auf Organisationsebene installieren. Wenn du mehrere Teams hast, kannst du Organisationseinstellungen nutzen, um die Einrichtung für jedes Team nicht immer wiederholen zu müssen. Der bestehende App-Link wird für alle Teams verwendet.

Nachdem du dein Team oder deine Organisation mit einer Jira-Instanz verbunden hast, wird in deinen Jira-Webhooks ein neuer Webhook für das Miro-Team oder die Organisation erstellt. Ein Webhook wird erstellt, um einen Kanal für Anfragen zu Updates einzurichten.

Wenn du Einstellungen auf Organisationsebene festlegst, behalten bereits verbundene Teams ihre aktuellen Einstellungen bei. Sie können jedoch jederzeit zu den Einstellungen auf Organisationsebene wechseln.

Zusätzlich können Teams bei Bedarf die Einstellungen auf Organisationsebene überschreiben, um eine Verbindung zu einer anderen Jira-Instanz herzustellen.

Wenn du ein Enterprise-Kunde bist und mehrere teambezogene Verbindungen auf die Standard-Organisationsverbindung migrieren möchtest, wende dich an dein Konto-Team.

:::warning
Wenn du mehrere Teams separat verbinden möchtest, empfehlen wir, dem Webhook für jedes Team einen eindeutigen Namen zu geben. Gehe zu deiner Jira-Webhooks-Seite und bearbeite jeden neu erstellten Webhook.
:::

Die Verbindung mehrerer Jira-Instanzen mit einem Miro-Team wird nicht unterstützt.

## Deaktivieren des Plugins

Für die Integration auf Teamebene, gehe zu **Teameinstellungen** > **Apps & Integrationen** > **Jira-Karten**. Wähle dann **Für das Team entfernen**.

Für die Integration auf Organisationsebene, um die Nutzung der Jira-App einzuschränken, gehe zu **Unternehmenseinstellungen** > **Apps** > **Apps verwalten** > **Jira-Karten**. Dann schiebe den Schalter in die Aus-Position.

:::warning
Wenn du Jira für die Organisation deaktivierst, können Nutzer aus allen Enterprise-Teams die Jira-Karten nicht mehr verwenden. Um mehr über App-Verwaltung und Einschränkungen zu erfahren, siehe [App-Verwaltung](https://help.miro.com/hc/articles/4404659741458).
:::

**Weitere Informationen:** Siehe [So benutzt du Jira-Karten](https://help.miro.com/hc/articles/360017572434).
