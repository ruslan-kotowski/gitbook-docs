---
title: "Zdolno\u015Bci AI i FAQ"
article_id: 30943405198994
translation_id: 30943405198994
locale: pl-pl
sidebar_position: 0
created_at: '2025-11-10T14:17:30Z'
updated_at: '2026-03-11T21:32:10Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-granular-admin-settings
---

Na Canvas 25 ogłosiliśmy przestrzeń roboczą dla innowacji z AI z wizualnymi przepływami pracy AI i asystentami AI dostępnymi na planszy. Oprócz funkcji dla użytkowników końcowych, wprowadzamy nowe możliwości administracyjne, które zapewniają większą widoczność, inteligentniejsze ustawienia i płynne sposoby na odblokowanie najnowszych narzędzi AI Miro dla Twoich zespołów.

Użyj tej strony, aby zgłębić możliwości AI Trust dostępne z dodatkiem Enterprise Guard. Każda sekcja rozpoczyna się krótkim przeglądem, po którym następują rozwijane często zadawane pytania obejmujące różne aspekty każdej funkcji.

- Szczegółowe ustawienia administracyjne Miro AI: ustaw dostęp do funkcji na poziomie funkcji (Wszyscy/Nikt/Wybrane zespoły) w każdej kategorii funkcji.
- [Zablokuj użycie Miro AI za pomocą Inteligentnych Zabezpieczeń](#h_block_ai_with_guardrails): użyj Inteligentnych Zabezpieczeń, aby zablokować wszystkie interakcje oparte na AI w Miro, gdy musisz chronić dane wrażliwe lub zastrzeżone.
- [Przegląd analityki administracyjnej](#h_admin_analytics_overview): śledź tablice, użytkowników, zespoły, licencje i szablony z analizą historycznych trendów i codziennym odświeżaniem.
- Moderacja AI (dostępna także w wersji Enterprise): ustaw poziomy filtrowania w całej organizacji (Rygorystyczny, Domyślny, Minimalny), aby przefiltrować prompty, które mogą prowadzić do szkodliwych lub nieodpowiednich wyników.
- Blokowanie promptów: blokuj prompty zawierające dane wrażliwe lub kod źródłowy w momencie ich przesyłania; zamiast przesyłać do LLM, wyświetl wiadomość z zasadą.
- Enterprise Guard i Microsoft Purview DSPM do integracji z AI: przekierowuj prompty i odpowiedzi do Purview w celu centralnego monitoringu, audytu i zarządzania.

## Szczegółowe ustawienia administracyjne Miro AI dla dodatku Enterprise Guard

Ustawienia administratora Miro AI umożliwiają administratorom firmy Enterprise decydowanie, które funkcje AI są dostępne w ich organizacji oraz zarządzanie, kto może z nich korzystać. Administratorzy mogą również wyświetlać modele napędzające każdą funkcję AI. Z dodatkiem Enterprise Guard, ustawienia Miro AI rozszerzają się do poziomu funkcji w ramach każdej kategorii, co pomaga priorytetyzować funkcje w oparciu o potrzeby organizacyjne i wymagania dotyczące bezpieczeństwa. Oprócz pełnej kategorii funkcji Miro AI, administratorzy mogą również włączać, ograniczać lub usuwać konkretne funkcje Miro AI. Na przykład w kategorii obrazy można włączyć funkcję tworzenia obrazów z AI i wyłączyć usuwanie tła. Użyj tych ustawień, aby bezpiecznie wprowadzać AI i spełniać wymagania dotyczące bezpieczeństwa, jednocześnie promując przyjęcie możliwości AI.  Aby uzyskać więcej informacji, zobacz [dokumentację szczegółowych ustawień administratora Miro AI](../../enterprise-guard/ai-trust/02-miro-ai-granular-admin-controls.md).

**Cel i zakres**

**Co to jest szczegółowe ustawienie Miro AI?**

Z dodatkiem Enterprise Guard, administratorzy firmy mogą włączyć, ograniczyć lub usunąć dostęp do poszczególnych funkcji AI w każdej kategorii możliwości. Pozwala to na precyzyjne ustalenie, z których funkcji mogą korzystać zespoły.

**Dlaczego warto używać szczegółowych ustawień?**

Aby zrównoważyć wdrożenie z bezpieczeństwem. Na przykład w przypadku obrazów można zezwolić na tworzenie obrazów, jednocześnie wyłączając opcję usuwania tła.

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

## Blokuj użycie Miro AI z wykorzystaniem zabezpieczeń

Użyj zabezpieczeń, aby zablokować wszystkie interakcje z obsługą AI w Miro, gdy trzeba chronić wrażliwe lub tajne dane. Gdy to zabezpieczenie ma zastosowanie, wszystkie narzędzia Miro AI są wyłączane na dotkniętych tablicach, podczas gdy współpraca bez AI pozostaje dostępna. Aby uzyskać informacje wstępne i instrukcje konfiguracji, zobacz przegląd zabezpieczeń i definiowanie zabezpieczeń.

**Cel i zakres**

**Co oznacza „Zablokowanie użycia Miro AI”?**

Wyłącza wszystkie funkcje Miro AI (na przykład generowanie tekstu, generowanie/rozpoznawanie obrazu, inteligentne sugestie) wszędzie tam, gdzie ma zastosowanie to ograniczenie, zapobiegając wszelkim interakcjom z treściami wrażliwymi lub zastrzeżonymi.

**Co pozostaje dostępne dla użytkowników?**

Użytkownicy mogą kontynuować regularną, niewspomaganą AI współpracę. Istniejące treści wygenerowane przez AI pozostają na tablicach i mogą być przeglądane, przenoszone lub ręcznie edytowane – ale użytkownicy nie mogą używać Miro AI do ich modyfikowania lub regenerowania.

**Dostęp i wymagania wstępne**

**Kto może konfigurować te zabezpieczenia i gdzie?**

Administratorzy treści wrażliwych konfigurują zabezpieczenia w *Enterprise Guard* pod Klasyfikacja danych → Zabezpieczenia. (Administratorzy firmy przypisują rolę administratora treści wrażliwych.)

**Co jest potrzebne przed przypisaniem tych zabezpieczeń?**

Zdefiniuj swoje poziomy klasyfikacji i (opcjonalnie) automatyczną klasyfikację, aby można było stosować zabezpieczenia na podstawie klasyfikacji (na przykład WEWNĘTRZNA, POUFNA).

**Zachowanie i wpływ**

**Kogo dotyczy zastosowanie tego zabezpieczenia?**

Wszyscy, w tym właściciele tablic i współwłaściciele, nie mogą uzyskać dostępu ani wywołać Miro AI na objętych tablicach.

**Czy usuwa istniejącą treść AI?**

Nie. Zapobiega dalszym interakcjom z AI; istniejąca zawartość AI pozostaje dostępna do wyświetlania i ręcznej edycji.

**Kiedy wprowadzone zmiany wchodzą w życie?**

Po opublikowaniu aktualizacji zabezpieczenia wymuszenie jest natychmiastowe na wszystkich objętych tablicach.

**Konfiguracja i ustawienia**

**Jak włączyć „Blokowanie użycia Miro AI” dla klasyfikacji?**

1. Przejdź do *Enterprise Guard* → Klasyfikacja danych → **Ograniczenia**.
2. Kliknij ikonę **Edytuj** dla wybranego poziomu klasyfikacji (na przykład POUFNE).
3. Zaznacz pole wyboru **Blokowane użycie Miro AI** i kliknij **Gotowe**.
4. Kliknij **Dalej**, aby przeglądnąć wpływ, a następnie **Publikuj**, aby zastosować.

**Czy powinienem używać trybu domyślnego czy rygorystycznego?**

W trybie domyślnym zabezpieczenia nie zastępują istniejących ustawień udostępniania. W trybie ścisłym zabezpieczenia zastępują aktywne udostępnianie i stosują najściślejsze kontrole. Wybierz w zależności od potrzeb związanych z zarządzaniem zmianami.

**Doświadczenie użytkownika**

**Co użytkownicy zobaczą na tablicach, na których AI jest zablokowana?**

Punkty wejścia AI w Miro będą wyglądały na wyłączone lub niedostępne, a użytkownicy nie będą mogli używać narzędzi AI z planszy ani menu na tych tablicach.

**Czy użytkownicy mogą prosić o wyjątki na pojedynczej tablicy?**

Nie. Zasada jest egzekwowana przez politykę klasyfikacji. Zmień klasyfikację tablicy (lub politykę dla tego poziomu), aby zmienić egzekwowanie.

**Interakcje z innymi kontrolami**

**W jaki sposób jest to związane ze szczegółowymi ustawieniami administracyjnymi Miro AI?**

Szczegółowe kontrole zarządzają tym, kto może korzystać z poszczególnych funkcji AI. Ochraniacz to warstwa zasad: gdy jest aktywny, blokuje AI bez względu na przełączniki funkcji.

**Czym to się różni od blokowania promptów lub moderacji AI?**

- **Blokowanie promptów** zatrzymuje wrażliwe polecenia podczas wysyłania; AI pozostaje dostępne dla niewrażliwych poleceń.
- **Moderacja AI** filtruje szkodliwe lub nieodpowiednie treści.
- **Zablokowanie użycia Miro AI** całkowicie wyłącza AI na dotkniętych tablicach.

**Rozwiązywanie problemów**

**AI nadal pojawia się na niektórych tablicach. Co powinienem sprawdzić?**

- Upewnij się, że klasyfikacja tablicy jest taka, gdzie zabezpieczenie jest włączone, i że kliknąłeś **Opublikuj** po edycji zabezpieczeń.
- Jeśli używasz automatycznej klasyfikacji, sprawdź, czy klasyfikacja tablicy została zaktualizowana na podstawie bieżącej zawartości.
- W trybach Ścisły vs Domyślny upewnij się, że Twoje oczekiwania odpowiadają wybranemu trybowi wdrożenia.

**Musimy ponownie włączyć AI dla części pracy.**

Dostosuj zabezpieczenie dla odpowiedniej klasyfikacji lub przeklasyfikuj tablice, które powinny zezwalać na AI, a następnie opublikuj aktualizację.

## Przegląd pulpitu Administratora Analityki

**Zakres i wskaźniki**

**Co obejmuje pulpit Przegląd?**

Tablice, Użytkownicy, Zespoły, Licencje i Szablony, z historycznymi trendami, gdzie to możliwe.

**Jak definiowane jest „Aktywne w tym okresie” dla Tablic, Użytkowników i Zespołów?**

- **Tablice:** Unikalne tablice otwarte od początku wybranego okresu. Zawiera tablice później przeniesione do kosza.
- **Użytkownicy:** Unikalni użytkownicy, którzy otworzyli tablicę przynajmniej raz od początku okresu. Zawiera użytkowników, którzy są teraz dezaktywowani.
- **Zespoły:** Unikalne zespoły z co najmniej jednym członkiem, który otworzył tablicę od początku okresu. Może zawierać zespoły później przeniesione do kosza.

**Czy sumy wykluczają elementy znajdujące się w koszu?**

Tak. Sumy dla tablic i zespołów wykluczają elementy, które są obecnie w koszu. Historyczne dane „aktywne” mogą zawierać elementy, które były później przeniesione do kosza.

**Co pokazuje wykres Licencji?**

Łączna liczba przydzielonych i używanych na przestrzeni czasu licencji Pełnych, Darmowych i bezpłatnych oraz ograniczonych, odzwierciedlająca liczbę obecnie wykorzystywanych licencji.

**Co pokazują szablony dziś?**

Najbardziej popularne szablony używane z poziomu tablicy. Inne źródła mogą zostać dodane w przyszłych wydaniach.

**Zachowanie czasu i historii**

**Jak są wyświetlane wartości historyczne na wykresach Przegląd?**

Widżety historyczne pokazują wartości z ostatniego dnia każdego okresu. Dostępna jest historia do jednego roku wstecz albo do punktu, w którym dane istnieją.

**Aktualność danych i sterowanie**

**Jak często dane w Przeglądzie są odświeżane i gdzie mogę je zobaczyć?**

Co najmniej raz na 24 godziny. Znak czasu „Ostatnia aktualizacja” jest dostępny na pulpicie.

**Jak zmienić zakres czasowy?**

Użyj selektora zakresu czasowego w prawym górnym rogu strony Analityka.

## Moderacja przez Miro AI

Dzięki moderacji Miro AI administratorzy firmy mogą dostosować poziomy filtrowania promptów, które mogą zawierać potencjalnie szkodliwy lub nieodpowiedni tekst. Możesz ustawić w całej organizacji poziom wrażliwości moderacji Miro AI, aby filtrować treści, w tym nienawiść, treści seksualne, przemoc i samookaleczenia. Pomaga to w dostosowaniu wykorzystania Miro AI do wymagań, zasad i tolerancji ryzyka Twojej organizacji. Aby uzyskać więcej informacji, zapoznaj się z [dokumentacją moderacji Miro AI](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Cel i zakres**

**Czym jest moderacja AI w Miro?**

Moderacja AI pozwala administratorom firmy ustawić poziom filtrowania dla całej organizacji (Ścisły, Domyślny lub Minimalny), który filtruje prompty mogące prowadzić do szkodliwych lub nieodpowiednich rezultatów (np. nienawiść, treści seksualne, przemoc, samookaleczenie).

**Kto może to skonfigurować i na jakich abonamentach?**

Administratorzy firmy na planie Enterprise z dodatkiem Enterprise Guard mogą skonfigurować ustawienia w ustawieniach organizacji.

**Czy działa, jeśli moja organizacja połączy swój własny LLM (np. bezpośrednią integrację dostawcy)?**

Jeśli zostanie podłączony niestandardowy LLM, wybór poziomu moderacji może być wyłączony dla tej integracji, a wcześniej wybrany poziom nie będzie miał zastosowania.

**Dostęp i wymagania wstępne**

**Kto może to aktywować i czego potrzebuję?**

Administratorzy firmy na wersji Enterprise z dodatkiem Enterprise Guard mogą skonfigurować Moderację AI w ustawieniach organizacji.

**Jak to włączyć?**

Przejdź do Ustawienia → Miro AI → Moderacja, wybierz Ścisłe/Domyślne/Minimalne, a następnie kliknij **Zapisz zmiany**. Egzekwowanie odbywa się natychmiast w całej organizacji.

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

- **Inteligentne zabezpieczenia:** Jeśli tablica jest objęta zabezpieczeniem „Blokuj korzystanie z Miro AI”, funkcja AI jest wyłączona niezależnie od poziomu moderacji.
- **Blokowanie promptów:** Działa wraz z moderacją. Blokowanie promptów zatrzymuje wrażliwe polecenia podczas wysyłania; moderacja filtruje szkodliwe kategorie.
- **Szczegółowe ustawienia administratora:** Przełączniki funkcji ustalają, kto może uzyskać dostęp do funkcji AI, gdy AI jest dostępne.

**Rozwiązywanie problemów i najlepsze praktyki**

**Widzimy zbyt wiele fałszywych alarmów.**

Rozważ zmianę z Ścisły → Domyślny (lub Domyślny → Minimalny) i opublikowanie przykładów akceptowalnego użycia. Jeśli po dopasowaniu ustawień problem nadal występuje, skontaktuj się z Twoim managerem ds. sukcesu klienta w Miro, aby zgłosić ten problem, a nasz zespół produktowy mógł to przeanalizować.

**Widzimy, że szkodliwe treści przechodzą niezauważone.**

Zmień na Domyślny lub Ścisły i zapewnij wewnętrzne wytyczne. Ponownie oceń po aktualizacjach zasad/regulacji. Jeśli problem będzie się utrzymywał po tych zmianach, skontaktuj się z Twoim managerem ds. sukcesu klienta w Miro, aby zgłosić ten problem, a nasz zespół produktowy mógł to przeanalizować.

## Blokowanie promptów

Blokowanie promptów pozwala administratorom treści wrażliwych uniemożliwić użytkownikom przesyłanie promptów AI zawierających informacje wrażliwe, pomagając utrzymać dane wrażliwe z dala od Miro AI w całej organizacji. Miro skanuje tekst, który użytkownik wpisuje w polu promptu oraz wszelkie treści tekstowe dodawane z tablicy. Jeśli te treści pasują do wybranych etykiet poufności lub wzorców kodu źródłowego skonfigurowanych w blokowaniu promptów, Miro blokuje przesłanie promptu.  Aby uzyskać więcej informacji, zobacz [dokumentację dotyczącą blokowania promptów](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md).

**Cel i zakres**

**Czym jest Prompt Blocking?**

Prompt Blocking zapobiega przesyłaniu przez użytkowników promptów AI, które zawierają informacje wrażliwe. Miro skanuje tekst wpisywany przez użytkownika w polu promptu oraz wszelkie treści tekstowe dodawane z tablicy; jeśli treść ta odpowiada wybranym etykietom poufności lub wzorom kodu źródłowego, przesyłanie zostaje zablokowane i wyświetlana jest wiadomość o zasadach. Aktualnie obsługujemy tylko treści tekstowe.

**Czym różni się Prompt Blocking od skanowania tablicy?**

Skanowanie tablicy wyszukuje treści wrażliwe na tablicach i może automatycznie klasyfikować tablice; Prompt Blocking sprawdza, co użytkownicy próbują wysłać do Miro AI w momencie przesyłania.

**Jakie etykiety poufności są obsługiwane?**

Użyj kategorii na poziomie organizacji wymienionych w referencji etykiet poufności i infotypów.

**Co to jest skanowanie kodu?**

Skanowanie kodu blokuje prompty zawierające rozpoznawalny kod źródłowy; z założenia wymaga minimalnego bloku kodu (np. 5+ linii), aby zostać aktywowane. Można je włączyć lub wyłączyć w konfiguracji blokowania promptów.

**Czy skanowane są treści nietekstowe (np. obrazy)?**

Nie. Na ten moment, blokowanie promptów obsługuje tylko treści tekstowe.

**Dostęp i wymagania wstępne**

**Kto może to aktywować i czego potrzebuję?**

Administratorzy treści wrażliwych na Enterprise z dodatkiem Enterprise Guard mogą to aktywować w Ustawieniach → Enterprise Guard → Wykrywanie danych → Konfiguracja.

**Jak to włączyć?**

Otwórz Prompt blocking → Aktywuj, wybierz Zaznacz wszystko lub konkretne kategorie etykiet, opcjonalnie włącz skanowanie kodu, następnie Aktywuj. Egzekwowanie jest natychmiastowe w całej organizacji.

**Zarządzanie i zmiany**

**Jak mogę później dostosować etykiety lub skanowanie kodu?**

Przejdź do Ustawienia → Enterprise Guard → Wykrywanie danych → Konfiguracja → Blokowanie promptów → Zarządzaj,

- **Etykiety:** Zaznacz pole wyboru *Wybierz wszystko*, aby zaznaczyć wszystkie kategorie, lub zaznacz pola wyboru konkretnej kategorii etykiet.
- **Skanowanie kodu:** Włącz skanowanie kodu, aby blokować prompty zawierające kod źródłowy (minimum 5 linijek). Więcej informacji znajdziesz w sekcji Skanowanie kodu.

Zmiany wchodzą w życie natychmiast.

**Co dzieje się z promptami po zmianie ustawień?**

Nowo odblokowane elementy będą przepuszczane. Elementy, które nadal pasują do zablokowanych wzorców, pozostaną zablokowane.

**Doświadczenia użytkowników**

**Co widzi użytkownik, gdy prompt jest blokowany?**

Pojawia się komunikat o zasadach w miejscu, gdzie wprowadzili prompt, a prośba nie jest wysyłana do żadnego LLM.

**Czy treści nietekstowe (np. obrazy) są skanowane?**

Nie. W chwili obecnej, blokowanie promptów obsługuje tylko treści tekstowe.

**Interakcje z innymi kontrolami**

**Jak działają blokady promptów w połączeniu z zabezpieczeniami i moderacją?**

- **Inteligentne zabezpieczenia:** Jeśli „Blokada użycia Miro AI” jest aktywna, AI zostaje wyłączone; Blokady promptów nie zadziałają, ponieważ nie można ich przesłać.
- **Moderacja AI:** Oba mogą się stosować, gdy AI jest dostępne—Blokady promptów zatrzymują dane wrażliwe; Moderacja filtruje szkodliwe kategorie.
- **Granularne kontrolki administratora:** Dostęp do funkcji dotyczy tylko wtedy, gdy AI jest dostępne i prompt nie jest zablokowany.

##

## Enterprise Guard i Microsoft Purview DSPM dla integracji AI

Dla organizacji korzystających z Microsoft Entra ID (wcześniej Azure AD) jako dostawcy tożsamości, Enterprise Guard bezpiecznie przekazuje prompty AI i odpowiedzi do Microsoft Purview Data Security Posture Management (DSPM) dla AI. Zespoły ds. bezpieczeństwa i zgodności mogą dzięki temu monitorować, audytować i kontrolować wykorzystanie generatywnej AI z jednego zaufanego źródła, co redukuje nakład operacyjny, minimalizuje ryzyko takie jak wyciek danych lub niewłaściwe użycie, oraz wzmacnia zarządzanie AI na poziomie przedsiębiorstwa oferowane przez Miro. Po więcej informacji zobacz [dokumentację Enterprise Guard i Microsoft Purview DSPM dla integracji AI](../integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).

**Cel i zakres**

**Czym jest integracja Miro z Microsoft Purview DSPM dla AI?**

To integracja, która przesyła prompty i odpowiedzi Miro AI do DSPM Microsoft Purview dla AI, dzięki czemu zespoły ds. bezpieczeństwa i zgodności mogą monitorować, audytować i zarządzać działaniami AI w jednym miejscu.

**Kto może korzystać z tej integracji?**

Wersje Enterprise z Enterprise Guard, zarządzane przez administratorów firmowych z dostępem do integracji Enterprise. Twoja organizacja Miro musi używać Microsoft Entra ID do SSO. Wymagana jest licencja Microsoft Purview.

**Jakie są korzyści?**

Centralna widoczność użycia Miro AI w centrum AI Purview, możliwość audytu promptów i odpowiedzi oraz zgodność z istniejącymi zasadami zarządzania w Purview.

**Jakie działania Miro AI są dziś uwzględnione?**

Obecnie przesyłane są tekstowe prompty i odpowiedzi w funkcjach Miro AI. Treści graficzne nie są przesyłane.

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

- **Miro:** Abonament Enterprise z Enterprise Guard, rola administratora firmy, skonfigurowane ID Entra dla pojedynczego logowania (SSO). Aby włączyć tę funkcję, skontaktuj się ze swoim managerem ds. sukcesu klienta.
- **Microsoft:** Licencja Microsoft Purview, ID dzierżawy Entra używany do SSO w Miro oraz rola Entra, która może przyznać zgodę administracyjną na poziomie dzierżawy.

**Jak mogę zweryfikować poprawność konfiguracji?**

Wykonaj proste działanie w Miro AI, poczekaj 10–30 minut, a następnie sprawdź Microsoft Purview → DSPM for AI → Eksplorator aktywności dla nowych wpisów z Miro.

**Jak mogę odłączyć lub zmienić dzierżawy?**

W Miro: integracje Enterprise → Microsoft Purview for AI → Odłącz. Aby zmienić dzierżawy, najpierw odłącz, a następnie ponownie połącz używając nowego ID dzierżawy.

**Użycie i zarządzanie**

**Gdzie mogę zobaczyć przesłane dane w Purview?**

Microsoft Purview → DSPM dla AI → Eksplorator działań. Możesz również sprawdzić szczegóły w dziennikach audytu.

**Czy mogę eksportować lub archiwizować dzienniki aktywności AI?**

Korzystaj z narzędzi eksportu Microsoft Purview. Miro przesyła aktywność do Twojego konta Microsoft, gdzie obowiązują Twoje zasady.

**Czy mogę stosować zasady Purview do danych Miro AI?**

Tak. Po ich zaimportowaniu dane podlegają modelowi zarządzania w Purview w Twojej organizacji.

**A co z odpowiedzialnością za prywatność i bezpieczeństwo?**

Miro przesyła prośby i odpowiedzi do Twojego konta Microsoft. Zarządzanie i kontrola dostępu odbywa się w Purview, w Twoim środowisku.

**Rozwiązywanie problemów i pomoc**

**Krok zgody się nie powiódł lub się powtarza. Co powinienem sprawdzić?**

Upewnij się, że konto używane do połączenia może udzielić globalnej zgody administratora w Entra lub zaangażuj globalnego administratora Microsoftu.

**Nie widzę żadnej aktywności w Purview. Co teraz?**

Potwierdź, że Enterprise Guard jest włączony oraz masz dostęp do integracji Enterprise. Zweryfikuj, czy identyfikator najemcy dokładnie odpowiada Twojemu tenantowi SSO w Miro. Upewnij się, że użytkownik uwierzytelniający się poprzez ten tenant wykonał jakąś testową akcję AI. Sprawdź licencję Purview i filtry. Poświęć do 30 minut na załadowanie.

**Używamy wielu dostawców tożsamości lub tenantów. Czy wszyscy użytkownicy będą zalogowani?**

Nie. Tylko działania użytkowników logujących się przez pojedynczy skonfigurowany tenant Entra są przekazywane.

**Kto za co odpowiada?**

Skontaktuj się z pomocą Miro w sprawie konfiguracji lub połączenia w Miro. W przypadku problemów wewnątrz Microsoft Purview skontaktuj się z pomocą Microsoftu.
