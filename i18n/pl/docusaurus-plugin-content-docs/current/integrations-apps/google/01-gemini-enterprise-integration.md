---
title: Integracja Gemini Enterprise (wersja beta)
article_id: 32304596526482
translation_id: 32304596526482
locale: pl-pl
sidebar_position: 1
created_at: '2026-01-05T10:38:04Z'
updated_at: '2026-02-17T09:38:53Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: 'Kto może to zrobić: administratorzy firmy Na jakich abonamentach: Business,
    Enterprise Na jakich platformach: Przeglądarka, Komputer'
---

Jako administrator firmy możesz włączyć i skonfigurować integrację Gemini Enterprise dla zespołów w swojej organizacji Miro.

Integracja Gemini Enterprise pozwala połączyć Gemini Enterprise jako [zasób wiedzy](../../using-miro/miro-ai/09-knowledge.md) w Miro. Na przykład używaj Gemini Enterprise do dostarczania inteligencji firmowej współpracownikom AI i przepływom.

Możesz także połączyć Gemini Enterprise z [samodzielną aplikacją czatu](../../using-miro/miro-ai/09-knowledge.md) w Miro.

Aby używać integracji Gemini Enterprise, wykonaj te kroki:

1. Włącz aplikację **Gemini Enterprise.**
   1. Jako **administrator firmy** przejdź do **Konsoli administracyjnej**.
   2. Wejdź do **Aplikacje i integracje** > **Aplikacje** > **Dodaj aplikacje**.
   3. Wyszukaj i znajdź **Gemini Enterprise**.
      Jeśli nie możesz znaleźć aplikacji po nazwie, wyszukaj za pomocą następującego identyfikatora klienta: `2392210303456548729`.
   4. W **profilu** aplikacji wybierz, czy dodać aplikację dla **wszystkich zespołów w \{Team name\}**, czy tylko w **specyficznych zespołach**.
   5. Kliknij **Dodaj**.
2. Skonfiguruj aplikację Gemini Enterprise.
   1. W **Admin Console**, przejdź do **Aplikacje i integracje** > **Aplikacje**.
   2. Dla Gemini Enterprise upewnij się, że opcja **Dozwolone** jest włączona. Następnie kliknij **Ustawienia**.
   3. Dodaj szczegóły konfiguracji Gemini Enterprise.
      Aby dowiedzieć się, jak znaleźć Project ID, zobacz (External) [Lokalizowanie Project ID](https://support.google.com/googleapi/answer/7014113?hl=en).
      Aby uzyskać App ID, przejdź do Gemini Enterprise > Apps i użyj wartości w kolumnie ID.
      ![](images/33222269064210_image (2).png)
      *Skonfiguruj aplikację Gemini Enterprise do użytku w Miro.*

      > ✏️ **Project ID** i **App ID** są wymagane. Pozostałe pola są opcjonalne.
   4. Kliknij **Zapisz**.

:::note
Gdy członek zespołu po raz pierwszy połączy Gemini Enterprise jako [zasób wiedzy](../../using-miro/miro-ai/09-knowledge.md), zostanie poproszony o uwierzytelnienie. Członek zespołu musi posiadać licencję Gemini Enterprise.
:::
