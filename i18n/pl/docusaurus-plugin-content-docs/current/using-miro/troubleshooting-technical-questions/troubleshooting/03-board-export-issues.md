---
title: Problemy z eksportem tablicy
article_id: 360020567820
translation_id: 360020567820
locale: pl-pl
sidebar_position: 3
created_at: '2021-03-18T12:15:46Z'
updated_at: '2025-11-05T13:45:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Możesz [wyeksportować swoją tablicę Miro](../../import-and-export/export/03-how-to-export-your-board.md) jako obraz, PDF lub plik CSV. Jeśli napotkasz problemy z eksportem tablicy Miro, zapoznaj się z możliwymi rozwiązaniami poniżej.

## Nie mogę wyeksportować tablicy

**Brak przycisku eksportu na mojej tablicy**

Przycisk eksportu znajduje się pod **menu z 3 kropkami** (**...**), a następnie w submenu **Tablica**.

Brak opcji eksportu w [menu tablicy](../../../getting-started/start-here/your-first-board/05-toolbars.md):

1. Sprawdź, czy właściciel lub współwłaściciel tablicy zezwolił użytkownikom na eksport tablicy w ustawieniach treści tablicy.

   Aby dowiedzieć się, kto jest właścicielem tablicy, kliknij nazwę tablicy w lewym górnym rogu, aby otworzyć kartę informacji o tablicy. Jeśli nie masz dostępu do tych informacji, możesz sprawdzić nazwisko użytkownika, który Cię zaprosił na tablicę w e-mailu z zaproszeniem.

   Skontaktuj się z właścicielem tablicy i poproś go, aby włączył tę opcję dla Ciebie w oknie **Udostępnij** > **Ustawienia udostępniania** > **Uprawnienia**. Właściciel/współwłaściciel musi wybrać, która kategoria użytkowników może [kopiować zawartość tablicy](../../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).
   ![.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044218642_.gif.png)
   *Konfiguracja uprawnień do kopiowania zawartości tablicy*
