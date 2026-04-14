---
title: "Skonfiguruj Asan\u0119 dla swojego zespo\u0142u"
article_id: 28252196453778
translation_id: 28252196453778
locale: pl-pl
sidebar_position: 2
created_at: '2025-07-22T13:30:20Z'
updated_at: '2026-02-20T09:00:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Ta sekcja zawiera kompleksowe szczegóły techniczne i administracyjne, niezbędne dla specjalistów IT i bezpieczeństwa odpowiadających za wdrożenie, bezpieczeństwo i bieżące zarządzanie integracją z Asaną w ich organizacji.

## Przegląd techniczny

Integracja z Asaną jest technicznie realizowana poprzez REST API. W celach uwierzytelniania i autoryzacji integracja wykorzystuje standardowy w branży protokół OAuth 2.0. Kluczowym elementem tej architektury jest wykorzystanie zintegrowanej platformy API jako podprocesora dla danych zewnętrznych. Ta platforma zapewnia zintegrowane API odpowiedzialne za uwierzytelnianie, normalizowanie i synchronizowanie danych między różnymi dostawcami API.

## Przepływy danych

Dogłębne zrozumienie przepływu danych jest kluczowe dla zarządzania bezpieczeństwem i zgodnością w Twojej organizacji.

### Diagram sekwencji na wysokim poziomie

Tworzenie widżetu karty Asana

![image (7).png](images/30597069070994_image%20(7).png)

Aktualizacja widżetu karty Asana

![image (8).png](images/30597084219154_image%20(8).png)

### Dane Asana w Miro

Kiedy użytkownicy importują zadania Asana na tablicę Miro, odpowiednie dane zadań stają się integralną częścią danych planszy Miro. Miro przechowuje następujące konkretne punkty danych dla zaimportowanych zadań, o ile są one dostępne w Asana:

- Tytuł
- Opis
- Przydzielony (w tym imię i/lub adres e-mail użytkownika)
- Stan
- Priorytet

Jawna enumeracja typów przechowywanych danych ma kluczowe znaczenie dla zarządzania danymi i zgodności organizacyjnej. Umożliwia administratorom dokładne ocenienie, jakie informacje, szczególnie dane wrażliwe, są replikowane do środowiska Miro. Ta przejrzystość gwarantuje zgodność z wewnętrznymi politykami zarządzania danymi w organizacji. Warto również podkreślić, że zgodnie z sekcją „Ograniczenia” pola niestandardowe nie są obsługiwane i tym samym nie są przechowywane, co jest kluczowym szczegółem dla mapowania danych i ocen zgodności. Miro stosuje hybrydowe podejście do przechowywania danych, minimalizując dane przechowywane bezpośrednio w karcie i pobierając dodatkowe szczegóły, gdy użytkownik otwiera widok edycji.

### Retencja przechowywanych informacji w Miro

Wszystkie zaimportowane dane Asana przechowywane w Miro są ściśle zgodne z standardową zasadą retencji danych Miro. Zasada ta jest stosowana konsekwentnie do wszystkich danych klienta, co zapewnia jednolite podejście do zarządzania cyklem życia danych.

## Uwierzytelnianie i autoryzacja

Integracja Asana inicjuje przepływ uwierzytelniania, kiedy użytkownik po raz pierwszy wchodzi w interakcję z integracją. Autoryzacja w Asana jest obsługiwana przez usługę integracyjną. Dla każdego użytkownika Miro zakłada konto z usługą integracyjną, a te dane dostępowe są następnie używane do wszystkich interakcji użytkownika z integracją.

Integracja zazwyczaj wymaga zatwierdzenia przez administratora Asany (lub administratora Microsoft Entra, jeśli Asana jest zarządzana przez Azure AD), aby autoryzować aplikację integracyjną w ekosystemie ich organizacji. Ponadto indywidualni użytkownicy muszą również autoryzować integrację Miro Asana przez stronę autoryzacji OAuth Asany, gdy po raz pierwszy próbują osadzić link Asany.

### Wymagane zakresy autoryzacji

