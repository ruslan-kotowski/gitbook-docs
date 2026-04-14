---
title: "Problemy z wydajno\u015Bci\u0105 i\_\u0142adowaniem tablicy"
article_id: 360013588560
translation_id: 360013588560
locale: pl-pl
sidebar_position: 4
created_at: '2020-05-06T08:17:24Z'
updated_at: '2025-04-01T16:57:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Zapoznaj się ze wskazówkami, jak poprawić wydajność tablicy podczas sesji współpracy oraz na dużych tablicach. Możesz też rozwiązywać problemy, takie jak niska wydajność i wolna nawigacja, zamrażanie tablic i niekończące się ładowanie.

## Jak poprawić wydajność tablicy

Wydajność tablicy może być wolniejsza podczas **sesji współpracy** z wieloma użytkownikami, a także na **dużych tablicach** z dużą ilością zawartości.

Wskazówki dotyczące sesji współpracyWskazówki dotyczące dużych tablic

Rosnąca liczba użytkowników na tablicy i ich intensywna aktywność mogą mieć wpływ na wydajność tablicy. Użytkownicy ze starszymi i mniej wydajnymi urządzeniami są bardziej narażeni na opóźnienia w wydajności.

**Jeśli bierzesz udział w sesji współpracy:**

- Otwórz tablicę w [przeglądarce](../technical-guidelines/02-supported-browsers-browser-restrictions.md) na komputerze.
- Zamknij wszystkie niepotrzebne karty i okna przeglądarki.
- Ukryj kursory współpracowników i zamknij wszystkie paski boczne.

  *![hiding_cursors_and_toolbars.gif](images/21358655510418_hiding%20cursors%20and%20toolbars.gif)
  Ukrywanie kursorów i pasków narzędzi współpracowników*
- Unikaj zaznaczania i zmieniania wielu obiektów na tablicy w tym samym czasie.
- Ogranicz do minimum nawigację na tablicy.
- W przypadku korzystania z Miro na laptopie upewnij się, że korzystasz z trybu wysokiej wydajności, a nie z trybu oszczędzania energii.

**Jeśli planujesz sesję współpracy w Miro:**

- Zapraszaj użytkowników, którzy nie potrzebują dostępu do edycji, jako wyświetlających. Dowiedz się, jak skonfigurować [uprawnienia dostępu do tablicy.](../../sharing-boards/01-board-access-rights.md)
- Pamiętaj, aby zachować porządek na tablicy – zapoznaj się ze **Wskazówkami dotyczącymi dużych tablic,** które znajdują się na drugiej karcie powyżej.

Maksymalna liczba obiektów, które można dodać do tablicy, wynosi 100 000. Jednak wydajność może być obniżona już od 1000 obiektów. Aby uzyskać dobrą wydajność, zalecamy zachowanie liczby obiektów na tablicy poniżej 5000.

**Aby znaleźć liczbę obiektów na tablicy:**

- Zaznacz wszystkie obiekty na tablicy (ctrl-A w systemie Windows, cmd-A na komputerze Mac lub przeciągnij pole wyboru wokół wszystkich obiektów).
- Pojawi się menu kontekstowe, w którym zobaczysz całkowitą liczbę obiektów.
- Kliknij **Filtr**, aby wyświetlić liczbę obiektów według typu.

![Number_of_objects_on_the_board.gif](images/21358609765010_Number%20of%20objects%20on%20the%20board.gif)
*Sprawdzanie liczby obiektów na tablicy*

Oprócz dużej liczby obiektów, wolniejsze działanie tablicy mogą również powodować większe i bardziej złożone obiekty (zwłaszcza przesłane pliki i dokumenty).

**Aby przyspieszyć działanie dużej tablicy, zachowaj na niej porządek:**

- Usuń niepotrzebne treści, zwłaszcza duże przesłane pliki i dokumenty (np. wektorowe pliki PDF zawierające wiele szczegółów lub obrazy w wysokiej rozdzielczości).
- Konwertuj duże pliki PDF i obrazy w wysokiej rozdzielczości na pliki PNG/JPG i prześlij je ponownie na tablicę.
- Zmniejsz skalę zawartości tablicy, jeśli wydaje się ona zbyt duża przy 100% powiększeniu:

