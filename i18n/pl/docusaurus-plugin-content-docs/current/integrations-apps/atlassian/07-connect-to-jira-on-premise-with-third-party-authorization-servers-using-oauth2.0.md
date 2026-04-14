---
title: Połącz się z Jira on-premise za pomocą serwerów autoryzacji innych firm wykorzystując
  OAuth2.0
article_id: 25692796700306
translation_id: 26751273742098
locale: pl-pl
sidebar_position: 9
created_at: '2025-05-16T09:13:26Z'
updated_at: '2025-11-25T15:50:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Kto może to zrobić: administratorzy firmy Jakie abonamenty: Enterprise'
---

> *✏️* Podłączenie Jira za pomocą serwera autoryzacji jest włączone tylko na poziomie organizacji.

Artykuł przedstawia kroki podłączenia Miro do Jira za pomocą serwera autoryzacji innych firm działającego lokalnie, wykorzystując OAuth2.0.

Aby poznać szczegóły techniczne dotyczące tej konfiguracji, zobacz artykuł referencyjny dla [Jira on-premise z autoryzacją firm trzecich przy użyciu OAuth 2.0](https://help.miro.com/hc/articles/26726425696530).

## Wymagania wstępne

- Upewnij się, że masz następujące uprawnienia:
  - Administrator firmy Miro
  - (Opcjonalnie) Admin systemu Jira, jeśli chcesz używać automatycznych webhooków.
- Na swoim serwerze autoryzacji utwórz aplikację OAuth 2.0.
- Skonfiguruj URL przekierowania w swojej aplikacji OAuth 2.0 na następujący URL:
  https://integrations.miro.com/api/external-auth/oauth2/callback
- Upewnij się, że masz gotowe następujące szczegóły z Twojej aplikacji OAuth 2.0 do skonfigurowania w Miro:
  - URL autoryzacji
  - URL tokena
  - ID klienta
  - Sekret klienta
  - Zakres

## Połącz z Jira on-premise za pomocą serwerów zewnętrznych, używając OAuth 2.0

1. Na pulpicie Miro, wybierz swój awatar w prawym górnym rogu i przejdź do **konsoli administratora** | **Ustawienia**.
2. Przejdź do **Aplikacje i integracje ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)**> **Aplikacje** > **Karta zarządzania aplikacjami** .
3. Upewnij się, że **Zezwalaj tylko na aplikacje z poniższej listy** jest włączone.
4. Pod kolumną **Aplikacja** wybierz **Ustawienia** dla **kart Jira**.
5. Kliknij **Dodaj nowe połączenie**.
6. W sekcji **Jira setup** kliknij **Centrum danych Jira**.
7. Pod **Metoda uwierzytelniania** wybierz **OAuth2.0 za pośrednictwem zewnętrznego serwera autoryzacji**.
8. W polu **Jira URL** wprowadź adres URL swojej instancji Jira.
   > *✏️* Możesz dodać swój zewnętrzny główny adres URL Jira lub wewnętrzny adres URL Jira. Jeśli używasz wewnętrznego URL Jira, musisz określić zewnętrzny URL bramy API w kroku 10.

   > *✏️* Ogólnie rzecz biorąc, użycie wewnętrznego adresu URL umożliwia dostosowanie funkcji nawigacji do źródła.
9. (Opcjonalne) Aby ustawić to połączenie jako domyślne dla wszystkich zespołów w twojej organizacji, zaznacz **Ustaw jako domyślne**.
10. (Opcjonalnie) Jeśli używasz bramy API do składania żądań do Jira, to dla **Podstawowy URL Jira API Gateway**, wpisz zewnętrzny URL swojej bramy API.
11. Wprowadź następujące szczegóły z aplikacji OAuth 2.0:
    - URL autoryzacji
    - URL tokena
    - Identyfikator klienta
    - Klucz tajny klienta
    - Zakres
12. (Opcjonalnie) Aby otrzymywać aktualizacje w czasie rzeczywistym z Jira w Miro, zaznacz **Utwórz webhook automatycznie**.
    > *✏️ Możesz ręcznie dodać webhook później.*
13. Kliknij **Połącz**.
14. Postępuj zgodnie z procesem uwierzytelniania dla swojego serwera autoryzacji. Jeśli zostaniesz poproszony, zaloguj się do swojego środowiska.
    Po zakończeniu połączenia Twoja instancja Jira zostanie wyświetlona pod **Połączone instancje** z następującą etykietą: **Serwer autoryzacji**.

