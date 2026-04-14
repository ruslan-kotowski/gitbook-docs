---
title: Importowanie tablic Freehand do Miro
article_id: 18580556555538
translation_id: 18580556555538
locale: pl-pl
sidebar_position: 9
created_at: '2024-04-26T16:34:28Z'
updated_at: '2025-11-25T15:42:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Lista osób: Wszyscy użytkownicy z kwalifikującymi się abonamentami Wersje:
    Starter, Business, Education, Enterprise Platformy: Przeglądarka, komputer, urządzenia
    mobilne (do uzyskiwania dostępu do Miro i inicjowania importu)'
---

Ten artykuł wyjaśnia, jak zaimportować tablice Freehand do Miro, w tym jak przygotować swoje tablice Freehand do importu pojedynczego i zbiorczego.

:::note
Edycje wprowadzone do zaimportowanej treści w Miro nie synchronizują się z ich oryginalną treścią w Freehand.
:::

:::note
Możesz importować tylko te tablice Freehand, które mają licencje bezpłatne lub bezpłatne z ograniczonym dostępem.
:::

## Importuj pojedynczą tablicę z Freehand do Miro

Możesz łatwo importować indywidualne tablice Freehand do Miro, eksportując je w formacie pliku Miro `.RTB`. Oto jak to zrobić:

1. Uzyskaj dostęp do tablicy Freehand, którą chcesz wyeksportować do Miro.
2. Pobierz plik w formacie .RTB, będący własnością Miro, bezpośrednio z Freehand. Przejdź do menu **Narzędzia** i wybierz **Eksportuj do tablicy Miro**. Plik zostanie zapisany w domyślnym folderze pobierania. Freehand powiadomi Cię, gdy pobieranie zostanie zakończone.
3. Otwórz pulpit Miro.
4. W prawym górnym obszarze pulpitu Miro kliknij przycisk **+ Utwórz nowy**, następnie kliknij **Importuj**, a potem kliknij **Importuj kopię zapasową**.
5. Wybierz wcześniej pobrany plik `.RTB` z systemu.
6. Cała treść jest teraz importowana do nowej tablicy Miro w edytowalnym formacie.
7. Chociaż większość treści przejdzie płynnie, mogą być konieczne drobne poprawki z powodu różnic w opcjach stylizacji i formatowania między Freehand a Miro. Aby uzyskać więcej wskazówek dotyczących potencjalnych różnic, przeczytaj sekcję Zrozumienie mapowania obiektów Freehand w Miro.

## Zbiorczy import wielu plików z Freehand do Miro

Aby migrować wiele tablic Freehand jednocześnie, Miro oferuje proces zbiorczego importowania. Najpierw upewnij się, że Twoje tablice Freehand są poprawnie przygotowane.

**Wymagania wstępne: Przygotuj swoje tablice Freehand do zbiorczego importu**

Wykonaj poniższe kroki w Freehand, aby przygotować swoje tablice:

1. W Freehand, w menu po lewej stronie, wybierz **Dokumenty**. Menu rozwijane otwiera się.
2. Wybierz **Wszystkie dokumenty** lub **Utworzone przeze mnie** i określ przedział czasowy dla tablic, które chcesz zaimportować do Miro.
3. Dla każdej tablicy, którą chcesz zaimportować, wybierz menu z 3 kropkami (**...**) i wybierz **Wybierz**.
4. W oknie dialogowym u dołu ekranu wybierz **Przenieś**.
5. Wybierz przestrzeń, aby przenieść swoje tablice. To konsoliduje je, aby ułatwić przetwarzanie za pomocą narzędzia do zbiorczego importu.

   Przygotowałeś(-aś) z powodzeniem wiele plików do importu zbiorczego do Miro.

Aby zbiorczo zaimportować przygotowane tablice Freehand do Miro, postępuj zgodnie z instrukcjami zawartymi w poniższym osadzonym przewodniku Miro:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1IT00=/?pres=1&amp;frameId=3458764590689727256&amp;embedId=507813406404&amp;&amp;autoplay=yep" width="100%"></iframe>

:::note
Ważne notatki do zbiorczego importu:
- Token Freehand używany przy zbiorczej migracji jest ważny tylko przez dwa tygodnie od daty jego otrzymania.
- Od 31 grudnia 2024 roku, od godziny 23:59 EST, Freehand i wszystkie powiązane tokeny migracji zostaną wycofane i unieważnione. Użytkownicy nie będą już mogli generować nowych tokenów ani uzyskiwać dostępu do Freehand w celu migracji.
:::

## Przejrzyj najlepsze praktyki

Aby zapewnić płynne przenoszenie, ważne jest zrozumienie najlepszych praktyk i kluczowych aspektów podczas przenoszenia treści z Freehand do Miro. Przejrzyj szczegółowe wskazówki w osadzonej poniżej tablicy Miro:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1FWSM=/?pres=1&amp;frameId=3458764590691451227&amp;embedId=480338444592&amp;autoplay=yep" width="100%"></iframe>

## Mapowanie obiektów w Miro

Ta tabela zapewnia kompleksowe porównanie sposobu, w jaki obiekty z Freehand są zazwyczaj importowane i reprezentowane w Miro, wraz z notatkami na temat ewentualnych ręcznych korekt, które mogą być potrzebne:

