---
title: "Dodaj zasad\u0119 retencji"
article_id: 19205113739282
translation_id: 19205113739282
locale: pl-pl
sidebar_position: 10
created_at: '2024-05-28T18:00:55Z'
updated_at: '2025-12-08T16:05:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Aby dodać zasady retencji, musisz mieć [rolę administratora zarządzania danymi](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby poprosić o tę rolę, skontaktuj się z administratorem firmy.
:::

Aby dodać zasadę retencji, wykonaj następujące kroki:

1. Przejdź do [ustawień Miro](https://miro.com/app/settings).
2. W lewym panelu, pod **Enterprise Guard**, kliknij **Cykl życia treści**.
3. Kliknij kartę **Retencja**.
   Pojawi się strona **Zasady retencji**.
4. Kliknij **Dodaj zasadę retencji**.
   Pojawi się strona **Zdefiniuj kryteria**.
5. Dodaj lub wybierz odpowiednie informacje dla każdego pola. Poniższa tabela wymienia każde pole oraz jego opis.

   |  |  |
   | --- | --- |
   | **Pole** | **Opis** |
   | **Nazwa**  **(wymagane)** | Nazwa zasady retencji.  Maks. 60 znaków. |
   | **Opis**  **(opcjonalny)** | Opis tej zasady retencji.  Maks. długość: 300 znaków. |
   | **Okres retencji**  **(wymagany)** | Zapobiegaj trwałemu usunięciu tablicy przez określony czas na podstawie jednego z następujących kryteriów: **Ostatni dostęp**, **Ostatnia modyfikacja** lub **Utworzono**. Wybierz liczbę, wybierz **miesiące** lub **lata**, a następnie wybierz wydarzenie, od którego będzie obliczany okres retencji.  Jeśli określisz okres retencji w miesiącach, musisz wybrać okres retencji między 1 a 120 miesięcy.  Jeśli określisz okres retencji w latach, musisz wybrać okres retencji między 1 a 10 lat. |
   | **Zakres**  **(wymagane)** | Wybierz zakres dla tej zasady retencji. Zakres wskazuje, do których tablic ta zasada retencji ma zastosowanie. Możesz ustawić zakres zasady retencji dla wszystkich tablic w organizacji lub dla określonych poziomów klasyfikacji tablic.  **Ustaw zasady retencji dla wszystkich tablic w organizacji** Jeśli chcesz ustawić zakres zasad retencji dla wszystkich tablic w organizacji, w liście **Zakres** wybierz **Wszystkie tablice w organizacji**.  **Ustaw zasady retencji dla jednego lub więcej zespołów w organizacji** Jeśli chcesz ustawić zakres zasad retencji dla jednego lub więcej zespołów w organizacji, wykonaj następujące kroki:  1. Na liście **Zakres** wybierz **Zespół**. 2. Kliknij pole Enter team i wybierz każdy zespół, do którego chcesz zastosować zasadę retencji. Obok wybranego zespołu pojawi się znaczek wyboru, który sygnalizuje przypisanie zespołu do zasady retencji.   ✏️ - Możesz wybrać wiele zespołów dla zasady retencji. Jednak dany zespół może być powiązany jedynie z jedną zasadą retencji naraz.  - Możesz wybrać dowolny zespół, w tym usunięte zespoły, jako zakres przy ustawianiu zasady retencji.   - Zespół, który jest wybrany jako zakres dla zasady retencji, nie może być trwale usunięty, dopóki nie zostanie usunięty z tego zakresu.  **Ustaw zasady retencji dla poziomu klasyfikacji tablicy**  ✏️ Aby ustawić zakres zasady retencji dla konkretnego poziomu klasyfikacji tablicy, musisz upewnić się, że funkcja Klasyfikacja danych jest włączona. Kiedy zasada retencji korzysta z poziomu klasyfikacji tablicy, nie można wyłączyć funkcji Klasyfikacja danych. Więcej informacji znajdziesz w dokumentacji dotyczącej [Klasyfikacji danych](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Jeśli chcesz określić zakres zasady retencji dla konkretnego poziomu klasyfikacji tablicy, wykonaj następujące kroki:  1. Na liście **Zakres** wybierz **Klasyfikacja**. 2. Kliknij listę obok listy **Klasyfikacja**, a następnie wybierz poziomy klasyfikacji, dla których chcesz zastosować zasadę retencji. Możesz również wyszukać poziomy klasyfikacji, a następnie je zaznaczyć.  Obok wybranych poziomów klasyfikacji pojawi się znak wyboru, co oznacza ich skojarzenie z zasadą retencji.  ✏️ **Notatki:** - Możesz wybrać kilka poziomów klasyfikacji jednocześnie. - Nie możesz ustawić tego samego poziomu klasyfikacji dla różnych zasad retencji. Jeśli dany poziom klasyfikacji jest już połączony z zasadą retencji, to wyświetla się jako wyszarzony.  - Gdy zasada retencji wykorzystuje poziom klasyfikacji tablicy, nie można wyłączyć funkcji klasyfikacji danych.  - Kiedy poziom klasyfikacji jest powiązany z zasadą retencji, nie można usunąć tego konkretnego poziomu klasyfikacji. - Kiedy tablica jest objęta obydwoma zasadami retencji dla wszystkich tablic w organizacji oraz dla poziomu klasyfikacji, stosowana jest zasada z dłuższym okresem retencji. |
6. Kliknij **Dalej**.
   Pojawia się **Strona przeglądu wpływu**.
7. Przeanalizuj wpływ zasady retencji. Strona przeglądu wpływu dostarcza następujące informacje:
   - **Podsumowanie:** konfiguracja zasady retencji, takie jak nazwa zasady, okres retencji i zakres.
   - **Wpływ zasady:** liczba tablic, które będą regulowane przez tę zasadę. Zasada retencji dotyczy również skasowanych tablic i są one uwzględnione w obliczeniach przeglądu wpływu.

   > ✏️ Gdy tablica podlega zarówno zasadzie retencji na bazie czasu, jak i zasadzie retencji opartej na klasyfikacji, obowiązuje zasada z dłuższym okresem retencji.
8. Aby zapisać konfigurację i zastosować zasadę retencji, kliknij **Opublikuj**.

:::note
Utworzenie, aktualizacja lub usunięcie zasady uruchamia proces polityk retencji, który może potrwać do 24 godzin. Natomiast zmiana nazwy lub opisu zasady odbywa się natychmiastowo, gdyż te działania nie uruchamiają procesu polityk retencji.
:::

#
