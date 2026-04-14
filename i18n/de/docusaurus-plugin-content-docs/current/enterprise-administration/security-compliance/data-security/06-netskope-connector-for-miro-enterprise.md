---
title: "Netskope Connector f\xFCr Miro Enterprise"
article_id: 4415711060498
translation_id: 4415711060498
locale: de
sidebar_position: 6
created_at: '2022-01-19T06:23:42Z'
updated_at: '2025-02-26T11:27:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Der benutzerdefinierte Miro Connector für Netskope ermöglicht die Sichtbarkeit von Datenleck-Ereignissen und erlaubt die Verwaltung des folgenden Datenverkehrs innerhalb von Miro:

- [Board-Backup herunterladen](../../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)

Dieser Leitfaden enthält Schritte, um Netskope für den Enterprise-Preisplan von Miro zu konfigurieren und beschreibt die Benutzererfahrung.

> **Verfügbar für**: [Enterprise-Preisplan](../../../plans-billing/miro-plans/04-enterprise-plan.md)

### Erstellen einer neuen Miro-App in Netskope

Gehe innerhalb deiner Netskope-Instanz zu **Einstellungen > Security Cloud Platform > App-Definition** und klicke auf **NEUE CLOUD-APP**:

new_cloud_app.jpg
![Erstellen einer Cloud-App in Netskope](blob:https://miro.atlassian.net/8cb061a4-e184-4bd6-bb95-774cd34fc8e7#media-blob-url=true&id=78b7a8cb-792a-41da-bf16-b26ca4480059&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.08.43.png&size=181298&height=513&width=1028&alt=)

Um eine neue App in Netskope zu erstellen, wirst du aufgefordert, die folgende JSON-Datei **miro-activities-for-netskope.json** zu importieren:

```
{
Version: 0.0.0.1,
{
"domain_name": "miro.com",
"uri_path": "/api/v1/boards/.+/",
"http_method": GUTE
"uri_param": [{ "key": "archive", "value": "true" }],
"resp_code": 200,
"Muster": "",
"activity_name": Herunterladen
{
{
"domain_name": "miro.com",
"uri_path": "/api/v1/boards/.+/resources/.+/files/original",
"http_method": GUTE
"uri_param": [],
"resp_code": 307,
"Muster": "",
"activity_name": Herunterladen
{
{
```

Gib den Anwendungsnamen ein, wähle die Option **Benutzerdefinierter Connector** und klicke auf **IMPORT AUS DATEI > Zur Aktivitätsliste hinzufügen,** um die im vorherigen Schritt heruntergeladene Datei **miro-activities-for-netskope.json** hochzuladen**.**

uploading_the_file.jpg
Hochladen der Datei

Nach dem Import der Datei **miro-activities-for-netskope.json** werden die aufgezeichneten Aktivitäten angezeigt. Jetzt kannst du mit einem Klick auf **SPEICHERN** fortfahren und die Miro-App erstellen.

save_the_app.jpg
![Speichern der App](blob:https://miro.atlassian.net/b9da4e19-b3b1-4c25-aed3-762f458fd639#media-blob-url=true&id=f7549007-0265-42e1-b946-a3e167124f12&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.26.58.png&size=209044&height=693&width=1028&alt=)

Nach der Erstellung der App musst du diese auswählen und dann auf **ÄNDERUNGEN ÜBERNEHMEN** klicken.

apply_changes.jpg
/strong>Die Option, Änderungen in der Miro-App anzuwenden

![](blob:https://miro.atlassian.net/82b8ac6e-1952-44e7-a62f-cefb7dbee6ab#media-blob-url=true&id=975f42e8-de5d-4bbb-ae07-c243cce9bb2f&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.32.06.png&size=257154&height=575&width=1780&alt=)

### Erstellen einer neuen Richtlinie für deine Miro-App in Netskope

Sobald die Anwendung erstellt ist, kannst du mit der Erstellung einer Richtlinie fortfahren. Navigiere dazu zu **Richtlinie > E****chtzeitschutz** und klicke auf **NEUE RICHTLINIE > Cloud-App-Zugriff.**

create_a_policy.jpg
![Erstellen einer Richtlinie für Miro-App](blob:https://miro.atlassian.net/d2ae8479-8f5c-4417-8b09-2b57ee344d90#media-blob-url=true&id=e9c82ee5-cdea-4b33-8491-9613a848be81&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.39.02.png&size=107320&height=321&width=635&alt=)

Hier in **Destination** musst du die Miro-App angeben, die du im vorherigen Schritt erstellt hast, einen **Richtliniennamen** einrichten und auf **SPEICHERN** klicken.

save_the_policy.jpg
/strong>Speichern der Richtlinie

![](blob:https://miro.atlassian.net/abf26593-27ad-40f4-b3e5-731a9e58d062#media-blob-url=true&id=0edd2e23-2762-4173-8f3f-9a7bb74bf217&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.45.14.png&size=200430&height=722&width=1575&alt=)altDann kannst du auswählen, wo du die Richtlinie platzieren möchtest und auf altSPEICHERN klicken.

move_policy.jpg
Auswählen, wo du die Richtlinie platzieren möchtest

Schließlich kannst du Änderungen anwenden, indem du auf die Schaltfläche **ÄNDERUNGEN ÜBERNEHMEN** klickst.

applying_changes.jpg
Änderungen übernehmen

![](blob:https://miro.atlassian.net/41cdf802-aa1c-4f9a-bd22-950ea6ad755e#media-blob-url=true&id=7f85d987-6550-4271-90da-c9273a0cbc9a&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2019.29.17.png&size=157218&height=490&width=1576&alt=)

### Visualisierung von Ereignissen

Sobald du alle Einstellungen vorgenommen hast, kannst du den Datenverkehr visualisieren, indem du zu **Skope IT** navigierst, nach der benutzerdefinierten Miro-App filterst und auf **Ereignisse anzeigen**, wie folgt, klickst:

see_events.jpg
Die Option zum Anzeigen von Datenverkehrs-Ereignissen

### Benutzererfahrung

Die Nutzer, für die die Download-Aktivitäten blockiert werden sollen, müssen den Netskope-Client auf ihrem Computer installiert haben.  Wenn die Nutzer versuchen, ein Download-Backup durchzuführen, blockiert Netskope die Aktion und zeigt ein Popup-Fenster des nativen Betriebssystems mit einer Meldung an.

alert.jpg
Eine Nachricht, die Nutzern angezeigt wird, die kein Backup eines Miro-Boards herunterladen dürfen
