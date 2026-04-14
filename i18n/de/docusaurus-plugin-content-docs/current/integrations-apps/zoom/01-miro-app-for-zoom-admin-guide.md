---
title: "Miro-App f\xFCr Zoom (Admin-Leitfaden)"
article_id: 360022039379
translation_id: 360022039379
locale: de
sidebar_position: 1
created_at: '2021-05-28T04:43:09Z'
updated_at: '2025-02-26T11:51:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: zoom
---

Die Miro-App für Zoom ermöglicht es Teams, einen digitalen Konferenzraum einzurichten und bei Meetings und Workshops effektiv zusammenzuarbeiten, indem sie Miro direkt in Zoom nutzen. Die App bietet die Zusammenarbeitsfunktionen von Miro direkt in Zoom und macht das Onboarding von Gästen besonders einfach. Einsteigern bei Miro bieten wir Whiteboarding mit registrierungsfreiem Zugriff an.

Diese Anleitung hilft Zoom- und Miro-Admins, diese Option für ihre Personen zu aktivieren.

:::note
Lies unseren [Nutzungsleitfaden für die Miro-App für Zoom](02-miro-app-for-zoom-user-guide.md).
:::

> **Erhältlich für:** alle Miro Preispläne, alle Zoom Preispläne
> *Bei den Zoom Business- und Enterprise-Preisplänen muss der Admin die Miro-App möglicherweise vorab genehmigen.
> **Verfügbar mit**: Desktop-Version

## So aktivierst du die App in Zoom

### App-Erkennung aktivieren

1. Melde dich im Zoom-Webportal als Admin mit Berechtigung zum Bearbeiten der Kontoeinstellungen an.
2. Klick im Navigationsbereich die **Kontoverwaltung** und dann die **Kontoeinstellungen** an.
3. Klick auf die Registerkarte **Zoom Apps**.
4. Vergewissere dich, dass die **Schnellstart-Schaltfläche für Zoom Apps** aktiviert ist.  So können die Nutzer deines Kontos die Schaltfläche Zoom Apps ![](../../../../../../docs/integrations-apps/zoom/images/21017682787474_mceclip0.png) mceclip0 alt.pngalt auf dem Desktop-Client  sehen.
5. Wenn die Einstellung deaktiviert ist, klicke auf den Kippschalter, um sie zu aktivieren. Wenn ein Bestätigungsdialog angezeigt wird, klicke auf **Einschalten**, um die Änderung zu bestätigen.