Zakres autoryzacji może się różnić w zależności od konkretnego systemu zewnętrznego. Jednak dla integracji z biletowaniem, takich jak Asana, Miro zazwyczaj wymaga dostępu do następujących danych:

| Zakres | Opis |
| --- | --- |
| Zadania (odczyt i zapis) | Udziela integracji pozwolenia na odczyt istniejących zadań oraz tworzenie lub modyfikację zadań w Asanie. |
| Użytkownicy (odczyt) | Udziela integracji pozwolenia na odczyt informacji o użytkownikach w Asanie, zazwyczaj w celu przypisywania zadań lub wyświetlania nazw osób przypisanych. |
| Tagi (odczyt) | Udziela integracji uprawnień do odczytu tagów powiązanych z zadaniami w Asana. |
| Kolekcje (odczyt) | Udziela integracji uprawnień do odczytu kolekcji zadań lub projektów w Asana. |

### Co jest przechowywane w Miro i w jaki sposób

Miro bezpiecznie przechowuje zarówno dane związane z autoryzacją, jak i z rozwijaniem powiązań dla integracji z Asana:

- **Dane związane z autoryzacją:** Obejmuje to wartości tokenów dostępu i tokenów odświeżania, które są przechowywane w bazie danych Miro przez ograniczony czas kilku dni. Te tokeny są automatycznie odnawiane po wygaśnięciu przy użyciu tokenów odświeżania, aby zapewnić ciągły dostęp. Wszystkie tego typu dane przechowywane w bazie danych dla tej integracji są szyfrowane za pomocą 256-bitowego standardu szyfrowania AES, zapewniając solidną warstwę bezpieczeństwa danych.
- **Dane związane z rozwijaniem:** Obejmuje to tytuły zadań, które są przechowywane jako część samych tablic Miro. Dodatkowo, tytuły i zaszyfrowane odniesienia do tych elementów są przechowywane w wewnętrznej usłudze, dodatkowo zabezpieczone poprzez szyfrowanie (zarządzanie kluczami szyfrowania).

### Unieważnianie tokenu

Jeśli zajdzie taka potrzeba, administratorzy lub indywidualni użytkownicy mogą cofnąć przyznane tokeny integracji z Asaną. Użytkownicy mogą przejść do ustawień integracji, otwierając przeglądarkę zadań integracji, klikając menu z 3 kropkami w prawym górnym rogu i wybierając **Ustawienia integracji**, lub przez kartę **Aplikacje** w ustawieniach zespołu Miro, znalezienie konkretnej integracji i kliknięcie na nią. Na stronie z ustawieniami można cofnąć autoryzację, klikając przycisk **Rozłącz**. Po tej akcji Miro odwoła dostęp do Asany i usunie powiązane konto użytkownika. W przypadku dezinstalacji na poziomie zespołu, administratorzy mogą postępować zgodnie z konkretnymi krokami opisanymi w sekcji „Rozwiązywanie problemów i FAQ (Admin)”.

## Jak skonfigurować integrację z Asaną

Proces konfiguracji integracji Miro + Asana obejmuje odrębne kroki dla administratorów i użytkowników końcowych, co zapewnia kontrolowane wdrożenie w organizacji.

1. **Upewnij się, że konta są aktywne:** Przed rozpoczęciem instalacji upewnij się, że dostępne są zarówno aktywne konta Miro, jak i Asana.
2. **Instalacja na poziomie zespołu (Działanie administratora):**
   - Administratorzy mogą być zobowiązani do wyraźnego autoryzowania integracji z Asaną dla swojego zespołu Miro. Członkowie zespołu mogą korzystać z integracji tylko wtedy, gdy jest ona zainstalowana na poziomie zespołu.
   - Administrator zespołu Miro może bezpośrednio zainstalować aplikację, otwierając tablicę Miro, wybierając **Narzędzia Media & Integrations (+)**, wyszukując "Asana" i klikając **Połącz** w celu autoryzacji integracji. Jeśli administrator zespołu Miro wykona tę czynność, aplikacja zostanie automatycznie autoryzowana i zainstalowana bez potrzeby dalszej zgody administracyjnej.
