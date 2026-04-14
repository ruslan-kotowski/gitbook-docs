---
title: "Tworzenie etykiet i s\u0142\xF3w kluczowych dla niestandardowych poufnych\
  \ informacji biznesowych"
article_id: 21626517022610
translation_id: 21626517022610
locale: pl-pl
sidebar_position: 11
created_at: '2024-09-26T21:36:45Z'
updated_at: '2026-03-04T22:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Twórz etykiety, aby określić warunki, takie jak słowa kluczowe lub widgety, które chcesz zidentyfikować i zlokalizować na tablicach Miro. Możesz utworzyć do 100 niestandardowych etykiet dla poufnych informacji biznesowych. Aby utworzyć etykietę, wykonaj następujące kroki:

:::note
Aby tworzyć niestandardowe etykiety, musisz mieć [rolę administratora treści wrażliwych](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby zażądać roli administratora treści wrażliwych, skontaktuj się z administratorem firmy.
:::

1. Przejdź do [ustawienia Miro](https://miro.com/app/settings).
2. Na lewym panelu, pod **Enterprise Guard**, kliknij **Odkrywanie danych**.
3. Na stronie **Odkrywanie danych** kliknij kartę **Konfiguracja**.
4. W sekcji **Poufne informacje biznesowe** kliknij przycisk **Utwórz**.
5. Na stronie **Zdefiniuj niestandardową etykietę** dodaj szczegóły etykiety.

   |  |  |
   | --- | --- |
   | **Pole** | **Opis** |
   | **Nazwa etykiety** | **Maksymalna długość:** 80 znaków  Opisowa nazwa dla niestandardowej etykiety. Możesz użyć wewnętrznej nazwy projektu firmy, jako że ta etykieta nie pojawia się w dziennikach.  **Uwaga:** Nazwa etykiety nie jest widoczna w dziennikach audytu. Jeśli chcesz przeszukiwać/wyświetlać dzienniki audytu związane z tą etykietą, możesz użyć identyfikatora etykiety. |
   | **Skrócona nazwa** | **Maksymalna długość:** 10 znaków alfanumerycznych  Skrócona wersja nazwy etykiety. Skrócona nazwa jest używana w wykrywaniu danych, eksploratorze treści i klasyfikacji danych. **Uwaga:** Skrócona nazwa nie jest widoczna w dziennikach audytu. Jeśli chcesz wyszukać/wyświetlić dzienniki audytu związane z tą etykietą, możesz użyć identyfikatora etykiety. |
   | **Opis** | **Maksymalna długość:** 500 znaków  Opis informacji, które ta etykieta wykrywa. Te informacje są przydatne dla innych administratorów. |
   | **Warunki** | Dodaj słowa kluczowe i typy widżetów, które chcesz wykrywać i dodać tę etykietę po ich wykryciu na tablicy Miro. Musisz dodać co najmniej jeden warunek.  Jeśli dodasz tylko słowa kluczowe i nie zaznaczysz żadnego pola wyboru widżetu, wykrywanie danych wykrywa wszystkie tablice zawierające dokładne dopasowania do podanych słów kluczowych dla wszystkich obsługiwanych widżetów. Obecna wersja obsługuje następujące elementy tablicy do wykrywania słów kluczowych: karteczki, karta, karta Jira, blok kodu, komentowanie, ramka, tabela, łącznik/lina, kształt, blok tekstu, tablica kanban, mapa historyjki użytkownika.  Możesz również wybrać wykrywanie tylko bloków kodu, kart Jira, kart Azure lub ekranów prototypów, bez dodawania słów kluczowych. Wykrywanie danych wtedy wykrywa wszystkie tablice zawierające te widżety.  Jeśli jako warunki dodasz zarówno słowa kluczowe, jak i widżety, kryteria zarówno słowa kluczowego, jak i widżetu muszą zostać spełnione, aby wykrywanie danych zidentyfikowało tablicę. Dzięki temu możesz doprecyzować wyszukiwanie i bardziej precyzyjnie kierować się na tablice za pomocą niestandardowych etykiet.  **Przykłady:**  - Jeśli chcesz zawęzić wykrywanie tablic do tablic związanych z rozwojem produktów, ale nie tablic związanych z marketingiem, i tablica musi zawierać nazwę projektu *Enterprise* *Guard*, a także chcesz znaleźć tylko tablice, które zawierają kartę Jira (ponieważ jest związana z rozwojem produktu), skonfigurujesz tę etykietę tak, aby zawierała słowo kluczowe *Enterprise* *Guard* i zaznaczysz pole wyboru karty Jira. Wykrywanie danych znajduje wtedy tablice, które zawierają słowo kluczowe Enterprise Guard i kartę Jira. Wykrywanie danych znajdzie również tablice, które zawierają karty Jira ze słowem kluczowym Enterprise Guard w tytule lub opisie. Jeśli tablica zawiera tylko słowo kluczowe *Enterprise* *Guard*, ale nie zawiera karty Jira, tablica nie zostanie wykryta, ponieważ nie spełnia obu określonych warunków.  - Jeśli chcesz wykryć wszystkie tablice zawierające słowo *Enterprise* *Guard* we wszystkich obsługiwanych typach widżetów, niezależnie od tego, jakie typy widżetów zawiera tablica, w sekcji **Dodaj słowa kluczowe** dodaj słowo kluczowe **Enterprise** **Guard**. W tym przypadku nie musisz dodawać żadnego typu widżetu.  - Jeśli chcesz wykryć wszystkie tablice z kartami Jira niezależnie od konkretnej zawartości, w sekcji **Dodaj typ widżetu**, zaznacz pole wyboru **karta Jira**. W tym przypadku nie musisz dodawać żadnego słowa kluczowego.    **Aby dodać słowo kluczowe:**  1. Kliknij **Dodaj słowa kluczowe**.  2. Wprowadź lub wklej słowa kluczowe oddzielone przecinkami. **Uwagi:**  - Słowa kluczowe mogą zawierać znaki alfanumeryczne i Unicode. - Możesz dodać do 100 słów kluczowych lub fraz. - Wiodące i końcowe spacje są ignorowane w słowach kluczowych. - Wykrywanie danych rozpoznaje dokładne dopasowania do podanych słów kluczowych, niezależnie od wielkości liter. - Jeśli dodasz spację przed słowem kluczowym, wykrywanie danych znajdzie dokładne dopasowania, które również mają spację przed słowem kluczowym.  - Obecne wydanie obsługuje następujące elementy tablic do wykrywania słów kluczowych: Karteczka, Karta, Karta Jira, Blok kodu, Ramka, Tabela, Łącznik/linia, Kształt, Blok tekstowy, Tablica Kanban, Mapa story (użytkownika). Notatki i komentarze nie są obecnie uwzględniane w skanowaniu wykrywania danych. Pracujemy nad włączeniem notatek i komentarzy w przyszłych aktualizacjach funkcji.  **Przykład:** Aby zidentyfikować i oznaczyć tablice zawierające słowa kluczowe *poufne* lub *wewnętrzne*, dodaj następujące słowa kluczowe: *poufne, wewnętrzne* (użyj przecinka, aby oddzielić każde słowo kluczowe). Wykrywanie danych znajdzie wówczas wszystkie tablice, które zawierają jedno z tych słów kluczowych.  **Aby dodać typ widgetu:**  1. Kliknij **Dodaj typ widgetu**.  2. Zaznacz pole wyboru dla typu widgetu, który chcesz wykrywać na tablicach Miro.  **Przykład:** Jeśli chcesz wykrywać i oznaczać tablice zawierające kartę Jira, zaznacz pole wyboru **karta Jira**. |
6. Kliknij **Dalej**.
7. Przejrzyj szczegóły niestandardowej etykiety.

   Jeśli chcesz edytować szczegóły niestandardowej etykiety, kliknij przycisk **Poprzedni**.

   Jeśli szczegóły niestandardowej etykiety są poprawne, kliknij przycisk **Utwórz niestandardową etykietę**.

   Po utworzeniu etykiety pierwsze skanowanie rozpocznie się automatycznie. Wyniki zgodne z wybranymi warunkami będą dostępne po kilku minutach lub godzinach, w zależności od liczby tablic Miro w Twojej organizacji.