Zoom bietet außerdem zusätzliche Dokumentation dazu, wie du Zoom-Apps nur für bestimmte Gruppen oder Personen aktivierst. Mehr dazu erfährst du hier/span> [im Zoom-Hilfecenter.](https://support.zoom.us/hc/articles/360061555152)

Zoom_apps_quick_launch.jpg
Schnellstart-Schaltfläche für Zoom Apps aktivieren

Dies aktiviert Zoom-Apps in der oberen Leiste im Haupt-Client von Zoom sowie in der unteren Leiste von Meeting-Clients für die Nutzer deines Kontos.

### So kannst du die App in Zoom vorab genehmigen

Wenn du Zoom-Admin für einen Zoom Business- oder Enterprise-Plan bist, musst du die Miro-App eventuell [hier](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA) vorab genehmigen, damit die Nutzer darauf zugreifen können.

![pre-approve_Miro_app.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653155474_pre-approve%20Miro%20app.jpg)*Vorabgenehmigung der Miro-App*

### Nutzer im Konto auswählen, die die App installieren können

Zusätzlich zur Vorabgenehmigung für die Miro-App kannst du auswählen, welche Personen oder Gruppen sie installieren können.

allow_users_to_install_the_app.jpg
/span>Nutzer und Gruppen auswählen, die die Miro-App installieren können

Sobald du die Miro-App genehmigt und in deinem Firmenkonto installiert hast, können deine Nutzer vom Zoom-Client aus auf sie zugreifen und sie installieren.

Weitere Informationen findest du in der [Dokumentation von Zoom](https://support.zoom.us/hc/articles/360061555152).

## So aktivierst du die App in Miro

> **Einrichtung durch:** Unternehmens-Admins im Enterprise-Preisplan

Wenn du den [Enterprise-Preisplan](../../plans-billing/miro-plans/04-enterprise-plan.md) hast und die Installation auf genehmigte Apps beschränkt hast, füge die Miro-App für Zoom bitte deiner Liste der genehmigten Apps in **Unternehmenseinstellungen > Apps > Apps verwalten** hinzu.  Hierzu kannst du die clientID 3074457354625507111 in die Suche einfügen und die App zur Installation aktivieren.

approve_Zoom_on_Enterprise_plan.jpg
Genehmigte Apps in den Unternehmenseinstellungen

## So können Nutzer die App installieren

Personen finden die Miro-App für Zoom im [Zoom Marketplace](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA) oder im [Miro Marketplace](https://miro.com/marketplace/zoom-app/).

Der erste Schritt im Installationsprozess ist das Autorisieren der Miro-App für Zoom.

install_Miro_app_for_Zoom.jpg
Zugang für Miro auf dein Zoom-Konto/span>

Sobald sie autorisiert wurde, leitet die App die Nutzer in ihre Zoom Desktop-App und zeigt die neu installierte Miro-App an.  Hinweis: Die Nutzer müssen bei ihrem Zoom-Konto angemeldet sein, um die App hinzuzufügen. /span>

Miro-Nutzer müssen **sich anmelden**, um ihre Boards zu sehen. Dadurch werden sie an den Browser ihres Systems weitergeleitet und aufgefordert, sich bei Miro anzumelden oder die App direkt in Miro zu autorisieren. Sie können die App für jedes Team installieren, zu dem sie Zugriff haben.

install_Zoom_for_a_Miro_team.jpg
Installiere die App für eines deiner Miro-Teams/span>

Nutzer werden anschließend zurück in die Zoom Desktop-App geleitet und sehen dort ihre Miro-Übersicht, einschließlich aller vorhandenen Teams und Boards.

![Miro_dashboard_in_Zoom.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653159442_Miro%20dashboard%20in%20Zoom.jpg)*Nutzer können ein Board aus ihrem Dashboard auswählen und es in Zoom öffnen*

## Zugriffseinstellungen für die gemeinsame Nutzung von Boards verstehen

Personen können die entsprechenden Berechtigungen für die gemeinsame Nutzung des Boards in einem Zoom-Meeting festlegen. Sie können zwischen vier Optionen wählen: **Jeder in Zoom kann bearbeiten/kommentieren/ansehen** oder **privat** (was bedeutet, dass die Freigabeeinstellungen dieselben sind wie auf der Miro-Seite).

board_embed_sharing_settings.jpg

*Zugriffseinstellungen für dein Board konfigurieren*

Die Option Zugriffseinstellungen folgt organisationsweiten Zugriffskontrollen.  Wenn du die öffentliche Linkfreigabe für Board-Einbettungen im [Enterprise-Plan](../../plans-billing/miro-plans/04-enterprise-plan.md) eingeschränkt hast, steht diese Option den Nutzern nicht zur Verfügung. Mehr erfährst du unter Verwalten der unternehmensweiten Freigaberichtlinien für Integrationen zum Einbetten[.](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)

publi_editing_is_turned_off.jpg
Die öffentliche Bearbeitung wurde durch einen Unternehmens-Admin deaktiviert

## Häufige Fragen

1. *Auf welche Daten greift die Miro App für Zoom zu?*
   - Die Miro-App für Zoom fragt Informationen zum Profil des Nutzers ab, um ein Board mit einem bestimmten Nutzer zu verknüpfen. Unsere App greift **nicht** auf Meeting-Inhalte wie Videos, Audios, Chats und/oder Meeting-Dateien zu und wird daher nicht in der Meldung über aktive Apps von Zoom angezeigt.
2. *Kann die App auf Tablets oder mobilen Geräten installiert werden?*
   - Nein, die Miro-App für Zoom ist nur auf dem Desktop verfügbar.
3. *Für welches Betriebssystem funktionieren die Zoom Apps?*
   - Mac OS und Windows.
4. *Welche Version von Zoom wird benötigt, um Zoom Apps zu nutzen?*
   Version: 5.7.3,
