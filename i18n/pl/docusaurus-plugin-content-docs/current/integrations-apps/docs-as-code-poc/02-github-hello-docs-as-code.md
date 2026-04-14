---
title: '[GitHub] Witaj, docs-as-code!'
article_id: 29239655610258
translation_id: 29239655610258
locale: pl-pl
sidebar_position: 2
created_at: '2025-09-04T17:11:12Z'
updated_at: '2026-01-23T15:01:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Ta sekcja dostarcza kompleksowych informacji technicznych i administracyjnych, niezbędnych dla specjalistów IT i bezpieczeństwa, odpowiedzialnych za wdrożenie, zabezpieczenie i bieżące zarządzanie integracją Trello w ich organizacji.

## Przegląd techniczny

Integracja Trello jest technicznie realizowana poprzez REST API. Do celów uwierzytelniania i autoryzacji, integracja wykorzystuje standardowy w branży protokół OAuth 2.0. Kluczowym elementem tej architektury jest zastosowanie zjednoczonej platformy API jako podprocesora dla danych stron trzecich. Ta platforma dostarcza ujednolicone API odpowiedzialne za uwierzytelnianie, normalizację i synchronizację danych z różnych dostawców API.

## Przepływy danych

Dokładne zrozumienie przepływu danych jest kluczowe dla zarządzania bezpieczeństwem i zgodnością w Twojej organizacji.

### Diagram sekwencji na wysokim poziomie

Tworzenie widżetu karty Trello

![image (7).png](images/32777103811218_image%20(7).png)

Aktualizacja widżetu karty Trello

![image (8).png](images/32777103814930_image%20(8).png)

### Dane Trello w Miro

Kiedy użytkownicy importują karty Trello na tablicę Miro, odpowiednie dane kart stają się integralną częścią danych planszy Miro. Miro przechowuje następujące konkretne dane zaimportowanych kart, o ile są one dostępne w Trello:

- Tytuł
- Opis
- Członkowie (w tym nazwy użytkowników i e-maile)
- Lista
- Etykiety

Jawne wyliczenie przechowywanych typów danych jest kluczowe dla organizacyjnego zarządzania danymi i zgodności. Pozwala administratorom dokładnie ocenić, jakie informacje, w szczególności dane wrażliwe, są replikowane w środowisku Miro. Ta przejrzystość zapewnia zgodność z wewnętrznymi politykami organizacji dotyczącymi obsługi danych. Warto także zauważyć, że zgodnie z sekcją „Ograniczenia”, pola niestandardowe nie są obsługiwane i tym samym nie są przechowywane, co jest kluczowym szczegółem dla mapowania danych i ocen zgodności. Miro stosuje hybrydowe podejście do przechowywania danych, minimalizując dane przechowywane bezpośrednio w widżecie karty i pobierając dodatkowe szczegóły podczas otwarcia widoku edycji przez użytkownika.

### Retencja przechowywanych informacji w Miro

Całe importowane dane z Trello przechowywane w Miro ściśle podlegają standardowej zasadzie retencji danych Miro. Zasada ta jest stosowana konsekwentnie do wszystkich danych klientów, zapewniając jednolite podejście do zarządzania cyklem życia danych.

## Uwierzytelnianie i autoryzacja

Integracja z Trello inicjuje przepływ uwierzytelniania, gdy użytkownik po raz pierwszy korzysta z integracji. Autoryzacja w Trello jest obsługiwana przez usługę integracji. Dla każdego użytkownika Miro zakłada konto w tej usłudze integracyjnej, a te dane dostępowe są następnie wykorzystywane do wszystkich interakcji użytkownika z integracją.

Integracja zazwyczaj wymaga aprobaty administratora Trello, aby autoryzować aplikację integracyjną w ekosystemie organizacji. Dodatkowo, indywidualni użytkownicy muszą również autoryzować integrację Miro z Trello za pomocą strony autoryzacji OAuth w Trello, gdy po raz pierwszy próbują osadzić link Trello.

### Wymagane zakresy autoryzacji

