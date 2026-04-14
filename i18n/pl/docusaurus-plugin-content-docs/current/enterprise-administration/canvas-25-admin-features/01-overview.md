---
title: "Przegl\u0105d"
article_id: 30969987585938
translation_id: 30969987585938
locale: pl-pl
sidebar_position: 1
created_at: '2025-11-11T12:42:45Z'
updated_at: '2026-01-12T16:04:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Na Canvas 25 ogłosiliśmy przestrzeń roboczą dla innowacji z AI z wizualnymi przepływami pracy AI i asystentami AI dostępnymi na planszy. Oprócz funkcji dla użytkowników końcowych, wprowadzamy nowe możliwości administracyjne, które zapewniają większą widoczność, inteligentniejsze ustawienia i płynne sposoby na odblokowanie najnowszych narzędzi AI Miro dla Twoich zespołów.

Użyj tej strony, aby zgłębić możliwości administracyjne AI dostępne dla administratorów na poziomie Enterprise. Każda sekcja rozpoczyna się krótkim przeglądem, po którym następują rozwijane często zadawane pytania obejmujące różne aspekty każdej zdolności.

- [Ustawienia administratora Miro AI:](01-overview.md) decyduj, które funkcje AI są dostępne w Twojej organizacji i zarządzaj, kto może z nich korzystać.
- Moderacja AI: ustaw poziomy filtrowania w całej organizacji (Rygorystyczny, Domyślny, Minimalny), aby przefiltrować prompty, które mogą prowadzić do szkodliwych lub nieodpowiednich wyników.
- Analityka administratora: korzystaj z pulpitów w produkcie (Przegląd i Miro AI) do śledzenia adopcji i zrozumienia aktywności organizacji, podziału licencji, wykorzystania szablonów i użycia Miro AI w Twojej organizacji.

:::note
W trakcie wersji beta AI Workflows, Warunki usługi AI Custom oraz szczegółowe ustawienia administracyjne Miro AI były dostępne dla klientów korzystających z AI Workflows. Teraz z AI Workflows w pełnej dostępności, te funkcje są dostępne tylko w ramach Enterprise Guard. Więcej informacji znajdziesz w [Zaawansowane zarządzanie AI z Enterprise Guard](01-overview.md).
:::

## Ustawienia administratora Miro AI

Ustawienia administratora Miro AI pomagają decydować, które funkcje AI są dostępne w Twojej organizacji oraz zarządzać, kto może z nich korzystać. Więcej informacji znajdziesz w [dokumentacji ustawień administratora Miro AI](../managing-enterprise-teams-and-content/01-miro-ai-admin-controls.md).

**Cel i zakres**

**Czym są kontrolki Miro AI dla administratorów?**

Kontrolki Miro AI dla administratorów pozwalają zarządzać dostępem do możliwości Miro AI w całej organizacji. W zależności od ustawień, możesz włączyć dostęp dla wszystkich, ograniczyć go do konkretnych zespołów lub wyłączyć całkowicie.

**Jaka jest różnica między możliwością AI a funkcją AI?**

**Możliwość** to kategoria funkcjonalności AI (na przykład tworzenie treści, praca z obrazami lub podsumowywanie aktywności). **Funkcja** to konkretne działanie w ramach możliwości (na przykład c*reate sticky notes* lub u*suń tło*).

Sterowanie na poziomie funkcji (zarządzanie poszczególnymi funkcjami w ramach możliwości) jest dostępne w ramach [Enterprise Guard](01-overview.md).

**Dostęp i wymagania wstępne**

**Gdzie zarządzać kontrolami administratora Miro AI?**

W konsoli administracyjnej przejdź do **Miro AI** > **Możliwości**. Tam możesz włączyć, ograniczyć lub usunąć dostęp do każdej możliwości AI (a jeśli to możliwe, do poszczególnych funkcji AI).

**Kto może skonfigurować te ustawienia?**

Administratorzy firmy mogą zarządzać dostępem do Miro AI w konsoli administracyjnej (dostępność funkcji AI zależy od Twojego abonamentu i włączonych dodatków).

