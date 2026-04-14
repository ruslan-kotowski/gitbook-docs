---
title: Konfigurowanie Miro Insights
article_id: 30122381753106
translation_id: 30122381753106
locale: pl-pl
sidebar_position: 0
created_at: '2025-10-10T10:26:28Z'
updated_at: '2025-11-25T15:54:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Łączenie narzędzi z Miro Insights to kluczowy pierwszy krok do uzyskania rzeczywistej wartości. Integracje pozwalają Miro Insights automatycznie pobierać opinie klientów oraz istotne dane z Twoich systemów. Ten przewodnik jest przeznaczony dla administratorów firmy, którzy umożliwią te połączenia.

Jeśli jesteś członkiem zespołu, który chce korzystać z Miro Insights po jego skonfigurowaniu, zobacz artykuł na temat [Korzystanie z Miro Insights](../../miro-insights/use-miro-insights).

## Wymagania wstępne

Aby skonfigurować integracje Miro Insights, musisz spełniać następujące wymagania:

- Musisz być **administratorem firmy w Miro**.
- Musisz mieć **dostęp administracyjny lub API na platformie zewnętrznej**, do której się podłączasz.

:::note
Upewnij się, że Twój **abonament Miro obejmuje Miro Insights**. Jeśli Miro Insights jest dodatkiem lub w ograniczonej wersji, Twoje konto musi być odpowiednie. Ponadto niektóre integracje mogą wymagać konkretnych wersji zewnętrznego oprogramowania. Na przykład dostęp do API CRM jest dostępny w wyższych planach.
:::

## Przygotuj swoje źródła danych

Przed podłączeniem swoich źródeł danych do Miro Insights ważne jest przygotowanie danych i ustanowienie jasnej taksonomii. To przygotowanie zapewni Ci najdokładniejsze, użyteczne spostrzeżenia z platformy.

### Oczyść i zoptymalizuj swoje dane

Zanim zsynchronizujesz dane z Miro Insights, oczyść i zoptymalizuj swoje źródła danych:

- Usuń duplikaty i przestarzałe elementy.
- Wyczyść niekonsekwentny lub nieistotny feedback.
- Zadbaj o jakość danych w swoich systemach źródłowych.
- Rozwiąż przedwcześnie poważne niespójności lub luki w danych.

### Ustal swoją taksonomię

Choć Miro Insights posiada podstawowe kategorie generowane przez AI, zaleca się zdefiniowanie własnej, standaryzowanej taksonomii przed wdrożeniem. Zapewnia to spójność i poprawia jakość obserwacji od samego początku.

Rozważ włączenie tych standardowych kategorii:

- Sugestie dotyczące funkcji
- Błędy
- Punkty bólu UX
- Segmenty klientów
- Poziomy priorytetu
- Jednostki biznesowe
- Inicjatywy strategiczne

Najlepsze praktyki dotyczące taksonomii:

- Używaj terminologii zgodnej z językiem Twojego zespołu.
- Stwórz jasne wytyczne dotyczące tego, jak i kiedy używać każdej kategorii.
- Udostępnij taksonomię swojemu zespołowi, aby zapewnić spójne użytkowanie.
- Regularnie przeglądaj i udoskonalaj kategorie w razie potrzeby.
- Rozważ mapowanie na swoje inicjatywy strategiczne i OKR.

:::tip
Skontaktuj się z pomocą Miro Insights, aby uzyskać pomoc w definiowaniu swojej taksonomii. Mogą dostarczyć przykłady i najlepsze praktyki, oparte na doświadczeniach innych klientów z Twojej branży.
:::

## Połącz integrację

Gdy Twoje dane są gotowe, możesz podłączyć swoje integracje. Miro Insights obsługuje różne popularne narzędzia w ramach CRM, pomocy, rozmów sprzedażowych, zarządzania projektami i platform czatu.

W karcie **Integracje i automatyzacje** w ustawieniach możesz wyświetlać i zarządzać wszystkimi podłączonymi integracjami. Każda integracja jest wymieniona wraz z jej statusom połączenia oraz opcjami konfiguracji lub odłączenia.

Aby podłączyć integrację:

1. W aplikacji **Miro Insights** wybierz ikonę **ustawienia** na górze lewego paska bocznego.
2. W panelu **ustawienia** przejdź do karty **Integracje i automatyzacje**.
3. Wybierz **Połącz** obok integracji, którą chcesz dodać.
4. **Autoryzuj dostęp**. Wyskakujące okienko poprosi Cię o autoryzację aplikacji Miro Insights do dostępu do tego narzędzia.
   Zwykle oznacza to logowanie się do zewnętrznej usługi i udzielanie uprawnień. Na przykład, łącząc się z Salesforce, musisz zalogować się na konto administratora Salesforce i zatwierdzić integrację. Dla Slacka wybierz przestrzeń roboczą i autoryzuj aplikację Miro Insights dla Slacka. Postępuj zgodnie z instrukcjami wyświetlanymi na ekranie dla każdej z usług.
