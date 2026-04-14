---
title: "Konfiguracja Linear (wersja beta) dla Twojego zespo\u0142u"
article_id: 30630697364626
translation_id: 30630697364626
locale: pl-pl
sidebar_position: 2
created_at: '2025-10-29T14:09:41Z'
updated_at: '2026-02-23T11:23:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Integracja Linear jest technicznie zrealizowana poprzez REST API. Do celów uwierzytelniania i autoryzacji wykorzystuje standardowy w branży protokół OAuth 2.0. Kluczowym elementem tej architektury jest zunifikowana platforma API używana jako podprocesor danych zewnętrznych do zarządzania uwierzytelnianiem, normalizacją i synchronizacją między różnymi dostawcami API.

## Przepływ danych

Zrozumienie przepływu danych jest kluczowe dla zarządzania bezpieczeństwem i zgodnością.

### Diagram sekwencji na wysokim poziomie

Tworzenie widżetu karty Linear

![Asana Cards (BETA) (1).jpg](images/30631712690066_Asana%20Cards%20(BETA) (1).jpg)

Aktualizowanie widżetu karty Linear

![Asana Cards (BETA) (1).jpg](images/30631712690066_Asana%20Cards%20(BETA) (1).jpg)

### Dane Linear w Miro

Kiedy użytkownicy importują zgłoszenia Linear na planszę Miro, następujące dane są integralne dla planszy Miro:

- Tytuł
- Opis
- Osoba przypisana (nazwa/e-mail)
- Stan
- Priorytet

Ta lista jest kluczowa dla zarządzania danymi, potwierdzając, jakie dane wrażliwe trafiają do środowiska Miro. Należy zauważyć, że pola niestandardowe nie są obsługiwane.

### Retencja danych

Wszystkie zaimportowane dane Linear przestrzegają ściśle standardowej zasady retencji danych Miro i są konsekwentnie stosowane do wszystkich danych klientów.

## Uwierzytelnianie i autoryzacja

Przy pierwszej interakcji integracja Linear inicjuje przepływ uwierzytelniania. Dla każdego użytkownika Miro tworzy dane dostępowe z usługą integracji dla kolejnych interakcji.

Integracja zazwyczaj wymaga aprobaty administratora Linear.

### Wymagane zakresy autoryzacji

| Zakres | Opis |
| --- | --- |
| Kolekcje | Dostęp do kolekcji zgłoszeń. |
| Użytkownicy | Czytaj informacje o użytkownikach do przypisania/wyświetlenia. |
| Zgłoszenia | Czytaj, twórz, modyfikuj zgłoszenia w Linear. |

## Co jest przechowywane w Miro i jak

- **Dane związane z autoryzacją:** Tokeny są przechowywane w bazie danych Miro przez kilka dni, kodowane za pomocą AES-256.
- **Dane związane z rozwijaniem:** Tytuły zgłoszeń są przechowywane z zaszyfrowanymi odwołaniami.

### Unieważnianie tokenu

Unieważnianie tokenów może odbywać się poprzez **Kartę Ustawienia integracji** lub kartę **Aplikacje** poprzez wybór **Rozłącz**. Ta akcja usuwa dostęp do Linear i kasuje dane dostępowe użytkownika.

## Jak skonfigurować integrację Linear

Kroki dla administratorów i użytkowników końcowych zapewniają kontrolowane wdrożenie.

1. **Upewnij się, że konta są aktywne:** Konta Miro i Linear muszą być aktywne.
2. **Instalacja na poziomie zespołu (działanie administratora):**
   - Administratorzy muszą autoryzować integrację Linear na poziomie zespołu.
   - Instalacja poprzez **Narzędzia Media i Integracje**, wyszukując "Linear" i łącząc się.
3. **Prośba użytkownika i zatwierdzenie przez administratora:**
   - W organizacjach wymagających ścisłej zgody, wklejenie linku Linear może wywołać prośbę o zatwierdzenie przez administratora.
   - Administratorzy mogą zatwierdzić za pomocą konsoli Miro lub Linear.
4. **Indywidualne połączenie użytkownika:**
   - Użytkownicy łączą się za pośrednictwem widżetu Linear i autoryzacji OAuth.

## Bezpieczeństwo i zgodność

### Ograniczenie dostępu do pliku źródłowego

Utrzymywanie ścisłej kontroli nad udostępnianiem tablic dostosowuje uprawnienia Linear do Miro.

### Obsługa błędów

Integracja oferuje eleganckie przejście interfejsu użytkownika w przypadku odrzucenia przez zewnętrzne źródła.

### Dodatek do przetwarzania danych Miro (DPA)

Zapoznaj się z [dodatkiem do przetwarzania danych Miro](https://miro.com/legal/customer-data-processing-addendum/) w celu uzyskania szczegółowych informacji prawnych i dotyczących zgodności.

## Rozwiązywanie problemów & FAQ

### Jak wyłączyć integrację (poziom zespołu)

Administratorzy mogą odinstalować z **Ustawienia zespołu Aplikacje & Integracje**, wybierając „Linear” i klikając **Odinstaluj dla zespołu**.

### Jak wyłączyć integrację (indywidualnie)

Użytkownicy mogą przejść do **Aplikacje & Integracje** i wybrać „Odinstaluj dla mnie” dla Linear.

### Uprawnienia administratora

Tylko administratorzy zespołów Miro mogą bezpośrednio instalować aplikację. Instalacje automatyczne odbywają się przy wklejaniu URL-e Linear na tablicę.

### Wymagania dotyczące dostępności

Integracja z Linear jest dostępna w abonamentach Business i Enterprise.

### Wymóg autoryzacji przez administratora

Tak, autoryzacja na poziomie zespołu przez administratorów jest konieczna do uzyskania dostępu zespołu.
