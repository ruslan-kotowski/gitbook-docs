---
title: "Mo\u017Cliwo\u015Bci zaufania AI i FAQ"
article_id: 30943405232914
translation_id: 30943405232914
locale: pl-pl
sidebar_position: 0
created_at: '2025-11-10T14:17:30Z'
updated_at: '2026-03-11T21:34:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Na Canvas 25 ogłosiliśmy przestrzeń roboczą dla innowacji z AI z wizualnymi przepływami pracy AI i asystentami AI dostępnymi na planszy. Oprócz funkcji dla użytkowników końcowych, wprowadzamy nowe możliwości administracyjne, które zapewniają większą widoczność, inteligentniejsze ustawienia i płynne sposoby na odblokowanie najnowszych narzędzi AI Miro dla Twoich zespołów.

Użyj tej strony, aby zgłębić możliwości zaufania do AI dostępne z dodatkiem Enterprise Guard. Każda sekcja rozpoczyna się krótkim przeglądem, po którym następują rozwijane FAQ obejmujące różne aspekty każdej zdolności.

- Szczegółowe ustawienia administracyjne Miro AI: ustaw dostęp do funkcji na poziomie funkcji (Wszyscy/Nikt/Wybrane zespoły) w każdej kategorii funkcji.
- [Blokowanie użycia Miro AI za pomocą zabezpieczeń inteligentnych](#h_block_ai_with_guardrails): użyj zabezpieczeń inteligentnych, aby zablokować wszelkie interakcje zasilane przez AI w Miro, gdy potrzebujesz chronić dane wrażliwe lub tajne.
- [Pulpit przeglądu analityki dla administratorów](#h_admin_analytics_overview): śledź tablice, użytkowników, zespoły, licencje i szablony z historycznymi trendami i codziennym odświeżaniem.
- Moderacja AI (dostępna także w wersji Enterpise): ustaw poziomy filtrowania dla całej organizacji (Rygorystyczny, Domyślny, Minimalny), aby przefiltrować prompty, które mogą prowadzić do szkodliwych lub nieodpowiednich wyników.
- Blokowanie promptów: blokuj prompty zawierające dane wrażliwe lub kod źródłowy w momencie ich przesyłania; wyświetl komunikat polityki zamiast wysyłać do LLM.
- Enterprise Guard i integracja z Microsoft Purview DSPM dla AI: przekierowuj prompty i odpowiedzi do Purview w celu centralnego monitoringu, audytu i zarządzania.

## Szczegółowe ustawienia administracyjne Miro AI dla dodatku Enterprise Guard

Ustawienia administratora Miro AI umożliwiają administratorom firmy Enterprise decydowanie, które funkcje AI są dostępne w ich organizacji oraz zarządzanie, kto może z nich korzystać. Administratorzy mogą także wyświetlać modele napędzające każdą funkcję AI. Dzięki dodatkowi Enterprise Guard, ustawienia Miro AI obejmują poziom funkcji w każdej kategorii funkcji, co pomaga priorytetyzować funkcje w oparciu o potrzeby organizacyjne i wymagania dotyczące bezpieczeństwa. Oprócz pełnej kategorii funkcji Miro AI, administratorzy mogą również włączać, ograniczać lub usuwać konkretne funkcje Miro AI. Na przykład w kategorii obrazy można włączyć funkcję tworzenia obrazów z AI i wyłączyć usuwanie tła. Użyj tych ustawień, aby bezpiecznie wprowadzać AI i spełniać wymagania dotyczące bezpieczeństwa, jednocześnie promując przyjęcie możliwości AI.  Więcej informacji znajdziesz w [dokumentacji szczegółowych ustawień administratora Miro AI](../../enterprise-guard/ai-trust/02-miro-ai-granular-admin-controls.md).

**Cel i zakres**

**Co to jest szczegółowe ustawienie Miro AI?**

Administratorzy firmy z dodatkiem Enterprise Guard mogą włączyć, ograniczyć lub usunąć dostęp do poszczególnych funkcji AI w każdej kategorii możliwości. Pozwala to na precyzyjne ustalenie, z których funkcji mogą korzystać zespoły.

**Dlaczego warto używać szczegółowych ustawień?**

Aby zrównoważyć wdrożenie z bezpieczeństwem. Na przykład w przypadku obrazów można włączyć opcję tworzenia obrazów, jednocześnie wyłączając opcję usuwania tła.

**Dostęp i wymagania wstępne**

**Kto może konfigurować szczegółowe ustawienia i na jakich abonamentach?**

Administratorzy firmy na abonamentach Enterprise z dodatkiem Enterprise Guard, w przeglądarce.

**Gdzie zarządzam dostępem do funkcji na poziomie szczegółowym?**

Konsola administratora → Miro AI → Funkcje. Rozwiń funkcję, aby zobaczyć i ustawić dostęp do jej poszczególnych cech.

**Ustawienia i zachowanie**

**Szczegółowe ustawienia: jaka jest różnica między ustawieniem na poziomie możliwości a ustawieniem na poziomie funkcji, i co się dzieje, gdy je włączam lub wyłączam?**

- **Poziom możliwości:** Wszyscy, Nikt lub Wybrane zespoły dotyczy całej kategorii. Jeśli dezaktywujesz możliwość, użytkownicy tracą dostęp do tej możliwości i wszystkich jej funkcji na tablicach. Jeśli dezaktywujesz wszystkie możliwości, opcja Twórz z pomocą AI jest wyłączona na tablicy.
- **Poziom funkcji:** Z Enterprise Guard, możesz ustawić Wszyscy, Nikt lub Wybrane zespoły dla każdej funkcji indywidualnie. Dezaktywacja funkcji usuwa dostęp tylko do tej funkcji; inne funkcje w tej samej możliwości pozostają dostępne, jeśli są włączone.

**Jakie opcje dostępu istnieją na poziomie funkcji?**

Dla każdej funkcji wybierz jedną z opcji: Wszyscy, Nikt lub Wybrane zespoły. Opcja Wszyscy włącza funkcję dla całej organizacji i nadpisuje ograniczenia na poziomie zespołu. Opcja Nikt usuwa dostęp dla wszystkich użytkowników. Opcja Wybrane zespoły kieruje funkcję tylko do wybranych zespołów.

**Co się dzieje, gdy dezaktywuję indywidualną funkcję?**

Użytkownicy nie mogą uzyskać dostępu do tej funkcji na żadnej tablicy, ale inne funkcje w tej samej kategorii pozostają dostępne, jeśli są włączone.

**Odniesienia i przykłady**

**Jakie funkcje mogę kontrolować indywidualnie?**

Zapoznaj się z odniesieniem w produkcie, aby zobaczyć aktualną listę. Przykłady w sekcji Tworzenie treści to Tworzenie karteczek, Kategoryzacja karteczek, Tworzenie i edycja dokumentów, tabel, diagramów oraz operacje na tekście takie jak przepisanie, skrócenie, zmiana stylu i tłumaczenie. Obrazy obejmują Tworzenie obrazów, Usuwanie tła i Dodawanie podpisów. Podsumowanie działań obejmuje Nowości i Podsumowanie konwersacji. Przepływy, współpracownicy AI oraz prototypowanie pojawiają się, jeśli są włączone dla Twojej organizacji.

**Czy mogę zobaczyć, które modele zasilają poszczególne funkcje?**

Tak. Administratorzy mogą wyświetlać modele powiązane z każdą funkcją AI w obszarze odniesienia, aby wspierać przegląd i zarządzanie.

## Blokowanie użycia Miro AI za pomocą zabezpieczeń Intelligent Guardrails

Użyj zabezpieczeń, aby zablokować wszystkie interakcje wspierane przez AI w Miro, gdy potrzebujesz chronić dane poufne lub sklasyfikowane. Kiedy to zabezpieczenie jest aktywne, wszystkie narzędzia Miro AI są wyłączone na dotkniętych tablicach, podczas gdy współpraca bez użycia AI pozostaje dostępna. Aby uzyskać więcej informacji i szczegóły konfiguracyjne, zobacz przegląd zabezpieczeń i Zdefiniuj zabezpieczenia.

**Cel i zakres**

**Co oznacza „Zablokowanie użycia Miro AI”?**

Wyłącza wszystkie funkcje Miro AI (na przykład generowanie tekstu, generowanie/rozpoznawanie obrazów, inteligentne sugestie) tam, gdzie obowiązuje ta zasada, zapobiegając jakiejkolwiek interakcji AI z wrażliwymi lub zastrzeżonymi treściami.

**Co pozostaje dostępne dla użytkowników?**

Użytkownicy mogą kontynuować standardową, nie bazującą na AI współpracę. Istniejące, wygenerowane przez AI treści pozostają na tablicach i mogą być wyświetlane, przenoszone lub ręcznie edytowane — ale użytkownicy nie mogą używać Miro AI do ich modyfikacji lub ponownego generowania.

**Dostęp i wymagania wstępne**

**Kto może skonfigurować to zabezpieczenie i gdzie?**

Administratorzy treści wrażliwych konfigurują zabezpieczenia w *Enterprise Guard* w sekcji Klasyfikacja danych → Zabezpieczenia. (Administratorzy firmy nadają rolę administratora treści wrażliwych.)

**Co jest potrzebne przed przypisaniem tego zabezpieczenia?**

Zdefiniuj swoje poziomy klasyfikacji i (opcjonalnie) autoklasyfikację, aby zabezpieczenie mogło być zastosowane przez klasyfikację (na przykład WEWNĘTRZNE, POUFNE).

**Zachowanie i wpływ**

**Kto jest dotknięty, gdy obowiązuje zabezpieczenie?**

Wszyscy — w tym właściciele i współwłaściciele tablic — nie mogą uzyskać dostępu ani uruchomić Miro AI na dotkniętych tablicach.

**Czy usuwa istniejącą treść AI?**

Nie. Zapobiega dalszym interakcjom z AI; istniejąca treść AI pozostaje dostępna do wyświetlania i ręcznej edycji.

**Kiedy wprowadzone zmiany wchodzą w życie?**

Po opublikowaniu aktualizacji zabezpieczenia, jego egzekwowanie następuje natychmiastowo na dotkniętych tablicach.

**Konfiguracja i ustawienia**

**Jak włączyć „Blokowanie użycia Miro AI” dla klasyfikacji?**

1. Przejdź do *Enterprise Guard* → Klasyfikacja danych → **Zabezpieczenia**.
2. Kliknij ikonę **Edycji** przy poziomie klasyfikacji (na przykład POUFNE).
3. Zaznacz pole wyboru **Blokowanie użycia Miro AI** i kliknij **Zrobione**.
4. Kliknij **Dalej** i przejrzyj wpływ, a następnie **Opublikuj** aby zastosować.

**Czy powinienem używać trybu Domyślny czy Ścisły?**

W trybie domyślnym zabezpieczenia nie zastępują istniejących ustawień udostępniania. W trybie ścisłym zabezpieczenia zastępują aktywne udostępnianie i stosują najbardziej rygorystyczne kontrole. Wybierz w zależności od potrzeb zarządzania zmianami.

**Doświadczenia użytkowników**

**Co zobaczą użytkownicy na tablicach, gdzie AI jest zablokowana?**

Punkty wejścia Miro AI wydają się wyłączone lub niedostępne, a użytkownicy nie mogą korzystać z narzędzi AI z planszy lub menu na tych tablicach.

**Czy użytkownicy mogą wnioskować o wyjątki na pojedynczej tablicy?**

Nie. Zabezpieczenie jest egzekwowane przez politykę klasyfikacyjną. Zmień klasyfikację tablicy (lub politykę dla tego poziomu), aby zmienić egzekwowanie.

**Interakcje z innymi ustawieniami**

**W jaki sposób jest to związane ze szczegółowymi ustawieniami administracyjnymi Miro AI?**

Szczegółowe ustawienia kontrolują, kto może korzystać z określonych funkcji AI. Zasada jest warstwą polityk: gdy jest aktywna, blokuje AI niezależnie od przełączników funkcji.

**Czym różni się to od blokowania promptów lub moderacji AI?**

- **Blokowanie promptów** zatrzymuje wrażliwe prompty podczas przesyłania; AI pozostaje dostępne dla niewrażliwych promptów.
- **Moderacja AI** filtruje szkodliwe lub nieodpowiednie treści.
- **Blokowanie użycia Miro AI** całkowicie wyłącza AI na dotkniętych tablicach.

**Rozwiązywanie problemów**

**Na niektórych tablicach wciąż pojawia się AI. Co powinienem sprawdzić?**

- Upewnij się, że klasyfikacja tablicy to taka, dla której włączono zabezpieczenie, oraz że kliknięto **Publikuj** po edycji zabezpieczeń.
- Jeśli korzystasz z automatycznej klasyfikacji, zweryfikuj, czy klasyfikacja tablicy została zaktualizowana na podstawie bieżącej zawartości.
- W trybach Ścisłym vs Domyślnym upewnij się, że Twoje oczekiwania są zgodne z wybranym trybem wdrożenia.

**Musimy ponownie włączyć AI dla wybranej części pracy.**

Dostosuj zabezpieczenie dla odpowiedniej klasyfikacji lub zmień klasyfikację tablic, które mają umożliwiać AI, a następnie opublikuj aktualizację.

## Przegląd pulpitów administratora

**Zakres i wskaźniki**

**Co obejmuje pulpit Przegląd?**

Tablice, użytkowników, zespoły, licencje i szablony, wraz z trendami historycznymi, tam gdzie to możliwe.

**Jak definiowane jest „Aktywne w tym okresie” dla tablic, użytkowników i zespołów?**

- **Tablice:** Unikalne tablice otwarte od początku wybranego okresu. Zawiera tablice później przeniesione do kosza.
- **Użytkownicy:** Unikalni użytkownicy, którzy otworzyli tablicę przynajmniej raz od początku okresu. Zawiera użytkowników, którzy zostali następnie dezaktywowani.
- **Zespoły:** Unikalne zespoły, w których przynajmniej jeden członek otworzył tablicę od początku okresu. Może zawierać zespoły później przeniesione do kosza.

**Czy sumy wykluczają elementy w koszu?**

Tak. Suma dla tablic i zespołów wyklucza elementy aktualnie znajdujące się w koszu. Historyczne liczby „aktywnych” mogą zawierać elementy, które później zostały przeniesione do kosza.

**Co pokazuje wykres Licencji?**

Łączna liczba przydziałów i historia dla pełnych, Free i bezpłatnych ograniczonych licencji, odzwierciedlające, ile licencji jest obecnie używanych.

**Co pokazuje "Szablony" dzisiaj?**

Najpopularniejsze szablony używane na tablicy. Inne źródła mogą być dodane w przyszłych wersjach.

**Zachowanie pod względem czasu i historii**

**Jak wyświetlane są wartości historyczne na wykresach Przeglądu?**

Widżety historyczne pokazują wartości z ostatniego dnia każdego okresu. Dostępna jest historia do roku wstecz lub tak daleko, jak istnieją dane.

**Świeżość danych i kontrole**

**Jak często odświeżane są dane w sekcji Przegląd i gdzie można je zobaczyć?**

Co najmniej raz na 24 godziny. Znacznik czasu „Ostatnia aktualizacja” jest dostępny w pulpicie.

**Jak zmienić zakres czasowy?**

Użyj selektora zakresu czasowego w prawym górnym rogu strony Analityki.

## Moderacja Miro AI

Dzięki moderacji Miro AI administratorzy firmy mogą dostosować poziomy filtrowania promptów, które mogą zawierać potencjalnie szkodliwy lub nieodpowiedni tekst. Możesz ustawić w całej organizacji poziom wrażliwości moderacji Miro AI, aby filtrować treści, w tym nienawiść, treści seksualne, przemoc i samookaleczenia. Pomaga to w dostosowaniu wykorzystania Miro AI do wymagań, zasad i tolerancji ryzyka Twojej organizacji. Więcej informacji znajdziesz w [dokumentacji moderacji Miro AI](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Cel i zakres**

**Czym jest moderacja AI w Miro?**

Moderacja AI umożliwia administratorom firmy ustawienie poziomu filtrowania (Ścisły, Domyślny lub Minimalny) w całej organizacji, który śledzi prompty mogące prowadzić do szkodliwych lub nieodpowiednich wyników (np. nienawiść, treści seksualne, przemoc, samookaleczenie).

**Kto może to skonfigurować i na jakich wersjach?**

Administratorzy firmy na Enterprise z Enterprise Guard mogą skonfigurować ustawienia w Ustawieniach organizacji.

**Czy działa, jeśli moja organizacja połączy własny LLM (np. bezpośrednią integrację dostawcy)?**

Jeśli zostanie podłączony niestandardowy LLM, wybór poziomu moderacji może być wyłączony dla tej integracji, a wcześniej wybrany poziom nie będzie miał zastosowania.

**Dostęp i wymagania wstępne**

**Kto może to aktywować i czego potrzebuję?**

Administratorzy firmy na Enterprise z dodatkiem Enterprise Guard mogą skonfigurować Moderację AI w ustawieniach organizacji.

**Jak to włączyć?**

Przejdź do Ustawienia → Miro AI → Moderacja, wybierz Ścisłe/Domyślne/Minimalne, a następnie kliknij **Zapisz zmiany**. Egzekwowanie jest natychmiastowe w całej organizacji.

**Poziomy i zachowanie**

**Co oznaczają poziomy?**

- **Ścisły:** Blokuje zawartość Domyślną + zawartość o niskim do średniego stopniu ryzyka (np. subtelne/zakodowane treści nienawistne, sugestywne treści seksualne, niegraficzna przemoc, wzmianki o samookaleczeniu bez szczegółów).
- **Domyślny (zalecany):** Blokuje treści o umiarkowanej do poważnej szkodliwości.
- **Minimalny:** Blokuje tylko treści o poważnej szkodliwości.

**Kiedy wprowadzone zmiany wchodzą w życie?**

Natychmiast dla całej organizacji.

**Czy zmiany są rejestrowane?**

Tak. Aktualizacje są zapisywane w ścieżce audytu Twojej organizacji.

**Konfiguracja i ustawienia**

**Gdzie mogę ustawić lub zaktualizować poziom moderacji?**

Przejdź do Ustawienia → Miro AI → Moderacja, wybierz Ścisłe/Domyślne/Minimalne, a następnie kliknij **Zapisz zmiany**.

**Jaki poziom startowy polecacie?**

Domyślna pasuje do większości organizacji; dostosuj na podstawie opinii z programu pilotażowego i tolerancji na ryzyko.

**Interakcje z innymi ustawieniami**

**Jak moderacja AI odnosi się do zabezpieczeń i ustawień promptów?**

- **Inteligentne zabezpieczenia:** Jeśli tablica jest objęta zabezpieczeniem "Blokuj korzystanie z Miro AI”, funkcja AI jest wyłączona niezależnie od poziomu moderacji.
- **Blokowanie promptów:** Działa razem z moderacją. Blokowanie promptów zatrzymuje wrażliwe polecenia podczas wysyłania; moderacja filtruje szkodliwe kategorie.
- **Szczegółowe ustawienia administratora:** Przełączniki funkcji ustalają, kto może uzyskać dostęp do funkcji AI, gdy AI jest dostępne.

**Rozwiązywanie problemów i najlepsze praktyki**

**Widzimy zbyt wiele fałszywych alarmów.**

Rozważ zmianę z surowego na domyślny (lub z domyślnego na minimalny) i opublikowanie przykładów akceptowalnego użycia. Jeśli po dopasowaniu ustawień problem nadal występuje, skontaktuj się z Twoim managerem ds. sukcesu klienta w Miro, aby zgłosić ten problem, a nasz zespół produktowy mógł to przeanalizować.

**Widzimy, że szkodliwe treści przechodzą niezauważone.**

Zmień na domyślny lub surowy i zapewnij wewnętrzne wytyczne. Ponownie oceń po aktualizacjach zasady/regulacji. Jeśli problem będzie się utrzymywał po tych zmianach, skontaktuj się z Twoim managerem ds. sukcesu klienta w Miro, aby zgłosić ten problem, a nasz zespół produktowy mógł to przeanalizować.

## Blokowanie promptów

Blokowanie promptów pozwala administratorom treści wrażliwych uniemożliwić użytkownikom przesyłanie promptów AI zawierających informacje wrażliwe, pomagając utrzymać dane wrażliwe z dala od Miro AI w całej organizacji. Miro skanuje tekst, który użytkownik wpisuje w polu promptu oraz wszelkie treści tekstowe dodawane z tablicy. Jeśli te treści pasują do wybranych etykiet poufności lub wzorców kodu źródłowego skonfigurowanych w blokowaniu promptów, Miro blokuje przesłanie promptu.  Więcej informacji znajdziesz w [dokumentacji dotyczącą blokowania promptów](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md).

**Cel i zakres**

**Czym jest Prompt Blocking?**

Prompt Blocking zapobiega przesyłaniu przez użytkowników promptów AI, które zawierają informacje wrażliwe. Miro skanuje tekst wpisywany przez użytkownika w polu promptu oraz wszelkie treści tekstowe dodawane z tablicy; jeśli treść ta odpowiada wybranym etykietom poufności lub wzorom kodu źródłowego, przesyłanie zostaje zablokowane i wyświetlana jest wiadomość o zasadach. W tej chwili obsługujemy jedynie treści tekstowe.

**Czym różni się Prompt Blocking od skanowania tablicy?**

Skanowanie tablicy wyszukuje treści wrażliwe na tablicach i może automatycznie klasyfikować tablice; Prompt Blocking sprawdza, co użytkownicy próbują wysłać do Miro AI w momencie przesyłania.

**Jakie etykiety poufności są obsługiwane?**

Użyj kategorii na poziomie organizacji wymienionych w referencji etykiet poufności i infotypów.

**Co to jest skanowanie kodu?**

Skanowanie kodu blokuje prompty zawierające rozpoznawalny kod źródłowy; z założenia wymaga minimalnego bloku kodu (np. 5+ linii), aby zostać aktywowane. Można je włączyć lub wyłączyć w konfiguracji blokowania promptów.

**Czy skanowane są treści nietekstowe (np. obrazy)?**

Nie. W tej chwili blokowanie promptów obsługuje tylko treści tekstowe.

**Dostęp i wymagania wstępne**

**Kto może aktywować to i czego potrzebuję?**

Administratorzy treści wrażliwych na Enterprise z dodatkiem Enterprise Guard mogą to aktywować w Ustawieniach → Enterprise Guard → Wykrywanie danych → Konfiguracja.

**Jak to włączyć?**

Otwórz Prompt Blocking → Aktywuj, wybierz Zaznacz wszystko lub konkretne kategorie etykiet, opcjonalnie włącz skanowanie kodu, następnie Aktywuj. Egzekwowanie jest natychmiastowe na poziomie całej organizacji.

**Zarządzanie i zmiany**

**Jak mogę później dostosować etykiety lub skanowanie kodu?**

Przejdź do Ustawienia → Enterprise Guard → Wykrywanie danych → Konfiguracja → Blokowanie promptów → Zarządzaj,

- **Etykiety:** Zaznacz pole wyboru *Wybierz wszystko*, aby zaznaczyć wszystkie kategorie, lub zaznacz pola wyboru konkretnej kategorii etykiet.
- **Skanowanie kodu:** Włącz skanowanie kodu, aby blokować prompty zawierające kod źródłowy (minimum 5 linijek). Aby uzyskać więcej informacji, zobacz Skanowanie kodu.

Zmiany wchodzą w życie natychmiast.

**Co dzieje się z promptami po zmianie ustawień?**

Nowo odblokowane elementy będą przepuszczane. Elementy, które nadal pasują do zablokowanych wzorców, pozostaną zablokowane.

**Doświadczenia użytkownika**

**Co widzi użytkownik, gdy prompt jest blokowany?**

Pojawia się komunikat o zasadach w miejscu, gdzie wprowadzili prompt, a prośba nie jest wysyłana do żadnego LLM.

**Czy treści nietekstowe (np. obrazy) są skanowane?**

Nie. W tej chwili blokowanie promptów obsługuje tylko treści tekstowe.

**Interakcje z innymi zabezpieczeniami**

**Jak działają blokady promptów w połączeniu z zabezpieczeniami i moderacją?**

- **Inteligentne zabezpieczenia:** Jeśli „Blokada użycia Miro AI” jest aktywna, AI zostaje wyłączone; Blokady promptów nie zadziałają, ponieważ nie można ich przesłać.
- **Moderacja AI:** Oba mogą się stosować, gdy AI jest dostępne—Blokady promptów zatrzymują dane wrażliwe; Moderacja filtruje szkodliwe kategorie.
- **Granularne kontrole administratora:** Dostęp do funkcji dotyczy tylko wtedy, gdy AI jest dostępne i prompt nie jest zablokowany.

##

## Enterprise Guard i Microsoft Purview DSPM dla integracji AI

Dla organizacji korzystających z Microsoft Entra ID (wcześniej Azure AD) jako dostawcy tożsamości, Enterprise Guard bezpiecznie przesyła prompty AI i odpowiedzi do Microsoft Purview Data Security Posture Management (DSPM) dla AI. Zespoły ds. bezpieczeństwa i zgodności mogą dzięki temu monitorować, audytować i kontrolować wykorzystanie generatywnej AI z jednego zaufanego źródła, co redukuje nakład operacyjny, minimalizuje ryzyko takie jak wyciek danych lub niewłaściwe użycie, oraz wzmacnia zarządzanie AI na poziomie przedsiębiorstwa oferowane przez Miro. Więcej informacji znajdziesz w [dokumentacji dotyczącej integracji Enterprise Guard i Microsoft Purview DSPM dla AI](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).

**Cel i zakres**

**Czym jest integracja Miro z Microsoft Purview DSPM dla AI?**

Integracja, która przesyła prompty i odpowiedzi Miro AI do DSPM Microsoft Purview dla AI, dzięki czemu zespoły ds. bezpieczeństwa i zgodności mogą monitorować, audytować i zarządzać działaniami AI w jednym miejscu.

**Kto może korzystać z tej integracji?**

Wersje Enterprise z Enterprise Guard, zarządzane przez administratorów firmowych z dostępem do integracji Enterprise. Twoja organizacja Miro musi używać Microsoft Entra ID do SSO. Wymagana jest licencja Microsoft Purview.

**Jakie są korzyści?**

Centralna widoczność użycia Miro AI w centrum AI Purview, możliwość audytu promptów i odpowiedzi oraz zgodność z istniejącymi zasadami zarządzania w Purview.

**Jakie działania Miro AI są dziś uwzględnione?**

Obecnie przesyłane są tekstowe prompty i odpowiedzi w ramach funkcji Miro AI. Treści graficzne nie są przesyłane.

**Czy działania wszystkich użytkowników są rejestrowane?**

Przesyłane są jedynie działania użytkowników, którzy logują się do Miro za pośrednictwem skonfigurowanego dzierżawcy Microsoft Entra do Purview.

**Jak długo trwa, zanim aktywność pojawi się w Purview?**

Zazwyczaj 10 do 30 minut po działaniu AI w Miro. Sprawdź w Microsoft Purview → DSPM dla AI → Eksplorator działań lub sprawdź dzienniki audytu.

**Czy są jakieś istotne ograniczenia?**

Obecnie można skonfigurować tylko jednego dzierżawcę Entra naraz. W środowiskach z wieloma dostawcami tożsamości lub dzierżawcami, rejestrowani są tylko użytkownicy uwierzytelniający się za pomocą skonfigurowanego dzierżawcy. Obrazy nie są wliczone.

**Konfiguracja i ustawienia**

**Jak włączyć integrację?**

w Miro: Ustawienia Enterprise → Integracje Enterprise → włączyć Microsoft Purview DSPM dla AI → wprowadzić ID dzierżawy Entra → Połącz → zalogować się na konto, które może przyznać zgodę administracyjną na poziomie dzierżawy → zaakceptować aplikację zarządzania Miro AI → potwierdzić Połączono w Miro.

**Jakie są wymagania wstępne?**

- **Miro:** Abonament Enterprise z Enterprise Guard, rola administratora firmy, skonfigurowane Entra ID dla SSO. Aby włączyć tę funkcję, skontaktuj się ze swoim managerem ds. sukcesu klienta.
- **Microsoft:** Licencja Microsoft Purview, ID dzierżawy Entra używane do SSO w Miro oraz rola Entra, która może przyznać zgodę administracyjną na poziomie dzierżawy.

**Jak mogę zweryfikować poprawność konfiguracji?**

Wykonaj proste działanie w Miro AI, poczekaj 10–30 minut, a następnie sprawdź Microsoft Purview → DSPM for AI → Eksplorator aktywności dla nowych wpisów z Miro.

**Jak mogę odłączyć lub zmienić dzierżawy?**

W Miro: integracje Enterprise → Microsoft Purview for AI → Odłącz. Aby zmienić dzierżawy, najpierw odłącz, a następnie ponownie połącz używając nowego ID dzierżawy.

**Użycie i zarządzanie**

**Gdzie mogę zobaczyć przesłane dane w Purview?**

Microsoft Purview → DSPM dla AI → Eksplorator Działań. Możesz również sprawdzić szczegóły w dziennikach audytu.

**Czy mogę eksportować lub archiwizować dzienniki aktywności AI?**

Użyj narzędzi eksportu Microsoft Purview. Miro przesyła aktywność do Twojego konta Microsoft, gdzie obowiązują Twoje zasady.

**Czy mogę stosować zasady Purview do danych Miro AI?**

Tak. Po zaimportowaniu dane podlegają modelowi zarządzania Purview w Twojej organizacji.

**A co z odpowiedzialnością za prywatność i bezpieczeństwo?**

Miro przesyła prompty i odpowiedzi do Twojego konta Microsoft. Zarządzanie i kontrola dostępu odbywa się w Purview, w Twoim środowisku.

**Rozwiązywanie problemów i pomoc**

**Krok zgody się nie powiódł lub się powtarza. Co powinienem sprawdzić?**

Upewnij się, że konto używane do połączenia może udzielić globalnej zgody administratora w Entra, lub zaangażuj globalnego administratora Microsoftu.

**Nie widzę żadnej aktywności w Purview. Co teraz?**

Potwierdź, że Enterprise Guard jest włączony i masz dostęp do integracji Enterprise. Zweryfikuj, czy identyfikator tenanta dokładnie odpowiada Twojemu tenantowi pojedynczego logowania Miro. Upewnij się, że użytkownik, uwierzytelniający się poprzez ten tenant, wykonał jakąś testową akcję AI. Sprawdź licencję Purview i filtry. Poświęć do 30 minut na załadowanie.

**Używamy wielu dostawców tożsamości lub tenantów. Czy wszyscy użytkownicy będą logowani?**

Nie. Tylko działania użytkowników logujących się przez pojedynczy skonfigurowany tenant Entra są przekazywane.

**Kto za co odpowiada?**

Skontaktuj się z pomocą Miro w sprawie konfiguracji lub połączenia w Miro. W przypadku problemów wewnątrz Microsoft Purview skontaktuj się z pomocą Microsoftu.