5. **Skonfiguruj ustawienia importu**. Po połączeniu integracja pojawi się jako „Połączona” z dodatkowymi opcjami ustawień. Tutaj możesz ustawić:
   - **Importuj rozmowy z:** Dla źródeł opartych na rozmowach, takich jak Gong czy Zendesk, możesz wybrać datę. Pozwala to uniknąć pobierania starych danych, chyba że tego chcesz.
   - **Automatyczne zasady importu:** Umożliwiają, by nowe elementy były importowane automatycznie. Możesz to włączyć, aby nowe rozmowy lub zgłoszenia były pobierane na bieżąco. Jeśli zostawisz tę opcję wyłączoną, możesz importować elementy ręcznie lub selektywnie.
   - **Jeśli AI wykryje prośby z:** Niektóre źródła pozwalają filtrować według wiarygodności wykrywania AI.
   - **Wykryj zgłoszenia**: Umożliwia Miro Insights automatyczne identyfikowanie i wyodrębnianie zgłoszeń z feedbacku klientów. Zgłoszenia te mogą obejmować wyzwania związane z użytecznością, problemy z wydajnością, obawy dotyczące bezpieczeństwa itp.

Inne opcje mogą się różnić w zależności od integracji. Na przykład w Jira możesz wybrać, z którego projektu/pów chcesz pobrać funkcje lub zmapować pola niestandardowe.

### Filtrowanie AI

Niektóre integracje pozwalają **filtrować przez wykrycie AI**. Oznacza to, że Insights zeskanuje transkrypt rozmowy i stworzy element feedbacku tylko wtedy, gdy będzie względnie pewne, że wspomniano o prośbie produktu. To zmniejsza hałas niepowiązanych rozmów. Możesz dostosować próg pewności lub wyłączyć tę funkcję, by importować wszystko.

### Filtry tagów lub pól

W narzędziach takich jak Zendesk możesz określić tag, na przykład "feature_request", wtedy tylko zgłoszenia z tym tagiem zostaną przetworzone. W Jira możesz wybrać konkretny projekt lub typ zgłoszenia do zaimportowania jako funkcje.

### Synchronizacja zgłoszeń

Dla narzędzi projektowych, takich jak Jira, możesz mieć opcje mapowania pól. Zrzut ekranu powyżej pokazuje przykład „Prześlij wartość dolara funkcji do pola niestandardowego” – możesz wybrać pole niestandardowe w Jira do wypełnienia obliczonym wpływem dolara z Miro Insights, zamykając pętlę z powrotem do działu inżynieryjnego. Ten krok jest opcjonalny, ale może być bardzo przydatny.

Podłącz wszystkie istotne systemy. Zalecamy podłączenie co najmniej jednego CRM oraz jednego źródła pomocy lub feedbacku na początek, aby uzyskać zarówno kontekst konta, jak i surowe opinie. Zawsze możesz dodać więcej później.

Po zakończeniu konfiguracja integracji z Miro Insights została pomyślnie zakończona. System rozpocznie synchronizację danych. Początkowa synchronizacja może zająć trochę czasu, jeśli istnieje dużo danych historycznych (zobaczysz ostatnio zsynchronizowane znaczniki czasu obok każdej integracji). Możesz monitorować status synchronizacji na liście Integracji – pokazuje ona ostatni czas synchronizacji i oferuje opcję Rozłączenia, jeśli będzie to potrzebne.

## Importuj elementy ręcznie

Możesz także ręcznie importować funkcje i elementy opinii, używając pliku CSV. Jest to przydatne do jednorazowych importów lub jeśli masz listę próśb o funkcje lub opinie z innego źródła.

Aby zaimportować funkcje za pomocą CSV:

1. W Miro Insights, przejdź do widoku **Backlog**.
2. Kliknij przycisk **Import** w prawym górnym rogu.
3. Wybierz **Upload CSV**.
4. Wybierz kolumnę w źródle danych CSV, która najlepiej odpowiada właściwościom Miro Insights.
5. Wybierz **Import funkcji**, aby zakończyć proces.

Zaimportowane funkcje pojawią się teraz w sekcji [Backlog](../../tools/use-miro-insights/05-backlog.md).

Aby zaimportować elementy feedbacku za pomocą pliku CSV:

