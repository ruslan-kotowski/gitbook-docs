---
title: "M\xF6gliche Probleme mit der Miro-App f\xFCr Confluence"
article_id: 360021388500
translation_id: 8636997439378
locale: de
sidebar_position: 21
created_at: '2022-11-18T11:01:45Z'
updated_at: '2025-02-26T11:23:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
---

Falls du bei der Verwendung des [Confluence-Plugins](https://help.miro.com/hc/articles/360020712594) auf ein Problem gestoßen bist, kannst du die folgenden Tipps zur Fehlerbehebung nutzen.

|  |  |  |
| --- | --- | --- |
| **Nachricht/Problem** | **Mögliche Ursachen** | **Schritte zur Behebung des Problems** |
| Das Miro-Auswahlfenster ist schwarz/leer, wenn du versuchst, dich bei Miro einzuloggen/Miro-Boards in Confluence-Seiten einzubetten. | Falsche Browsereinstellungen. | Gehe zu den Einstellungen deines Browsers und stelle sicher, dass:   - das Kontrollkästchen **Websiteübergreifende Nachverfolgung verhindern** deaktiviert ist - das Kontrollkästchen **Alle Cookies blockieren** deaktiviert ist:   mceclip0.png   - **Pop-up-Fenster** auf den Websites von Miro und Atlassian erlaubt sind:   mceclip1.png |
| Du hast die Berechtigung, dieses Whiteboard nur zu betrachten und kannst es nicht freigeben oder einbetten.  **mceclip0.png** | Du bist kein Bearbeiter/Eigentümer des Boards. | Stelle sicher, dass:   - du ein Bearbeiter oder der Board-Eigentümer bist. - du in deinem Browser in Miro mit den richtigen Anmeldedaten autorisiert bist. - du das Whiteboard in Confluence im selben Browser einbettest. |
| Nachdem du ein Miro-Board eingebettet hast, siehst du die Meldung: "Miro benötigt Zugriff auf deine Cookie-Dateien" | Dein Browser lässt das Speichern von Drittanbieter-Cookies nicht zu. | Um das Einbetten zu aktivieren, musst du die Cookies in deinem Browser aktivieren. Dies tritt meist in Mozilla und Safari auf. |
| Das eingebettete Board zeigt die Fehlermeldung „Deine Sitzung ist abgelaufen“ an. |
| Wenn du versuchst, ein Board einzubetten, bekommst du die folgende Meldung: "Du bist kein Mitglied eines Teams. Bitte logge dich bei der Vollversion des Produkts ein und erstelle dein Team oder lass dich von jemandem in das bestehende Team einladen.“  mceclip0.png | Du bist kein Mitglied eines Teams unter dem im Browser autorisierten Miro-Profil. | Öffne [Miro](https://miro.com/app/dashboard/) und erstelle ein Team. Wenn du dir sicher bist, dass du Mitglied eines oder mehrerer Teams in Miro bist, kannst du Miro in einer anderen Browserregisterkarte öffnen und überprüfen, ob du mit der **richtigen E-Mail-Adresse** autorisiert bist. |
