---
title: Amazon Q (Betaversion)
article_id: 31347586131346
translation_id: 31347586131346
locale: de
sidebar_position: 3
created_at: '2025-11-25T13:35:45Z'
updated_at: '2025-12-29T15:25:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: 'Verfügbar für: Board-Eigentümer, Board-Miteigentümer, Board-Bearbeiter,
    Teammitglieder, Team-Admins, Nutzer-Admins, Content-Admins, (Einrichtungs-) Unternehmens-Admins;
    Amazon Q-Admin Welche Preispläne: Business, Enterprise Welche Plattformen: Browser,
    Desktop'
---

Die Amazon Q-Integration ermöglicht es Teams, Unternehmenswissen über die Miro AI-Plattform mithilfe von KI-Kollegen und Flows abzurufen. Unternehmensintelligenz wird direkt in Miro bereitgestellt und visualisiert.

:::note
Du kannst die Amazon Q-Integration nur mit der Miro AI-Plattform verwenden. [Hier registrieren](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb), um Zugang zu erhalten.  Du wirst benachrichtigt, wenn die Miro AI-Plattform für deine Organisation freigeschaltet ist.
:::

Unternehmenswissen ist oft auf zahlreiche Tools wie Slack, Confluence, Salesforce, Google Drive und interne Repositories verstreut, was Produktmanagern, Engineering-Führungskräften und Technologie-Teams wertvolle Zeit kostet, um entscheidende Details zu suchen und Erkenntnisse abzustimmen.

Die folgenden Miro- und Miro AI-Funktionalitäten unterstützen die Amazon Q-Integration:

- [**Workflows**](../../using-miro/miro-ai/04-flows-overview.md)
  Visualisiere Workflows, die verstreute Informationen in klare Ergebnisse umwandeln und Teams dabei unterstützen, automatisch und standardisiert Erkenntnisse in Aktionen umzusetzen.
- [**Sidekicks**](../../using-miro/miro-ai/06-sidekicks-overview.md)
  Arbeite mit KI-Assistenten zusammen, die über Board-Inhalte und Unternehmensdaten nachdenken, um neue Artefakte zu erstellen, sofortige Einblicke zu geben und die Ideenfindung, Dokumentation und Gestaltung zu beschleunigen.

## Amazon Q-Integration einrichten

Stelle sicher, dass du dich [hier angemeldet](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb) hast und eine Bestätigung von Miro erhalten hast, dass die Miro AI-Plattform für deine Organisation aktiviert ist. Schließe dann die folgenden zwei Schritte ab.

Um die Amazon Q-Integration mit Miro einzurichten, musst du Miro als Datenzugriffsprogramm in Amazon Q Business hinzufügen und dann den Amazon Q-Index mit der Admin-Konsole in Miro verbinden.

### Miro als Datenzugriffsprogramm in Amazon Q Business hinzufügen

1. Klicke im Amazon Q Business Console im Navigationsbereich auf **Apps**.
2. Klicke auf die App, zu der du einen Datenzugreifer hinzufügen möchtest.
3. Klicke im Navigationsbereich auf **Datenzugreifer**.
4. Klicke auf **Datenzugreifer hinzufügen**.
5. Unter **Datenzugreifer** klicke bei **Miro** auf das Pluszeichen (**+**).
6. Für **Externe ID** füge deine Miro-Organisations-ID hinzu.
   Um deine Miro-Organisations-ID zu erhalten, gehe in Miro zur Admin-Konsole. Kopiere die Organisations-ID aus der URL-Leiste des Browsers.
   ![](../../../../../../docs/integrations-apps/amazon-web-services-aws/images/31367058137746_image.png)
   *Finde die Organisations-ID in der Admin-Konsole. Du kannst die ID aus der URL-Leiste des Browsers kopieren.*
7. Klicke auf **Datenzugriffsverwalter hinzufügen**.
8. Notiere dir die folgenden Details. Du benötigst jeden Wert, um die Einrichtung in der Miro Admin-Konsole abzuschließen:
   - Anwendungs-ID
   - IdC-Anwendungs-ARN
   - Retriever-ID
   - Anwendungsregion
   - IdC-Anwendungsregion

### Verbinde einen Amazon Q-Index mit der Admin-Konsole in Miro

1. Gehe in Miro zu **Admin-Konsole** > **Apps & Integrationen** > **Apps** > **Apps hinzufügen**.
2. Suche nach Amazon Q.

   > ✏️ Falls Amazon Q nicht per Name auffindbar ist, suche mit der folgenden Client-ID: `1601842442647206821`.
3. Wähle im App-Profil aus, ob die App für **Alle Teams** oder **Bestimmte Teams** hinzugefügt werden soll.
4. Prüfe die Berechtigungsseite.

   > ✏️ Die Amazon Q-App wird von Miro entwickelt und gepflegt und erfordert keine spezifischen Berechtigungen.
5. Klicke auf **Hinzufügen**.
6. Gehe zu **Apps** > **Apps verwalten**.
7. Suche und finde Amazon Q.
8. Klicke auf **Einstellungen**.
9. Füge die Details des Amazon Q-Datenzugriffs hinzu. Siehe den letzten Schritt unter Füge Miro als Datenzugriff in Amazon Q Business hinzu.
10. Klicke auf **Speichern**.
    Deine Konfiguration wird angewendet.
