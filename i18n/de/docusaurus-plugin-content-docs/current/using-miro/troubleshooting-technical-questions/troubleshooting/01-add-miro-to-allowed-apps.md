---
title: Miro zu erlaubten Apps hinzufügen
article_id: 360017572694
translation_id: 360017572694
locale: de
sidebar_position: 1
created_at: '2019-02-11T10:14:41Z'
updated_at: '2026-03-03T20:16:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Relevant für: alle Miro-Nutzer'
---

Es kann vorkommen, dass Miro-Funktionen nicht richtig funktionieren, wenn Miro kein Zugriff gewährt wird. Dies kann aufgrund von Problemen oder Einschränkungen bei deiner Netzwerkverbindung oder der von dir genutzten Umgebung passieren. Der folgende Artikel listet die häufigsten Ursachen für solche Probleme auf.

## WebSockets

Die Miro-App – insbesondere die *Board*-Seiten – benötigt WebSocket-Verbindungen. Wenn du Probleme hast, deine Boards zu öffnen, das Dashboard und die Einstellungsseiten aber ganz normal geöffnet werden, kann das bedeuten, dass deine Verbindung keine WebSockets unterstützt.

Um deine Verbindung zu testen, öffne bitte [diese Website](http://websocketstest.com).

Wenn die Websockets erkannt werden, siehst du die folgende Meldung:

![wensocket_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264610066_wensocket%20connection.jpg)

Wenn das Ergebnis anders aussieht, blockiert wahrscheinlich etwas in deinem Netzwerk die WebSocket-Verbindungen. Wenn dies der Fall ist, versuche Folgendes:

- Verwende eine andere Netzwerkverbindung
- Verwende ein VPN oder schalte es aus
- Solltest du eine Firmenverbindung nutzen, wende dich an deine Netzwerkadmins und bitte sie, die WebSocket-Verbindungen auf Port 80 und 443 (SSL) zu aktivieren. Aus Sicherheitsgründen können diese innerhalb deines Unternehmensnetzwerks geschlossen oder gefiltert werden. Um eine Verbindung herzustellen, sollten diese Ports für den Zugriff von Miro-Adressen geöffnet sein (siehe Adressen im Abschnitt „Wenn du eine Firewall verwendest“ unten)

Wenn die Websockets korrekt identifiziert werden, es aber immer noch Probleme beim Verbindungsaufbau gibt, wende dich bitte an den [Miro-Support](https://help.miro.com/hc/requests/new?referer=help-center-article).

## Wenn du eine Firewall verwendest

Du musst unsere statischen IP-Adressen in die Zulassungsliste aufnehmen. Hinweis: Die IP-Adressen werden nur verwendet, um die Atlassian-Systeme in Bezug auf die Jira-Integrationen zu erreichen, die wir haben. Die IP-Adressen der Miro-App sind *dynamisch*.
52.16.47.17,
54.216.81.236,
54.217.180.21,
54.73.153.141,
34.249.78.135,
46.51.161.49,
54.217.110.122,
54.220.142.217,
54.228.53.200,
54.73.173.202,
54.73.41.83,
54.74.0.207,
54.74.167.92,
54.75.137.71,
52.64.11.98,
13.55.76.39,
13.54.151.233
3.131.34.166,
13.59.239.75,
13.59.239.75

### Miro-Domains Zulassungsliste

Organisationen, die ein gesichertes Netzwerk nutzen, müssen alle Miro-Domains zulassen. Um die vollständige Liste der zuzulassenden Domains zu sehen, siehe [Miro-Domains](../technical-guidelines/07-miro-domains-reference.md).

## Wenn du einen Proxy verwendest

Bitte stelle sicher, dass du Miro einen Bypass zur Verfügung stellst. Die folgenden Angaben sind hilfreich.

- Der Proxyserver muss WebSocket-Verbindungen (HTTP/2) unterstützen.
- Die HTTP-Version des Proxys sollte auf 1.1 eingestellt werden.
- Quell-IP/Host: siehe die NAT-IPs oben (nur für Atlassian-Integrationen verwendet).
- Quellport: **80.** 80 wird für Nutzer verwendet, die über HTTP auf Miro zugreifen, um sie zu HTTPS zu leiten (es wird nicht empfohlen, 80 zu blockieren).
- Zielport: **443 (SSL).**443 wird für HTTPS verwendet.
- Protokoll: HTTPS
- TLS: 1.2. (Wir werden in AWS gehostet und verwenden AWS Security Policies. Sobald AWS und alle unsere Plugin-Partner die 1.3. unterstützen, können auch wir migrieren).
- Der Timeout-Wert auf dem Proxyserver sollte verlängert werden. Wahrscheinlich wartet dein System etwa 60-90 Sekunden, um sich zu verbinden. Es wäre am besten, die Zeit auf 120-180 Sekunden zu verlängern.
- Der Proxyserver sollte die Anfrage- und Antwort-Header nicht abschneiden. Bitte überprüfe, ob die *Upgrade*und *Connection*Header vom Client verwendet werden.

[Hier ist ein Artikel](../../tools/troubleshooting/02-allowlist-miro-mailers.md) mit mehr Informationen über die Zulassungslisten der benötigten Mailer.
