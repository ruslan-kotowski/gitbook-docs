---
title: Teams in der Organisation mit den Standard-Jira-Einstellungen verbinden
article_id: 26438407676434
translation_id: 26441928112658
locale: de
sidebar_position: 6
created_at: '2025-05-02T14:34:41Z'
updated_at: '2025-10-21T12:08:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Wer kann es tun: Unternehmens-Admins Welche Preispläne: Enterprise Welche
    Plattformen: Browser, Desktop'
---

Unternehmens-Admins können Teams in ihrer Organisation in einer Massenaktion verbinden, um globale Jira-Einstellungen zu verwenden, die die auf Teamebene angegebenen Einstellungen überschreiben.

## Voraussetzungen

- Stelle sicher, dass du die Rolle des Unternehmens-Admins in Miro hast.
- Stelle sicher, dass du eine Standardverbindung zu einem [Connect to Jira Data Center using OAuth 2.0](https://help.miro.com/hc/articles/25753304280466) hast.

## Teams mit den Standard-Jira-Einstellungen verbinden

1. Wähle auf deinem Miro-Dashboard deinen Avatar oben rechts aus und gehe zur **Admin-Konsole** | **Einstellungen**.
2. Gehe in der linken Seitenleiste zu **Apps und Integrationen ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Apps** > **Apps verwalten**-Tab.
3. Vergewissere dich, dass **Nur Apps aus der Liste unten zulassen** aktiviert ist.
4. Unter der Spalte **App**, wähle für **Jira-Karten** **Einstellungen** aus.
5. Wähle unter **Teams zur Standardinstanz hinzufügen** jedes Team aus, das du verbinden möchtest, oder klicke auf **Alle auswählen**.

   > ✏️ Die Liste zeigt nur Teams an, die keine globalen Organisationseinstellungen verwenden.
6. Klicke auf **&lt;Anzahl der Teams&gt; zur Standardinstanz hinzufügen**.

   > ✏️ Nutzer, die die globale Jira-Instanz in deiner Organisation nicht bereits verwenden, werden migriert und müssen sich erneut authentifizieren.

   > ✏️ Nutzer, die von einer anderen Jira-Instanz migriert wurden, werden aufgefordert, sich erneut zu authentifizieren, wenn sie zum ersten Mal eine Jira-bezogene Aktion in Miro versuchen.

## häufige Fragen

**Verwenden Teams die globale Jira-Verbindung auf unbegrenzte Zeit?**

Nein. Du kannst die Jira-Einstellungen für ein bestimmtes Team später ändern.

**Welche Teams sollten die globale Jira-Verbindung verwenden?**

Die Verwendung der Organisationseinstellungen wird im Allgemeinen bevorzugt, da du dafür weniger Verwaltung benötigst. Wenn eine deiner Teamverbindungen die gleichen Einstellungen wie die Organisation aufweist, empfehlen wir den Onboarding-Teams, die Standardeinstellungen für die Organisation aus diesem Grund zu verwenden.
