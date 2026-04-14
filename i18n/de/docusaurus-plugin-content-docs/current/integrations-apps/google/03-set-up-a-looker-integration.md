---
title: Die Looker-Integration einrichten
article_id: 25112862440978
translation_id: 25112862440978
locale: de
sidebar_position: 4
created_at: '2025-03-05T14:00:46Z'
updated_at: '2025-06-04T08:30:26Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: looker
---

:::note
Für umfassende Admin-Dokumente mit Details und weiteren Informationen zur Miro + Looker-Integration, sieh dir bitte die [Looker-Admin-Dokumentation](https://docs.google.com/document/d/1AUCQWRwDICLygwVmwSxXpz7RmRivPit0EIKgBMIkT6A/edit?usp=sharing) an.
:::

Um eine **Looker**-Integration mit Miro einzurichten, musst du die OAuth-App in Looker registrieren.

## Voraussetzungen

- Stelle sicher, dass ein **Unternehmens-Admin** Looker für deine Miro-Organisation genehmigt hat.

## OAuth-App in Looker registrieren

1. Im **Looker Marketplace** findest du die **API Explorer-Erweiterung** und wählst sie aus.
2. **Installieren** auswählen.
3. Gehe zu **Startseite** > **Anwendungen** > **API-Erweiterung**.
4. Such und wähle **OAuth-App registrieren** aus.
5. **Ausführen** auswählen.
6. Es öffnet sich ein Menü, in dem du Anfragedaten hinzufügen kannst.
   Füge die folgenden Werte hinzu.
   - **client_guid**: `15609152-a12a-4fa1-b364-337e7896d25d`
   - **Körper**:

   ```
   {
     "redirect_uri": "https://integrations.miro.com/api/contenthub/public/oauth/callback",
     Anzeigename Miro
     Beschreibung Miro-Looker-Integration
     "aktiviert": true,
     "group_id": ""
   }
   ```
7. Wähle **Mir ist bewusst, dass dieser API-Endpunkt Daten ändern wird** aus.
8. **Ausführen** auswählen.
9. Ein erfolgreicher Durchlauf gibt den Textkörper mit einem **HTTP 200**-Antwortcode zurück.
   - 💡 Wenn der zurückgegebene Body `"enabled":false` enthält, dann führe die Update OAuth App API mit den gleichen Werten wie in Schritt 6 aus.

Jetzt hast du die Looker-Integration mit Miro eingerichtet.

## Weitere Informationen

- Siehe [Looker API-Referenz](https://developers.looker.com/api/explorer/4.0/methods/Auth/register_oauth_client_app) (extern).
