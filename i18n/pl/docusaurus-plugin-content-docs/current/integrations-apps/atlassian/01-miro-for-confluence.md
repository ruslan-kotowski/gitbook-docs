---
title: Miro dla Confluence
article_id: 360020712594
translation_id: 21892959665810
locale: pl-pl
sidebar_position: 3
created_at: '2024-10-10T08:11:17Z'
updated_at: '2026-03-12T09:15:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: 'Dostępne dla: Wszystkie abonamenty Miro; Confluence Cloud (osadzanie w Miro),
    Confluence Cloud/Server/DC (osadzanie w Confluence) Kto może to zrobić: Administrator
    Confluence'
---

Miro i Confluence współpracują ze sobą dzięki dwukierunkowej synchronizacji, zapewniając dostęp do najbardziej aktualnych treści z obu platform, gdziekolwiek pracujesz.

## Jak Miro współpracuje z Confluence

Osadzaj swoje tablice Miro i dokumenty Confluence, i śledź zmiany dzięki natychmiastowej synchronizacji. Możesz ustawiać poziomy dostępu do osadzonych treści, aby właściwi użytkownicy mieli dostęp do odpowiednich informacji w każdym momencie.

Osadź dokumenty Confluence w tablicach Miro

Osadź tablice Miro w dokumentach Confluence

## Osadzanie dokumentów Confluence na tablicach Miro

Możesz osadzić dokumenty Confluence w Miro, po prostu wklejając link na tablicę Miro. Pamiętaj, że **osadzanie dokumentów Confluence w Miro wymaga Confluence Cloud.**

