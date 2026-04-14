---
title: Einrichtung der Power BI Integration (Admin-Leitfaden) (BETA)
article_id: 18945328862994
translation_id: 18945328862994
locale: de
sidebar_position: 8
created_at: '2024-05-15T12:57:57Z'
updated_at: '2025-11-25T15:42:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
availability:
  notes: 'Verfügbar für: Free-, Starter-, Business-, Education- und Enterprise-Preispläne
    Verfügbar im: Browser, Desktop-App Erforderliche Rolle: Unternehmens-Admin'
---

Unternehmen, die Microsoft Power BI in Miro integrieren möchten, finden in diesem Leitfaden eine Schritt-für-Schritt-Anleitung zum Einrichten der Integration, zum Aktivieren für ihr Team und zum Umgang mit Sicherheitsaspekten.

Die wichtigsten Funktionen:

- Power BI Reports und Dashboards in Miro-Boards einbetten
- Bestimmte Diagramme in Miro-Boards importieren
- Aktualisierte Power BI Inhalte direkt in Miro-Boards anfordern

:::tip
Die Power BI Integration befindet sich derzeit in der privaten Beta-Phase.
:::

### Technische Implementierung

Miro ist über die [REST-API](https://learn.microsoft.com/rest/api/power-bi/) in Power BI integriert, zusammen mit den [eingebetteten Power BI Analytics-Client-APIs](https://learn.microsoft.com/javascript/api/overview/powerbi/). Nutzer können ihre Power BI Reports oder Dashboards ganz einfach mit Miro-Boards verknüpfen, indem sie den Power BI Zugriff autorisieren. Zur Authentifizierung verwenden wir [OAuth2.0](https://learn.microsoft.com/entra/identity-platform/v2-protocols).

### Integrationsanforderungen

Vergewissere dich, dass dein Abo Folgendes enthält:

- Power BI Cloud
- Unterstützte Abos:
  - Power BI Premium per capacity SKU
  - Fabric Capacity Reservation SKU

## Die Power BI Integration einrichten

1. Melde dich bei Microsoft Entra als Admin an.
2. Gehe zu **Enterprise-Apps** > **Einwilligung und Berechtigungen** > **Admin-Zustimmungseinstellungen**
3. Unter **Admin-Zustimmungsanfragen** kannst du **Ja** festlegen, **damit Nutzer die Admin-Zustimmung für Apps anfordern können, denen sie nicht zustimmen können**.
4. Unter **Wer kann Admin-Zustimmungsanfragen überprüfen**, wähle die erforderlichen Nutzer, Rollen und Gruppen aus, die Admin-Zustimmungsanfragen überprüfen dürfen.
5. Nutzer können dann um Genehmigung bitten. Um den Bildschirm für die Genehmigungsanfragen anzuzeigen, kann ein Nicht-Admin-Nutzer einen Power BI Link in ein Miro-Board im Miro-Team einfügen, das für den Miro + Power BI Integrationstest aktiviert wurde.
6. Die in Schritt 4 ausgewählten Admins können die ausstehende Anfrage im Admin-Bildschirm für Genehmigungsanfragen genehmigen.
7. Sobald sie genehmigt wurde, kann jeder Nutzer die Miro + Power BI Integration selbst autorisieren.
8. Um zu überprüfen, ob die Integration funktioniert, füge einen Link zu einem Power BI Dashboard oder einem Report in einem Miro-Board ein, das zu einem Team gehört, für das du die Integration aktiviert hast.
9. Klicke auf **Verbinden**, um die Autorisierung auf der Power BI Webseite zu bestätigen.
10. Es öffnet sich ein Dialogfenster, in dem du auswählen kannst, welche Diagramme du einbetten möchtest. Wähle ein Diagramm aus und klicke auf **Diagramm hinzufügen**.
11. Die Diagramme werden als Bilder zu deinem Miro-Board hinzugefügt.

## Die Power BI Integration desaktivieren

Admins können die Berechtigung widerrufen, indem sie die Miro-App aus den Enterprise-Apps in Microsoft Entra löschen.

1. Melde dich bei Microsoft Entra an.
2. Klicke auf **Enterprise-Apps**  > **Einwilligung und Berechtigungen**.
3. Wähle **Alle Apps** aus der Liste der Apps aus.
4. Suche die App **Contenthub Microsoft Power BI Integration** in der Liste.
5. Klicke auf die App, um auf ihre Eigenschaften zuzugreifen.
6. Klicke in den App-Eigenschaften auf **Löschen**.

## Integrationsbeschränkungen

- Das Einbetten in öffentliche Boards ist nicht möglich.
- Das Einbetten von Datensatz-Links wird nicht unterstützt.
- Das Einbetten von Links aus dem Freigabemenü wird nicht unterstützt.

## Datenaufbewahrung

Die eingebetteten Power BI Daten unterliegen der Standard-Datenaufbewahrungsrichtlinie von Miro, die für alle Kundendaten gilt. Hier findest du unseren [Zusatz zur Datenverarbeitung bei Miro](https://miro.com/legal/documents/Miro-Data-Processing-Addendum.pdf).

Verschiedene Datentypen aus eingefügten Power BI Links werden als Bild abgerufen und in Miro gespeichert:

- Bilder von Kacheln aus Power BI Dashboards
- Bilder von Grafiken aus Power BI Reports
- Titel von Power BI Dashboards, Berichten, Grafiken und Kacheln
- Seitennamen aus Power BI Reports
- Filternamen und -werte aus Power BI Reports

## Häufige Fragen

Warum ist die Power BI Integration in der Beta-Phase?

In der Beta-Phase wird Feedback gesammelt, um die Stabilität und das Nutzererlebnis zu verbessern. Die Sicherheit hat weiterhin höchste Priorität.