- Przejdź do mapy w prawym dolnym rogu i ustaw powiększenie na 100%.
- Jeśli przy tym powiększeniu zawartość wygląda na zbyt dużą, zaznacz ją za pomocą **Ctrl + A** (Windows) lub **Cmd + A** (Mac) i zmniejsz ją.
- Rozważ również zmniejszenie wszelkich dużych obrazów.

  *![downscaling_content.gif](images/21358609765650_downscaling%20content.gif)**Zmniejszanie skali zawartości*

- [Zamknij komentarze](../../facilitation-tools/asynchronous-tools/01-comments.md).
- Konwertuj odręczne pismo [piórem](../../essential-tools/10-pen.md) na obrazy:

- zrób zrzut ekranu rysunku
- prześlij go na tablicę
- usuń rysunek.

- Jeśli to możliwe, podziel tablicę na kilka mniejszych:

- skopiuj część zawartości tablicy, zaznaczając ją i naciskając **Ctrl + C** (Windows) lub **Cmd + C** (Mac)
- [utwórz nową tablicę](../../../getting-started/start-here/your-first-board/01-create-a-miro-board.md) i wklej na niej skopiowaną zawartość
- usuń skopiowaną zawartość z oryginalnej tablicy.

## Jak rozwiązać problemy ze słabą wydajnością lub niekończącym się ładowaniem

Urządzenie, połączenie internetowe, przeglądarka i inne czynniki mogą mieć wpływ na wydajność i szybkość ładowania tablicy. Jeśli masz problem z wydajnością lub ładowaniem tablicy lub pulpitu nawigacyjnego w przeglądarce, aplikacji komputerowej, na tablecie lub urządzeniu mobilnym, spróbuj wykonać poniższe czynności.

