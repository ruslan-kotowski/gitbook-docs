---
title: "Dodaj zasad\u0119 usuwania"
article_id: 19551031552018
translation_id: 19551031552018
locale: pl-pl
sidebar_position: 17
created_at: '2024-06-14T19:49:31Z'
updated_at: '2025-12-08T16:13:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Aby dodać zasady usuwania, musisz posiadać rolę [administratora zarządzania danymi](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby poprosić o rolę administratora zarządzania danymi, skontaktuj się z administratorem firmy.
:::

Aby dodać zasadę usuwania, wykonaj następujące kroki:

1. Przejdź do [ustawień Miro](https://miro.com/app/settings).
2. W lewym panelu, w sekcji **Enterprise Guard**, kliknij **Cykl życia treści**.
3. Kliknij kartę **Usuwanie**.
   Pojawi się strona **Zasady usuwania**.
4. Kliknij **Dodaj zasadę usuwania**.
5. Wpisz lub wybierz odpowiednie informacje dla każdego pola. Poniższa tabela zawiera opis każdego pola.

   |  |  |
   | --- | --- |
   | **Pole** | **Opis** |
   | **Nazwa**  **(wymagane)** | Nazwa zasady usuwania.  Maks. 60 znaków. |
   | **Opis**  **(opcjonalne)** | Opis tej zasady usuwania.  Maks. 300 znaków. |
   | **Okres usuwania**  **(wymagane)** | Określ, kiedy tablice są automatycznie przenoszone do kosza. Wybierz liczbę, zaznacz **miesiące** lub **lata**, a następnie wybierz, czy okres jest liczony od daty **ostatniej modyfikacji** tablicy, czy **ostatniego dostępu**.  Jeśli określisz okres usuwania w miesiącach, musisz wybrać okres od 1 do 120 miesięcy.  Jeśli określisz okres usuwania w latach, musisz wybrać okres od 1 do 10 lat.  Na przykład, jeśli chcesz, aby tablice były przenoszone do kosza, gdy nie były modyfikowane przez rok, możesz wybrać 1 rok i wybrać **Ostatnia modyfikacja**. |
   | **Zakres**  **(wymagane)** | Wybierz zakres dla tej zasady usuwania. Zakres wskazuje tablice, dla których ta zasada usuwania będzie obowiązywać. Możesz ustawić zakres zasady usuwania dla wszystkich tablic w organizacji lub dla określonych poziomów klasyfikacji tablic.  **Ustaw zasady usuwania dla wszystkich tablic w organizacji** Jeśli chcesz ustawić zakres zasady usuwania dla wszystkich tablic w organizacji, na liście **Zakres** wybierz **Wszystkie tablice w organizacji**.  **Ustaw zasady usuwania dla jednego lub więcej zespołów w organizacji** Jeśli chcesz ustawić zakres zasad usuwania dla jednego lub więcej zespołów w organizacji, wykonaj następujące kroki:  1. Na liście **Zakres** wybierz **Zespół**. 2. Kliknij pole **Wprowadź zespół** i wybierz każdy zespół, dla którego chcesz zastosować zasadę usuwania. Przy zespole, który wybrałeś, aby powiązać z zasadą usuwania, pojawi się znacznik wyboru.   ✏️ - Możesz wybrać wiele zespołów dla zasady usuwania. Jednak każdy dany zespół może być powiązany tylko z jedną zasadą usuwania na raz.  - Możesz wybrać jakikolwiek zespół, w tym usunięte zespoły, jako zakres przy ustawianiu zasady usuwania.   - Zespół, który jest wybrany jako zakres zasady usuwania, nie może być trwale usunięty, dopóki nie zostanie usunięty z tego zakresu.  **Ustaw zasady usuwania dla poziomu klasyfikacji tablicy**  ✏️ Aby ustawić zakres zasady usuwania dla konkretnego poziomu klasyfikacji tablicy, musisz upewnić się, że funkcja klasyfikacji danych jest włączona. Gdy zasada usuwania wykorzystuje poziom klasyfikacji tablicy, nie możesz wyłączyć funkcji klasyfikacji danych. Więcej informacji znajdziesz w dokumentacji dotyczącej [Klasyfikacji danych](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Jeśli chcesz ustawić zakres zasady usuwania dla określonego poziomu klasyfikacji tablicy, wykonaj następujące kroki:  1. Na liście **Zakres** wybierz **Klasyfikacja**. 2. Kliknij listę obok listy **Klasyfikacja**, a następnie wybierz poziomy klasyfikacji, dla których chcesz zastosować zasadę usuwania. Możesz również wyszukać poziomy klasyfikacji, a następnie je wybrać.  Obok poziomów klasyfikacji, które wybrałeś do skojarzenia z zasadą usuwania, pojawia się znacznik wyboru.  ✏️ **Uwagi:** - Możesz wybrać wiele poziomów klasyfikacji jednocześnie. - Nie można ustawić tego samego poziomu klasyfikacji dla różnych zasad usuwania. Jeśli dany poziom klasyfikacji jest już powiązany z zasadą usuwania, ten poziom klasyfikacji jest wyszarzony.  - Gdy zasada usuwania korzysta z poziomu klasyfikacji tablicy, nie można wyłączyć funkcji klasyfikacji danych.  -Kiedy poziom klasyfikacji jest powiązany z zasadą usuwania, nie można usunąć tego konkretnego poziomu klasyfikacji. - Kiedy tablica jest objęta zarówno zasadami usuwania dla wszystkich tablic w zakresie organizacji, jak i zasadami usuwania w zakresie klasyfikacji, stosowana jest zasada z dłuższym okresem usuwania. |
6. Kliknij **Dalej**.
   Pojawi się **strona przeglądu wpływu**.
7. Przejrzyj wpływ zasady usuwania. Strona przeglądu wpływu zawiera następujące informacje:
   - **Podsumowanie:** konfiguracja zasady usuwania, taka jak nazwa zasady, okres usuwania i zakres.
   - **Wpływ zasady:** liczba tablic, które będą objęte tą zasadą.
8. Aby zapisać konfigurację i zastosować zasadę usuwania, kliknij **Opublikuj**.
   Pojawi się okno dialogowe **Włącz powiadomienie o usuwaniu**.
9. **Powiadomienia o usuwaniu** umożliwiają użytkownikom otrzymywanie wcześniejszych alertów przed automatycznym przeniesieniem tablicy do kosza z powodu braku aktywności. Te alerty pomagają użytkownikom podjąć odpowiednie działania, jeśli chcą zachować swój content.

   Jeśli chcesz włączyć powiadomienia o usuwaniu:

   a. Kliknij **Powiadom**.

   b. Skonfiguruj, ile dni wcześniej powiadomienie powinno zostać wysłane — dowolna wartość między **1 a 30 dniami**.

   Jeśli włączenie powiadomień spowoduje, że **niektóre tablice zostaną natychmiast przeniesione do kosza** (ponieważ przekroczyły już próg), zostaniesz zapytany, czy powiadomić użytkowników o tych tablicach. Możesz wybrać:

   - **Tak** – aby powiadomić właścicieli i współwłaścicieli tablic, nawet jeśli tablica jest natychmiast przenoszona do kosza.

   - **Nie** – aby przenieść tablice bez wysyłania powiadomienia o tym natychmiastowym działaniu.

   Po włączeniu użytkownicy, których tablice podlegają jakiejkolwiek zasadzie usuwania z włączonymi powiadomieniami, będą:

   - Otrzymywać powiadomienia w swoich Miro **Aktualnościach** w czasie skonfigurowanego okna inspekcji.

   - Mieli możliwość otwarcia tablicy bezpośrednio z powiadomienia.

   - Zobaczą **baner** na tablicy ostrzegający o zbliżającym się automatycznym przeniesieniu do kosza, z opcją **Zachowaj tablicę**, jeśli chcą ją zatrzymać.

:::note
Utworzenie, zaktualizowanie lub usunięcie zasady uruchamia proces usuwania, który może potrwać do 24 godzin. Jednak aktualizacja nazwy lub opisu zasady odbywa się natychmiastowo, ponieważ te działania nie uruchamiają procesu usuwania.
:::

#