|  |  |  |
| --- | --- | --- |
| **Odręcznie** | **Miro** | **Wymagane poprawki** |
| Tablice | kanban | Brak |
| Karty | Karty | Karty Jira w Freehand zostaną zaimportowane jako karty Jira w Miro. Jednak nie będą połączeni z istniejącą instancją, ponieważ użytkownicy będą musieli ponownie uwierzytelnić swoje konta Jira w Miro.    Karty ADO, Trello, Asana nie są obsługiwane. |
| Współpracownicy i udostępnianie | Można odtworzyć ręcznie | Brak |
| Komentarze | Można ponownie utworzyć ręcznie | Brak |
| Łączniki/Linie | Łączniki/Linie | Brak |
| Rysunki/Diagramy/Kształty | Kształty, tekst i łączniki | Brak |
| Dynamiczne tabele danych | CSV | Zawartość można pobrać i edytować jako plik .CSV z tablicy Miro. |
| Osadzanie:    Google i Microsoft Dokumenty, YouTube, Spotify, Loom | Nazwa źródła (np. Google, YouTube) oraz URL do osadzenia | Jeżeli użytkownicy chcą ponownie osadzić dokument, mogą [przesłać go za pomocą URL](../../using-miro/import-and-export/import/05-uploading-files-to-boards.md). |
| Reakcje emoji | Można odtworzyć ręcznie | Brak |
| Ramki | Ramki | Brak |
| Tabelki (tabele) | Tabele | Brak |
| Zgrupowane obiekty | Niegrupowane obiekty | Aby pogrupować obiekty, wybierz wszystkie odpowiednie obiekty i naciśnij **Cmd/Ctrl + G** lub kliknij **Grupuj obiekty** z menu kontekstowego. |
| Obrazy | Obrazy | Brak |
| Strony | Osadzony dokument | Zawartość można pobrać i edytować jako plik .docx z tablicy Miro. |
| Prototypy | Nazwa źródła (InVision) i URL do osadzenia | Jeśli użytkownicy chcą ponownie osadzić dokument, mogą przesłać przez URL, aby ponownie osadzić. |
| Inteligentne widżety:    Odwracana karta, Ankieta, To czy Tamto, Wykresy, Licznik, Tablica wyników, Koło fortuny, Buzzer, Lista osób, Story points, Rozmiar koszulki, Timer, Przyciski akcji | Tworzony jest plik PNG inteligentnego widżetu w momencie importu | Treść nie jest edytowalna. |
| Karteczki | Karteczki | Rozmiary czcionek tekstu na karteczkach mogą wymagać dostosowania. |
| Oś czasu (Gantt) | CSV | Zawartość można pobrać i edytować jako plik .CSV z tablicy Miro. |
| Wireframy | Makiety | Niektóre obiekty mogą wymagać ponownego narysowania. |

## Kluczowe ograniczenia

Zwróć uwagę na następujące ograniczenia i różnice strukturalne podczas przenoszenia treści z Freehand do Miro, aby zapewnić płynniejsze przejście:

- Pola tekstowe w Miro mogą pomieścić do 6000 znaków, wliczając spacje. Tekst przekraczający ten limit zostanie przycięty.
- Karteczki Miro nie obsługują korygowania palety kolorów ani wypunktowywania tekstu w taki sam sposób jak Freehand; niektóre opcje formatowania mogą się różnić.
- Widżety Smart z Freehand są importowane jako statyczne obrazy (PNG) i nie można ich edytować w Miro.
- Komentarze, reakcje emoji i prototypy z Freehand nie są migrowane do Miro.
- Token Freehand wymagany do zbiorczego importu jest ważny tylko przez dwa tygodnie od daty jego otrzymania.
- Od 31 grudnia 2024 r., od godziny 23:59 czasu EST, Freehand i wszystkie powiązane tokeny migracyjne zostaną wycofane i unieważnione. Użytkownicy nie będą już mogli generować nowych tokenów ani uzyskiwać dostępu do Freehanda.

### Porównaj strukturę organizacyjną między Freehand a Miro

Aby skutecznie zaplanować migrację, ważne jest, aby zrozumieć, jak struktury organizacyjne w Freehand odpowiadają tym w Miro.

**Bezwarstwowa organizacja**

- Zespoły Każda subdomena, do której masz dostęp w InVision, jest uważana za zespół. Jeśli masz dostęp tylko do jednej subdomeny, masz jeden zespół.
- Grupy: Foldery dokumentów, które pomagają w grupowaniu i udostępnianiu dokumentów w zespole.
- Przestrzenie: Dodatkowa warstwa organizacji w grupach dla Twoich dokumentów.

:::note
Jeśli Twój zespół korzystał z funkcji przeglądu przestrzeni w Freehand, będziesz musiał ręcznie przenieść tę zawartość do Miro. Zalecamy skopiowanie zawartości przeglądu przestrzeni do tablicy Miro.
:::

**Miro – warstwy organizacyjne**

- Organizacje: Zazwyczaj masz dostęp do jednej organizacji w Miro.
- Zespoły: Udostępnione przestrzenie robocze, w których użytkownicy współpracują na tablicach i projektach (dawniej znane jako Przestrzenie w niektórych kontekstach, bądź świadom zmieniającej się terminologii Miro; ogólnie zespoły są główną przestrzenią do współpracy).
- Projekty: Kolekcje tablic w ramach zespołu, ułatwiające organizację, wyszukiwanie i udostępnianie tablic.

Traktuj swoje grupy w InVision jako mniej więcej odpowiednik Projektów w Miro (lub coś, co mogłoby być konceptualnie podobne do folderów/przestrzeni do organizowania tablic w ramach zespołu). Dla każdej grupy InVision, którą planujesz przenieść, zalecamy utworzenie projektu Miro o tej samej nazwie. Na przykład, jeśli masz grupę w InVision o nazwie "Acme Corp Relaunch Project", proponujemy utworzyć projekt w Miro o identycznej nazwie "Acme Corp Relaunch Project" w odpowiednim Zespole Miro.

:::tip
W przypadku dalszych pytań dotyczących migracji Freehand, skontaktuj się z [pomocą Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) lub skontaktuj się bezpośrednio ze swoim managerem ds. sukcesu klienta Miro.
:::
