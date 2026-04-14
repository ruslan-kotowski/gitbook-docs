---
title: Amazon Q (wersja beta)
article_id: 31347586131346
translation_id: 31347586131346
locale: pl-pl
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
  notes: 'Kto może to zrobić: Właściciele tablic, współwłaściciele tablic, edytujący
    tablic, członkowie zespołów, administratorzy zespołu, administratorzy użytkowników,
    administratorzy treści, administratorzy firmy; administrator Amazon Q Jakie abonamenty:
    Business, Enterprise Na jakich platformach: Przeglądarka, Komputer'
---

Integracja Amazon Q umożliwia zespołom pobieranie wiedzy firmowej do platformy Miro AI za pomocą funkcji współpracownika AI i przepływów. Inteligencja przedsiębiorstwa jest dostarczana i wizualizowana bezpośrednio w Miro.

:::note
Możesz używać integracji Amazon Q wyłącznie na platformie Miro AI. [Zarejestruj się tutaj](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb), aby uzyskać dostęp. Zostaniesz powiadomiony, gdy platforma Miro AI zostanie włączona dla Twojej organizacji.
:::

Wiedza przedsiębiorstwa jest często rozproszona w różnych narzędziach jak Slack, Confluence, Salesforce, Google Drive i wewnętrzne repozytoria, co zmusza menedżerów produktu, liderów inżynierii oraz zespoły technologiczne do tracenia cennego czasu na wyszukiwanie istotnych szczegółów i uzgadnianie obserwacji.

Następujące funkcjonalności Miro i Miro AI wspierają integrację Amazon Q:

- [**Flowy**](../../using-miro/miro-ai/04-flows-overview.md)
  Wizualizuj przepływy pracy, które przekształcają rozproszone informacje w przejrzyste rezultaty, pomagając zespołom w automatyzacji i standaryzacji sposobu, w jaki przekształcają obserwacje w działanie.
- [**Asystenci**](../../using-miro/miro-ai/06-sidekicks-overview.md)
  Pracuj w tandemie z agentami AI, którzy analizują zawartość tablicy oraz dane przedsiębiorstwa, aby generować nowe artefakty, dostarczać natychmiastowe wglądy i przyspieszać ideację, dokumentację oraz projektowanie.

## Konfiguracja integracji Amazon Q

Upewnij się, że [zarejestrowałeś się tutaj](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb) i otrzymałeś potwierdzenie od Miro, że platforma Miro AI została włączona dla Twojej organizacji. Następnie wykonaj następujące dwa procedury.

Aby skonfigurować integrację Amazon Q z Miro, musisz dodać Miro jako dostęp do danych w Amazon Q Business, a następnie połączyć indeks Amazon Q z konsolą administracyjną w Miro.

### Dodaj Miro jako dostęp do danych w Amazon Q Business

1. W konsoli Amazon Q Business, w panelu nawigacyjnym kliknij **Aplikacje**.
2. Kliknij aplikację, do której chcesz dodać dostęp do danych.
3. W panelu nawigacyjnym kliknij **Dostęp do danych**.
4. Kliknij **Dodaj dostęp do danych**.
5. Pod **Dostęp do danych**, dla **Miro** kliknij ikonę plus (**+**).
6. Dla **ID Zewnętrzny**, dodaj ID Twojej organizacji Miro.
   Aby uzyskać ID organizacji Miro, w Miro przejdź do konsoli administracyjnej. Skopiuj ID organizacji z paska URL przeglądarki.
   ![](../../../../../../docs/integrations-apps/amazon-web-services-aws/images/31367058137746_image.png)
   *Znajdź ID swojej organizacji w konsoli administracyjnej. Możesz skopiować ID z paska URL przeglądarki.*
7. Kliknij **Dodaj dostęp do danych**.
ID aplikacji

1. W Miro, przejdź do **Konsola administracyjna** > **Aplikacje i integracje** > **Aplikacje** > **Dodaj aplikacje**.
2. Wyszukaj i zlokalizuj Amazon Q.

   > ✏️ Jeśli nie możesz znaleźć Amazon Q po nazwie, wyszukaj za pomocą poniższego identyfikatora klienta: `1601842442647206821`.
3. W profilu aplikacji, wybierz czy dodać aplikację dla **Wszystkich zespołów** czy **Konkretnych zespołów**.
4. Sprawdź stronę z uprawnieniami.

   > ✏️ Aplikacja Amazon Q jest rozwijana i utrzymywana przez Miro, i nie wymaga określonych uprawnień.
5. Kliknij **Dodaj**.
6. Przejdź do **Aplikacje** > **Zarządzaj aplikacjami**.
7. Wyszukaj i zlokalizuj Amazon Q.
8. Kliknij **Ustawienia**.
9. Dodaj szczegóły dostępu do danych Amazon Q. Zobacz ostatni krok w Dodaj Miro jako dostęp do danych w Amazon Q Business.
10. Kliknij **Zapisz**.
    Twoja konfiguracja została zastosowana.
