---
title: Dysk Google
article_id: 360017731253
translation_id: 360017731253
locale: pl-pl
sidebar_position: 6
created_at: '2019-02-11T10:14:01Z'
updated_at: '2025-01-13T14:51:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-drive-onedrive
---

**Dysk Google** umożliwia bezpieczne przechowywanie plików online, uzyskiwanie do nich dostępu z dowolnego miejsca i współpracę z innymi. Dzięki integracji z Dyskiem Google łatwiej jest skupić się na zadaniach i śledzić dokumenty bezpośrednio na tablicy.

![Google_Drive_on_the_Upload_menu.jpg](https://help.miro.com/hc/article_attachments/21857866755218)

> **Konfiguracja przez:** każdego użytkownika osobno (administratorzy mogą ograniczyć instalowanie aplikacji przez użytkowników niebędących administratorami).
> **Dostępne wersje:** przeglądarka, [aplikacja](../../getting-started/apps-for-devices/05-desktop-app.md) komputerowa (pełna funkcjonalność i pliki edycji); [aplikacja na](../../getting-started/apps-for-devices/11-tablet-app.md) tablety, [aplikacja mobilna](../../getting-started/apps-for-devices/08-mobile-app.md) (ograniczona funkcjonalność, edycja nie jest obsługiwana).

### Włączanie Dysku Google

Aby rozpocząć dodawanie plików z Dysku Google, musisz zainstalować wtyczkę i połączyć swój Dysk Google z Miro.

:::warning
Użytkownicy niebędący administratorami nie mogą zainstalować aplikacji, jeśli jest to niedozwolone w ustawieniach **aplikacji i** integracji.
:::

Zainstaluj aplikację z [Miro Marketplace](https://miro.com/marketplace/google-drive/?backUrl=%2Fmarketplace%2F). Po kliknięciu **Pobierz aplikację** otrzymasz sugestię wyboru zespołu, do którego ma zostać zainstalowana wtyczka ![](https://help.miro.com/hc/article_attachments/21857866759826)*for.install_Google_Drive.jpgWybór zespołu podczas instalowania wtyczki Dysku Google*altalt

Możesz również zainstalować wtyczkę z tablicy. Kliknij strzałki na pasku narzędzi tworzenia, wyszukaj **Dysk Google** i wybierz **Dodaj**. Kliknij **Pobierz aplikację** w wyskakującym oknie.

![Google_Drive_on_the_toolbar.jpg](https://help.miro.com/hc/article_attachments/21857851816594)

Następnie połącz Dysk Google z Miro. Istnieją dwa proste sposoby.

1.  Przejdź do **ustawień profilu (klikając** koło zębate w lewym górnym rogu tablicy lub na pulpicie nawigacyjnym, klikając ikonę profilu i wybierając **Ustawienia).** Następnie kliknij kartę Integracje, znajdź **Dysk Google** i kliknij **Połącz**:

![connect_Google_Drive.jpg](https://help.miro.com/hc/article_attachments/21857866765202)*Dysk Google na stronie Integracje*

2. Połącz swój profil Miro z Dyskiem Google z poziomu tablicy, klikając **Dysk Google** w menu **Prześlij** na pasku narzędzi:

![Google_Drive_on_the_Upload_menu.jpg](https://help.miro.com/hc/article_attachments/21857866755218)*Ikona Dysku Google na pasku narzędzi*

Potwierdź autoryzację dla potrzebnego konta Google i **Zezwól** aplikacji na dostęp do plików:

![permissions.jpg](https://help.miro.com/hc/article_attachments/21857851822098)
*Uprawnienia z Dysku Google*

Pamiętaj, że są to standardowe uprawnienia dla Dysku Google.

– **Wyświetlanie i pobieranie wszystkich plików na Dysku Google** – dla selektora plików na Dysku Google na tablicy. Umożliwia importowanie dokumentów z Dysku Google do Miro

- **Oglądaj, edytować, tworzyć i usuwać tylko określone pliki na Dysku Google używane w** tej aplikacji, aby móc zapisywać tablicę Miro na Dysku Google.

Aplikacja Dysku Google zarządza tylko plikami tworzonymi na Dysku (linki do tablic itp.).  Miro nie ma możliwości zarządzania żadnymi treściami na Dysku Google. Aby wdrożyć integrację, używamy **interfejsu API Dysku Google v3**. W tym interfejsie API zakresy są pogrupowane w taki sposób, że uprawnienia dostępu do zapisu nie mogą być wymagane oddzielnie od uprawnień dostępu do pełnego dysku. Jeśli chcesz sprawdzić, sprawdź uprawnienia w artykule Google, [Zakresy dla interfejsów API Google](https://developers.google.com/identity/protocols/googlescopes).

Jeśli chcesz zmienić konto Google połączone z Miro, przejdź do **Ustawień profilu** > **Integracje**, kliknij **Wyloguj** się obok **Dysku Google** i połącz z innym kontem.

![Google_Drive_log_out_in_settings.jpg](https://help.miro.com/hc/article_attachments/21857851823890)*Połączenie z Dyskiem Google w ustawieniach profilu*

### Dodawanie plików z Dysku Google i dysków współdzielonych

> **Dostępne wersje:** [przeglądarkowa, aplikacji](../../getting-started/apps-for-devices/05-desktop-app.md) komputerowej, [aplikacji](../../getting-started/apps-for-devices/08-mobile-app.md) [na](../../getting-started/apps-for-devices/11-tablet-app.md) tablety, aplikacji mobilnej (ograniczona funkcjonalność)

:::warning
Każdy, kto ma dostęp do tablicy Miro, może wyodrębnić zaimportowane dokumenty, nawet jeśli są one ograniczone po stronie Google. Aby chronić pliki, ważne jest, aby unikać udostępniania tablicy osobom, które nie powinny mieć dostępu do dokumentów.
:::

Aby dodać plik z Dysku Google:

1. Wklej adres URL dokumentu bezpośrednio na tablicy (pamiętaj, że wklejenie adresu URL do [kształtu](../../using-miro/essential-tools/11-shapes.md) lub [karteczki](../../using-miro/essential-tools/14-sticky-notes.md) nie spowoduje osadzenia dokumentu na tablicy, ale doda link jako prosty tekst). Po skopiowaniu linku do określonego arkusza z arkuszy kalkulacyjnych Google i wklejeniu go na tablicę Miro, wklejony arkusz kalkulacyjny nadal będzie się rozpoczynał od pierwszej strony w Miro.

   lub:
2. Kliknij przycisk **Prześlij** na pasku narzędzi (pokazany na powyższym zrzucie ekranu) i wybierz **Dysk Google**. Zobaczysz wtedy menu selektora. Zaznacz wszystkie dokumenty, które chcesz dodać, i kliknij **Wybierz**. Możesz również użyć paska wyszukiwania, aby znaleźć dokumenty na Dysku Google.

:::tip
Aby dodać dokument z Dysku Google na tablicy w aplikacji [mobilnej,](../../getting-started/apps-for-devices/08-mobile-app.md) wklej adres URL dokumentu za pośrednictwem menu Prześlij.
:::

![select_a_file_in_Google_Drive.gif](https://help.miro.com/hc/article_attachments/21857866779282)*Wybieranie dokumentu na Dysku Google*

Dodaj dokumenty z **dysków** współdzielonych – przełącz się na kartę i wybierz pliki.

![team_drive.jpg](https://help.miro.com/hc/article_attachments/21857851832978)*Dysk zespołu w selektorze Dysku Google*

### Edytowanie dokumentów Google

> **Dostępne na:** wersja przeglądarkowa, [aplikacja](../../getting-started/apps-for-devices/05-desktop-app.md) komputerowa

Możesz osadzać Dokumenty Google, arkusze kalkulacyjne i slajdy bezpośrednio na tablicy, przenosić je i zmieniać rozmiar, a także przesuwać strony dokumentów.

Kliknij dokument, a zobaczysz menu kontekstowe z opcjami przełączania stron, **przypięcia** strony, **wyodrębniania** stron, **edytowania** treści, przeładowania, **aktualizacji** lub przejścia do **źródła danych**.

Aby rozpocząć edycję dokumentu, kliknij ikonę ołówka w menu kontekstowym lub kliknij dwukrotnie dokument. Dokument otwiera się w wyskakującym okienku i można go edytować tak, jakby był na Dysku Google. Kliknij **Zamknij** lub szary obszar, aby zakończyć edycję. Wszystkie zmiany są automatycznie zapisywane i widoczne na tablicy i w dokumentach Google.

![google_drive_edit_docs.gif](https://help.miro.com/hc/article_attachments/21857851835026)*Edytowanie osadzonego dokumentu Google*

Jeśli wolisz, możesz również kliknąć przycisk **źródła** i dokument zostanie otwarty do edycji w następnej karcie.

Jeśli dokonałeś jakichkolwiek edycji bezpośrednio z Dysku Google (zwłaszcza podczas pracy offline), odśwież osadzenie na tablicy za pomocą przycisku **Aktualizuj** w menu kontekstowym. Osadzone pliki na Dysku Google nie są automatycznie aktualizowane na tablicach Miro (chyba że plik jest edytowany z Miro).

![update_button.jpg](https://help.miro.com/hc/article_attachments/21857851836690)*Przycisk aktualizacji*

### Zarządzanie uprawnieniami dostępu

Pamiętaj, że uprawnienia dostępu na Dysku Google i w Miro są ustawiane *oddzielnie*. Oznacza to, że aby umożliwić komuś edycję dokumentu Google na tablicy, musisz udostępnić mu dokument na Dysku Google z uprawnieniami *edytującego,* a także [zaprosić go jako *edytującego* do tablicy](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

Jeśli zezwolisz komuś na edycję dokumentu w Google, ale zaproś go do tablicy tylko z [uprawnieniami do wyświetlania lub](../../using-miro/sharing-boards/01-board-access-rights.md) komentowania, nie będzie mógł aktywować trybu edycji dokumentu. I odwrotnie, jeśli zaprosisz osobę do tablicy jako edytującego, ale nie udostępniasz jej dokumentu na Dysku Google, Google nie zezwoli na jego edycję.

Upewnij się, że Ty i Twój zespół macie dostęp do poziomu wymaganego do pomyślnej współpracy.

### Zapisywanie tablicy na Dysku Google

> **Konfigurują:** właścicieli tablic

Kliknij ikonę **Eksportuj** > **Zapisz na** Dysku Google, a tablica będzie dostępna na Dysku tak jak jeden z dokumentów.

![export_menu_export_to_google_drive.png](https://help.miro.com/hc/article_attachments/21857851844242)
*Tworzenie linku do tablicy na Dysku Google*

Na Dysku Google możesz teraz kliknąć zapisaną tablicę, która otworzy się w oddzielnej karcie przeglądarki. Jeśli usuniesz tablicę z Dysku Google, nadal będzie ona dostępna w Miro. Jeśli jednak usuniesz tablicę w Miro, nie będziesz już mógł uzyskać do niej dostępu z Dysku Google.

:::warning
Jeśli nie jesteś właścicielem tablicy, otrzymasz komunikat o błędzie jak poniżej.
:::

![Google_Drive_error.jpg](https://help.miro.com/hc/article_attachments/21857851848210)*Komunikat o błędzie niewystarczającego zapisu uprawnień*

### Odinstalowywanie wtyczki

Aby odinstalować wtyczkę dla zespołu, znajdź ją w sekcji **Aplikacje i integracje** w ustawieniach zespołu i kliknij **Odinstaluj dla zespołu**.

![uninstall_Google_Drive_app.jpg](https://help.miro.com/hc/article_attachments/21857851852306)*Odinstalowywanie Dysku Google dla zespołu*

Aby odłączyć Miro od Dysku Google, otwórz stronę **Integracje** w ustawieniach profilu i kliknij **Wyloguj** się obok ikony Dysku Google.

![Google_Drive_log_out_in_settings.jpg](https://help.miro.com/hc/article_attachments/21857851823890)*Odłączanie Dysku Google z Miro*

### Funkcje niedostępne dla osadzonych plików na Dysku Google

**Ogólne**

- Strona początkowa Dysku Google
- Przenoszenie plików między folderami
- Udostępnianie
- Pomoc w wyszukiwaniu

**Prezentacje Google**

- Tryb prezentacji

### Rozwiązywanie możliwych problemów

**Nie można przesłać błędu**

Jeśli pojawi się komunikat o błędzie Przepraszamy, wygląda na **to, że nie masz uprawnień do przesłania tego pliku lub plik został usunięty. Sprawdź dostęp bezpośrednio i spróbuj** ponownie, próbując przesłać plik Dysku Google na tablicę Miro. Poproś administratora Google o zezwolenie użytkownikom na dostęp do Dysku Google za pomocą interfejsu API zestawu SDK:

1. Zaloguj się do [konsoli administratora Google.](https://admin.google.com/)
2. Kliknij **Strona główna > Aplikacje > Google Workspace**. Upewnij się, że **Dysk i Dokumenty** są **WŁĄCZONE dla wszystkich.**
3. Kliknij **Dysk i Dokumenty > Funkcje i aplikacje**. Upewnij się, że **zezwalaj użytkownikom na dostęp do Dysku Google, gdy interfejs API dysku SDK jest** **WŁĄCZONY**.

![unable_to_upload.png](https://help.miro.com/hc/article_attachments/21857866799378)
*Nie można przesłać wiadomości ostrzegawczej*

**Problem z autoryzacją**

Jeśli nie możesz połączyć swojego Dysku Google z Miro, upewnij się, że zapewniłeś Miro dostęp do **Wyświetlania i pobierania wszystkich plików** Dysku Google oraz aby **wyświetlać, edytować, tworzyć i usuwać tylko określone pliki Dysku Google używane z tą aplikacją** podczas łączenia się z Dyskiem Google. W tym celu przejdź do [ustawień profilu Miro](../../using-miro/managing-your-profile/01-profile-settings.md) > **Integracje**, usuń połączenie z Dyskiem Google i skonfiguruj je ponownie.

![Permissions.png](https://help.miro.com/hc/article_attachments/21857866801042)
*Dostęp Miro do konta na Dysku Google*

### Często zadawane pytania

1. *Czy mogę otworzyć osadzony plik na Dysku Google?*
   - Tak, wybierz dokument i kliknij przycisk **źródłowy** w menu kontekstowym.
2. *Czy mogę wkleić zawartość tablic Miro do pliku na Dysku Google?*
   - Możesz [skopiować zawartość tablicy jako tekst lub obraz](../../using-miro/working-on-the-board/09-copy-as-text-or-as-an-image.md) i wkleić ją do pliku na Dysku Google.
