---
title: Karty Azure
article_id: 360033799934
translation_id: 360033799934
locale: pl-pl
sidebar_position: 4
created_at: '2019-08-13T10:01:30Z'
updated_at: '2025-11-25T16:05:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: azure-cards
availability:
  notes: 'Osoby: Wszyscy użytkownicy Plany: Business, Enterprise Platformy: Przeglądarka,
    aplikacja komputerowa, urządzenia mobilne'
---

Karty Azure umożliwiają importowanie elementów roboczych z Azure Boards (części usług Azure DevOps, wcześniej rozwiązania VSTS - chmura) na tablice Miro. Mogą stać się niezbędne do zdalnych retrospektyw, doboru rozmiaru historyjek, priorytetyzacji backlogu, mapowania historyjek i innych działań zespołu. Możesz również używać ich w Miro Kanban i strukturach mapowania historyjki użytkownika.

Karty Azure poprawiają Twoje doświadczenie z Miro, integrując się bezpośrednio z Azure Boards, co umożliwia płynne zarządzanie przepływem pracy dla różnych działań zespołowych.

## Najważniejsze funkcje

Integracja Azure Cards oferuje kilka kluczowych funkcjonalności:

- Importuj karty Azure za pomocą selektora elementów roboczych Azure Boards w aplikacji. Obejmuje to różne opcje sortowania.
- Wyszukaj elementy robocze Azure Boards w selektorze w aplikacji.
- Zautomatyzowane, łatwe do odczytania zmiany widoku kart podczas powiększania i oddalania.

:::note
Gwarantuj, że karty Azure są zawsze aktualizowane dzięki ankietom kart, co zapewnia, że użytkownicy zawsze otrzymują aktualizacje kart, nawet jeśli [webhook](../atlassian/14-how-to-set-up-webhooks-for-jira-data-center.md) zawiedzie.
:::

## Konfiguracja integracji kart Azure

Konfiguracja jest wymagana na dwóch poziomach:

1. Aplikacja musi zostać dodana albo na poziomie organizacji dla wszystkich zespołów, albo na poziomie zespołu dla konkretnych zespołów.
2. Po dodaniu aplikacji, integracja musi być połączona i autoryzowana na poziomie osobistym, aby importować karty Azure.

Ten proces wymaga specyficznych uprawnień administracyjnych zarówno w Miro, jak i Azure DevOps.

:::note
Aby pomyślnie skonfigurować karty Azure za pomocą Miro, **administrator Azure i administrator Miro muszą być tym samym kontem**.

Chociaż dodanie kart Azure wymaga uprawnień zespołu Miro lub administratora firmy **i** uprawnień administratora grupy kolekcji projektów w Azure Boards, te uprawnienia mogą zostać obniżone po zakończeniu połączenia. Administrator nie może zostać usunięty i musi zachować dostęp do projektu Azure.
:::

### Dodaj karty Azure do swojej organizacji lub zespołu

Administratorzy firmy Miro mogą dodawać karty Azure dla wszystkich zespołów, podczas gdy administratorzy zespołu mogą je dodawać dla konkretnych zespołów, którymi zarządzają. Ten krok udostępnia aplikację Azure Cards do połączenia.

> Aby połączyć karty Azure na poziomie zespołu, musisz być administratorem zespołu.

1. Przejdź do swoich **ustawień profilu** (kliknij ikonę menu głównego i wybierz **Ustawienia profilu**, lub z pulpitu, kliknij swój awatar w prawym górnym rogu i wybierz **Ustawienia**).
2. Kliknij **Aplikacje**, a następnie przejdź do karty **Dodaj aplikacje** po prawej stronie.
3. Wpisz „Karty Azure” i wybierz ją z listy rozwijanej. Kliknij **Dodaj**.
4. W następnym oknie dialogowym wybierz **Wszystkie zespoły** lub **W określonych zespołach** (w razie potrzeby wybierz swój zespół), a następnie kliknij **Następny krok**.
5. Na ekranie „Sprawdź i dodaj karty Azure” kliknij **Dodaj**. Aplikacja zostanie dodana dla Twojej firmy lub zespołu.
6. Przejdź na kartę **Zarządzanie aplikacjami**, wyszukaj Azure Cards i kliknij **Zatwierdź**. Aplikacja zostanie teraz zatwierdzona na poziomie firmy lub zespołu.
7. Następnie połącz swoją organizację Azure z Miro. Z panelu Aplikacje przejdź do **sekcji Zarządzaj aplikacjami.**
8. Wyszukaj „Azure Cards” na liście aplikacji i kliknij **Ustawienia.**
9. W panelu ustawień dla kart Azure dodaj adres URL swojej **instancji Azure** i kliknij **Połącz**. Podaj swoje dane dostępowe do logowania w Microsoft Azure.
10. W oknie dialogowym autoryzacji kliknij **Zaakceptuj**, aby zakończyć łączenie platformy Azure z Miro.