:::warning
Zanim skorzystasz z poniższych rozwiązań, sprawdź [Stronę stanu Miro](https://status.miro.com/) pod kątem raportów o pogorszeniu wydajności.
:::

Przeglądarka Aplikacja komputerowa Tablet, urządzenia mobilne

1. Otwórz Miro w trybie [incognito](https://support.google.com/chrome/answer/95464) **(prywatnym)** lub w **innej przeglądarce.**Jeśli Miro działa w trybie incognito lub w innej przeglądarce, wyczyść pamięć podręczną przeglądarki i pliki cookie.

**Jak wyczyścić dane witryny Miro w Chrome**

1. Przejdź na stronę `https://miro.com/` i otwórz **Narzędzia dla programistów** w Chrome (**Command + Option + J** *w systemie Mac*, **Ctrl + Shift + J** *w systemie Windows*).
2. Wybierz kartę **Aplikacja > Pamięć masowa**. Kliknij **Wyczyść dane witryny.**​ W ten sposób usuniesz wszelkie dane Miro zapisane w przeglądarce Chrome i możesz rozpocząć nową sesję. Pamiętaj, że wylogujemy Cię z profilu Miro.

![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)*Opcja wyczyszczenia danych witryny w Chrome*

Może być również konieczne zaktualizowanie przeglądarki do najnowszej wersji lub wyłączenie niektórych rozszerzeń. Sprawdź listę [obsługiwanych przeglądarek](../technical-guidelines/02-supported-browsers-browser-restrictions.md).

2. Sprawdź **połączenie internetowe**. Jeśli przepustowość sieci nie osiąga minimum 8 Mb/s, przełącz się na inną, najlepiej szybszą sieć.

3. Upewnij się, że urządzenie spełnia **[wymagania systemowe](../technical-guidelines/01-system-requirements.md)**:

- Procesor – 3 GHz (2 rdzenie/ 4 wątki)
- Pamięć RAM – 8 GB

4. jeśli korzystasz z Miro na laptopie, upewnij się, że korzystasz z trybu **wysokiej wydajności**, a nie z trybu oszczędzania energii.

5. Jeśli wystąpił problem z określonymi tablicami, spróbuj **[je zduplikować](../../managing-boards/03-how-to-duplicate-a-board.md)** i sprawdź, czy problem powtarza się na skopiowanej tablicy.

**Dla użytkowników, którzy nie mogą załadować i otworzyć Miro:**

6. Sprawdź, czy połączenie obsługuje **WebSockets.** Przeczytaj więcej o WebSockets i rozwiązywaniu problemów w sekcji [Jak dodać Miro do dozwolonych aplikacji](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md).

7. Dowiedz się w dziale IT, czy Twoja firma używa **zapór sieciowych** lub **serwera proxy**, które mogą blokować Miro. Postępuj zgodnie ze wskazówkami, aby dodać Miro do listy dozwolonych aplikacji lub podaj informacje określone w sekcji [Jak dodać Miro do dozwolonych aplikacji](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md).

Jeśli problem nie ustąpi, [skontaktuj się z pomocą techniczną Miro](../../tools/troubleshooting/06-contacting-miro-support.md) i wyślij nam [dzienniki konsoli przeglądarki](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

1. Sprawdź, czy przy użyciu **[wersji internetowej](https://miro.com/app/dashboard/)** masz problem z niską wydajnością lub niekończącym się ładowaniem. Jeśli nie możesz uzyskać dostępu do Miro w wersji internetowej, zapoznaj się z przewodnikiem rozwiązywania problemów dla **przeglądarki.**
2. Jeśli nie występują żadne problemy w przeglądarce, **zresetuj dane aplikacji.**


   **Jak zresetować dane aplikacji w systemie Windows**

   Naciśnij Alt, kliknij **Pomoc** w prawym górnym rogu i wybierz **Resetuj dane aplikacji**:


   ![reset_app_data_on_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725434514_reset%20app%20data%20on%20Windows.jpg)
   *Resetowanie danych aplikacji w aplikacji komputerowej dla systemu Windows*

   Jeśli nie możesz znaleźć menu, prawdopodobnie używasz aplikacji pobranej z MS Store. W takim przypadku, aby zresetować dane aplikacji, otwórz **Ustawienia** systemu Windows> **Aplikacje** > **Aplikacje i funkcje** > znajdź **Miro** na liście > **Opcje zaawansowane** > **Resetuj**.

   **Jak zresetować dane aplikacji w systemie Mac**

   W aplikacji Miro kliknij **Pomoc** w górnym menu i wybierz **Resetuj dane aplikacji**:


   ![reset_app_data_on_Mac.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
   *Resetowanie danych aplikacji w systemie Mac*
3. Jeśli problem nie ustąpi, spróbuj usunąć aplikację i [**ponownie ją zainstalować**](https://miro.com/apps/).

Jeśli nadal masz problemy, [skontaktuj się z pomocą techniczną Miro](../../tools/troubleshooting/06-contacting-miro-support.md) i wyślij nam [dzienniki konsoli aplikacji](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

1. Sprawdź **połączenie internetowe**. Jeśli przepustowość sieci nie osiąga minimum 8 Mb/s, przełącz się na inną, najlepiej szybszą sieć.
2. Upewnij się, że urządzenie spełnia **wymagania techniczne**:

- Miro na tabletach:
  - 6 GB pamięci RAM
  - iOS 12.0 lub wyższa wersja, Android 6.0 lub wyższa wersja, Windows 10 w wersji 1607 lub wyższej
  - rozdzielczość ekranu 768 × 1024 pikseli lub wyższa.
- Miro na urządzeniach mobilnych:
  - iOS 12.0 lub wyższa wersja
  - Android 6.0 lub wyższa wersja.

- Usuń i **zainstaluj ponownie aplikację** na urządzeniu.

**Dla użytkowników iPada:**
Pamiętaj, że pogorszenie wydajności tablicy na iPadzie może być spowodowane ograniczeniami pamięci RAM. Wykonaj następujące czynności:

1. Zamknij wszystkie niepotrzebne aplikacje w tle przed użyciem Miro – powinno to poprawić wydajność.
2. Pracuj na mniejszych tablicach – powinno to zmniejszyć obciążenie systemu przez aplikację.
3. Przełącz się na inne urządzenie (laptop lub komputer) z lepszą pamięcią RAM i użyj wersji przeglądarkowej Miro.

## Jak rozwiązywać typowe problemy

Synchronizacja... Proszę czekać Połączenie przywrócone

Wyskakujące powiadomienie **Synchronizacja... Proszę czekać** zazwyczaj oznacza, że przetwarzana jest duża ilość danych, a brakuje niezbędnej mocy, aby proces zakończył się w oczekiwanym czasie. Komunikat może więc pojawić się, jeśli pracujesz na tablicy z wyjątkowo dużą ilością danych podczas przenoszenia zbiorczego, na przykład wielu obiektów, lub jeśli nastąpiła utrata pakietów. Pamiętaj, że nawet jeśli tablica wygląda stosunkowo prosto, w Miro dużymi obiektami będą obrazy w wysokiej rozdzielczości, pliki PDF, rysunki piórem (ponieważ są to grafiki wektorowe, które są trudne do renderowania) lub tabele. Może to spowodować pogorszenie wydajności powodujące wyświetlenie powyższego komunikatu.

Spróbuj podzielić tablicę na mniejsze, kopiując i wklejając zawartość do nowej tablicy, i sprawdź, czy problem się utrzymuje. Jeśli to nie pomoże:

- Upewnij się, że urządzenie spełnia minimalne wymagania systemowe i że przeglądarka została zaktualizowana do najnowszej wersji.
- Jeśli w przeglądarce masz otwarte wiele kart, spróbuj je zamknąć lub zamrozić przed rozpoczęciem pracy w Miro, aby przeglądarka mogła skierować całą moc obliczeniową do aplikacji Miro bez potrzeby dzielenia jej między wieloma kartami.
- Przetestuj Miro w trybie incognito (prywatnym) (aby wykluczyć możliwość ingerencji rozszerzeń przeglądarki) oraz w innej przeglądarce. W razie potrzeby zamknij wszystkie karty przeglądarki i aplikacje działające w tle.
- Wyczyść pamięć podręczną przeglądarki i pliki cookie, uruchom ponownie przeglądarkę i odśwież stronę, klikając kilka razy F5 (lub Ctrl/Cmd + R).
- Jeśli wystąpią problemy z określonymi tablicami, spróbuj je zduplikować i sprawdź, czy problem się powtarza. Możesz również spróbować otworzyć tablicę z mniejszą liczbą elementów lub mniejszą tablicę, aby sprawdzić, czy problem nadal występuje.
- Jeśli korzystasz z VPN, sprawdź, czy problem utrzymuje się po jego wyłączeniu.
- Spróbuj zduplikować tablicę i sprawdź, czy błąd powtarza się na nowej.

Ogólnie rzecz biorąc, błąd **Przywracanie połączenia...**, **Połączenie przywrócone** może pojawić się w poniższych przypadkach:

- Jeśli po Twojej stronie występują problemy z łącznością. Upewnij się, że połączenie sieciowe spełnia minimalne wymagania. Spróbuj przełączyć się na szybszą sieć.
- Podczas pracy na wielu obszernych tablicach otwartych w tej samej przeglądarce. Jeśli tak jest w Twoim przypadku, zamknij wszystkie dodatkowe karty i uruchomione aplikacje w przeglądarce i odśwież stronę przeglądarki.

Warto również sprawdzić połączenie WebSocket (zwłaszcza jeśli występują problemy na wszystkich tablicach, nawet najmniejszych). Skontaktuj się z działem IT i poproś o włączenie połączeń WebSocket na portach 80 i 443 (SSL) oraz [sprawdzenie, czy przyczyną może być jeszcze coś innego](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md).

## Często zadawane pytania

*Czy wydajność tablicy zależy od abonamentu (wersja płatna/bezpłatna)?*

Nie, rodzaj abonamentu nie ma wpływu na wydajność tablicy

*Czy ustawienia udostępniania tablicy mają wpływ na wydajność?*

Ustawienia udostępniania nie powinny mieć wpływu na wydajność tablicy, ale liczba użytkowników na tablicy może mieć na to wpływ. Możesz użyć wyżej wymienionych porad dotyczących sesji współpracy.
