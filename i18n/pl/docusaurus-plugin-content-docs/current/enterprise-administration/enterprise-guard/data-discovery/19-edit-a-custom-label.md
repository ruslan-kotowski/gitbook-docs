---
title: "Edytuj etykiet\u0119 w\u0142asn\u0105"
article_id: 21690361870354
translation_id: 21690361870354
locale: pl-pl
sidebar_position: 18
created_at: '2024-09-30T13:43:27Z'
updated_at: '2026-03-04T23:02:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

:::note
Zalecamy edytowanie etykiet wyłącznie przed ich powiązaniem z poziomem klasyfikacji.
:::

Edytuj etykiety, aby zaktualizować warunki, takie jak słowa kluczowe lub widgety, które chcesz zidentyfikować i zlokalizować na tablicach Miro. Aby edytować etykietę, wykonaj następujące kroki:

:::note
Aby edytować etykiety niestandardowe, musisz mieć [rolę administratora treści wrażliwych](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby uzyskać rolę administratora treści wrażliwych, skontaktuj się z administratorem firmy.
:::

1. Przejdź do swoich [ustawień Miro](https://miro.com/app/settings).
2. W lewym panelu, pod **Enterprise Guard,** kliknij **Odkrywanie danych**.
3. Na stronie **Odkrywanie danych** **Przegląd**, kliknij menu z 3 kropkami w wierszu etykiety, którą chcesz edytować, a następnie kliknij **Edytuj etykietę**.
4. Na stronie **Edycja niestandardowej etykiety** edytuj szczegóły etykiety.

   |  |  |
   | --- | --- |
   | **Pole** | **Opis** |
   | **Nazwa etykiety** | **Maksymalna długość:** 80 znaków  Opisowa nazwa dla niestandardowej etykiety. Możesz użyć wewnętrznej nazwy projektu firmy, ponieważ ta etykieta nie pojawia się w dziennikach.  **Uwaga:** Nazwa etykiety nie jest widoczna w dziennikach audytu. Jeśli chcesz przeszukiwać/wyświetlać dzienniki audytu związane z tą etykietą, możesz użyć identyfikatora etykiety. |
   | **Skrócona nazwa** | **Maksymalna długość:** 10 znaków alfanumerycznych  Skrócona wersja nazwy etykiety. Skrócona nazwa jest używana do odniesienia się do tej niestandardowej etykiety w wykrywaniu danych i eksploratorze treści. **Uwaga:** Skrócona nazwa nie jest widoczna w dziennikach audytu. Jeśli chcesz przeszukiwać/wyświetlać dzienniki audytu związane z tą etykietą, możesz użyć identyfikatora etykiety. |
   | **Opis** | **Maksymalna długość:** 500 znaków  Opis informacji, które ta etykieta wykrywa. Te informacje są użyteczne dla innych administratorów. |
   | **Warunki** | Dodaj słowa kluczowe i typy widgetów, które chcesz wykrywać i do których chcesz przypisać tę etykietę po wykryciu na tablicy Miro. Musisz dodać co najmniej jeden warunek.  Jeśli dodasz tylko słowa kluczowe i nie zaznaczysz żadnego pola wyboru widgetu, wykrywanie danych wykrywa wszystkie tablice zawierające dokładne dopasowania podanych przez Ciebie słów kluczowych dla wszystkich obsługiwanych widgetów. Obecna wersja obsługuje następujące elementy tablic dla wykrywania słów kluczowych: karteczka, karta, karta Jira, blok kodu, komentowanie, ramka, tabela, łącze/kreska, kształt, blok tekstu, tablica kanban, mapa historyjki użytkownika.  Możesz również wybrać tylko wykrywanie bloków kodu, kart Jira, kart Azure lub ekranów prototypowania, bez dodawania słów kluczowych. Wtedy wykrywanie danych wykrywa wszystkie tablice zawierające te widgety.  Jeśli dodasz zarówno słowa kluczowe, jak i widżety jako warunki, zarówno kryteria związane ze słowami kluczowymi, jak i widżetami muszą być spełnione, aby wykrywanie danych mogło wykryć tablicę. To pozwala precyzyjniej dostosować wyszukiwanie i celować w tablice z użyciem niestandardowych etykiet.  **Przykłady:**  - Jeśli chcesz zawęzić wykrywanie tablic, aby wykrywały wyłącznie tablice związane z rozwojem produktów, ale nie z marketingiem, a tablica musi zawierać nazwę projektu *Enterprise* *Guard*, i chcesz znaleźć tylko te tablice, które również zawierają kartę Jira (ponieważ jest związana z rozwojem produktów), skonfigurujesz tę etykietę, aby zawierała słowo kluczowe *Enterprise* *Guard* i zaznaczyć pole wyboru karty Jira. Wykrywanie danych następnie znajduje tablice zawierające słowo kluczowe Enterprise Guard oraz kartę Jira. Wykrywanie danych znajduje również tablice, które zawierają karty Jira ze słowem kluczowym Enterprise Guard w tytule lub opisie. Jeśli tablica zawiera tylko słowo kluczowe *Enterprise* *Guard*, ale nie zawiera karty Jira, tablica nie jest wykrywana, ponieważ nie spełnia obu określonych warunków.  - Jeśli chcesz wykryć wszystkie tablice z napisem *Enterprise* *Guard* dla wszystkich obsługiwanych typów widżetów, niezależnie od typów widżetów, jakie tablica zawiera, w sekcji **Dodaj słowa kluczowe** dodaj słowo kluczowe **Enterprise** **Guard**. W tym przykładzie nie musisz dodawać żadnego rodzaju widżetu.  - Jeśli chcesz wykryć wszystkie tablice z kartami Jira, niezależnie od jakiejkolwiek treści, w sekcji **Dodaj typ widżetu** zaznacz pole wyboru **karta Jira**. W tym przykładzie nie musisz dodawać żadnego słowa kluczowego.    **Aby dodać słowo kluczowe:**  1. Kliknij **Dodaj słowa kluczowe**.  2. Wprowadź lub wklej słowa kluczowe oddzielone przecinkami. **Uwagi:**  - Słowa kluczowe mogą zawierać znaki alfanumeryczne i Unicode.  - Możesz dodać do 100 słów kluczowych lub fraz. - Wykrywanie danych wykrywa dokładne dopasowania do dostarczonych słów kluczowych, niezależnie od wielkości liter. - Aktualna wersja obsługuje następujące elementy tablicy do wykrywania słów kluczowych: karteczka, karta, karta Jira, blok kodu, ramka, tabela, konektor/linia, kształt, blok tekstu, tablica kanban, mapa historyjki użytkownika. Notatki i komentarze nie są obecnie uwzględnione w skanowaniu wykrywania danych. Pracujemy nad uwzględnieniem notatek i komentarzy w kolejnych wersjach ulepszających funkcje.  **Przykład:** Aby zidentyfikować i oznaczyć tablice zawierające słowa kluczowe *poufne* lub *wewnętrzne*, dodaj następujące słowa kluczowe: *poufne, wewnętrzne* (użyj przecinka, aby oddzielić każde słowo kluczowe). Wykrywanie danych następnie znajdzie wszystkie tablice, które zawierają któreś z tych słów kluczowych.  **Aby dodać typ widgetu:**  1. Kliknij **Dodaj typ widgetu**.  2. Zaznacz pole wyboru dla typu widżetu, który chcesz wykrywać na tablicach Miro.  **Przykład:** Jeśli chcesz wykrywać i etykietować tablice zawierające kartę Jira, zaznacz pole wyboru **karta Jira**. |
5. Kliknij **Dalej**.
6. Przejrzyj szczegóły niestandardowej etykiety.

   Jeśli chcesz zaktualizować szczegóły niestandardowej etykiety, kliknij przycisk **Wstecz**.

   Jeśli szczegóły niestandardowej etykiety są poprawne, kliknij przycisk **Zaktualizuj niestandardową etykietę**.

   Po zaktualizowaniu niestandardowej etykiety skanowanie rozpocznie się automatycznie. Wyniki zgodne z wybranymi warunkami będą dostępne po kilku minutach lub godzinach, w zależności od liczby tablic Miro w Twojej organizacji.
