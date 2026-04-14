---
title: Slack
article_id: 360017572494
translation_id: 360017572494
locale: de
sidebar_position: 15
created_at: '2019-02-11T10:13:25Z'
updated_at: '2025-02-26T12:10:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
---

Erhalte Slack-Benachrichtigungen von neuen Kommentaren und Erwähnungen auf deinen Boards sowie von anderen Änderungen in Bezug auf dein Profil, teile deine Miro-Boards von Slack aus und öffne Board-Links automatisch. In diesem Artikel erfährst du, wie du Slack mit Miro verbindest und Zugriff auf all die tollen Funktionen hast.

> ️ ✏️ Manche Slack-User können sich ganz einfach über Slack bei Miro anmelden, indem sie auf einen Link zu einem Miro-Board klicken, der in einem Slack-Kanal gepostet wurde.  Dies ist derzeit eine Beta-Funktion und wird von Slack verwaltet. Dazu muss unsere Anwendung nicht im Slack-Workspace installiert werden.
> Workspace-Admins können die Funktion Mit Slack anmelden in den Slack-Workspace-Einstellungen deaktivieren (Einstellungen „App-Verwaltung“ > Einstellungen „Mit Slack anmelden“)./span> Enterprise Grid Org und ihre Workspaces sind von dieser Funktion in der Beta-Phase ausgenommen.

> ️ ✏️ Wenn du Hilfe mit der Slack-App brauchst, dann sende eine E-Mail an [slack_integration_support@miro.com](mailto:slack_integration_support@miro.com) [oder gehe auf die Seite](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) So kontaktierst du den Miro-Support.

## Aktivieren der App

Die Integration der Slack-App wird von jedem Benutzer selbst in seinem Profil eingerichtet. Um die Integration zu aktivieren, öffne deine Miro [Profil-Einstellungen](../../using-miro/managing-your-profile/01-profile-settings.md).

