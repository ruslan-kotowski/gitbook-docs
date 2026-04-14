---
title: Airtable
article_id: 360012807619
translation_id: 360012807619
locale: pl-pl
sidebar_position: 1
created_at: '2020-03-24T12:09:00Z'
updated_at: '2025-08-05T07:33:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Osoby: Wszyscy użytkownicy Miro, użytkownicy płatnych abonamentów Airtable
    Wersje Miro: Wszystkie wersje Platformy: Przeglądarka'
---

Wykorzystaj moc wizualizacji na tablicy w swojej pracy z Airtable! Możesz eksportować dane z Miro do Airtable i osadzać tablice Miro w bazach Airtable, aby przeglądać, komentować i edytować je bezpośrednio w Airtable.

## Eksport danych z tablic Miro do Airtable

Integracja Airtable Sync pozwala na eksport danych (np. karteczki, karty) z tablic Miro i ich organizację w Airtable. Aby dowiedzieć się więcej o konfiguracji i używaniu tej funkcji, odwiedź [oficjalną dokumentację Airtable](https://support.airtable.com/docs/airtable-sync-integration-miro).

## Osadź tablice Miro w bazach Airtable

### Zainstaluj aplikację Miro w Airtable

:::warning
Aplikacja Miro dla Airtable **nie** jest dostępna w przeglądarce **Safari**.
:::

Edytorzy baz w Airtable mogą instalować aplikację Miro. Aby to zrobić:

1. Otwórz swoją bazę w Airtable i kliknij **Rozszerzenia** w prawym górnym rogu.

   ![Airtable extensions button in the top right corner.](../../../../../../docs/integrations-apps/more-integrations/images/21017651877394_Airtable%20extensions.jpg)
   *Przycisk rozszerzeń w prawym górnym rogu bazy Airtable.*
2. Kliknij **Dodaj rozszerzenie**.

   ![Add an extension option in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017647938834_add%20an%20extension.jpg)
   *Opcja dodania nowego rozszerzenia.*
3. Wyszukaj "Miro" w Marketplace Airtable i kliknij **Dodaj**.

   ![Miro app in Airtable Marketplace.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933714_Miro%20in%20Airtable.jpg)
   *Aplikacja Miro w Marketplace Airtable.*

### Dodaj istniejące tablice Miro do baz Airtable

Gdy aplikacja Miro zostanie dodana do bazy Airtable, kliknij **Dodaj tablicę** w sekcji aplikacji Miro, która pojawi się w panelu rozszerzeń.

![Add a Miro board button in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651876498_add%20a%20Miro%20board.jpg)
*Dodawanie tablicy Miro za pomocą aplikacji Miro w Airtable.*

Pojawi się selektor tablic Miro. Jeśli nie jesteś zalogowany do Miro w swojej przeglądarce, zostaniesz poproszony o zalogowanie się lub utworzenie konta Miro.

Po wybraniu tablicy ustaw uprawnienia do udostępniania za pomocą menu rozwijanego, aby określić, jak będzie wyświetlana w Airtable. Masz trzy opcje:

- **Każdy może wyświetlać:** Każdy w Airtable może [wyświetlać](../../using-miro/sharing-boards/01-board-access-rights.md) zawartość osadzonej tablicy.
- **Każdy może komentować:** Każdy w Airtable może [zostawiać komentarze](../../using-miro/sharing-boards/01-board-access-rights.md) na osadzonej tablicy. (Uwaga: Ta opcja nie jest dostępna dla tablic przechowywanych w Miro [wersji Free](../../plans-billing/miro-plans/09-free-plan.md).)
- **Prywatne:** Tablica będzie stosować się do istniejących ustawień udostępniania skonfigurowanych po stronie Miro.

  > ✏️ Dla użytkowników korzystających z Miro [abonamentu Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), ustawienia dostępu będą zgodne z kontrolami dostępu obowiązującymi w całej organizacji, co może oznaczać, że niektóre opcje udostępniania są ograniczone. Dowiedz się więcej: [Zarządzanie zasadami udostępniania Enterprise dla integracji osadzania](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).

![Sharing settings options when adding a Miro board to Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651879826_board%20access%20in%20Airtable.jpg)
*Ustawienia udostępniania podczas dodawania tablicy Miro do Airtable.*

Osadzona tablica Miro pojawi się wtedy w twojej bazie Airtable, gdzie możesz ją wyświetlać, komentować lub edytować w zależności od ustawionych uprawnień.

![Embedded Miro board within an Airtable base.](../../../../../../docs/integrations-apps/more-integrations/images/21017651872402_Miro%20board%20in%20Airtable.jpg)
*Osadzona tablica Miro w Airtable.*

Aby zamienić osadzoną tablicę na inną, kliknij ikonę koła zębatego (**Ustawienia**) dla aplikacji Miro w Airtable, wybierz **Wybierz tablicę** i wybierz inną tablicę z selektora Miro.

![Replacing an embedded Miro board in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017647932690_replacing%20a%20board.jpg)
*Zamiana osadzonej tablicy Miro w Airtable.*

### Utwórz nowe tablice Miro z Airtable

Aby utworzyć nową tablicę Miro bezpośrednio z Airtable:

1. W sekcji aplikacji Miro w Airtable kliknij **Dodaj tablicę** (lub **Wybierz tablicę**, jeśli jedna jest już osadzona i ją zastępujesz).
2. W selektorze Miro wybierz opcję utworzenia **Nowej tablicy**.

![Creating a new Miro board from the picker within Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651880466_add%20a%20new%20board%20to%20Airtable.jpg)
*Tworzenie nowej tablicy Miro z selektora w Airtable.*

Nowa tablica zostanie utworzona na Twoim koncie Miro i osadzona w Twojej bazie Airtable.

### Usuń tablice Miro z Airtable

Aby usunąć osadzoną tablicę Miro z bazy Airtable, musisz usunąć lub skonfigurować na nowo rozszerzenie aplikacji Miro w tej bazie. Kliknij menu rozwijane na aplikacji Miro w panelu rozszerzeń i wybierz opcję usunięcia lub zarządzania rozszerzeniem.

![Deleting the Miro app from Airtable extensions panel.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933074_deleting%20the%20app.jpg)
*Usuwanie aplikacji Miro z panelu rozszerzeń Airtable.*