Kiedy wkleisz link do Confluence na tablicę Miro, pojawi się on jako [Miro smart link](https://help.miro.com/hc/articles/360017730993). Podczas pierwszego wklejania linku do Confluence, będziesz musiał kliknąć **Połącz**, aby autoryzować dostęp do Confluence.

:::warning
Ze względów bezpieczeństwa nie pokazujemy szczegółów linku Confluence na publicznych tablicach Miro, a użytkownicy mogą widzieć tylko tytuł linku Confluence na prywatnych tablicach. Użytkownicy zobaczą tytuł strony dopiero po autoryzacji swojego konta Confluence, co umożliwi im rozwinięcie i edycję dokumentu Confluence (zależnie od nadanych poziomów dostępu).
:::

![Connect_Confluence.png](https://help.miro.com/hc/article_attachments/21892975555730)*Łączenie strony Confluence w Miro*

Po autoryzacji Confluence użytkownicy, którzy uzyskają dostęp do tablicy, będą mogli zobaczyć teraz Tytuł dokumentu, Ikonę dostawcy oraz Źródło linku. Użytkownicy będą mogli także rozwinąć inteligentny link Miro do trybu pełnoekranowego.

:::tip
Tytuły inteligentnych linków Miro są pozyskiwane z adresu URL. Jeśli edytujesz tytuł dokumentu Confluence, musisz ponownie wkleić link, aby zobaczyć zaktualizowany tytuł w Twoim inteligentnym linku Miro.
:::

![Connected_Confluence_card.png](https://help.miro.com/hc/article_attachments/21892959571730)*Połączona strona Confluence jako inteligentny link Miro*

Kiedy użytkownicy klikną na ikonę rozwiń, będą musieli autoryzować swoje własne konto Confluence, zanim będą mogli wyświetlić i edytować dokument w Miro.

![Expanded_Confluence_card.png](https://help.miro.com/hc/article_attachments/21892959580306)*Rozwinięty dokument Confluence*

## Osadź tablice Miro w dokumentach Confluence

Możesz osadzić tablice Miro w dokumentach Confluence za pomocą wtyczki Miro dla Confluence lub bezpośrednio przez Atlassian Smart Links. Można to zrobić w Confluence Cloud, Server, lub DC.

### Krok 1: Konfiguracja wtyczki Miro

Najpierw zainstaluj [aplikację Miro dla Confluence](https://marketplace.atlassian.com/apps/1217530/miro-for-confluence?tab=reviews&hosting=cloud) z Marketplace Atlassian.

**Jak zainstalować aplikację Miro dla Confluence**

> **Kto może to zrobić**: Administrator Confluence

1. Zaloguj się do swojej instancji Confluence jako administrator
2. Kliknij menu rozwijane admina i wybierz **add-ony (aplikacje)**
3. Wybierz **Znajdź nowe aplikacje** lub **Znajdź nowe add-ony**
4. Wyszukaj **Miro for Confluence**
5. Kliknij **Pobierz aplikację**

![Miro_for_Confluence.png](https://help.miro.com/hc/article_attachments/21892975576082)*Aplikacja Miro for Confluence*

Zobaczysz następujący komunikat, gdy aplikacja zostanie pomyślnie zainstalowana:

![success_message.jpg](https://help.miro.com/hc/article_attachments/21892975586066)
*Aplikacja została pomyślnie zainstalowana*

### Krok 2: Osadź tablicę na stronie Confluence

Istnieją trzy sposoby osadzania tablicy Miro na stronie Confluence:

1. Poprzez wpisanie **/miro** bezpośrednio w dokumencie Confluence.
   ![Typing_miro_on_the_doc.png](https://help.miro.com/hc/article_attachments/21892959609490)
   *Wpisanie /miro na stronie Confluence w celu osadzenia tablicy*
2. Poprzez wyszukiwanie Miro z paska narzędzi aplikacji. W dokumencie Confluence, kliknij **Wstaw** i wybierz **Miro** z listy aplikacji.
   ![Miro_plugin.jpg](https://help.miro.com/hc/article_attachments/21892975603218)
   *Wybieranie Miro z listy aplikacji w celu osadzenia tablicy*
3. Poprzez wklejenie linku Miro bezpośrednio do Confluence z Atlassian Smart Links.

### Krok 3: Wybierz tablicę z selektora tablic

Otworzy się selektor tablic. Wybierz tablicę, którą chcesz osadzić, z listy rozwijanej lub wyszukaj tablicę. Użytkownicy zobaczą tylko te tablice w Miro, które są dla nich dostępne, i mogą osadzić tablice tylko wtedy, gdy mają do nich uprawnienia do edycji.

![Board_picker.png](https://help.miro.com/hc/article_attachments/21892975610258)*Wybieranie tablicy do osadzenia z selektora tablic*

Wybierz **Początkowe wyświetlanie** dla osadzonej tablicy.

![Set-the-starting-view-for-your-embed.png](https://help.miro.com/hc/article_attachments/21892975613970)*Ustawianie początkowego widoku dla osadzonej tablicy Miro*

Wybierz poziom dostępu dla **Wszystkich odwiedzających** stronę Confluence.

- **Mogą wyświetlać:** Pozwala każdemu odwiedzającemu stronę Confluence zobaczyć tablicę.
- **Wymaga dostępu:** Ogranicza wyświetlanie do osób mających dostęp do tablicy w Miro.

![Access-level-for-embed.png](https://help.miro.com/hc/article_attachments/21892959631378)*Ustawianie poziomu dostępu do tablicy Miro na stronie Confluence*

### Krok 4: Osadź tablicę

Po kliknięciu **Osadź tablicę**, tablica Miro zostanie wstawiona na stronie Confluence jako iFrame. Użytkownicy mogą ją oglądać i poruszać się po tablicy.

:::note
Dla użytkowników z abonamentem Enterprise poziomy dostępu będą przestrzegać ustawień dostępu na poziomie całej organizacji, co może oznaczać ograniczenia niektórych uprawnień. Więcej informacji o [zarządzaniu osadzonymi tablicami dla wersji Enterprise](https://help.miro.com/hc/articles/4405088016274).
:::

![Miro-board-embedded-in-confluence.png](https://help.miro.com/hc/article_attachments/21892959635218)*Tablica Miro osadzona na stronie Confluence*

Aby otworzyć tablicę bezpośrednio w Miro, kliknij logo Miro.

![Open-embedded-board-in-miro.png](https://help.miro.com/hc/article_attachments/21892959637394)
*Opcja otwarcia tablicy w Miro*

#### **Doświadczenie użytkownika w Confluence Cloud a Confluence Server**

Menu rozmiaru okna dla osadzonych tablic różni się w Confluence Cloud i Confluence Server.

W Confluence Cloud zobaczysz następujące menu rozmiaru okna z możliwością **Przejdź na pełną szerokość**:

![Go-full-width-Miro-board-confluence.png](https://help.miro.com/hc/article_attachments/21892975630866)
*Menu rozmiaru okna w przeglądarce Confluence*

W Confluence Server zobaczysz menu z opcją wyboru małego, średniego lub dużego (**S/M/L**) rozmiaru okna:

![Miro_in_Confluence_Server.jpg](https://help.miro.com/hc/article_attachments/21892975632786)*Menu rozmiaru okna w aplikacji Confluence*

## Osadzanie tablic Miro poprzez Atlassian Smart Links

Możesz również osadzić tablice Miro w Confluence za pomocą funkcji Atlassian Smart Links. Funkcja ta pozwala na automatyczne osadzenie tablicy bez konieczności instalowania aplikacji.

Przejdź do strony Confluence i po prostu wklej link do tablicy lub wpisz **/link**, aby go wstawić. Jeśli używasz tej funkcji po raz pierwszy, pojawi się prośba o połączenie zespołu Miro. Kliknij **Połącz, aby wyświetlić podgląd**, autoryzuj w Miro i wybierz zespół, z którego będziesz osadzać tablice.

:::note
Tylko użytkownicy, którzy mają dostęp do osadzonej tablicy po stronie Miro, będą mogli pracować z podglądem osadzonej tablicy Miro po połączeniu swoich kont Miro i Atlassian. Jeśli chcesz, aby podgląd tablicy był dostępny dla wszystkich użytkowników Confluence, możesz użyć aplikacji Miro.
:::

![install_Atllassian_links.jpg](https://help.miro.com/hc/article_attachments/21892975635602)
*Wybieranie zespołu do osadzenia tablic*

Gdy wkleisz link do tablicy Miro na stronie Confluence, link automatycznie zmieni się w widget. Kliknij link, aby zobaczyć opcje wyświetlania. Możesz wybrać wyświetlanie tablicy Miro jako **URL**, w formie tekstu **w linii**, jako **karta** lub jako **osadzenie**.

![Confluence_widget.png](https://help.miro.com/hc/article_attachments/21892959652370)*Widżet tablicy Miro w Confluence*

Jeśli wybierzesz wyświetlanie tablicy jako osadzenie, możesz zmienić jego rozmiar przeciągając boki.

![changing_embed_size.gif](https://help.miro.com/hc/article_attachments/21892975644306)
*Zmiana rozmiaru osadzenia Miro w Confluence*

:::warning
Jeśli w przeglądarce zablokowane są ciasteczka stron trzecich, mogą wystąpić nieoczekiwane problemy z wyświetlaniem osadzonych tablic.
:::

## Wyłączanie aplikacji Miro dla Confluence

Aby wyłączyć aplikację, przejdź do **Atlassian Marketplace** > **Zarządzaj aplikacjami** > **Miro for Confluence Cloud** > **Odinstaluj.**

*![Uninstall_Confluence_plugin.jpg](https://help.miro.com/hc/article_attachments/21892975647378)*
*Aplikacja Miro for Confluence na liście zainstalowanych aplikacji Atlassian*

## Migracja i wpływ na tablice w Confluence

Niezależnie od tego, czy migrujesz z wersji On-premise do Cloud, czy z Cloud do Cloud, wtyczka Miro nie wymaga dedykowanych kroków migracyjnych. Confluence wyświetla tablice Miro przy użyciu iFrame, które są osadzeniami opartymi na URL, co oznacza, że Confluence przechowuje tylko link do tablicy, podczas gdy tablica pozostaje w Miro.