## Upewnij się, że Twój zespół może się uwierzytelnić

Teraz, gdy masz połączoną instancję Jira na poziomie organizacji, możesz zacząć używać Jira na poziomie zespołu.

1. Na pulpicie Miro wybierz swój awatar w prawym górnym rogu i przejdź do **Konsoli Administratora**.
2. Wybierz **Zespoły** > **Twój zespół**.
   Suwak **Twój zespół** otwiera się.
3. Wybierz kartę **Aplikacje**.
4. Z listy aplikacji wybierz **karty Jira**.
5. W **ustawieniach administratora** sprawdź, czy Twoja konfiguracja Jira pokazuje etykietę **GLOBAL CONNECTION** i czy widoczny jest poprawny adres URL instancji Jira, a następnie wykonaj jedną z poniższych czynności:
   - Jeśli tak, ukończyłeś tę procedurę. Możesz przejść do [Co dalej?](https://help.miro.com/hc/articles/25699264170386)
   - Jeśli nie, wybierz **Zmień konfigurację** > **Globalne ustawienia organizacji** > **Twoją instancję Jira**.
6. Wybierz **Zapisz ustawienia**.

## Co dalej?

Każdy członek zespołu musi autoryzować swoje konto użytkownika. Aby zapewnić, że każdy użytkownik uzyska tokeny dostępu i odświeżenia, gdy członek zespołu podejmie próbę działania związanego z Jira na tablicy Miro, zostanie poproszony o autoryzację swojego konta.

## FAQ

**Z których serwerów autoryzacji mogę korzystać?**

Możesz użyć dowolnego serwera autoryzacyjnego, który obsługuje standardowe protokoły OAuth 2.0 dla środowisk lokalnych. Na przykład, Azure Active Directory (Entra ID) i Okta.

**Czy mogę używać tego samego serwera autoryzacji dla wielu organizacji?**

Tak, ale musisz ręcznie dodać serwer do każdej organizacji.

**Czy mogę zaktualizować sekret klienta dla serwera autoryzacji?**

Nie. Jeśli musisz zmienić sekret klienta, musisz odłączyć i ponownie połączyć swoją instancję.

**Czy administratorzy organizacji i zespołu mogą nadal korzystać z natywnej autoryzacji w Jira?**

Tak. W zależności od wybranej konfiguracji, administratorzy mogą nadal korzystać z natywnego procesu autoryzacji w Jira.

**Co się stanie, jeśli zespół jest już połączony z inną instancją Jira?**

Możesz zaktualizować zespoły do domyślnych [ustawień Jiry Twojej organizacji](https://help.miro.com/hc/articles/26438407676434).

**Czy Miro kontroluje mapowanie pomiędzy autoryzowanymi użytkownikami a użytkownikami Jira?**

Nie. Mapowanie między uprawnionymi użytkownikami a użytkownikami Jira jest odpowiedzialnością środowiska klienta za pośrednictwem ich gateway API. Miro nie kontroluje tej bramy.

**Jak mogę stwierdzić, czy OAuth 2.0 za pomocą zewnętrznego serwera autoryzacyjnego jest odpowiednim rozwiązaniem dla mojej organizacji?**

Jeśli wszystkie z poniższych elementów są prawdziwe, OAuth 2.0 za pośrednictwem serwera autoryzacji stron trzecich jest dobrym rozwiązaniem:

- Twoja instancja Jira jest hostowana lokalnie.
- Dostęp zewnętrzny do Jira jest możliwy tylko za pomocą API Gateway.
- Bramka API egzekwuje autoryzację przy użyciu niestandardowego serwera autoryzacji.
- Musisz połączyć Miro z Jira, nie ujawniając publicznego adresu bazowego Jira.

**Jaki problem rozwiązuje to rozwiązanie?**

To rozwiązanie zostało zaprojektowane dla organizacji, które hostują Jirę lokalnie i kierują zewnętrzny ruch API przez bramę API. W tym ustawieniu Jira nie jest publicznie dostępna, a dostęp jest kontrolowany za pomocą niestandardowego serwera autoryzacji. Zamiast mieć publiczny podstawowy URL dla Jira, to rozwiązanie pozwala połączyć instancje Jira w środowisku lokalnym, konfigurując Miro do uwierzytelniania za pośrednictwem własnego serwera autoryzacji.
