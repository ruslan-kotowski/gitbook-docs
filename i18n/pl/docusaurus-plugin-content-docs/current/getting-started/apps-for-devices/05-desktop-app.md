---
title: Aplikacja komputerowa
article_id: 360017572854
translation_id: 360017572854
locale: pl-pl
sidebar_position: 5
created_at: '2019-02-11T10:15:04Z'
updated_at: '2025-11-25T16:00:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
---

Uruchom aplikację Miro na komputerze w kilka sekund bezpośrednio z pulpitu i pracuj nad tablicami bez zakłóceń. Aplikacja obsługuje wszystkie podstawowe funkcje wersji przeglądarkowej.

:::tip
Pobierz aplikację Miro z [naszej strony internetowej](https://miro.com/apps/).
:::

## Pobierz aplikację komputerową Miro

### Windows

- Windows 64-bit - [pobierz aplikację](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.exe)

:::note
Windows 32-bit został wycofany i nie jest już dostępny.
:::

### macOS

- Maki z układami Apple silicon - [pobierz aplikację](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro.dmg)
- Maki z układami Intel - [pobierz aplikację](https://desktop.miro.com/platforms/darwin/Install-Miro.dmg)

Aby sprawdzić, jaki procesor posiadasz, wykonaj te kroki:

1. Kliknij ikonę Apple w lewym górnym rogu swojego Maca.
2. Otworzy to menu rozwijane. Kliknij opcję **O tym Macu**.

W oknie powinny znaleźć się potrzebne informacje, w tym rodzaj procesora (Intel lub Apple silicon).

## Zainstaluj Miro na wielu urządzeniach

Miro oferuje różne wersje instalatorów, które administratorzy mogą wykorzystać do wdrożenia Miro użytkownikom na tysiącach maszyn. Istnieją dwa podstawowe sposoby na to: instalacja per użytkownik lub per urządzenie. Dla każdej z tych opcji dostępne są wersje z automatycznymi aktualizacjami i bez. Wersja z automatycznymi aktualizacjami oznacza, że użytkownicy otrzymają zaktualizowaną wersję aplikacji zaraz po jej opublikowaniu. Wersja bez automatycznych aktualizacji daje Ci większą kontrolę nad wersją Miro, z której korzystają Twoi pracownicy.

### Dla Windows

#### Wdrożenie Miro do Program Files

Miro może być również zainstalowane w katalogu Program Files, dzięki czemu jest dostępne dla każdego użytkownika urządzenia, zachowując jednocześnie oddzielne profile. Pojedyncza instalacja na maszynie oznacza mniejszy ślad na dysku twardym na dużej skali, jednocześnie udostępniając Miro wszystkim użytkownikom tej maszyny. Jeśli wybierzesz wersję z automatycznymi aktualizacjami, pamiętaj, że do zainstalowania aktualizacji potrzebne są uprawnienia administratora.

- Windows MSI 64 bit z automatycznymi aktualizacjami - [pobierz aplikację](https://desktop.miro.com/platforms/win-nsis/Miro-setup.msi)
- Windows MSI 64 bit bez automatycznych aktualizacji - [pobierz aplikację](https://desktop.miro.com/platforms/win-nsis/Miro-no-updates.msi)

#### Wdrażanie Miro dla konkretnego użytkownika

Miro oferuje różne wersje instalatora, które administratorzy IT mogą użyć do wdrożenia Miro dla pojedynczego użytkownika. Ta wersja może być aktualizowana bez uprawnień administracyjnych i jest instalowana tylko dla wybranego użytkownika(ów).

- Windows MSI 64 bit z automatycznymi aktualizacjami - [pobierz aplikację](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.msi)
- Windows MSI 64 bit bez automatycznych aktualizacji - [pobierz aplikację](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-no-updates.msi)

### Dla MacOS

- Apple silicon Mac bez automatycznych aktualizacji - [pobierz aplikację](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro-no-updates.dmg)
- Intel Mac bez automatycznych aktualizacji - [pobierz aplikację](https://desktop.miro.com/platforms/darwin/Install-Miro-no-updates.dmg)

## Wymagania systemowe aplikacji

### Dla Windows

|  |  |  |
| --- | --- | --- |
|  | **Minimalne** | **Zalecane** |
| **Procesor** | 3 GHz (2 rdzenie/4 wątki) | 2,8 GHz (4 rdzenie/8 wątków) |
| **Pamięć RAM** | 8 GB | 16 GB (DDR4) |
| **System operacyjny** | Windows 10 lub nowszy dla aplikacji z Microsoft Store + Microsoft .NET Framework 4.5 (Proszę zauważyć, że wersja ARM systemu Windows nie jest obsługiwana) | Najbardziej aktualny system operacyjny |
| **Sieć** | 8 Mb/s lub szybsze | 32 Mb/s |

### Dla macOS

|  |  |  |
| --- | --- | --- |
|  | **Minimalne** | **Zalecane** |
| **CPU** | 64-bitowy Intel lub Apple M1 |  |
| **OS** | MacOS 12 (Monterey) lub nowszy | Najnowszy OS |
| **Sieć** | 8 Mb/s lub szybciej | 32 Mb/s |

Zwróć uwagę, że aplikacja będzie uruchomiona w kilku instancjach na Twoim urządzeniu:

- proces główny
- proces okna (renderowanie interfejsu użytkownika)
- akceleracja sprzętowa
- obsługa awarii
- + 1 proces na każdą otwartą kartę (ponieważ każda karta ma widok internetowy)

Na przykład, jeśli masz otwarte 3 karty podczas pracy, zobaczysz 7 instancji Miro.exe. Więcej informacji o tej architekturze można znaleźć [tutaj](https://www.electronjs.org/docs/glossary#process) i [tutaj](https://www.chromium.org/developers/design-documents/multi-process-architecture).

## Skróty specyficzne dla aplikacji

Aplikacja komputerowa ma dodatkowe [skróty klawiszowe](../../using-miro/working-on-the-board/06-shortcuts-and-hotkeys.md):

- **Ctrl + R** *(dla Windows)* / **Cmd + R** *(dla Mac)* aby odświeżyć kartę
- **Ctrl + W** *(dla Windows)* / **Cmd + W** *(dla Mac)* aby zamknąć kartę
- **Ctrl + Q** *(dla Windows)* / **Cmd + Q** *(dla Mac)* aby zamknąć aplikację
- **Ctrl + Shift + L** *(dla Windows)* / **Cmd + Shift + L** *(dla Mac)* aby skopiować link do tablicy
- **Ctrl + ~** *(dla Windows)* **/ Cmd + ~** *(dla Mac)* aby zrobić zoom

## Działania aplikacji

Poniższa tabela pokazuje, które dostępne działania w aplikacji komputerowej Miro mogą różnić się od tych w przeglądarce:

| Działanie | **Aplikacje Win & Mac z** [**Miro Apps**](https://miro.com/apps/) |
| --- | --- |
| Zapisz jako obraz (Niski, Średni, Wysoki) | ✔ |
| Zapisz jako obraz (Wektorowy) | ✔ |
| Zapisz jako PDF (Niski) | ✔ |
| Zapisz jako PDF (wektorowy) | ✔ |
| Eksport do arkusza kalkulacyjnego (CSV) | ✔ |
| Czat wideo | ✔ |
| Wklejanie z arkusza kalkulacyjnego | ✔ |
| Wtyczka do Confluence | ✔ |

### Działania niedostępne

Następujące działania są niedostępne w aplikacji komputerowej Miro:

- Odwiedzający nie mogą się zalogować.

  > ✏️ Do aplikacji komputerowej mogą się logować tylko zarejestrowani użytkownicy Miro.
- Brak opcji kopiowania-wklejania ze Sketch
- W niektórych wersjach Jira Server, nie można edytować kart Jira z powodów bezpieczeństwa.

## Sprawdzanie pisowni

Jeśli chcesz wyłączyć automatyczną funkcję sprawdzania pisowni w aplikacji komputerowej, wykonaj te kroki:

- Naciśnij **Alt** (*tylko dla Windows*)
- Kliknij **Wyświetlanie** na głównym pasku nawigacyjnym na górze
- Odznacz przycisk **Pokaż sprawdzanie pisowni**

Uwaga: opcja wyłączenia sprawdzania pisowni nie jest dostępna w aplikacji pobranej z Microsoft Store.

## Możliwe problemy i ich rozwiązania

### Jak zresetować dane aplikacji

W wielu przypadkach, gdy pojawia się problem (szczególnie jeśli masz trudności z procedurą logowania), pomocne może być **zresetowanie danych aplikacji**, co czyści pamięć aplikacji.

:::tip
Jeśli problem utrzymuje się po zresetowaniu danych, możesz także usunąć aplikację i ponownie ją zainstalować, [pobierając najnowszą wersję](https://miro.com/apps/).
:::

#### Dla Windows

Naciśnij **Alt > Pomoc** i wybierz opcję zresetowania danych aplikacji, jak pokazano na poniższym zrzucie ekranu:

![reset app data on Windows.png](../../../../../../docs/getting-started/apps-for-devices/images/21016134171922_reset%20app%20data%20on%20Windows.png)
*Resetowanie danych aplikacji w aplikacji komputerowej dla Windows*

Jeśli nie możesz znaleźć menu, prawdopodobnie używasz aplikacji pobranej z MS Store. W tym przypadku, aby zresetować dane aplikacji, otwórz **Ustawienia** Windows > **Aplikacje** > **Aplikacje i funkcje** > znajdź **Miro** na liście > **Opcje zaawansowane** > **Resetuj**.

Jeśli to nie pomoże od razu, usuń wszystkie pliki aplikacji z **C:\Users\username\AppData\Roaming\RealtimeBoard** i **C:\Users\username\AppData\Local\Programs\RealtimeBoard**

> **✏️** Jeśli folder **Appdata** jest ukryty, zobacz [tutaj](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5), jak można go ujawnić.

#### Dla macOS

Kliknij Miro w górnym menu i wybierz **Zresetuj dane aplikacji** zgodnie z pokazanym poniżej zrzutem ekranu:

![reset app data on Mac.png](../../../../../../docs/getting-started/apps-for-devices/images/21016120799378_reset%20app%20data%20on%20Mac.png)
*Resetowanie danych aplikacji na Macu*

Po tym spróbuj zalogować się do aplikacji ponownie i sprawdź, czy problem został rozwiązany.

Jeśli zresetowanie nie przynosi natychmiastowej pomocy, otwórz okno Findera > naciśnij **Command + Shift + G** > wklej **~/Library/Application Support/RealtimeBoard** i usuń wszystkie pliki aplikacji.

Jeśli używasz MDM dla Mac

Jeśli napotkasz problem z brakiem możliwości załadowania aplikacji, zablokowaniem w pętli, upewnij się, że twoja konfiguracja pozwala naszemu auto-aktualizatorowi działać. `https://github.com/Squirrel/Squirrel.Mac` musi mieć prawa do:

- odczytu, zapisu i wykonywania dla katalogu „Application”,
- odczytu i zapisu dla „~/Application Support/Caches/” do pracy z katalogiem „com.electron.realtimeboard.ShipIt” oraz z katalogiem tymczasowym „private/var/folders”.

Jeśli coś pójdzie nie tak podczas procesu aktualizacji, Squirrel tworzy plik `ShipIt_stderr.log` w `~/Application Support/Caches/com.electron.realtimeboard.ShipIt`. Więcej informacji o problemie można znaleźć tam.
Zwróć uwagę, że Skype i Slack używają podobnego procesu aktualizacji, więc jeśli masz już skonfigurowane MDM dla nich, możesz zastosować te same ustawienia dla aplikacji komputerowej Miro.

## Często zadawane pytania

1. *Gdzie można pobrać aplikację komputerową?*
   - Można ją pobrać z naszej [strony internetowej](https://miro.com/apps/).
2. *Jak mogę usunąć wyskakujące okienko do otwarcia aplikacji komputerowej, gdy uruchamiam Miro w przeglądarce?*
   - Wypróbuj kroki z [tego artykułu](../../using-miro/troubleshooting-technical-questions/technical-guidelines/04-how-to-disable-miro-desktop-app-pop-up-in-your-browser.md).
3. *Czy jest dostępna wersja aplikacji komputerowej na Linux?*
   - Nie, na ten moment nie mamy takiej wersji.
4. *Jak mogę skopiować link do otwartej tablicy w aplikacji komputerowej?*
   - Możesz otworzyć menu **Udostępnij** tablicy i stamtąd skopiować link do tablicy. Innym sposobem jest kliknięcie **Plik** w prawym górnym rogu > **Kopiuj link do tablicy**. Możesz także użyć skrótu **Ctrl + Shift + L** *(dla Windows)* / **Cmd + Shift + L** *(dla Maca).*
5. *Kiedy naciskam **Alt** w aplikacji komputerowej na Windows, menu się nie pojawia. Jak mogę je uzyskać?*
   - Należy pamiętać, że menu nie jest obsługiwane w aplikacji pobranej ze sklepu Microsoft Store. Możesz zresetować dane aplikacji w ustawieniach systemu Windows (**System > Aplikacje & Funkcje > Znajdź Miro > Opcje zaawansowane > Resetuj**) lub [zainstalować oryginalną wersję aplikacji](https://miro.com/apps/).
6. *Jeśli usunę aplikację komputerową, czy moje tablice zostaną usunięte?*
   - Nie, Twoje treści są powiązane z Twoim profilem Miro. Możesz uzyskać do nich dostęp w przeglądarce, [aplikacji na tablety](11-tablet-app.md), [aplikacji mobilnej](08-mobile-app.md) również.
