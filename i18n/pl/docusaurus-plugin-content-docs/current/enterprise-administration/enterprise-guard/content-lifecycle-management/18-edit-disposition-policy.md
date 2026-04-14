---
title: "Edytuj zasad\u0119 usuwania"
article_id: 19551033354002
translation_id: 19551033354002
locale: pl-pl
sidebar_position: 18
created_at: '2024-06-14T19:50:51Z'
updated_at: '2025-12-08T16:14:46Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Aby edytować zasady usuwania, musisz mieć [rolę administratora zarządzania danymi](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby poprosić o tę rolę, skontaktuj się z administratorem firmy.
:::

Aby edytować zasadę usuwania, wykonaj następujące kroki:

1. Przejdź do swoich [ustawień Miro](https://miro.com/app/settings).
2. Na lewym panelu, pod **Enterprise Guard**, kliknij **Cykl życia treści**.
3. Kliknij kartę **Zasady usuwania**.
   Pojawi się strona **Zasady usuwania**.
4. Na stronie **Zasady usuwania**, kliknij zasadę usuwania, którą chcesz edytować.
   Pojawi się strona wyświetlająca informacje związane z zasadą.
5. Kliknij **Edytuj** w prawym górnym rogu strony, a następnie edytuj wymagane pola. Poniższa tabela zawiera listę każdego pola i jego opis.

   |  |  |
   | --- | --- |
   | **Pole** | **Opis** |
   | **Nazwa**  **(wymagane)** | Nazwa zasady usuwania.  Maks. 60 znaków. |
   | **Opis**  **(opcjonalny)** | Opis tej zasady usuwania.  Maks. długość: 300 znaków. |
   | **Okres usuwania**  **(wymagany)** | Określ, kiedy tablice są automatycznie przenoszone do kosza. Wybierz liczbę, wybierz **miesiące** lub **lata**, a następnie wybierz, czy okres jest liczony od daty **ostatniej modyfikacji** tablicy, czy od daty **ostatniego dostępu**.  Jeśli określisz okres usuwania w miesiącach, musisz wybrać okres usuwania między 1 a 120 miesięcy.  Jeśli określisz okres usuwania w latach, musisz wybrać okres usuwania między 1 a 10 lat.  Na przykład, jeśli chcesz, aby tablice były przenoszone do kosza, gdy nie były modyfikowane przez rok, możesz wybrać 1 rok i wybrać **Ostatnia modyfikacja**. |
   | **Zakres**  **(wymagane)** | Wybierz zakres dla tej zasady usuwania. Zakres określa tablice, dla których zasada usuwania ma zastosowanie. Możesz ustawić zakres dla wszystkich tablic w organizacji lub dla konkretnych poziomów klasyfikacji tablic.  **Ustaw zasady usuwania dla wszystkich tablic w organizacji** Jeśli chcesz ustawić zakres zasady usuwania dla wszystkich tablic w organizacji, na liście **Zakres** wybierz **Wszystkie tablice w organizacji**.  **Ustaw zasadę usuwania dla jednego lub kilku zespołów w organizacji** Jeśli chcesz ustawić zakres zasady usuwania dla jednego lub więcej zespołów w organizacji, wykonaj następujące kroki:  1. Na liście **Zakres** wybierz **Zespół**. 2. Kliknij pole **Wprowadź zespół** i wybierz każdy zespół, dla którego chcesz zastosować zasadę usuwania. Obok wybranego zespołu pojawi się znak wyboru, aby go przypisać do zasady usuwania.   ✏️ - Możesz wybrać wiele zespołów dla zasady usuwania. Jednak dany zespół może być powiązany z tylko jedną zasadą usuwania w danym czasie.  - Możesz wybrać dowolny zespół, w tym usunięte zespoły, jako zakres podczas tworzenia zasady usuwania.   - Zespół, który jest wybrany jako zakres dla zasady usuwania, nie może zostać trwale usunięty, dopóki nie zostanie usunięty z danego zakresu.  **Ustaw zasady usuwania dla poziomu klasyfikacji tablicy**  ✏️ Aby ustawić zakres zasady usuwania dla określonego poziomu klasyfikacji tablicy, musisz upewnić się, że funkcja klasyfikacji jest włączona. Po przypisaniu zasady usuwania dla poziomu klasyfikacji tablicy, nie można wyłączyć funkcji klasyfikacji. Więcej informacji znajdziesz w dokumentacji na temat [Klasyfikacja](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Jeśli chcesz ustawić zakres zasady usuwania dla konkretnego poziomu klasyfikacji tablicy, wykonaj następujące kroki:  1. Na liście **Zakres** wybierz **Klasyfikacja**. 2. Kliknij listę obok listy **Klasyfikacja** i wybierz poziomy klasyfikacji, dla których chcesz zastosować zasadę usuwania. Możesz także wyszukać poziomy klasyfikacji, a następnie je wybrać.  Obok wybranych poziomów klasyfikacji, które powiązałeś(aś) z zasadą usuwania, pojawi się znak wyboru.  ✏️ **Uwagi:** - Możesz wybrać kilka poziomów klasyfikacji jednocześnie. - Nie możesz ustawić tego samego poziomu klasyfikacji dla różnych zasad usuwania. Jeśli konkretny poziom klasyfikacji jest już powiązany z zasadą usuwania, ten poziom klasyfikacji będzie niedostępny.  - Jeśli zasada usuwania używa poziomu klasyfikacji tablicy, nie możesz wyłączyć funkcji klasyfikacji danych.  -Po przypisaniu poziomu klasyfikacji do zasady usuwania nie można usunąć tego konkretnego poziomu klasyfikacji. - Kiedy tablica podlega zarówno zasadom usuwania dotyczących wszystkich tablic w organizacji, jak i zasadom z zakresem klasyfikacji, stosuje się zasadę z dłuższym okresem usuwania. |
6. Kliknij **Dalej**.
   Pojawi się **strona przeglądu wpływu**.
7. Sprawdź wpływ zasady usuwania. Strona przeglądu wpływu dostarcza następujących informacji:
   - **Podsumowanie:** konfiguracja zasady usuwania, jak nazwa zasady, okres usuwania oraz zakres.
   - **Wpływ zasady:** liczba tablic, które będą objęte tą zasadą.
8. Aby zapisać konfigurację i zastosować zasadę usuwania, kliknij **Opublikuj**.
   Jeśli nie masz włączonych powiadomień o usuwaniu, pojawi się okno dialogowe **Włącz powiadomienia o usuwaniu**.
9. **Powiadomienia o usuwaniu** pozwalają użytkownikom otrzymywać wcześniejsze powiadomienia zanim tablica zostanie automatycznie przeniesiona do kosza z powodu nieaktywności. Takie powiadomienia pomagają użytkownikom podjąć działanie, jeśli chcą zachować swoje treści.

   Jeśli chcesz włączyć powiadomienia o usuwaniu:

   a. Kliknij **Powiadom**.

   b. Skonfiguruj, ile dni wcześniej powinno zostać wysłane powiadomienie — każda wartość od **1 do 30 dni**.

   Jeśli włączenie powiadomień spowoduje, że **niektóre tablice zostaną natychmiast przeniesione do kosza** (ponieważ już przekroczyły próg), system zapyta, czy powiadomić użytkowników o tych konkretnych tablicach. Możesz wybrać:

   - **Tak** – aby powiadomić właścicieli i współwłaścicieli tablic, nawet jeśli tablica jest przenoszona do kosza natychmiast.

   - **Nie** – aby przenieść tablice bez wysyłania powiadomienia o tej natychmiastowej akcji.

   Po włączeniu użytkownicy mający tablice w zakresie jakiejkolwiek zasady usuwania z włączonymi powiadomieniami będą:

   - Otrzymywać powiadomienie w ich Miro **Aktualnościach** podczas skonfigurowanego okna inspekcji.

   - Mogli otworzyć tablicę bezpośrednio z powiadomienia.

   - Zobaczyć **baner** na tablicy ostrzegający o zbliżającym się automatycznym przeniesieniu do kosza, z opcją **Zachowaj tablicę**, jeśli chcą ją zatrzymać.

:::note
Utworzenie, zaktualizowanie lub usunięcie zasady uruchamia proces usuwania, który może zająć do 24 godzin. Jednak aktualizacja nazwy lub opisu zasady jest natychmiastowa, ponieważ te działania nie uruchamiają procesu usuwania.
:::

#
