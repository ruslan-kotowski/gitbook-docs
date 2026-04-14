---
title: Jira OAuth 1.0 in Miro veraltet
article_id: 28738797627538
translation_id: 28739453426194
locale: de
sidebar_position: 13
created_at: '2025-08-13T12:34:16Z'
updated_at: '2025-10-20T14:49:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Personen: Unternehmens-Admins Pläne: Starter, Business, Enterprise, Education
    Plattformen: Browser, Desktop'
---

Die Jira OAuth 1.0-Authentifizierung ist ab August 2025 veraltet.

Wenn Ihre Organisation bereits auf Jira OAuth 2.0 aktualisiert hat, können Sie diesen Artikel ignorieren. Es sind keine Maßnahmen von Ihrem Unternehmens-Admin erforderlich. Sie können mit Ihrem Unternehmens-Admin bestätigen, dass Ihre Organisation OAuth 2.0 verwendet.

:::warning
Wenn Ihre Organisation nicht auf OAuth 2.0 aktualisiert hat, kann Ihre Jira-Integration mit Miro, einschließlich Jira Cloud, Server und Data Center, unterbrochen werden.
:::

Nur Unternehmens-Admins können Teams in ihrer Organisation upgraden.

Im Falle einer Unterbrechung stoppt die Synchronisierung zwischen Miro und Jira, bis Ihre Organisation auf OAuth 2.0-Authentifizierung aktualisiert. Bestehende Jira-Karten bleiben auf Ihren Miro-Boards.

Unterbrechung bedeutet, dass der Import nicht verfügbar ist, Karten nicht aktualisiert werden, Details nicht geladen werden können und das Erstellen und Aktualisieren eines Planers nicht möglich ist.

Um eine Unterbrechung zu vermeiden, empfiehlt Miro, dass Ihre Unternehmens-Admin(s) sofort auf Jira OAuth 2.0 aktualisieren.

:::tip
Admins können Ihre OAuth-Version überprüfen.
:::

## Warum wird OAuth 1.0 eingestellt?

Atlassian hat das OAuth 1.0-Authentifizierungsprotokoll eingestellt und unterstützt es nicht mehr.

**Mehr Informationen:** Siehe (Extern) [OAuth 1.0a für REST-APIs (Veraltet)](https://developer.atlassian.com/cloud/jira/platform/jira-rest-api-oauth-authentication/).

## Überprüfe deine OAuth-Version

Als Enterprise-Team-Admin oder als Admin eines Starter- oder Business-Preisplans kannst du überprüfen, ob dein Team OAuth 1.0 oder OAuth 2.0 verwendet.

Befolge diese Schritte:

1. Klicke in deinem Miro-Dashboard auf deinen Avatar oben rechts und wähle **Admin-Konsole** aus.
2. Gehe zu **Teams** > **[Teamname]**.
3. Klicke auf **Apps**.
4. Finde und klicke auf **Jira-Karten**.
5. Gehe zu **Admin-Einstellungen** > **Jira-Konfiguration**.
   Die Konfiguration zeigt an, welche OAuth-Version dein Team verwendet.
6. (Optional) Wiederhole die Schritte 1-5 für andere Teams, die du überprüfen möchtest.
7. Benachrichtige deine Unternehmens-Admins über alle Teams, die nicht OAuth 2.0 verwenden.

## Finde deinen Unternehmens-Admin

Um deine Unternehmens-Admins zu identifizieren, gehe wie folgt vor:

:::note
(Enterprise) Wenn Vertraulichkeitsschutz für Teams aktiviert ist, können Nicht-Unternehmens-Admins keine Mitgliederlisten ansehen.
:::

1. Gehe zu den **Team-Profil-Einstellungen** in Miro.
2. Öffne die Seite **Mitglieder**.
3. Klicke auf **Zusätzliche Rollen**.
4. Finde Nutzer mit der **Unternehmens-Admin**-Rolle.

:::tip
Um sicherzustellen, dass dein Team auf OAuth 2.0 upgraded und mögliche Störungen vermieden werden, teile diesen Artikel mit deinen Unternehmens-Admins.
:::

## Upgrade auf OAuth 2.0 für Unternehmens-Admins

Als Unternehmens-Admin stehen Ihnen die folgenden Ressourcen zur Verfügung, um Ihr Unternehmen auf OAuth 2.0 umzustellen:

- [Verbindung zu Jira Cloud mit OAuth 2.0 herstellen](https://help.miro.com/hc/articles/8588617184402)
- [Verbindung zu Jira Data Center mit OAuth 2.0 herstellen](https://help.miro.com/hc/articles/25753304280466)
- [Teams in der Organisation zu den Standard-Jira-Einstellungen verbinden](https://help.miro.com/hc/articles/26438407676434)

## Zwischenlösung

Wenn OAuth 2.0 derzeit keine Option für deine Organisation ist, bietet Miro eine [Zwischenlösung mit OAuth 1.0](https://help.miro.com/hc/articles/27689156602514) an.

Miro empfiehlt jedoch, auf OAuth 2.0 zu wechseln, um die sicherste und zukunftssicherste Authentifizierungsmethode zu nutzen, die den aktuellen Standards von Atlassian entspricht.

## Zusätzliche Hilfe

Wenn du oder dein Unternehmens-Admin Fragen habt, kontaktiere den [Miro Support](https://help.miro.com/hc/articles/360020185799).
