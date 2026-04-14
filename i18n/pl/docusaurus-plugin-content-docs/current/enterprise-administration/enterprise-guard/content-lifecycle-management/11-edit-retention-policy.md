---
title: "Edytuj zasad\u0119 retencji"
article_id: 19205184829330
translation_id: 19205184829330
locale: pl-pl
sidebar_position: 11
created_at: '2024-05-28T18:01:39Z'
updated_at: '2025-12-08T16:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Aby edytować zasady retencji, musisz mieć [rolę administratora zarządzania danymi](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby poprosić o rolę administratora zarządzania danymi, skontaktuj się z Twoim administratorem firmy.
:::

Aby edytować zasadę retencji, wykonaj następujące kroki:

1. Przejdź do [ustawień Miro](https://miro.com/app/settings).
2. Na lewym pasku, pod **Enterprise Guard,** kliknij **Cykl życia treści**.
3. Kliknij kartę **Retencja**.
4. Na stronie **Retencji** **zasady**, kliknij zasadę, którą chcesz edytować.
   Pojawi się strona wyświetlająca informacje związane z zasadą.
5. Kliknij **Edytuj** w prawym górnym rogu strony, a następnie edytuj potrzebne pole. Poniższa tabela wymienia każde pole i jego opis.

   |  |  |
   | --- | --- |
   | **Pole** | **Opis** |
   | **Nazwa**  **(wymagane)** | Nazwa zasady retencji.  Maks. długość: 60 znaków. |
   | **Opis**  **(opcjonalne)** | Opis tej zasady retencji.  Maks. 300 znaków. |
   | **Okres retencji**  **(wymagane)** | Zabezpiecz tablice przed trwałym usunięciem na określony czas w oparciu o jedno z następujących kryteriów: **Ostatni dostęp**, **Ostatnia modyfikacja** lub **Utworzono**. Wybierz liczbę, określ **Miesiące** lub **Lata**, a następnie wybierz zdarzenie, od którego obliczany jest okres retencji.  Jeśli okres retencji określasz w miesiącach, musisz wybrać okres retencji pomiędzy 1 a 120 miesięcy.  Jeśli okres retencji określasz w latach, musisz wybrać okres retencji pomiędzy 1 a 10 lat. |
   | **Zakres**  **(wymagane)** | Wybierz zakres dla tej zasady retencji. Zakres wskazuje, do których tablic odnosi się ta zasada retencji. Możesz ustawić zakres zasady retencji dla wszystkich tablic w organizacji lub dla określonych poziomów klasyfikacji tablic.  **Ustaw zasadę retencji dla wszystkich tablic w organizacji** Jeśli chcesz ustawić zakres zasady retencji dla wszystkich tablic w organizacji, na liście **Zakres** wybierz **Wszystkie tablice w organizacji**.  **Ustaw zasadę retencji dla jednego lub więcej zespołów w organizacji** Jeśli chcesz ustawić zakres zasady retencji dla jednego lub więcej zespołów w organizacji, wykonaj następujące kroki:  1. Na liście **Zakres** wybierz **Zespół**. 2. Kliknij pole Enter zespół i wybierz każdy zespół, dla którego chcesz zastosować zasadę retencji. Obok zespołu, który wybrałeś do powiązania z zasadą retencji, pojawi się znacznik wyboru.   ✏️ - Możesz wybrać wiele zespołów dla jednej zasady retencji. Jednakże, dany zespół może być związany tylko z jedną zasadą retencji naraz. - Możesz wybrać dowolny zespół, w tym zespoły usunięte, jako zakres przy ustalaniu zasady retencji.   - Zespół wybrany jako zakres dla zasady retencji nie może być trwale usunięty, dopóki nie zostanie usunięty z tego zakresu.  **Ustaw zasady retencji dla poziomu klasyfikacji tablicy**  ✏️ Aby ustawić zakres zasady retencji na określony poziom klasyfikacji tablicy, konieczne jest włączenie funkcji klasyfikacji danych. Po tym, jak zasada retencji zacznie wykorzystywać poziom klasyfikacji tablicy, nie można wyłączyć funkcji klasyfikacji danych. Więcej informacji znajdziesz w dokumentacji na temat [Klasyfikacji danych](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Jeśli chcesz ustawić zakres zasady retencji dla konkretnego poziomu klasyfikacji tablicy, wykonaj następujące kroki:  1. Na liście **Zakres** wybierz **Klasyfikacja**. 2. Kliknij listę obok listy **Klasyfikacja**, a następnie wybierz poziomy klasyfikacji, dla których chcesz zastosować zasadę retencji. Możesz również wyszukać poziomy klasyfikacji, a następnie je wybrać.  Obok poziomów klasyfikacji, które są powiązane z zasadą retencji, pojawia się znacznik wyboru.  ✏️ **Notatki:** - Możesz wybrać wiele poziomów klasyfikacji jednocześnie. - Nie możesz ustawić tego samego poziomu klasyfikacji dla różnych zasad retencji. Jeśli konkretny poziom klasyfikacji jest już przypisany do zasady retencji, poziom klasyfikacji zostanie wyświetlony jako wyszarzony.  - Po użyciu poziomu klasyfikacji tablicy w zasadzie retencji nie można wyłączyć funkcji klasyfikacji danych.  - Jeśli poziom klasyfikacji jest związany z zasadą retencji, nie można usunąć tego konkretnego poziomu klasyfikacji. - Kiedy tablica jest zarządzana zarówno przez zasady retencji dla wszystkich tablic w zakresie organizacji, jak i w zakresie klasyfikacji, obowiązuje zasada z dłuższym okresem retencji. |
6. Gdy skończysz, kliknij **Dalej**.
   Pojawi się **strona przeglądu wpływu**.
7. Przejrzyj wpływ zasady retencji. Strona przeglądu wpływu zawiera następujące informacje:
   - **Podsumowanie:** konfiguracja zasady retencji, taka jak nazwa zasady, okres retencji i zakres.
   - **Wpływ zasady:** liczba tablic, które będą objęte tą zasadą. Zasada retencji ma również zastosowanie do tablic znajdujących się w koszu i są one uwzględniane w obliczeniach dotyczących wpływu przeglądu.

   > ✏️ Jeśli tablica jest objęta zarówno zasadą retencji opartą na czasie, jak i zasadą opartą na klasyfikacji, obowiązuje zasada z dłuższym okresem retencji.
8. Aby zapisać konfigurację i zastosować zasadę retencji, kliknij **Opublikuj**.

:::note
Tworzenie, aktualizacja lub usunięcie zasady uruchamia proces zarządzania zasadami retencji, który może potrwać do 24 godzin. Aktualizacja nazwy lub opisu zasady odbywa się jednak natychmiastowo, gdyż te działania nie uruchamiają procesu zarządzania zasadami retencji.
:::
