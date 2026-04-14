---
title: "Skonfiguruj Trello dla swojego zespo\u0142u"
article_id: 30634093325842
translation_id: 30634093325842
locale: pl-pl
sidebar_position: 2
created_at: '2025-10-29T15:59:48Z'
updated_at: '2026-02-23T11:40:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Techniczna implementacja integracji z Trello odbywa się za pomocą REST API. W celu uwierzytelnienia i autoryzacji integracja korzysta z protokołu OAuth 2.0, który jest standardem branżowym. Kluczowym elementem tej architektury jest wykorzystanie jednolitej platformy API jako podprocesora dotyczącego danych stron trzecich. Platforma ta udostępnia zunifikowane API odpowiedzialne za uwierzytelnienie, normalizację i synchronizację danych między różnymi dostawcami API.

## Przepływy danych

Dogłębne zrozumienie przepływu danych jest kluczowe dla zarządzania bezpieczeństwem i zgodnością w Twojej organizacji.

### Diagram sekwencji wysokiego poziomu

Tworzenie widżetu karty Trello

![Trello (BETA) 2.jpg](images/30635017559186_Trello%20(BETA) 2.jpg)

Aktualizacja widżetu karty Trello

![Trello (BETA) 2.jpg](images/30635017559186_Trello%20(BETA) 2.jpg)

### Dane Trello w Miro

Kiedy użytkownicy importują karty Trello na tablicę Miro, odpowiednie dane tych kart stają się integralną częścią danych na planszy Miro. Miro przechowuje następujące szczegółowe punkty danych dla importowanych kart, pod warunkiem, że są dostępne w Trello:

- Tytuł
- Opis
- Użytkownicy (w tym imiona i e-maile)
- Lista
- Etykiety

Jawna enumeracja przechowywanych typów danych jest kluczowa dla zarządzania danymi i zgodności organizacyjnej. Umożliwia administratorom dokładne ocenienie, jakie informacje, zwłaszcza ewentualnie dane wrażliwe, są replikowane w środowisku Miro. Ta przejrzystość zapewnia zgodność z wewnętrznymi politykami organizacji dotyczącymi przetwarzania danych. Warto również zauważyć, że zgodnie z rozdziałem "Ograniczenia" niestandardowe pola nie są obsługiwane, a zatem nie są przechowywane, co jest kluczowym szczegółem do mapowania danych i ocen zgodności. Miro wykorzystuje hybrydowe podejście do przechowywania danych, minimalizując dane przechowywane bezpośrednio w widżecie karty i pobierając dodatkowe szczegóły, gdy użytkownik otwiera widok edycji.

### Retencja przechowywanych informacji w Miro

Wszystkie zaimportowane dane Trello, które są przechowywane w Miro, ściśle przestrzegają standardowej zasady retencji danych Miro. Ta zasada jest stosowana konsekwentnie do wszystkich danych klientów, zapewniając jednolite podejście do zarządzania cyklem życia danych.

## Uwierzytelnianie i autoryzacja

Integracja Trello inicjuje przepływ uwierzytelniania, gdy użytkownik po raz pierwszy wchodzi w interakcję z integracją. Autoryzacja w Trello jest obsługiwana przez usługę integracyjną. Dla każdego indywidualnego użytkownika Miro ustanawia konto w tej usłudze integracyjnej, a powiązane dane dostępowe są następnie używane we wszystkich interakcjach użytkownika z integracją.

Integracja zwykle wymaga zgody administratora Trello na autoryzację aplikacji integracyjnej w ekosystemie organizacji. Dodatkowo, indywidualni użytkownicy muszą także autoryzować integrację Miro Trello przez stronę autoryzacji OAuth Trello, gdy po raz pierwszy próbują osadzić link Trello.

### Wymagane zakresy autoryzacji

Zakres autoryzacji może się różnić w zależności od konkretnego systemu zewnętrznego. Jednak w przypadku integracji zarządzania kartami, takich jak Trello, Miro zazwyczaj wymaga dostępu do następujących danych:

| Zakres | Opis |
| --- | --- |
| Karty (odczyt i zapis) | Udziela integracji pozwolenia na odczyt istniejących kart (biletów) oraz tworzenie lub modyfikację kart w Trello. |
| Użytkownicy (odczyt) | Udziela integracji pozwolenia na odczyt informacji o użytkownikach w Trello, zazwyczaj w celu przypisania kart lub wyświetlania nazw członków. |
| Zbiory (odczyt) | Udziela integracji pozwolenia na odczyt zbiorów, tablic i list w Trello. |

### Co jest przechowywane w Miro i jak

Miro bezpiecznie przechowuje zarówno dane związane z autoryzacją, jak i z rozwijaniem dla integracji Trello:

- **Dane związane z autoryzacją:** Obejmują one wartości tokenów dostępu i tokenów odświeżania, które są przechowywane w bazie danych Miro przez ograniczony czas, zwykle kilka dni. Te tokeny są automatycznie odświeżane po wygaśnięciu za pomocą tokena odświeżania, aby zapewnić ciągły dostęp. Wszystkie dane przechowywane w bazie danych na potrzeby tej integracji są szyfrowane przy użyciu standardu szyfrowania Advanced Encryption Standard 256-bit, co zapewnia solidną warstwę ochrony danych.
- **Dane związane z funkcją unfurl:** Zawierają tytuły kart, które są przechowywane jako część samych tablic Miro. Dodatkowo, tytuły i zaszyfrowane odniesienia do tych elementów są przechowywane w wewnętrznej usłudze, dodatkowo zabezpieczone poprzez szyfrowanie (zarządzanie kluczami szyfrowania).

### Unieważnianie tokena

Jeśli zajdzie taka konieczność, administratorzy lub indywidualni użytkownicy mogą cofnąć przyznane tokeny dla integracji z Trello. Użytkownicy mogą przejść do ustawień integracji, otwierając menu wyboru kart integracji, klikając menu z 3 kropkami w prawym górnym rogu i wybierając **Ustawienia integracji**, lub przechodząc do zakładki **Aplikacje** zespołu w ustawieniach zespołu Miro, wyszukując konkretną integrację i klikając na nią. Na stronie ustawień autoryzację można cofnąć przez kliknięcie przycisku **Rozłącz**. Po wykonaniu tej akcji Miro cofnie dostęp do Trello i usunie powiązane konto użytkownika. W przypadku odinstalowania na poziomie zespołu administratorzy mogą postępować zgodnie z konkretnymi krokami opisanymi w sekcji „Rozwiązywanie problemów i często zadawane pytania (administracja)”.

## Jak skonfigurować integrację z Trello

Proces konfiguracji integracji Miro + Trello obejmuje odrębne kroki dla administratorów i użytkowników końcowych, co zapewnia kontrolowane wdrożenie w organizacji.

1. **Zapewnij aktywne konta:** Przed rozpoczęciem instalacji upewnij się, że oba konta Miro i Trello są aktywne.
2. **Instalacja na poziomie zespołu (akcja administratora):**
   - Administratorzy mogą potrzebować wyraźnie autoryzować integrację Trello dla swojego zespołu w Miro. Członkowie zespołu mogą korzystać z integracji tylko wtedy, gdy została ona zainstalowana na poziomie zespołu.
   - Administrator zespołu Miro może bezpośrednio zainstalować aplikację, otwierając tablicę Miro, wybierając **Narzędzia Media & Integracje (+)**, wyszukując "Trello" i klikając **Połącz**, aby autoryzować integrację. Jeśli tę czynność wykona administrator zespołu Miro, aplikacja zostanie automatycznie autoryzowana i zainstalowana bez potrzeby uzyskiwania dalszej zatwierdzeń administracyjnych.