### Zastosuj niestandardowe ustawienia kart Azure dla określonych zespołów

Jeśli potrzebujesz innych ustawień dla określonych zespołów niż globalna konfiguracja na poziomie firmy, administratorzy zespołów mogą to skonfigurować w obszarze **Aplikacje i integracje** zespołu.

1. Na stronie ustawień profilu kliknij **Zespoły**.
2. Kliknij zespół, do którego chcesz zastosować ustawienia niestandardowe.
3. W panelu Zespoły kliknij **Aplikacje i integracje**.
4. Znajdź **Karty Azure** i kliknij na nią.
5. W panelu ustawień aplikacji wybierz **Zastosuj ustawienia niestandardowe** z rozwijanego menu po prawej stronie, a następnie połącz konto Azure, które chcesz mieć ustawienia niestandardowe.
6. Autoryzuj Miro w Azure DevOps za pomocą swojego konta Microsoft: kliknij **Połącz** obok „Konta Microsoft” i zaloguj się na swoje konto Microsoft, umożliwiając Miro korzystanie z niego.
7. Wprowadź **adres URL organizacji Azure** (który można skopiować z Azure DevOps) i kliknij **Połącz.** Miro zaakceptuje spersonalizowany adres URL Twojej instancji lub ogólny adres `https://dev.azure.com/`, kończący się nazwą Twojej instancji.
   ![Animacja pokazująca, jak zastosować niestandardowe ustawienia kart Azure dla określonego zespołu.](https://help.miro.com/hc/article_attachments/21857720699410)
   *Dodawanie niestandardowych ustawień kart Azure do określonych zespołów*

### Połącz swoje osobiste konto Azure, aby korzystać z kart Azure

Po zainstalowaniu i zaakceptowaniu aplikacji przez administratora Miro, każdy członek zespołu, który chce korzystać z kart Azure, musi osobiście autoryzować połączenie z ich kontem Azure. Personalizuje to selektor kart i pozwala na importowanie wszystkich elementów roboczych Azure, do których użytkownik ma dostęp.

Możesz znaleźć ikonę Azure Cards na pasku narzędzi tworzenia. Jeśli ikony nie ma, być może będziesz musiał(a) jej poszukać:

1. W pasku szukania wybierz **Narzędzia, media i integracje** (**+**).
   Panel **Narzędzia, media i integracje** otwiera się.
2. Na karcie **Narzędzia** wyszukaj i wybierz Karty Azure.

Aby połączyć swoje konto:

1. Kliknij ikonę Azure Cards na pasku narzędzi. Wyskakujące okienko poprosi Cię o **Autoryzację**.
2. Kliknij przycisk **Autoryzuj** i kliknij **Kontynuuj**. Zostaniesz przeniesiony do ustawień zespołu > strony Aplikacje i integracje.
3. Użyj panelu Ustawienia aplikacji, aby połączyć swoje konto Microsoft z Miro i określić instancję platformy Azure, której chcesz użyć. Ten adres URL można skopiować z Azure DevOps; Miro zaakceptuje spersonalizowany adres URL Twojej instancji lub ogólny adres `https://dev.azure.com/` kończący się nazwą Twojej instancji.
   ![Specyfikacja adresu URL organizacji Azure w ustawieniach aplikacji Miro.](https://help.miro.com/hc/article_attachments/21857687519634)

:::note
Pamiętaj, że tylko administratorzy zespołu mogą skonfigurować początkową konfigurację zespołu lub na poziomie firmy. Jeśli nie widzisz przycisku **Połącz** obok adresu URL organizacji Azure podczas konfiguracji administratora, upewnij się, że masz [uprawnienia administratora zespołu dla zespołu](../../administration/user-management/06-how-to-manage-admin-roles.md).
:::

## Importuj elementy robocze Azure na tablicę Miro

Po skonfigurowaniu aplikacji Azure Cards i połączeniu swojego konta osobistego, możesz importować elementy robocze Azure do dowolnej tablicy Miro powiązanej z połączonym zespołem. Istnieją dwa główne sposoby, aby to zrobić:

- Skopiuj adres URL elementu roboczego Azure i wklej go bezpośrednio na tablicę Miro. Element automatycznie zmieni się w kartę Azure.
- Użyj selektora kart Azure: Kliknij ikonę **Azure Cards** na pasku narzędzi, aby otworzyć selektor.

  ![Azure Cards picker interface in Miro.](https://help.miro.com/hc/article_attachments/21857687527186)*Selektor kart Azure*

  Selektor obsługuje wyszukiwanie we wszystkich polach, co pozwala znaleźć kartę po jej tytule, typie, stanie itp. Możesz również użyć solidnego [wyszukiwania słów kluczowych](https://docs.microsoft.com/azure/devops/project/search/get-started-search?view=azure-devops#start-your-search-with-a-keyword) od Microsoft.

  ![Animation showing search functionality within the Azure Cards picker.](https://help.miro.com/hc/article_attachments/21857720726802)*Wyszukaj karty Azure w selektorze*

  Karty możesz filtrować według projektu, osoby, typu, obszaru i stanu, co odblokowuje zaawansowane filtrowanie elementów pracy Azure bezpośrednio w Miro.

  ![Filtering options within the Azure Cards picker.](https://help.miro.com/hc/article_attachments/21857720729618)*Filtruj karty Azure w selektorze*

  Aby przejść do oryginalnego elementu pracy platformy Azure, wybierz kartę na tablicy i kliknij **Źródło** w menu kontekstowym.

  ![Source button on an Azure Card linking to the item in Azure DevOps.](https://help.miro.com/hc/article_attachments/21857687543058)*Przycisk źródłowy karty*

  Karty Azure mogą być używane jako samodzielne widżety tablic lub jako komponenty interaktywnych struktur [kanban](../../using-miro/advanced-tools/02-columns-formerly-kanban.md) i [map historyjek użytkowników](../../using-miro/advanced-tools/07-user-story-mapping.md). Możesz dodać karty Azure do tych ramek, przeciągając je.

  ![Animation showing Azure Cards being used within a Miro Kanban board.](https://help.miro.com/hc/article_attachments/21857687547538)*Praca z kartami Azure w kanbanie*

## Twórz i edytuj karty Azure bezpośrednio w Miro

Dwukierunkowa integracja między Miro i Azure DevOps umożliwia zespołom tworzenie nowych elementów roboczych Azure i edytowanie istniejących bezpośrednio z tablicy Miro. Możesz również przekształcać istniejące karty Miro i karteczki w karty Azure.

### Utwórz nową kartę Azure

Aby utworzyć nowy element roboczy Azure z Miro:

1. Wybierz **Karty Azure** z paska narzędzi tworzenia i wybierz **Utwórz element roboczy** w prawym górnym rogu selektora.
2. Wypełnij pola karty, wybierz projekt, typ elementu, osobę przypisaną i kliknij **Utwórz**. Nowy element zostanie utworzony w Twoim katalogu Azure DevOps oraz na Twojej tablicy Miro.

![Animation showing the process of creating a new Azure Card from Miro.](https://help.miro.com/hc/article_attachments/21857720742802)*Tworzenie karty Azure w Miro*

### Konwertuj karty Miro lub karteczki na karty Azure

Aby przekonwertować istniejącą kartę Miro lub karteczkę na kartę Azure:

1. Wybierz karteczkę lub kartę na tablicy.
2. Kliknij opcję konwertowania (zwykle ikonę Azure DevOps lub "Konwertuj na element pracy platformy Azure") w menu kontekstowym obiektu.
3. Ustaw parametry karty (takie jak projekt, typ elementu) w oknie dialogowym i kliknij **Konwertuj**. Tekst na karteczce lub karcie zostanie przekształcony w tytuł karty.

> **💡** Oszczędzaj czas, zbiorczo konwertując karteczki lub karty Miro na karty Azure. Kliknij i przeciągnij, aby zaznaczyć wszystkie obiekty, które chcesz przekonwertować, i w menu kontekstowym wybierz **Konwertuj na elementy pracy platformy Azure**.

![Converting a Miro sticky note into an Azure Card.](https://help.miro.com/hc/article_attachments/21857720746642)*Konwertowanie karteczki na kartę Azure*

### Edytowanie karty Azure

Opcja edycji kart Azure w Miro usuwa kłopot z przełączaniem się między narzędziami. Aby edytować kartę:

1. Kliknij kartę Azure na swojej tablicy Miro.
2. Kliknij **ikonę ołówka (edycja)** w menu kontekstowym karty. Otworzy się wyskakujące okno, umożliwiające edycję pól elementu.
3. Kliknij **Aktualizuj**, aby zapisać zmiany. Zmiany zostaną również odzwierciedlone w Azure DevOps.

![Editing an Azure Card's details directly within Miro.](https://help.miro.com/hc/article_attachments/21857687557778)*Opcja edytowania karty Azure w Miro*

### Zmień kolor karty Azure

Aby dostosować wygląd kart Azure na tablicy:

Aby zmienić kolor wypełnienia karty, kliknij kartę lub karty i wybierz **kolor wypełnienia** z menu kontekstowego. Jeśli utworzysz duplikat karty lub kart, wszystkie kolejne kopie będą miały ten sam kolor wypełnienia.

## Odinstaluj integrację kart Azure

Jeśli nie potrzebujesz już integracji Azure Cards, możesz ją odinstalować. Odinstalowanie na poziomie zespołu wymaga uprawnień administratora zespołu.

1. Przejdź do **ustawień zespołu > Aplikacje i integracje > Karty Azure**.
2. Przewiń w dół i kliknij **Odinstaluj dla zespołu.**
3. Aby odinstalować karty Azure tylko dla swojego konta osobistego, kliknij **Odinstaluj dla mnie.**

![Options to uninstall Azure Cards for the team or for an individual user.](https://help.miro.com/hc/article_attachments/21857720717842)*Odinstaluj aplikację dla całego zespołu lub tylko dla siebie*

## Obsługiwane pola karty Azure

Miro obsługuje następujące pola dla kart Azure:

- Tytuł
- Projekt
- Typ
- Stan
- Opis (Edycja nie jest obsługiwana)
- Nadrzędne WI
- Przypisana osoba
- Priorytet
- Story points
- Obszar
- Iteracja
- Kryteria akceptacji

Pola niestandardowe nie są obsługiwane.

## Rozwiązywanie problemów z Kartami Azure

Jeśli napotkasz problemy z integracją kart Azure, zapoznaj się z poniższymi typowymi problemami i ich rozwiązaniami.

Adres URL jest nieprawidłowy

Podany adres URL jest nieprawidłowy. Sprawdź pisownię i formatowanie. Na przykład adres organizacji Azure musi kończyć się ukośnikiem.

Nie można uzyskać adresu URL organizacji Azure

Podany adres URL nie istnieje. Wprowadź istniejący URL lub sprawdź pisownię. Sprawdź także następujące elementy:

- Upewnij się, że Twoja organizacja może akceptować autoryzację przez firmę trzecich: w **Ustawieniach organizacji > Zasady (Bezpieczeństwo)** **>** upewnij się, że włączona jest opcja „Dostęp aplikacji innych firm za pośrednictwem usługi OAuth”.
- Twoja organizacja Azure jest w sieci prywatnej / zapora sieciowa firmy blokuje połączenia z siecią zewnętrzną. Wprowadź niezbędne zmiany w konfiguracji zapory sieciowej i VPN, dodając nasze domeny do listy dozwolonych: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com, realtimeboard.com*, *.realtimeboard.com, *static.miro-apps.com. Jeśli używasz serwera proxy, skonfiguruj odwrotny umożliwiający nam dostęp. Pamiętaj, aby wypełnić pole **URL usługi Azure DevOps** w ustawieniach adresem, do którego mamy dostęp (adres może różnić się od rzeczywistego adresu usługi Azure DevOps z ograniczeniami). Możesz również chcieć przedłużyć wartość limitu czasu na serwerze proxy.
- Wszystkie prośby o integrację przechodzą przez narzędzie równoważenia obciążenia Amazon, więc podanie określonych informacji sieciowych nie jest możliwe w Miro.

Nie udało się utworzyć subskrypcji haka do usługi

Obecnie zalogowany użytkownik platformy Azure nie ma niezbędnych uprawnień. Użytkownik platformy Azure, którego imieniu instancja Azure zostanie połączona z Miro, musi mieć dostęp do tych metod REST API:

- [*Utwórz subskrypcję haka usługi*](https://docs.microsoft.com/rest/api/azure/devops/hooks/subscriptions/create?view=azure-devops-rest-6.0) (wymagany zakres „*vso.serviceendpoint_manage*" [zakres](https://docs.microsoft.com/azure/devops/integrate/get-started/authentication/oauth?view=azure-devops#scopes))
- [*Otrzymuj metadane o projektach (informacje te są używane do prawidłowego określania elementów pracy w zdarzeniach subskrypcji)*](https://docs.microsoft.com/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-6.0)
- *Następujące metody są również wymagane, aby były dostępne dla wszystkich użytkowników korzystających z integracji:*
  - [*Pobierz elementy*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/get%20work%20item?view=azure-devops-rest-6.0)
  - [*Lista elementów*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/list?view=azure-devops-rest-6.0)
  - [*Uzyskaj typy elementów*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/get?view=azure-devops-rest-6.0)
  - [*Lista typów elementów*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/list?view=azure-devops-rest-6.0)

Użytkownik **username@microsoft.com** nie ma dostępu do żadnego projektu w określonym adresie URL organizacji Azure.

Nie możesz uzyskać dostępu do żadnych projektów w używanej organizacji Azure. Aby zaimportować karty, powinieneś mieć do nich dostęp po stronie Azure Boards. Skontaktuj się z właścicielem organizacji Azure i poproś go o zaproszenie Cię do organizacji Azure. [Ten artykuł](https://docs.microsoft.com/azure/devops/organizations/security/look-up-organization-owner?view=azure-devops) może pomóc znaleźć nazwę właściciela organizacji.

Nie udało się utworzyć subskrypcji haka usługi: użytkownik **username@microsoft.com** nie jest właścicielem organizacji. Poproś właściciela organizacji o skonfigurowanie tego kroku.

Powinieneś być zarówno właścicielem organizacji Azure, jak i administratorem firmy Miro, aby skonfigurować karty Azure w Miro.

Autoryzacja wygasła. Połącz ponownie integrację w ustawieniach zespołu.

Autoryzacja Azure wygasła. Połącz ponownie integrację na poziomie osobistym, jak opisano w sekcji "Połącz swoje osobiste konto Azure, aby korzystać z kart Azure" powyżej.

Karta, z którą pracujesz, pokazuje nieoczekiwane zachowanie.

- Może się to zdarzyć, jeśli karta została niezsynchronizowana z organizacją platformy Azure. Na przykład jeśli skopiowałeś kartę z innej tablicy lub pracujesz na tablicy, która została przeniesiona między zespołami. Aby rozwiązać sytuację, dodaj ponownie element platformy Azure na tablicę.

Liczba zwróconych elementów roboczych przekracza limit rozmiaru 200. Zmień zapytanie, aby zwrócić mniej elementów.

Jeśli zobaczysz ten komunikat o błędzie, oznacza to, że wybrano zbyt wiele zadań, aby dodać je do tablicy jako karty. Ogranicz liczbę zadań, korzystając z paska wyszukiwania. W tej chwili po otwarciu selektora nie są stosowane żadne filtry i wyświetlane są wszystkie zadania z ostatnich trzech miesięcy. Za każdym razem, gdy selektor spróbuje wyświetlić więcej niż 200 zadań, otrzymasz ten komunikat o błędzie.

Nie widzę przycisku **Połącz** podczas próby połączenia mojej organizacji Azure z Miro w ustawieniach Miro.

Upewnij się, że masz prawa administratora zespołu. Przejdź do karty **Aktywni użytkownicy** w ustawieniach zespołu i [promuj się na administratora zespołu](../../administration/user-management/06-how-to-manage-admin-roles.md) w razie potrzeby. Odnosi się to do początkowej konfiguracji połączenia organizacji Azure przez administratora.

:::note
Jeśli wystąpią inne problemy, skontaktuj się z [pomocą techniczną Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).
:::

## Karty Azure - często zadawane pytania

Oto odpowiedzi na niektóre często zadawane pytania dotyczące integracji Kart Azure.

Jakie adresy IP powinny być dozwolone na liście dla Azure Cards?

Aby integracja Azure Cards działała poprawnie, zwłaszcza w ograniczonych środowiskach sieciowych, może być konieczne dodanie do listy dozwolonych następujących adresów IP:

- 18.203.61.162
- 54.220.74.201
- 54.216.81.236
- 54.73.153.141
- 52.215.228.26
- 52.16.47.17
- 54.217.180.21

Co stanie się z istniejącymi kartami Azure po odłączeniu i odinstalowaniu aplikacji Azure Cards?

Karty pozostają nienaruszone na tablicach Miro bez utraty danych; jednak przestają synchronizować się z Azure, a przycisk źródłowy znika.
