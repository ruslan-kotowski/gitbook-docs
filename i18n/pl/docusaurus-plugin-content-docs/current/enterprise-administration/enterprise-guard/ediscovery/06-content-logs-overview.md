---
title: Dzienniki treści
article_id: 17774729839378
translation_id: 17774729839378
locale: pl-pl
sidebar_position: 5
created_at: '2024-03-19T13:00:06Z'
updated_at: '2026-03-15T21:32:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
availability:
  notes: 'Ustawione przez: Administratorzy firmy, Administratorzy zabezpieczeń'
---

Dzienniki treści pozwalają klientom korporacyjnym na zbieranie szczegółowych zapisów działalności użytkowników na tablicach i wykorzystywanie ich do badań lub archiwizacji regulacyjnej.

Dzienniki treści mogą być używane w różnych specjalistycznych narzędziach do celów prawnych, zgodności i bezpieczeństwa. Poprzez rozwiązanie umożliwiające eksport danych o aktywności użytkowników na dużą skalę, Miro zmniejsza ryzyko dla klientów i otwiera możliwości dla większej ilości pracowników wiedzy w przedsiębiorstwie, by doświadczać korzystania z Miro przy jednoczesnym przestrzeganiu rygorystycznych wymagań dotyczących bezpieczeństwa i zgodności.

## Dane dziennika treści

Kiedy użytkownik aktualizuje widget na tablicy, tworzony jest wpis z informacjami, takimi jak czas akcji użytkownika, szczegóły użytkownika, typ działania (utworzenie, aktualizacja, usunięcie), identyfikatory tablicy i widgetu, a także inne istotne informacje o stanie widgetu w wyniku działań użytkowników. Dzienniki treści *nie* rejestrują aktualizacji w pozycji, rozmiarze ani obrocie widgetu.

## Zbieranie dzienników treści

Zdarzenia są rejestrowane od momentu, gdy administrator włączy zbieranie dzienników treści. Zebrane zdarzenia są przechowywane przez 30 dni domyślnie.

Aby włączyć zbieranie dzienników treści, wykonaj następujące kroki:

1. Przejdź do ustawień firmy.
2. Na panelu po lewej stronie kliknij **Bezpieczeństwo** > **Dzienniki audytu**.
3. W sekcji **Dzienniki audytu** kliknij kartę **Ustawienia**.
4. W sekcji **Dzienniki treści** kliknij, aby włączyć przełącznik **Zbieraj dzienniki treści**.
   ![content_logs.png](images/34049621972498_content_logs.png)
   *Włączanie zbierania dzienników treści*

## Dostęp do dzienników treści przez API

Administratorzy mogą używać [Content logs API](https://developers.miro.com/reference/board-content-logs), aby programowo uzyskać dostęp do danych dzienników treści w ramach swojej organizacji. Administratorzy mogą również zbierać dane dzienników treści przy pomocy wspieranych integracji, takich jak Smarsh czy Theta Lake.

Aby uwierzytelnić dostęp do API, administratorzy mogą wybrać jedną z następujących opcji:

- Włącz przełącznik eDiscovery w Enterprise Integrations.
- Utwórz aplikację platformową i nadaj jej dostęp do zakresu Content log:read.
- Zainstaluj i autoryzuj jedną z integracji eDiscovery z Marketplace.

## Usuwanie dzienników treści

Administratorzy mogą ustalić zasady retencji dla dzienników treści, wybierając jedną z opcji: 30, 90, 180, lub 365 dni. Domyślnie okres retencji jest ustawiony na 30 dni.

:::note
Po usunięciu dzienników treści nie można ich odzyskać.
:::

Aby ustawić okres usuwania, wykonaj następujące kroki:

1. Przejdź do ustawień firmy.
2. W panelu po lewej stronie kliknij **Bezpieczeństwo** > **Dzienniki audytu**.
3. W sekcji **Dzienniki audytu** kliknij kartę **Ustawienia**.
4. W sekcji **Dzienniki treści** wybierz opcję z rozwijanej listy. Zostaniesz poproszony o potwierdzenie wyboru.
   ![content_logs_duration.png](images/34049621972754_content_logs_duration.png)
   *Ustawienie zasady retencji dzienników treści*