1. W Miro Insights przejdź do widoku **Feedback**.
2. Kliknij przycisk **Import** w prawym górnym rogu.
3. Wybierz **Upload CSV**.
4. Dopasuj kolumny w swoim pliku CSV do właściwości opinii w Miro Insights (np. tytuł, opis, źródło).
5. Wybierz opcję **Import feedback**, aby zakończyć proces.

Zaimportowane elementy feedbacku pojawią się teraz w sekcji [Feedback](../../tools/use-miro-insights/07-feedback.md).

## Podłączanie nieobsługiwanych narzędzi za pomocą Zapier

Jeśli masz narzędzie, które nie jest bezpośrednio wspierane, często możesz użyć [Zapier](http://zapier.com/), aby przesłać dane do Miro Insights. Na przykład, możesz stworzyć następujący przepływ pracy w Zapier. Kiedy formularz Google zostanie złożony lub pojawi się nowe zgłoszenie w niestandardowej bazie danych, stwórz element feedbacku w Miro Insights.

Aby uzyskać szczegółowe kroki, zobacz artykuł o [Korzystaniu z Zapier z Miro Insights](../../miro-insights/set-up-and-manage-miro-insights/03-connect-tools-with-zapier.md).

## Dodatkowe kroki

Po połączeniu integracji możesz wykonać kilka opcjonalnych kroków, aby upewnić się, że wszystko jest prawidłowo skonfigurowane:

### Import lub weryfikacja funkcji

Jeśli połączyłeś narzędzie do śledzenia zadań, takie jak Jira, sprawdź backlog w Miro Insights, aby upewnić się, że Twoje istniejące funkcje lub epiki się pojawiły. Jeśli nie, możesz użyć przycisku Importuj w widoku backlogu, aby przesłać plik CSV lub uruchomić pobieranie z Jiry. Upewnij się, że każda zaimportowana funkcja ma jasny tytuł i opis; AI polega na tym tekście, aby dopasować odpowiednie opinie.

### Skonfiguruj polecenia Slack lub przekazywanie e-maili

Jeśli dodałeś Slacka, poinformuj swój zespół, jak wysyłać wiadomości do Insights. Na przykład, kliknij prawym przyciskiem wiadomość > „Wyślij do Miro Insights”.

W przypadku e-maili lub innych kanałów możesz skonfigurować przekazywanie. Niektóre zespoły ustawiają konkretny adres e-mail, który automatycznie przekazuje do narzędzia takich jak Intercom lub do hooka Zapier do przetwarzania danych.

> **Wskazówka**: Dobrą praktyką jest okresowe przeglądanie ustawień integracji. Na przykład, jeśli zauważysz, że z danego źródła dociera zbyt wiele trywialnych opinii, zaostrzyć filtry lub zwiększyć próg pewności AI. Z kolei, jeśli brakuje oczekiwanych danych, upewnij się, że integracja jest połączona z odpowiednim zakresem (np. poprawnym projektem lub tagiem). Dobrze dostrojona integracja utrzymuje wysoki poziom sygnału i niski poziom szumów w Twoich obserwacjach.

## Odłącz integrację

Jeśli kiedykolwiek potrzebujesz odłączyć integrację:

1. Przejdź do **Ustawienia** > **Integracje i automatyzacje**.
2. Znajdź integrację, którą chcesz usunąć.
3. Wybierz **Rozłącz** obok niej.
4. Potwierdź rozłączenie w wyświetlonym promptcie.

Spowoduje to zatrzymanie przyszłych synchronizacji danych z tego źródła.

> **Ważne**: W niektórych przypadkach, na przykład Gong, rozłączenie może również usunąć wcześniej zaimportowane elementy feedbacku. W innych przypadkach, takich jak Jira, istniejące funkcje mogą pozostać, ale nie będą aktualizowane. Sprawdź specyficzne zachowanie każdej integracji w dokumentacji lub skontaktuj się z pomocą, jeśli nie jesteś pewien.

Upewnij się, że skonsultujesz się z zespołem, jeśli odłączasz główne źródło, ponieważ może to wpłynąć na kompletność backlogu i feedbacku w Miro Insights.

## Co dalej?

Łącząc integracje, położyłeś fundamenty dla Miro Insights, aby dostarczać bogate, ciągłe obserwacje produktowe. Dane zaczną napływać, a AI zacznie nawiązywać połączenia.

Teraz możesz przejść do [używania Miro Insights](../../miro-insights/use-miro-insights) lub dowiedzieć się więcej o zadaniach administracyjnych, w tym ustawieniach ogólnych, zarządzaniu zespołem, powiadomieniach i dostępie do API w [przewodniku administracyjnym Miro Insights](../../miro-insights/set-up-and-manage-miro-insights/02-manage-miro-insights.md).