3. **Przepływ zgłoszeń użytkowników i zatwierdzenie administratora (jeśli dotyczy):**
   - W organizacjach, w których wymagana jest ścisła zgoda administracyjna, użytkownik niebędący administratorem w zespole Miro skonfigurowanym do integracji z Trello może wkleić link Trello na tablicę Miro. Działanie to może wywołać okno dialogowe "prośba o instalację aplikacji" dla użytkownika, zachęcając go do uzyskania zgody administracyjnej.
   - Wyznaczeni administratorzy mogą następnie przejrzeć i zatwierdzić to oczekujące zgłoszenie za pośrednictwem swoich konsol administracyjnych Miro lub Trello, w zależności od skonfigurowanego przepływu zgody.
4. **Przyłączenie indywidualnego użytkownika:**
   - Po pomyślnym zainstalowaniu i autoryzowaniu integracji na poziomie zespołu przez administratora, użytkownicy indywidualni klikną **Połącz** na widżecie Trello, który pojawia się na tablicy Miro.
   - Użytkownicy zostaną następnie przekierowani do strony autoryzacji Trello, gdzie umożliwią Miro dostęp do swojego indywidualnego konta Trello, tym samym potwierdzając osobistą zgodę na osadzanie i interakcję z treścią.

## Zagadnienia dotyczące bezpieczeństwa i zgodności

### Ograniczenie dostępu do pliku źródłowego

Aby zapewnić, że dostęp do osadzonych danych Trello pozostaje ograniczony do tych samych osób co na oryginalnej tablicy Trello, administratorzy organizacji Miro muszą utrzymywać ścisłą kontrolę nad udostępnianiem tablic oraz eksportem treści. Podczas gdy podstawowa integracja Trello respektuje indywidualne uprawnienia do interakcji na żywo, każdy eksport lub statyczny zrzut zawartości tablicy może potencjalnie ujawnić dane nieupoważnionym osobom, jeśli sama tablica Miro nie jest zarządzana w sposób bezpieczny.

### Obsługa błędów

Integracja jest zaprojektowana z łagodnym przejściem w interfejsie użytkownika i obsługą błędów w sytuacjach, gdy aktualizacje danych kart nie powiodą się z powodu odrzucenia przez strony trzecie.

### Dodatkowe postanowienie dotyczące przetwarzania danych Miro (DPA)

W celu uzyskania szczegółowych informacji prawnych i wymaganych do zgodności dotyczących praktyk przetwarzania danych przez Miro, administratorzy są kierowani do zapoznania się z [Miro Data Processing Addendum](https://miro.com/legal/customer-data-processing-addendum/).

## Rozwiązywanie problemów i FAQ

### Jak wyłączyć integrację na poziomie zespołu?

Administrator zespołu Miro może odinstalować integrację z Trello na poziomie zespołu. Ta akcja wyłącza integrację dla wszystkich członków zespołu. Aby to zrobić, przejdź do **Ustawienia zespołu Aplikacje i integracje**. Znajdź "Trello" lub "Zarządzanie Kartami Trello" na liście zainstalowanych aplikacji, przewiń w dół i kliknij **Odinstaluj dla zespołu**.

### Jak wyłączyć integrację indywidualnie?

Indywidualni użytkownicy mogą odinstalować integrację dla siebie. Przejdź do **Aplikacje i integracje** w swoich ustawieniach Miro. Znajdź "Trello" lub "Zarządzanie kartami Trello" i kliknij **Odinstaluj dla mnie**.

### Którzy administratorzy mogą zainstalować integrację Trello dla swojego zespołu?

Tylko administratorzy zespołów Miro mogą bezpośrednio zainstalować aplikację. Jeśli administrator zespołu Miro wklei adres URL Trello na tablicy Miro, aplikacja zostanie automatycznie autoryzowana i zainstalowana bez wymagania dalszych działań.

### Jakie są wymagania dotyczące dostępności integracji Trello?

Integracja Trello jest dostępna w ramach abonamentów Business i Enterprise Miro.

### Czy administratorzy muszą autoryzować integrację Trello dla swojego zespołu?

Tak, administratorzy mogą potrzebować autoryzować integrację z Trello dla swojego zespołu w Miro. Członkowie zespołu mogą korzystać z integracji z Trello tylko wtedy, gdy została ona zainstalowana na poziomie zespołu.