Zakres autoryzacji może się różnić w zależności od konkretnego systemu zewnętrznego. Jednak dla integracji z zarządzaniem kartami, jak w przypadku Trello, Miro zazwyczaj wymaga dostępu do następujących danych:

| Zakres | Opis |
| --- | --- |
| Karty (odczyt i zapis) | Udziela integracji uprawnienia do odczytywania istniejących kart oraz tworzenia lub modyfikowania kart w Trello. |
| Członkowie (odczyt) | Udziela integracji uprawnienia do odczytywania informacji o członkach w Trello, zazwyczaj do przypisywania kart lub wyświetlania nazw członków. |
| Etykiety (odczyt) | Udziela integracji uprawnienia do odczytywania etykiet powiązanych z kartami w Trello. |
| Tablice (odczyt) | Udziela integracji uprawnienia do odczytywania informacji o tablicach i listach w Trello. |

### Co jest przechowywane w Miro i w jaki sposób

Miro bezpiecznie przechowuje zarówno dane związane z autoryzacją, jak i niektóre związane z rozwijaniem dla integracji z Trello:

- **Dane dotyczące autoryzacji:** Obejmują one wartości tokenów dostępu i tokenów odświeżania, które są przechowywane w bazie danych Miro przez ograniczony czas kilku dni. Te tokeny są automatycznie odnawiane po wygaśnięciu przy użyciu tokena odświeżania, aby zapewnić ciągły dostęp. Wszystkie takie dane przechowywane w bazie danych w ramach tej integracji są szyfrowane za pomocą 256-bitowego zaawansowanego standardu szyfrowania, co zapewnia solidną warstwę bezpieczeństwa danych.
- **Dane dotyczące rozwijania:** Obejmują one tytuły kart, które są przechowywane jako część samych tablic Miro. Dodatkowo, tytuły i zaszyfrowane odwołania do tych elementów są przechowywane w wewnętrznej usłudze, dodatkowo zabezpieczone szyfrowaniem (zarządzanie kluczami szyfrowania).

### Unieważnianie tokena

Jeśli zajdzie taka potrzeba, administratorzy lub indywidualni użytkownicy mogą cofnąć tokeny przyznane integracji z Trello. Użytkownicy mogą przejść do ustawień integracji, otwierając kartę wyboru integracji, klikając menu z 3 kropkami w prawym górnym rogu i wybierając **Ustawienia integracji**, lub uzyskując dostęp do karty **Aplikacje** w ustawieniach zespołu w Miro, znajdując konkretną integrację i klikając na nią. Na stronie ustawień autoryzację można cofnąć, klikając przycisk **Rozłącz**. Po tym działaniu Miro cofa dostęp do Trello i usuwa powiązane konto użytkownika. W przypadku dezinstalacji na poziomie zespołu, administratorzy mogą postępować zgodnie z określonymi krokami opisanymi w sekcji „Rozwiązywanie problemów i FAQ (Administrator)”.

## Jak skonfigurować integrację z Trello

Proces konfiguracji integracji Miro + Trello obejmuje różne kroki zarówno dla administratorów, jak i użytkowników końcowych, co zapewnia kontrolowane wdrożenie w organizacji.

1. **Zadbaj o aktywne konta:** Przed rozpoczęciem instalacji upewnij się, że dostępne są aktywne konta Miro i Trello.
2. **Instalacja na poziomie zespołu (akcja administratora):**
   - Administratorzy mogą być zobowiązani do wyraźnego autoryzowania integracji z Trello dla swojego zespołu Miro. Członkowie zespołu mogą korzystać z integracji tylko wtedy, gdy została zainstalowana na poziomie zespołu.
   - Administrator zespołu Miro może bezpośrednio zainstalować aplikację, otwierając tablicę Miro, wybierając **Narzędzia Media i Integracje (+)**, szukając „Trello” i klikając **Połącz**, aby autoryzować integrację. Jeśli administrator zespołu Miro wykona tę czynność, aplikacja zostanie automatycznie autoryzowana i zainstalowana bez konieczności dalszej akceptacji administracyjnej.
