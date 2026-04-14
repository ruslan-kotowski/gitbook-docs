---
title: Konfiguracja integracji z Looker
article_id: 25112862440978
translation_id: 25112862440978
locale: pl-pl
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
Aby uzyskać wszechstronne dokumenty administratora z szczegółami i dalszymi informacjami na temat integracji Miro + Looker, zapoznaj się z [dokumentacją administratora Looker](https://docs.google.com/document/d/1AUCQWRwDICLygwVmwSxXpz7RmRivPit0EIKgBMIkT6A/edit?usp=sharing).
:::

Aby skonfigurować integrację **Looker** z Miro, musisz zarejestrować aplikację OAuth w Looker.

## Wymagania wstępne

- Upewnij się, że **administrator firmy** zatwierdził Looker dla Twojej organizacji w Miro.

## Zarejestruj aplikację OAuth w Lookerze

1. W **Looker Marketplace** znajdź i wybierz **rozszerzenie API Explorer**.
2. Wybierz **Zainstaluj**.
3. Przejdź do **Home** > **Aplikacje** > **Rozszerzenie API**.
4. Znajdź i wybierz **Zarejestruj aplikację OAuth**.
5. Wybierz **Uruchom**.
6. Otwiera się menu, w którym możesz dodać dane prośby.
   Dodaj następujące wartości:
   - **client_guid**: `15609152-a12a-4fa1-b364-337e7896d25d`
   - **tekst**:

   ```
     "redirect_uri": "https://integrations.miro.com/api/contenthub/public/oauth/callback"
     "display_name": "nazwa_wyświetlana" Miro
     opis Integracja Miro z Lookerem
     "włączone": true,
     "group_id": ""
   }
   ```
7. Wybierz **Rozumiem, że ten punkt końcowy API zmieni dane**.
8. Wybierz **Uruchom**.
9. Udane uruchomienie zwraca treść z odpowiedzią **HTTP 200**.
   - 💡 Jeśli zwracany korpus zawiera `"enabled":false`, uruchom zaktualizowaną aplikację OAuth API z tymi samymi wartościami, co w kroku 6.

Integracja Looker z Miro została pomyślnie skonfigurowana.

## Więcej informacji

- Zobacz [dokumentację referencyjną Looker API](https://developers.looker.com/api/explorer/4.0/methods/Auth/register_oauth_client_app) (zewnętrzna).