**Opcje dostępu i zachowanie**

**Co oznaczają opcje dostępu (Wszyscy, Nikt, Konkretne zespoły)?**

Użyj rozwijanego menu obok możliwości (lub funkcji, jeśli dostępne), aby wybrać, jak przyznawany jest dostęp.

| Opcja | Funkcje | Kiedy używać |
| --- | --- | --- |
| **Wszyscy** | Umożliwia dostęp dla wszystkich użytkowników i zespołów w Twojej organizacji (w tym zespołów utworzonych później). Każde ograniczenie na poziomie zespołu zostaje unieważnione. | Standardowa implementacja w całej organizacji. |
| **Nikt** | Usuwa dostęp dla wszystkich. Zostaniesz poproszony(a) o potwierdzenie usunięcia. | Blokada użycia w całej organizacji. |
| **Wybrane zespoły** | Umożliwia dostęp tylko dla wybranych zespołów. | Pilot z podzbiorem zespołów lub stopniowa implementacja. |

**Co się stanie, jeśli dezaktywuję funkcję?**

Po dezaktywacji funkcji użytkownicy tracą dostęp do tej funkcji oraz powiązanych z nią cech na tablicach. Gdy wszystkie możliwości Miro AI zostaną dezaktywowane, opcja **Twórz z pomocą AI** pojawi się jako wyłączona na tablicy.

**Czy te ustawienia mają zastosowanie do nowo utworzonych zespołów?**

Jeśli ustawisz funkcję dla **Wszyscy**, zastosuje się to do całej organizacji, w tym nowo utworzonych zespołów. W przypadku wyboru **Konkretnych zespołów**, będziesz musiał(a) zaktualizować wybór, aby uwzględnić nowe zespoły (jeśli chcesz je włączyć).

**Enterprise Guard i kontrola na poziomie funkcji**

**W jaki sposób Enterprise Guard zmienia to, co mogę kontrolować?**

Dzięki [Enterprise Guard](01-overview.md) możesz zarządzać dostępem na **poziomie funkcji** w ramach każdej zdolności (nie tylko na poziomie kategorii). Pozwala to na włączenie niektórych funkcji przy jednoczesnym ograniczeniu innych w ramach tej samej zdolności.

Przykład: możesz włączyć t*worzenie obrazów* i ograniczyć u*swawanie tła* (w ramach zdolności Obrazy).

**Widoczność i dostępność**

**Dlaczego nie widzę ustawień dla przepływów, współpracowników AI lub prototypowania?**

Niektóre funkcje (jak **przepływy**, **współpracownik AI** i **prototypowanie**) są widoczne i zarządzalne tylko, jeśli są włączone dla Twojej organizacji.

**Czy mogę zobaczyć, który model AI napędza daną funkcję?**

Tak. W konsoli administracyjnej > **Miro AI** > **Funkcje**, administratorzy mogą wyświetlić modele, które napędzają każdą funkcję AI.

**Czy goście lub odwiedzający mogą korzystać z Miro AI, jeśli ją włączę?**

Miro AI jest dostępna dla **członków**. Goście i odwiedzający nie mogą korzystać z Miro AI.

**Rozwiązywanie problemów i najlepsze praktyki**

**Zmieniłem ustawienia dostępu, ale użytkownicy nadal widzą Miro AI. Co powinienem sprawdzić?**

- **Potwierdź zakres:** Upewnij się, że zaktualizowałeś właściwą funkcję (lub konkretną funkcję, jeśli dotyczą jej ustawienia na poziomie funkcji).
- **Sprawdź ustawienia zespołowe:** Jeśli ustawiono na *Określone zespoły*, upewnij się, że zespół użytkownika jest wybrany.
- **Pozwól na propagację zmian:** W niektórych przypadkach zmiany mogą zająć chwilę, aby zastosować się we wszystkich sesjach.
- **Odśwież sesję:** Poproś użytkownika o odświeżenie karty przeglądarki, wylogowanie i zalogowanie się ponownie lub ponowne uruchomienie aplikacji komputerowej (jeśli dotyczy).