3. **Przepływ prośby użytkownika i zgody administratora (jeśli dotyczy):**
   - W organizacjach, gdzie wymagana jest ścisła zgoda administracyjna, użytkownik niebędący administratorem w zespole Miro skonfigurowanym dla integracji Asana może wkleić link Asany na tablicę Miro. Ta akcja może uruchomić dialog "prośba o zainstalowanie aplikacji" dla użytkownika, zachęcając go do zasięgnięcia zgody administratora.
   - Wyznaczeni administratorzy mogą następnie przejrzeć i zatwierdzić to oczekujące żądanie za pośrednictwem swoich konsol administracyjnych Miro lub Asany, w zależności od skonfigurowanego przepływu zgód.
4. **Indywidualne połączenie użytkownika:**
   - Po pomyślnym zainstalowaniu i autoryzacji integracji na poziomie zespołu przez administratora, indywidualni użytkownicy będą kontynuować proces, klikając **Połącz** na widżecie Asana, który pojawia się na tablicy Miro.
   - Użytkownicy zostaną wtedy przekierowani na stronę autoryzacji Asana, gdzie udzielą Miro dostępu do swojego indywidualnego konta Asana, potwierdzając tym samym ich osobistą autoryzację do osadzania i interakcji z treściami.

## Kwestie bezpieczeństwa i zgodności

### Ograniczenie dostępu do pliku źródłowego

Aby zagwarantować, że dostęp do osadzonych danych Asany pozostanie ograniczony do tych samych osób, co dostęp do pliku źródłowego Asany, administratorzy organizacji Miro muszą ściśle kontrolować udostępnianie tablic i eksport treści. Podczas gdy podstawowa integracja z Asaną respektuje indywidualne uprawnienia do interakcji na żywo, każdy eksport lub statyczny zrzut treści tablicy może potencjalnie ujawnić dane osobom nieuprawnionym, jeśli tablica Miro sama w sobie nie jest odpowiednio zabezpieczona.

### Obsługa błędów

Integracja została zaprojektowana z łagodnym interfejsem użytkownika na wypadek niepowodzenia aktualizacji danych na kartach z powodu odrzucenia przez zewnętrzny system.

### Dodatek do przetwarzania danych Miro (DPA)

W celu uzyskania szczegółowych informacji prawnych i dotyczących zgodności w odniesieniu do praktyk przetwarzania danych przez Miro, administratorzy powinni zapoznać się z [dodatkiem do przetwarzania danych przez Miro](https://miro.com/legal/customer-data-processing-addendum/).

## Rozwiązywanie problemów i FAQ

### Jak wyłączyć integrację (odinstalowanie na poziomie zespołu)?

Administrator zespołu Miro może odinstalować integrację Asana na poziomie zespołu. Ta czynność wyłącza integrację dla wszystkich członków zespołu. Aby to zrobić, przejdź do **Ustawienia zespołu Integracje i aplikacje**. Znajdź „Asana Ticketing” na liście zainstalowanych aplikacji, przewiń w dół i kliknij **Odinstaluj dla zespołu**.

### Jak wyłączyć integrację (indywidualne odinstalowanie)?

Użytkownicy mogą odinstalować integrację dla siebie. Przejdź do **Aplikacje i integracje** w ustawieniach Miro. Znajdź "Asana Ticketing" i kliknij **Odinstaluj dla siebie**.

### Którzy administratorzy mogą zainstalować integrację Asana dla swojego zespołu?

Tylko administratorzy zespołów Miro mogą bezpośrednio zainstalować aplikację. Jeśli administrator zespołu Miro wklei URL Asany na tablicę Miro, aplikacja zostanie automatycznie autoryzowana i zainstalowana bez potrzeby dalszych działań.

### Jakie są wymagania dostępności dla integracji Asana?

Integracja Asana jest dostępna dla abonamentów Business i Enterprise Miro.

### Czy administratorzy muszą autoryzować integrację Asana dla swojego zespołu?

Tak, administratorzy mogą potrzebować autoryzować integrację Asany dla swojego zespołu Miro. Członkowie zespołu mogą korzystać z integracji Asany tylko wtedy, gdy została ona zainstalowana na poziomie zespołu.