3. **Przepływ prośby użytkownika i zatwierdzenia przez administratora (jeśli dotyczy):**
   - W organizacjach, gdzie wymagana jest ścisła zgoda administracyjna, użytkownik nie będący administratorem w zespole Miro skonfigurowanym do integracji z Trello może wkleić link Trello na tablicę Miro. Ta akcja może wywołać okno dialogowe „zapytanie o instalację aplikacji”, co skłoni użytkownika do szukania zgody administratora.
   - Wyznaczeni administratorzy mogą następnie przejrzeć i zatwierdzić to oczekujące zapytanie za pośrednictwem swoich konsoli administracyjnych Miro lub Trello, w zależności od skonfigurowanego przepływu zgody.
4. **Połączenie indywidualnego użytkownika:**
   - Po pomyślnym zainstalowaniu i autoryzowaniu integracji na poziomie zespołu przez administratora, indywidualni użytkownicy będą klikać "**Połącz**" w widżecie Trello, który pojawia się na tablicy Miro.
   - Użytkownicy zostaną przekierowani na stronę autoryzacji Trello, gdzie udzielą Miro dostępu do swojego indywidualnego konta Trello, tym samym potwierdzając swoją osobistą autoryzację do osadzania i interakcji z treściami.

## Względy bezpieczeństwa i zgodności

### Ograniczenie dostępu do pliku źródłowego

Aby zapewnić, że dostęp do osadzonych danych z Trello pozostaje ograniczony do tych samych osób co na źródłowej tablicy Trello, administratorzy organizacji Miro muszą utrzymywać ścisłą kontrolę nad udostępnianiem tablic oraz eksportem treści. Chociaż podstawowa integracja Trello respektuje indywidualne uprawnienia do interakcji na żywo, każdy eksport lub statyczny zrzut treści tablicy mógłby potencjalnie ujawnić dane osobom nieupoważnionym, jeśli sama tablica Miro nie jest odpowiednio zabezpieczona.

### Obsługa błędów

Integracja została zaprojektowana z zabezpieczeniem UI i obsługą błędów w przypadku, gdy aktualizacje danych kart zawodzą z powodu odrzucenia przez stronę trzecią.

### Dodatkowa umowa o przetwarzaniu danych Miro (DPA)

Aby uzyskać pełne informacje prawne i zgodności dotyczące praktyk przetwarzania danych przez Miro, administratorzy są proszeni o zapoznanie się z dokumentem [Miro Data Processing Addendum](https://miro.com/legal/customer-data-processing-addendum/).

## Rozwiązywanie problemów i FAQ

### Jak można wyłączyć integrację (odinstalowanie na poziomie zespołu)?

Administrator zespołu Miro może odinstalować integrację Trello na poziomie zespołu. Ta czynność wyłącza integrację dla wszystkich członków zespołu. Aby to zrobić, przejdź do **Ustawienia zespołu & Integracje**. Znajdź "Trello" lub "Zarządzanie Kartami Trello" na liście zainstalowanych aplikacji, przewiń w dół i kliknij **Odinstaluj dla zespołu**.

### Jak można wyłączyć integrację (odinstalowanie indywidualne)?

Pojedynczy użytkownicy mogą odinstalować integrację dla siebie. Przejdź do sekcji **Aplikacje i Integracje** w swoich ustawieniach Miro. Znajdź „Trello” lub „Zarządzanie kartami Trello” i kliknij **Odinstaluj dla mnie**.

### Którzy administratorzy mogą zainstalować integrację Trello dla swojego zespołu?

Tylko administratorzy zespołów Miro mogą bezpośrednio zainstalować aplikację. Jeśli administrator zespołu Miro wklei adres URL Trello na tablicę Miro, aplikacja zostanie automatycznie autoryzowana i zainstalowana bez potrzeby dalszej interwencji.

### Jakie są wymagania dotyczące dostępności integracji Trello?

Integracja Trello jest dostępna dla wersji Business i Enterprise Miro. REST API

### Czy administratorzy muszą autoryzować integrację Trello dla swojego zespołu?

Tak, administratorzy mogą potrzebować autoryzować integrację Trello dla swojego zespołu w Miro. Członkowie zespołu mogą korzystać z tej integracji tylko wtedy, gdy została zainstalowana na poziomie zespołu.