2. Upewnij się, że przeglądarka, abonament i urządzenie wspierają eksport. Możesz sprawdzić dostępność poniżej. Jeśli przeglądarka, abonament lub urządzenie nie obsługuje eksportu, zalecamy przejście na inną przeglądarkę lub urządzenie albo [zmianę zespołu na wyższą wersję](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

   |  |  |  |  |  |  |
   | --- | --- | --- | --- | --- | --- |
   |  | Wersja Free | | Abonamenty Starter, Business, Enterprise, Education | | Eksport do CSV (wszystkie abonamenty) |
   |  | Niska rozdzielczość | Wysoka rozdzielczość bez znaku wodnego | Niska  rozdzielczość | Wysoka rozdzielczość  bez znaku wodnego |
   | Google Chrome | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Safari | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Firefox | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Opera | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Edge < 79 | ✘ | ✘ | ✘ | ✔ | ✘ |
   | [Aplikacja komputerowa](../../../getting-started/apps-for-devices/05-desktop-app.md) | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Tablet | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Mobilne | ✘ | ✘ | ✘ | ✘ | ✘ |

**W przypadku eksportów niskiej jakości**

Aby rozwiązać problem, zamknij karty przeglądarki oraz zakładki działające w tle. Możesz także spróbować zmienić przeglądarkę.

Aby uzyskać eksporty wysokiej jakości, wykonaj następujące kroki:

- Ukryj ramki, które nie chcesz eksportować. Zawartość ukrytych ramek nie jest eksportowana.
- Podziel tablicę na mniejsze tablice do eksportu.

**Ogólne wskazówki**

- Umieść wszystko, co chcesz eksportować, w ramkach, ponieważ tylko widżety wewnątrz ramek są eksportowane.
- Unikaj PDF w PDF. Jeśli masz PDF na tablicy, który chcesz eksportować jako PDF, zamień PDF na tablicy na obrazy niskiej jakości.
- Przekonwertuj obrazy wysokiej rozdzielczości do formatu JPEG lub zmniejsz ich rozmiar za pomocą narzędzia zewnętrznego.
- Sprawdź stronę Miro Status, aby uzyskać informacje o istotnych incydentach.
- Podziel tablicę na ramki i eksportuj ramki osobno. Oddzielne pliki PDF można później połączyć za pomocą narzędzia zewnętrznego.
- Podziel duże tablice na mniejsze tablice i użyj [Przestrzeni](../../spaces/01-spaces.md), aby pomóc sobie zorganizować i pogrupować tablice, które do siebie należą.

**„Przepraszamy, coś poszło nie tak podczas generowania dokumentu PDF”**

Spróbuj podzielić tablicę na ramki i eksportować ramki osobno, ponieważ problem może być spowodowany wielkością tablicy.

Jeśli to nie pomoże, sprawdź [logi konsoli przeglądarki](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md). Jeśli logi zawierają następującą wiadomość:

```
ERR_CONNECTION_ABORTED
```

*gdzie:*

Eksport jest blokowany przez oprogramowanie zabezpieczające na Twoim urządzeniu lub zaporę sieciową w Twojej sieci.

Ty lub Twój administrator systemu musicie skonfigurować ustawienia programu antywirusowego i/lub zapory sieciowej, aby umożliwić Miro wykonanie procedury eksportu.

W razie wątpliwości, [skontaktuj się z pomocą Miro](../../tools/troubleshooting/06-contacting-miro-support.md).

**Nic się nie dzieje, gdy próbuję wyeksportować tablicę do formatu PDF, a Miro nie pokazuje błędu**

Ten znany problem występuje głównie w przeglądarce Safari, gdy okna pop-up są zablokowane. Aby rozwiązać problem dla Safari, [wykonaj te kroki](https://support.apple.com/en-gb/guide/safari/sfri40696/mac). Upewnij się, że włączasz wyskakujące okna dla miro.com lub wszystkich stron. Wróć do Miro i ponownie spróbuj wyeksportować swoją tablicę.

Dla Chrome, [wykonaj te kroki](https://support.google.com/chrome/answer/95472?hl=en&co=GENIE.Platform%3DDesktop).

## Mam problemy z wyeksportowanymi plikami (PDF, obrazami, CSV)

**Obrazy/PDF są rozmazane w wyeksportowanym dokumencie**

Jeśli przesłane obrazy lub pliki PDF są rozmazane w zapisanym pliku:

1. Ustaw poziom powiększenia tablicy na 100% i pozwól obrazom/plikom PDF wyrenderować się przed eksportowaniem tablicy
2. Przesłany obraz/plik PDF może być zbyt złożony lub duży do eksportu. Aby zmniejszyć jego rozmiar, skonwertuj obraz/plik PDF na format PNG i zamień go na tablicy. Następnie ponownie wyeksportuj tablicę

Abonament Free wspiera eksport tylko w niskiej jakości. Jeśli potrzebujesz eksportować tablicę w wysokiej jakości, zalecamy [przenieść ją do płatnego zespołu](../../managing-boards/04-how-to-move-a-board.md) lub [zmienić zespół na wyższą wersję](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

**Kolejność stron nie jest taka sama jak kolejność ramek na tablicy**

Kolejność ramek eksportowanych do PDF jest taka sama jak w panelu ramek. Aby zmienić kolejność ramek:

1. Otwórz przegląd tablicy w lewym dolnym rogu
2. Przeciągnij ramki, aby zmienić ich pozycję na liście. Możesz również użyć [Magic organize](../../essential-tools/07-frames.md), aby szybko ułożyć ramki w kolejności, w jakiej są umieszczone na tablicy
   ![move_frames.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057584914_move%20frames.gif)
   *Zmiana kolejności ramek*

**Przycięty plik po eksporcie**

Gdy **eksportujesz tablicę jako obraz**, upewnij się, że wybrany obszar eksportu zawiera całą zawartość, którą chcesz wyeksportować.

![save_as_image.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057583890_save%20as%20image.gif)
*Eksport tablicy jako obrazu*

Gdy **eksportujesz tablicę jako PDF**, stwórz ramkę, która obejmie całą zawartość, którą chcesz wyeksportować. Następnie [eksportuj ramkę](../../import-and-export/export/03-how-to-export-your-board.md).

**Wyeksportowany plik PDF nie zawiera nazw ramek**

Podczas eksportu tablicy do pliku PDF tytuły ramek nie są uwzględniane. Możesz zastąpić tytuły ramek używając narzędzia [tekst](../../essential-tools/16-text.md) i umieścić tekst na ramkach. Tytuły pojawią się w Twoim pliku PDF.

**Dane w wyeksportowanym pliku CSV nie są ustrukturyzowane**

Obecnie eksport do CSV nie zachowuje struktury tablicy ani relacji. Jednakże, jeśli eksportujesz [tabele](../../advanced-tools/05-grid.md) jako plik CSV, struktura zostaje zachowana.

Jeśli potrzebujesz wyeksportować [mapę myśli](../../advanced-tools/03-mind-map.md) jako plik z inteligentnymi danymi, użyj [Mindmap downloader](https://miro.com/marketplace/mindmapdownloader/?backUrl=%2Fmarketplace%2F).

**Czcionki na tablicy różnią się od czcionek w wyeksportowanym pliku**

Eksport Miro używa czcionek zainstalowanych w systemie operacyjnym Twojego urządzenia. Jeśli czcionka nie jest obecna w Twoim systemie, zamiast niej zostanie użyta podobna czcionka z systemu. Jeśli potrzebujesz takiej samej czcionki jak na swojej tablicy Miro, wybierz inną czcionkę na tablicy lub zainstaluj potrzebną czcionkę na swoim urządzeniu.

## Nie mogę zlokalizować wyeksportowanego pliku

**Nie mogę znaleźć wyeksportowanego pliku na moim urządzeniu**

**Jeśli używasz Miro w przeglądarce**

Pliki będą przechowywane w folderze, gdzie domyślnie zapisywane są pobrane z przeglądarki pliki. Możesz sprawdzić ustawienia pobierania w opcjach przeglądarki.

**Jeśli używasz aplikacji Miro komputerowej lub aplikacji na tablety**

Sprawdź folder Pobrane na swoim urządzeniu. Możesz także przeszukać pliki używając nazwy tablicy.

**Miro tworzy nowy folder za każdym razem, gdy eksportuję tablicę**

> **Dotyczy**: [aplikacja komputerowa Windows](../../../getting-started/apps-for-devices/05-desktop-app.md)

Możliwe, że ścieżka została zapisana w ustawieniach aplikacji Miro. Aby usunąć ścieżkę:

1. Usuń aplikację komputerową Miro
2. Na dole po lewej w Windows (pasek wyszukiwania), wpisz **%AppData%** i otwórz folder **Local,** następnie usuń folder **RealTimeBoard**
3. Otwórz ponownie **%AppData%** , przejdź do folderu **Roaming,** i usuń folder **RealTimeBoard**

Zainstaluj ponownie najnowszą [aplikację Miro](https://miro.com/apps/).

Jeśli żadne z rozwiązań nie pomoże, [skontaktuj się z Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).
