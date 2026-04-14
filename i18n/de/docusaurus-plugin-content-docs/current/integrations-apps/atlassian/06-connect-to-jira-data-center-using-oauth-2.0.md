---
title: Über OAuth 2.0 mit dem Jira Data Center verbinden
article_id: 25753304280466
translation_id: 26513375357842
locale: de
sidebar_position: 8
created_at: '2025-05-06T09:04:13Z'
updated_at: '2025-05-21T09:26:43Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Wer kann das machen: Unternehmens-Admins mit Jira-System-Admin-Berechtigungen
    Preispläne: Unternehmen Plattformen: Browser, Desktop'
---

:::note
Die Verbindung mit dem Jira Data Center über OAuth 2.0 ist nur auf Organisationsebene aktiviert.
:::

## Voraussetzungen

- Vergewissere dich, dass du die folgenden Berechtigungen hast:
  - Jira-System-Admin-Berechtigungen
  - Unternehmens-Admin-Rolle bei Miro
- Erstelle einen OAuth 2.0 App-Link im Jira Data Center. Um zu erfahren wie, sieh (externer) [Support für Atlassian Jira-Apps](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Create%20an%20incoming%20link%20using%20application%20links).
  - Verwende die folgende Umleitungs-URL, wenn du dazu aufgefordert wirst:
    https://integrations.miro.com/api/external-auth/oauth2/callback
  - Um automatische Webhooks zu verwenden, wähle **Admin** für deinen Umfang aus.

## Verbinde Miro mit dem Jira Data Center über OAuth 2.0

1. Wähle auf deinem Miro-Dashboard deinen Avatar oben rechts aus und gehe zur (Enterprise) **Admin-Konsole** oder(Starter und Business) **Einstellungen**.
2. Gehe in der linken Seitenleiste zu **Apps und Integrationen ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Apps** > **Tab Apps verwalten**.
3. Vergewissere dich, dass **Nur Apps aus der Liste unten zulassen** aktiviert ist.
4. In der **App**-Spalte, für **Jira-Karten** wähle **Einstellungen** aus.
5. Wähle **Neue Verbindung hinzufügen** aus.
6. Wähle unter **Jira-Einrichtung** **Jira-Datencenter** aus.
7. Wähle unter **Authentifizierungsmethode** **OAuth 2.0** aus.
8. Für **Jira-URL** gib die URL deiner Jira-Instanz ein.
9. (Optional) Um diese Verbindung zur Standardverbindung für alle Teams in deiner Organisation zu machen, klicke auf **Als Standard festlegen**.
10. Gib die Jira-**Client-ID** ein.
    **Weitere Informationen**: Siehe (Extern) [Einen eingehenden Link konfigurieren](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
11. Gib das Jira-**Client-Geheimnis** ein.
    **Weitere Informationen**: Siehe (Extern) [Konfigurieren eines eingehenden Links](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
12. Wähle deinen Bereich aus.
    Um automatische Webhooks zu verwenden, wähle **Admin** oder **System-Admin** aus.
13. (Optional) Um Echtzeit-Updates von Jira in Miro zu erhalten, aktiviere **Webhook automatisch erstellen**.
    > ✏️ Optional, kannst du den Webhook später manuell hinzufügen.
14. Wähle **Verbinden** aus.
    > ✏️ Beim ersten Versuch eines Nutzers, eine Jira-bezogene Aktion auszuführen, wird er zur Authentifizierung aufgefordert. Sie müssen sich nicht erneut authentifizieren.

## Was kommt als Nächstes?

Um deine verbundenen Jira-Instanzen anzuzeigen und zu verwalten, gehe zu **Admin-Konsole** | **Einstellungen** > **Apps und Integrationen ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Apps verwalten**. Wähle dann unter der **App**-Spalte für **Jira-Karten** **Einstellungen** aus.

Um zu erfahren, wie du deine Teams mit der Jira-Standardinstanz verbindest, siehe [Teams in der Organisation mit den Jira-Standardeinstellungen verbinden.](https://help.miro.com/hc/articles/26438407676434)

## Häufig gestellte Fragen

**Erfordert die Auswahl von Admin für den Bereich, dass alle Nutzer Admin-Berechtigungen in Jira haben?**

Nein. Der Admin-Bereich bedeutet, dass Admin der höchste Geltungsbereich ist, den ein Nutzer in Miro haben kann. Der Bereich ist pro Nutzer ohnehin begrenzt, je nachdem, welche Berechtigungen jemand in Jira hat.

**Kann ich das Jira Data Center auf Teamebene mit OAuth 2.0 verbinden?**

Nein. Nur auf Organisationsebene.
