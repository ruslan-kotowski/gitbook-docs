---
title: "Glean f\xFCr Miro einrichten (Admin-Leitfaden)"
article_id: 27581463837330
translation_id: 27581463837330
locale: de
sidebar_position: 2
created_at: '2025-06-23T10:52:57Z'
updated_at: '2026-01-02T09:57:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Voraussetzungen

1. Du bist ein **Miro Org Admin** und ein **Glean Admin**.
2. Registriere in Glean eine **OAuth-Client-ID.** Lies die [Glean-Dokumentation](https://developers.glean.com/api-info/client/authentication/oauth) für mehr Details.
3. Aktiviere die benutzerspezifische Datenschutzeinstellung **Erlaube das Speichern des Chatverlaufs bis zu 30 Tage**.

## Installiere die Glean-App

Um zu beginnen, installiere die Glean-App aus dem Miro Marketplace für die relevanten Teams in deiner Organisation.

1. Wechsle zu deinen **Unternehmenseinstellungen** und klicke auf **Apps & Integrationen**.
2. Klicke im **Apps**-Tab auf **Apps hinzufügen**, um den Marketplace zu öffnen.
3. Suche nach "Glean". Du kannst es auch finden, indem du seine Client-ID in die Suchleiste einfügst: `1202342442818548396`.
4. Wähle im Profil der App, wo die App hinzugefügt werden soll: entweder für **alle Teams** oder **spezifische Teams...** auswählen.
5. Überprüfe die Berechtigungsseite. Die Glean-App wird von Miro entwickelt und gewartet und erfordert keine spezifischen Berechtigungen.
6. Wähle **Hinzufügen**, um die Installation abzuschließen.

## Single Sign-On Setup (Okta)

Falls deine Organisation Okta als Single Sign-on (SSO)-Anbieter verwendet, musst du eine Okta OpenID Connect (OIDC) Web-App erstellen, bevor du mit den nächsten Abschnitten fortfährst.

1. Erstelle eine neue Okta-App unter Verwendung der in der Dokumentation [hier](https://help.okta.com/en-us/content/topics/apps/apps_app_integration_wizard_oidc.htm) genannten Schritte.
   1. Wähle **OIDC - OpenID Connect** als Anmeldemethode.
   2. Wähle **Webanwendung** als App-Typ.
   3. Stelle sicher, dass das **Refresh Token** im Abschnitt **Grant type** > **Core grants** aktiviert ist.
   4. Füge `https://integrations.miro.com/api/external-auth/oauth2/callback` als **Sign-in redirect URIs** hinzu.
   5. Wähle **Speichern**.
2. Kopiere die **ClientId** und das **Client Secret** aus dem Abschnitt Anmeldeinformationen. Diese werden in den nächsten Abschnitten benötigt, um die Integration abzuschließen.

## Single Sign-on (SSO) konfigurieren

Folge diesen Schritten, um die App zu konfigurieren:

1. Gehe auf der Seite **Apps & Integrations** zu **Manage apps**.
2. Finde "Glean" in deiner Liste der installierten Apps und klicke auf dessen **Einstellungen**. Falls du die App nicht siehst, suche sie mit der Client-ID (`1202342442818548396`) und genehmige sie zuerst.
\{1>OKTA<1\}3. Klicke auf **Speichern**, um die Konfiguration zu übernehmen.

:::note
Wenn du Azure verwendest, stelle sicher, dass dein Microsoft Entra-Admin "Im Namen deiner Organisation zustimmen" für die Glean-App im Microsoft Entra-Admincenter ausgewählt hat, damit sich Nutzer korrekt authentifizieren können.
:::

## Glean Admin-Konsole konfigurieren

Bevor du Glean in Miro verwenden kannst, musst du den Zugriff über OAuth-Token in deiner Glean Admin-Konsole konfigurieren.

1. Öffnen Sie Ihre **Glean Admin-Konsole** und navigieren Sie zu **Einstellungen** > **Drittanbieterzugang (OAuth)**.
2. Aktivieren Sie im Abschnitt **IDP-konfiguriertes OAuth** die Option **IDP OAuth für API-Zugriff aktivieren**.
3. Klicken Sie auf **Einstellungen verwalten** und wählen Sie Ihren **SSO-Anbieter** aus.
4. Fülle die Anbieterdetails basierend auf deinem Single Sign-on (SSO) Anbieter aus.
   - **Okta**
     - Autorisierungsserver-URL: `https://<subdomain>.okta.com`
     - Erlaubte Client-ID(s): Client-ID der Okta-App, die im vorherigen Abschnitt erstellt wurde.
     - Der Rest der Formularfelder kann leer gelassen werden.
   - **Azure**
     - Aussteller-Subdomain: `https://login.microsoftonline.com/<tenant-id>/v2.0`
     - Erlaubte Client-IDs: `a49fdb25-3b5f-4d3b-bedf-6da7be2b4bf4`
   - **GSuite**
     - Erlaubte Client-IDs: `1062019541050-pf2ndc9f3o4lrmkupj3cj0fep5hkecns.apps.googleusercontent.com`
5. Wähle **Speichern**, um die Einstellungen anzuwenden.

> ⏰ **Hinweis:** Es kann bis zu 30 Minuten dauern, bis Änderungen in der Glean Admin-Konsole wirksam werden.

## Die Glean-App nutzen

Sobald du die App installiert und konfiguriert hast, können Nutzer in den zugewiesenen Teams sie nutzen. Beim ersten Öffnen der Glean-App in Miro wird der Nutzer zur Authentifizierung aufgefordert.

1. Öffne ein Miro-Board und klicke auf das Glean-Symbol in der Symbolleiste, um das seitliche Feld zu öffnen.
2. Klicke auf **Glean verbinden**, um die Autorisierung zu starten.
3. Es erscheint ein Dialogfeld zur Single Sign-on (SSO)-Autorisierung.
4. Nach erfolgreicher Authentifizierung erscheint die Glean-Benutzeroberfläche, bereit zur Nutzung.

## Sicherheit

Weitere Informationen zu Daten und Sicherheit findest du in diesem [Sicherheitsdokument](https://docs.google.com/document/d/1lGLF7eASQb2uMRmMEAaH-GzFhyz4UKfwMeqSQOSYPdM/edit?tab=t.0#heading=h.gu9ng058yy7y).
