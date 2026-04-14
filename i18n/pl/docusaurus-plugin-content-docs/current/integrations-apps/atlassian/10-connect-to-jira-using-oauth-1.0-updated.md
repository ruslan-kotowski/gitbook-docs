---
title: Połącz się z Jira używając OAuth 1.0 (Zaktualizowane)
article_id: 27689156602514
translation_id: 27689205631250
locale: pl-pl
sidebar_position: 12
created_at: '2025-06-27T13:20:14Z'
updated_at: '2025-11-25T15:52:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Kto może to zrobić: administratorzy firmy, administratorzy zespołu Które
    abonamenty: Starter, Business, Enterprise, Education Na których platformach: Przeglądarka,
    Komputer'
---

Organizacje, które nie są gotowe na migrację do OAuth 2.0, mogą skorzystać z poniższej procedury, aby połączyć Miro z Jira przy użyciu OAuth 1.0.

Atlassian [wycofał OAuth 1.0](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively), a metoda podana w tym artykule jest rozwiązaniem przejściowym. Aby uniknąć problemów i dostosować się do najlepszych praktyk w zakresie bezpieczeństwa i kompatybilności, Miro zdecydowanie zaleca migrację do OAuth 2.0 tak szybko, jak to możliwe.

:::note
Dotychczasowa metoda uwierzytelniania OAuth 1.0 [jest wycofana](https://help.miro.com/hc/articles/360019501754-Set-up-and-disable-Jira-Cards-OAuth-1-0) i zostanie usunięta 31 lipca 2025 roku.
:::

Artykuł ten wyjaśnia również, jak używać jednego serwera Jira dla kilku zespołów Miro oraz jak wyłączyć karty Jira na poziomie organizacji i zespołu.

## Wymagania wstępne

- Upewnij się, że masz następujące uprawnienia:
  - (Business, Enterprise) Miro Company admin
    (Starter, Education) administrator zespołu Miro
  - administrator systemu Jira

    > ✏️ Aby ukończyć procedurę, musisz być w stanie utworzyć link aplikacji w Jira.
- W Jira usuń istniejące linki aplikacji do Miro.

## Procedura

Aby połączyć się z Jira za pomocą OAuth1.0, wykonaj te kroki:

1. Na pulpicie Miro, kliknij swój awatar w prawym górnym rogu, a następnie wybierz **Konsola administracyjna**.
2. W lewym pasku bocznym przejdź do **Aplikacje i integracje** > **Aplikacje** > karta **Zarządzaj aplikacjami**.
3. Upewnij się, że opcja **Zezwalaj tylko na aplikacje z poniższej listy** jest włączona.
4. W kolumnie **Aplikacja**, dla **Karty Jira** wybierz **Ustawienia**.
5. Na karcie **Domyślne ustawienia**, wybierz **Dodaj nowe połączenie**.
6. W sekcji **Konfiguracja Jira** wybierz **Jira Cloud** lub **Jira Data Center**.
7. W sekcji **Metoda uwierzytelniania** wybierz **OAuth 1.0x (Zaktualizowany)**.
8. W sekcji **URL Jira** wpisz URL swojej instancji Jira.
9. (Opcjonalnie) Aby uczynić to połączenie domyślnym połączeniem dla wszystkich zespołów w Twojej organizacji, zaznacz **Ustaw jako domyślne**.
10. W sekcji **Instrukcje konfiguracji** upewnij się, że masz następujące właściwości:
    - URL
    - Klucz klienta
    - Nazwa klienta
    - Klucz publiczny
11. W Jira, utwórz link aplikacji.
    1. (Cloud) Przejdź do **Ustawienia** > **Produkty** > **Linki aplikacji**.
       (Data Center) W ustawieniach administracyjnych Jira przejdź do **Produkty** > **Linki aplikacji**.
    2. Kliknij **Utwórz link**.
    3. (Cloud) Dla **Typ aplikacji** wybierz **Aplikacja bezpośrednia**.
       (Data Center) Dla **Typ aplikacji** wybierz **Produkt Atlassian**.
    4. Dla **URL aplikacji**, wklej URL z instrukcji konfiguracji Miro. Zobacz krok 10.
    5. Kliknij **Kontynuuj**.
    6. Dla **Nazwa aplikacji**, nadaj nazwę swojej aplikacji.

       > **⚠️** Nie wprowadzaj danych w żadne inne pole. Dane z Miro podasz w kolejnym kroku.
    7. Zaznacz **Utwórz przychodzące połączenie**.
    8. Kliknij **Kontynuuj**.
    9. Skopiuj i wklej swój klucz konsumenta, nazwę konsumenta i klucz publiczny z instrukcji konfiguracji Miro. Zobacz krok 10.
    10. Kliknij **Kontynuuj**.
        Stworzyłeś link do swojej aplikacji.
12. W Miro, kliknij **Połącz**.
    Połączyłeś Miro z Jira za pomocą OAuth 1.0.

## Co dalej?

Skonfigurowałeś i połączyłeś integrację Jira z Miro, używając Jira OAuth1.0. Gdy użytkownik po raz pierwszy podejmuje działanie związane z Jirą w Miro, zostaje poproszony o autoryzację.

**Więcej informacji:** Zobacz [Jak korzystać z kart Jira](https://help.miro.com/hc/articles/360017572434).

## Jedna instancja Jiry dla kilku zespołów Miro

Możesz zainstalować karty Jira na poziomie organizacyjnym lub zespołowym. Jeśli masz wiele zespołów, możesz określić ustawienia organizacyjne, aby uniknąć powtarzającej się konfiguracji dla każdego zespołu. Istniejące łącze aplikacyjne jest wtedy używane dla wszystkich zespołów.

:::note
Połączenie kilku instancji Jiry z jednym zespołem Miro nie jest obsługiwane.
:::

W przypadku żądań aktualizacji, po połączeniu swojej organizacji lub zespołu z instancją Jira, webhook jest dodawany do webhooków Jira dla tej organizacji lub zespołu w Miro.

:::tip
Nadaj każdemu webhookowi unikalną nazwę dla każdego zespołu. Przejdź do strony WebHooków w Jira i edytuj każdy nowo utworzony webhook.
:::

Jeśli określisz ustawienia na poziomie organizacji, zespoły, które mają już własne ustawienia zespołowe, zachowują swoją konfigurację. Każdy zespół z własnymi ustawieniami może w dowolnym momencie przełączyć się na ustawienia organizacyjne.

W przeciwnym razie, każdy zespół może nadpisać ustawienia organizacyjne, aby połączyć się z osobną instancją Jira.

## Wyłącz karty Jira

### Poziom organizacji

Aby wyłączyć karty Jira na poziomie organizacji, wykonaj te kroki:

1. Na pulpicie Miro kliknij swój awatar w prawym górnym rogu i wybierz **Konsola administracyjna**.
2. Przejdź do **Aplikacje i integracje** > **Zarządzaj aplikacjami**.
3. Znajdź **Karty Jira**.
4. Dla kart Jira, przełącz opcję **Dopuszczone** na pozycję wyłączoną.

:::warning
Jeśli wyłączysz karty Jira dla organizacji, to członkowie wszystkich zespołów Enterprise nie będą mogli korzystać z kart Jira. Aby dowiedzieć się więcej o zarządzaniu aplikacjami, zobacz [Zarządzanie aplikacjami](https://help.miro.com/hc/articles/4404659741458).
:::

### Poziom zespołu

Aby wyłączyć karty Jira na poziomie zespołu, wykonaj te kroki:

1. Na pulpicie Miro kliknij swój awatar w prawym górnym rogu, a następnie kliknij **Konsola administracyjna**.
2. Przejdź do **Zespoły**.
3. Kliknij wiersz dla zespołu, którym chcesz zarządzać.
   Otworzy się panel ustawień zespołu.
4. Kliknij kartę **Aplikacje**.
5. Znajdź i kliknij **Karty Jira**.
6. Kliknij **Usuń dla zespołu**.