getting_to_profile_settings.jpg
[So gelangst du vom Miro Dashboard zu den Profileinstellungen](https://miro.com/app/dashboard/)

Wechsle zur Registerkarte **Integrationen**, suche **Miro Feed (Slack-App)** und klicke auf **Verbinden**:

connect_Slack.jpg
Slack-App verbinden

Du kannst sie auch direkt auf der [Registerkarte Benachrichtigungen](https://miro.com/app/account/profile/notifications/) aktivieren:

connect_Slack_from_notifications.jpg
Aktivieren der Slack-App auf der Benachrichtigungsseite

Du wirst zur Autorisierung in Slack umgeleitet. Gib deine Anmeldeinformationen ein und melde dich bei Slack an.

authorize_Slack.jpg
Miro Zugriff zum Workspace gewähren

## Benachrichtigungen konfigurieren

Passe den Feed an, den du erhältst, indem du die Ereignisse auswählst, über die du benachrichtigt werden möchtest.

Du kannst die folgenden Ereignisse mitverfolgen:

- Anmeldungen von Personen, die eingeladen wurden
- Jemand bittet um Zugriff auf ein Team oder ein Board
- Du wurdest zu einem Projekt eingeladen
- wenn ein Board für dich freigegeben wird
- Es gibt einen neuen Kommentar auf deinem Board oder eine Antwort auf deinen Kommentar auf einem Board
- Jemand @erwähnt dich in einem Kommentar oder einer Antwort

Öffne die [Benachrichtigungsseite](https://miro.com/app/account/profile/notifications/) und richte deine Einstellungen ein:

notification_settings.jpg
Benachrichtigungseinstellungen

Beachte, dass du in einigen Fällen nur dann eine Benachrichtigung erhältst, *wenn der Benachrichtigende beschließt*, diese Benachrichtigung zu senden.

## Auf Benachrichtigungen direkt in Slack reagieren

Wenn jemand um Zugriff auf dein Board bittet, kannst du ihn direkt in Slack gewähren. Wähle die Option und klicke auf die Schaltfläche:

react_in_Slack.jpg
Zugriff auf ein Board im Slack-Kanal gewähren

## Whiteboard-Links öffnen

Die neueste Version der Miro-Slack-App öffnet Links zu Miro-Boards, indem die Namen, Beschreibungen und die Miniaturansicht des Boards hinzugefügt werden.

unfurl_a_board_link.jpg
*/span>Board-Name, -Beschreibung und -Miniaturansicht im Slack-Kanal*

Installiere deine Integration mit Slack erneut, um Zugriff auf diese Funktion zu erhalten: Gehe zu Miro **Profileinstellungen > Integrationen** und klicke auf **Abmelden** neben **Miro Feed (Slack-App)**.  Klicke dann auf Verbinden und erneut autorisieren.

:::note
Für eine erneute Autorisierung benötigst du eventuell die Genehmigung des Slack-Workspace-Admins.
:::

Um eine Board-Miniaturansicht festzulegen, öffne deine Board-Informationskarte in deinem Miro-Board, indem du auf den Titel in der linken oberen Ecke deines Boards klickst. Klicke im Popup-Fenster auf das Bild in der oberen linken Ecke und lade ein Bild von deinem Gerät hoch oder wähle einen Bereich deines Boards aus. Die Miniaturansicht erscheint dann in Slack, wenn du den Board-Link freigibst.

change_board_thumbnail.gif
Festlegen der Board-Miniaturansicht

## Ein Board von Slack aus teilen

Wenn du einen Board-Link in Slack postest, siehst du eine Benachrichtigung mit den Benutzern, die keinen Zugriff auf das Board haben. Du kannst sie ganz einfach direkt über Slack zum Board einladen.  Du kannst [das Board gerne auch öffentlich machen](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), damit jeder, der den Link hat, es ansehen und kommentieren kann.

share_from_Slack.jpg
/span>Ein Miro-Board von Slack aus teilen /em>

>  Falls du diese Option nicht siehst, installiere die App über die Einstellungen erneut oder bitte deinen oder deine Admin, das Plugin in Slack Marketplace zu aktualisieren.

## Ein Board von Slack aus erstellen

Mit dem Miro-Shortcut kannst du ein Board direkt von Slack aus erstellen.  Suche nach Miro und wähle **Ein Board erstellen**.

Miro_shortcut.jpg
/span>Ein Board von Slack aus erstellen

Gib einen Titel für das Board ein, wähle ein Miro-Team aus und füge eine kurze Nachricht hinzu, die gemeinsam mit dem Link zum neu erstellten Board in Slack gesendet werden soll.

create_board_modal.jpg
/span>Parameter für ein neues Board in Slack festlegen

Sobald das Board erstellt wurde, wird die Nachricht an den Kanal/das Gespräch zusammen mit dem Board-Link gesendet.

new_board_message.jpg
Eine Nachricht wird nach der Erstellung eines Board von Slack aus gepostet

Falls einige Mitglieder in dem Kanal keinen Zugriff auf das neu erstellte Board haben, wird dir vorgeschlagen, [das Board von Slack aus mit ihnen zu teilen](#h_007785b5-df52-43e2-9eb0-ccb53b795955).

## Deaktivieren der App

Um die Integration zu deaktivieren, gehe zu **Profileinstellungen > Integrationen** und klicke auf **Abmelden**:

Slack_log_out.jpg
Miro Feed deaktivieren

Um die App vollständig von Slack zu entfernen, öffne die **Miro** Kanaleinstellungen in Slack und klicke auf **Konfiguration**.

Miro_Slack_configuration.jpg
Konfiguration der Miro-App für Slack

Du wirst zur Seite mit den Einstellungen für die Miro-App weitergeleitet. Scrolle nach unten, suche deinen Namen in der Liste der autorisierten Benutzer und klicke auf **Widerrufen**.

revoke_access.jpg
Den Zugriff von Miro auf Slack entfernen

Workspace-Admins haben auch die Möglichkeit, die App vom *gesamten Workspace* zu entfernen.

remove_app.jpg
Die App von Slack entfernen

## Häufige Fragen und mögliche Probleme

*1. Wenn ein Nutzer Miro zu Slack hinzufügt, kann Miro dann seine Slack-Kanäle lesen?*
- Nein, Miro zeigt nur die grundlegenden Informationen über die öffentlichen Kanäle im Arbeitsbereich an (). Das bedeutet, dass Miro die Liste der Kanalnamen lesen kann, aber nicht die Nachrichten in den Kanälen.

2. *Ich erhalte die Meldung "Etwas ist schief gelaufen", wenn ich versuche, den Miro Feed für Slack zu verbinden.*
- Bitte überprüfe, ob dein Browser Pop-ups von der Domain miro.com zulässt. Eventuell wird auf einer zusätzlichen Seite nach den App-Berechtigungen gefragt./span>

3. 3. *Ich bekomme keine Benachrichtigungen von Miro-Slack und es hat nicht geholfen, die Miro-App in Slack erneut zu installieren.*  Wie kann ich das beheben?
- Bitte versuche, Miro und Slack auf der Seite von Miro erneut zu verbinden**(Profileinstellungen > [Integrationen](https://miro.com/app/account/profile/integrations/)**).