## Moderacja przez Miro AI

Dzięki moderacji Miro AI administratorzy firmy mogą dostosować poziomy filtrowania promptów, które mogą zawierać potencjalnie szkodliwy lub nieodpowiedni tekst. Możesz ustawić w całej organizacji poziom wrażliwości moderacji Miro AI, aby filtrować treści, w tym nienawiść, treści seksualne, przemoc i samookaleczenia. Pomaga to w dostosowaniu wykorzystania Miro AI do wymagań, zasad i tolerancji ryzyka Twojej organizacji. Więcej informacji znajdziesz w [dokumentacji moderacji Miro AI](../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Cel i zakres**

**Czym jest moderacja AI w Miro?**

Moderacja AI umożliwia administratorom firmy ustawienie poziomu filtrowania (Ścisły, Domyślny lub Minimalny) w całej organizacji, który śledzi prompty mogące prowadzić do szkodliwych lub nieodpowiednich wyników (np. nienawiść, treści seksualne, przemoc, samookaleczenie).

**Kto może to skonfigurować i na jakich wersjach?**

Administratorzy firmy na wersji Enterprise z dodatkiem Miro AI Workflows mogą skonfigurować ustawienia w ustawieniach organizacji.

**Czy działa, jeśli moja organizacja połączy własny LLM (np. bezpośrednią integrację dostawcy)?**

Jeśli zostanie podłączony niestandardowy LLM, wybór poziomu moderacji może być wyłączony dla tej integracji, a wcześniej wybrany poziom nie będzie miał zastosowania.

**Dostęp i wymagania wstępne**

**Kto może to aktywować i czego potrzebuję?**

Administratorzy firm na wersji Enterprise z dodatkiem AI Workflows mogą skonfigurować Moderację AI w ustawieniach organizacji.

**Jak to włączyć?**

Przejdź do Ustawienia → Miro AI → Moderacja, wybierz Ścisłe/Domyślne/Minimalne, a następnie kliknij **Zapisz zmiany**. Egzekwowanie jest natychmiastowe dla całej organizacji.

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

**Interakcje z innymi kontrolami**

**Jak moderacja AI odnosi się do zabezpieczeń i kontroli promptów?**

- **Inteligentne zabezpieczenia:** Jeśli tablica jest objęta zabezpieczeniem „Blokuj korzystanie z Miro AI”, funkcja AI jest wyłączona niezależnie od poziomu moderacji.
- **Blokowanie promptów:** Działa w parze z moderacją. Blokowanie promptów zatrzymuje wrażliwe polecenia podczas ich przesyłania; moderacja filtruje szkodliwe kategorie.
- **Szczegółowe kontrolki administratora:** Przełączniki funkcji ustalają, kto może uzyskać dostęp do funkcji AI, gdy AI jest dostępne.

**Rozwiązywanie problemów i najlepsze praktyki**

**Widzimy zbyt wiele fałszywych alarmów.**

Rozważ zmianę z trybu Surowość na Domyślny (lub z Domyślny na Minimalny) i opublikowanie przykładów akceptowalnego użycia. Jeśli po dopasowaniu ustawień problem nadal występuje, skontaktuj się z Twoim managerem ds. sukcesu klienta w Miro, aby zgłosić ten problem, a nasz zespół produktowy mógł to przeanalizować.

**Widzimy, że szkodliwe treści przechodzą niezauważone.**

Zmień na Domyślny lub Surowość i zapewnij wewnętrzne wytyczne. Ponownie oceń po aktualizacjach zasad/regulacji. Jeśli problem będzie się utrzymywał po tych zmianach, skontaktuj się z Twoim managerem ds. sukcesu klienta w Miro, aby zgłosić ten problem, a nasz zespół produktowy mógł to przeanalizować.

## Analizy administratora

Admin Analytics zapewnia administratorom firmy dane umożliwiające podjęcie działania, oparte na danych analizy, dotyczących wdrażania, użycia i zarządzania Miro na dużą skalę. Zawiera dwa pulpity: **Przegląd** i **Miro AI**. Więcej informacji można znaleźć w artykułach [Przegląd Analiz](../getting-started/admin-analytics/01-analytics-overview.md), [pulpit Przegląd](../getting-started/admin-analytics/02-overview-dashboard.md) oraz [pulpit Miro AI](../getting-started/admin-analytics/03-miro-ai-dashboard.md).

**Cel i zakres**

**Czym jest Admin Analytics?**

Admin Analytics dostarcza zaufane, wbudowane w produkt wskaźniki, które pomagają zrozumieć, jak Miro jest wykorzystywane, zarządzać organizacją, wspierać adopcję oraz potrzeby związane z bezpieczeństwem i zgodnością.

**Jakie pulpity są zawarte?**

Admin Analytics zawiera dwa pulpity: **Przegląd** (aktywność i adopcja w organizacji obejmujące tablice, użytkowników, zespoły, licencje i szablony) oraz **Miro AI** (adopcja i użycie Miro AI w całej organizacji).

**Pulpity i nawigacja**

**Jak przełączać się pomiędzy pulpitami?**

Użyj kart na górze strony Analytics, aby przełączać się pomiędzy **Przeglądem** i **Miro AI**.

**Jak zmienić zakres czasu?**

Użyj **selektora zakresu czasu** w prawym górnym rogu strony Analytics, aby dostosować wyświetlany zakres czasu (**codziennie**, **tygodniowo**, **miesięcznie** lub **kwartalnie**).

**Kiedy dane są odświeżane?**

Metryki są odświeżane **codziennie**. Każdy pulpit pokazuje znacznik czasu **Ostatnia aktualizacja**.

**Pulpit przeglądu**

**Co mogę śledzić na pulpicie przeglądu?**

Pulpit przeglądu pomaga śledzić wdrożenie i zrozumieć aktywność organizacji, korzystając z tych grup wskaźników:

- **Tablice:** łączna liczba tablic, aktywne tablice i trendy historyczne.
- **Użytkownicy:** trendy aktywnych użytkowników. Możesz także śledzić według roli, takich jak członkowie, administratorzy firmy, goście lub goście zespołu.
- **Zespoły:** liczba zespołów i poziomy aktywności.
- **Licencje:** rodzaje przydzielonych licencji i jak zmienia się ich alokacja w czasie.
- **Szablony:** które szablony są najczęściej używane w Twojej organizacji.

**Jak interpretować wykresy historyczne?**

- W widżetach pokazujących dane historyczne wartości przedstawiają dane na **ostatni dzień każdego okresu**.
- **Obecny trwający okres** nie jest wyświetlany na wykresach historycznych.
- Dane historyczne są dostępne do **jednego roku** wstecz lub tak daleko, jak istnieją dane.

**Pulpit Miro AI**

**Co mogę śledzić na pulpicie Miro AI?**

Pulpit Miro AI pomaga śledzić zastosowanie i zrozumieć, jak Miro AI jest używane w ramach Twojej organizacji, wykorzystując te wskaźniki:

- **Zespoły korzystające z AI:** zespoły aktywnie korzystające z funkcji AI, w tym informacje o łącznej liczbie zespołów korzystających i niekorzystających z AI. Możesz filtrować użycie według przypadku użycia.
- **Lista osób korzystających z AI:** łączna liczba użytkowników korzystających i niekorzystających z AI, z miesięczną historią użycia.
- **AI według przypadku użycia:** użycie w czasie podzielone na **tworzenie AI** i **automatyzację AI**.
- **Współpraca z współpracownikami AI:** jak często zespoły angażują się w interakcje z współpracownikami poprzez sesje czatu (prompty, pytania uzupełniające i odpowiedzi). Analizy pokazują liczbę rozpoczętych sesji.
- **Wykonane przepływy AI:** ile razy użytkownicy uruchomili przepływ AI z co najmniej dwoma kolejnymi krokami lub węzłami. Wykonanie jest liczone na podstawie znacznika czasu pierwszego zdarzenia związanego z przepływem.

**Jak są definiowane przypadki użycia AI?**

- **Tworzenie AI:** działania takie jak tworzenie na podstawie promptów i kontekstu wizualnego.
- **Automatyzacja AI:** działania takie jak iterowanie przez czat lub menu kontekstowe, edycja tekstu, kategoryzacja i usuwanie tła obrazu.

**Czy użycie tokenów na AI jest tym samym co wskaźniki użycia AI?**

Nie. **Tokeny na AI nie są bezpośrednio skorelowane** z wskaźnikami użycia AI wyświetlanymi na tym pulpicie.

**Uwagi dotyczące danych**

**Dlaczego widzę niepełne dane?**

Jeśli funkcja została wyłączona na część wybranego okresu, możesz zobaczyć niepełne dane w historii wskaźników (na przykład, gdy funkcja została włączona w połowie miesiąca).

**Dlaczego wykresy nie pokazują danych dla pewnego okresu?**

Jeśli w danym okresie (dzień, tydzień lub miesiąc) nie zarejestrowano żadnych aktywności, wykres nie wyświetli danych dla tego przedziału czasowego.

**Starsze dane wyglądają na brakujące. Co powinienem zrobić?**

Dane historyczne są dostępne do jednego roku wstecz lub do czasu, kiedy dane istnieją. Jeśli starsze dane wyglądają na brakujące, skontaktuj się z pomocą Miro, aby poprosić o weryfikację uzupełnienia.

**Rozwiązywanie problemów i najlepsze praktyki**

**Nasze wyniki wyglądają na niższe niż oczekiwano. Co powinienem sprawdzić?**

- Potwierdź **zakres czasu** i typ okresu (dzienny, tygodniowy, miesięczny, kwartalny).
- Pamiętaj, że **historyczne wykresy pokazują zakończone okresy**, a nie aktualnie trwające.
- Jeśli funkcja została włączona w połowie okresu, spodziewaj się **częściowych danych** dla tego okresu.

**Jak mogę skutecznie wykorzystać te wnioski?**

Wykorzystaj wskaźniki Przeglądu do identyfikacji zespołów, szablonów lub trendów licencjonowania z niższym użyciem, a następnie przeprowadź ukierunkowaną aktywację. Wskaźniki Miro AI pomogą zidentyfikować, gdzie rośnie adopcja AI, wesprzeć liderów i poprowadzić odpowiedzialne wdrożenie.

## Zaawansowane zarządzanie AI za pomocą Enterprise Guard

Enterprise Guard zapewnia dodatkowe, zaawansowane możliwości zarządzania AI dla administratorów Enterprise. Użyj tych kontroli, aby dostosować dostęp, chronić informacje wrażliwe oraz wzmocnić monitorowanie i zgodność w zakresie użycia AI w Miro. Więcej informacji znajdziesz w artykule [Enterprise Guard AI Trust capabilities and FAQs](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md).

- [Szczegółowe ustawienia administracyjne Miro AI](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): ustaw dostęp do funkcji na poziomie funkcji (Wszyscy/Nikt/Wybrane zespoły) w każdej kategorii możliwości.
- [Blokuj użycie Miro AI za pomocą inteligentnych zabezpieczeń](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): użyj inteligentnych zabezpieczeń, aby zablokować wszystkie interakcje wspierane przez AI w Miro, gdy potrzebujesz chronić dane wrażliwe lub sklasyfikowane.
- [Blokowanie promptów](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): blokuj prompty zawierające dane wrażliwe lub kod źródłowy w momencie przesłania; zamiast wysyłać je do LLM, pokaż komunikat dotyczący zasady.
- [Enterprise Guard i Microsoft Purview DSPM dla AI](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): przekierowuj prompty i odpowiedzi do Purview w celu centralnego monitoringu, audytu i zarządzania.
