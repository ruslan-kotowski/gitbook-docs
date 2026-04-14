---
title: Miro dla Jira Cloud
article_id: 360017572414
translation_id: 21857714524818
locale: pl-pl
sidebar_position: 4
created_at: '2024-10-08T15:10:22Z'
updated_at: '2024-10-08T15:10:22Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Wizualizuj dowolne elementy razem ze swoim zespołem — pracuj nad backlogiem produktu za pomocą cyfrowych karteczek, twórz schematy blokowe, diagramy i szkielety. Dołączaj tablice do zgłoszeń Jira i współpracuj ze swoim zespołem w czasie rzeczywistym, np. na spotkaniu na tablicy.

> **Platforma:** plany Starter, Business i Enterprise.
> Tylko w Jira Cloud

> Możesz również osadzać tablice Miro za pomocą funkcji linku Atlassian Smart.

:::note
Pamiętaj, że Miro oferuje dwa rodzaje integracji Jira: **Miro dla Jira Cloud** (która umożliwia osadzanie tablic Miro po stronie Jira) i **kart Jira**. Aby dowiedzieć się więcej o kartach Jira, odwiedź [ten artykuł](https://help.miro.com/hc/articles/360017572434).
:::

## Jak zainstalować

Proces instalacji jest standardowy dla wszystkich dodatków Jira. Najpierw zaloguj się do swojej platformy Jira za pomocą uprawnień administracyjnych, a następnie pobierz dodatek [tutaj](https://marketplace.atlassian.com/apps/1215456/miro-for-jira-cloud?tab=overview&hosting=cloud) (aplikację można również znaleźć na **stronie Atlassian Marketplace** > **Znajdź nowe** aplikacje> **Miro dla Jira Cloud):** kliknij **Pobierz aplikację** i **Pobierz ją teraz**.
To wszystko! Instalacja została zakończona.

![Miro_for_Jira.jpg](https://help.miro.com/hc/article_attachments/21857763254034)
*Powiadomienie Jira o pomyślnej instalacji*

Pamiętaj, że jako administrator nie musisz mapować użytkowników Miro na użytkowników Jira podczas konfiguracji. Każdy użytkownik będzie musiał dokonać autoryzacji w Miro w ramach Jira.

## Jak korzystać z dodatku

### Dołączanie tablic do zgłoszeń Jira

Aby dołączyć tablicę do zgłoszenia Jira, otwórz zgłoszenie w systemie Jira. Kliknij **Dodaj** tablicę w sekcji **Tablice** Miro.
![add_Miro_boards_in_Jira.jpg](https://help.miro.com/hc/article_attachments/21857714454162)
*Przycisk dodatku pojawia się po instalacji*

:::tip
Jeśli nie masz sekcji tablic Miro, znajdź ją w menu kontekstowym zgłoszenia.
:::

![Miro_boards_section.jpg](https://help.miro.com/hc/article_attachments/21857763269906)
*Dodawanie sekcji tablic Miro do zgłoszenia Jira*

Zobaczysz selektor z tablicami Miro. Wybierz tablicę, którą chcesz dodać (możesz przełączać się między swoimi zespołami w selektorze). Jeśli nie masz autoryzacji w Miro, najpierw musisz się zalogować.

Ustaw ustawienia udostępniania tablicy w menu rozwijanym. Możesz udostępnić tablicę do wyświetlania i komentowania, aby użytkownicy nie mieli profilu w Miro również mieli do niej dostęp.

:::note
Dla użytkowników wersji [Enterprise](https://help.miro.com/hc/articles/360017571534) Miro ustawienia dostępu będą zgodne z kontrolą dostępu obowiązującą w całej organizacji, co może oznaczać, że niektóre opcje udostępniania mogą być ograniczone. Dowiedz się więcej: [Zarządzanie zasadami udostępniania Enterprise dla integracji osadzania](https://help.miro.com/hc/articles/4405088016274).
:::

![embed_a_board_in_Jira.jpg](https://help.miro.com/hc/article_attachments/21857763280402)
*Ustawienia udostępniania podczas dołączania tablicy do zgłoszenia Jira*

Pamiętaj, że możesz osadzać tylko tablice, na których masz dostęp do edytującego.

Twoja tablica jest teraz dołączona do wybranego zgłoszenia Jira:

![Miro_board_in_Jira.jpg](https://help.miro.com/hc/article_attachments/21857714472466)
 *Tablica Miro dołączona do zgłoszenia Jira*

### Tworzenie nowych tablic z Jiry

Aby utworzyć nową tablicę bezpośrednio ze zgłoszenia Jira, kliknij **Dodaj** tablicę i utwórz nową **tablicę** z poziomu selektora.

![create_a_new_board_from_the_picker.jpg](https://help.miro.com/hc/article_attachments/21857763290258)
*Tworzenie tablicy z selektora*

### Wyświetlanie, komentowanie i edytowanie tablic

Wystarczy kliknąć załączoną tablicę, aby ją wyświetlić/komentować/edytować, w zależności od ustawionych praw dostępu. Okno tablicy otworzy się jako nakładka, umożliwiając pracę i współpracę tak, jakbyś był w Miro.

![Miro_embed_in_Jira.jpg](https://help.miro.com/hc/article_attachments/21857763294098)
*Nakładka tablicy w Jira*

 Możesz również kliknąć przycisk źródła, aby otworzyć tablicę w Miro w nowej karcie dla Twojej wygody.

![source_button.jpg](https://help.miro.com/hc/article_attachments/21857763302290)
*Przycisk przejścia do aplikacji Miro*

### Odłączanie tablic

Aby odłączyć tablicę, wystarczy kliknąć ikonę krzyżyka, a załącznik zostanie natychmiast usunięty ze zgłoszenia (po stronie Miro tablica nie będzie miała wpływu).

![remove_an_attached_board.jpg](https://help.miro.com/hc/article_attachments/21857763310098)
*Opcja usunięcia załączonej tablicy*

## Jak wyłączyć dodatek

Aby wyłączyć integrację, otwórz **Atlassian Marketplace** > **Zarządzaj** aplikacjami> otwórz stronę dodatku i kliknij **Odinstaluj**:

![uninstall_Jira_add-on.jpg](https://help.miro.com/hc/article_attachments/21857763314962)
*Opcja **Odinstaluj** w sekcji Dodatki Jira*

## Atlassian Smart Link dla Miro

Możesz osadzać tablice Miro w zgłoszeniach Jira za pomocą funkcji Atlassian Smart Link. Funkcja ta umożliwia automatyczne osadzanie tablicy bez konieczności instalowania wtyczki.

:::note
Pamiętaj, że tylko użytkownicy, którzy mają dostęp do osadzonej tablicy po stronie Miro, będą mogli pracować z podglądem po połączeniu swoich kont Miro i Atlassian. Jeśli chcesz udostępnić podgląd wszystkim użytkownikom Jira, możesz korzystać z dodatku Jira.
:::

Przejdź do zgłoszenia Jira i wklej link do tablicy lub wpisz /link, aby wstawić. Jeśli używasz funkcji po raz pierwszy, zostaniesz poproszony o połączenie ze swoim zespołem Miro. Kliknij **Połącz z** podglądem, autoryzuj w Miro i wybierz zespół, z którego będziesz osadzać swoje tablice.

![install_Atllassian_links.jpg](https://help.miro.com/hc/article_attachments/21857714504722)
*Wybieranie zespołu, z którego chcesz osadzać tablice,*

Po wklejeniu linku do tablicy Miro do zgłoszenia Jira, zostanie on automatycznie przekształcony w widżet Jira. Kliknij link, a zobaczysz opcje wyświetlania linku jako karty lub osadzenia.

![display_as_link.gif](https://help.miro.com/hc/article_attachments/21857714509074)
*Opcje wyświetlania linku do tablicy Miro jako linku, karty lub osadzenia.*

Jeśli zdecydujesz się wyświetlić tablicę jako osadzenie, możesz zmienić rozmiar osadzenia, przeciągając jej stronę.

![changing_embed_size_in_Jira.gif](https://help.miro.com/hc/article_attachments/21857714514706)
*Zmiana rozmiaru osadzenia Miro w Jira*

> Jeśli pliki cookie innych firm są zablokowane w przeglądarce, mogą wystąpić nieoczekiwane problemy z wyświetlaniem osadzonych tablic.

## Często zadawane pytania

Czy mogę ukryć sekcję tablic Miro w zgłoszeniach Jira?

Tak, kliknij menu z 3 kropkami w prawym górnym rogu sekcji i wybierz **Ukryj tablice Miro**.
![hide_Miro_boards.jpg](https://help.miro.com/hc/article_attachments/21857763329554)
*Ukrywanie tablic Miro w Jirze*

Czy dodatek działa w projektach Jira Next-gen?

Tak. Możesz dołączać swoje tablice do takich projektów.

Czy są jakieś dodatkowe koszty za dodatek Jira?

Miro dla Jira Cloud jest dostępne dla wszystkich płatnych planów bez dodatkowych kosztów (wersje Starter, Business i Enterprise).

Zamierzamy migrować Jira z jednej instancji chmury do drugiej. Czy wpłynie to na tablice Miro osadzone w zgłoszeniach Jira?

Nie powinno być problemów z osadzonymi tablicami Miro, jeśli zawartość zostanie przeniesiona bez zmian.
