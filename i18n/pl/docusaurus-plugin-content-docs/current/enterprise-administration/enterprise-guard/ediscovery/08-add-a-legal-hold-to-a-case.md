---
title: "Dodaj prawn\u0105 blokad\u0119 danych do sprawy"
article_id: 22120471564946
translation_id: 22120471564946
locale: pl-pl
sidebar_position: 7
created_at: '2024-10-21T23:29:24Z'
updated_at: '2025-11-25T16:22:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Utworzenie prawnej blokady danych to kluczowy proces dla [administratorów eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md), gdy przewidywane jest postępowanie sądowe lub dochodzenie. Prawne blokady danych zapewniają, że istotne tablice Miro są zachowane i zabezpieczone przed zmianą, usunięciem lub zniszczeniem. Jest to niezbędne dla utrzymania zgodności z wymaganiami prawnymi i regulacyjnymi, zapobiegania utracie lub modyfikacji kluczowych danych, a także dla ochrony ważnych dowodów przez cały czas trwania sprawy prawnej. Prawna blokada danych umożliwia administratorom zabezpieczenie danych, zapewniając, że wszystkie istotne tablice Miro są dostępne do przeglądu w każdej chwili.

Tworzenie prawnej blokady danych polega na zidentyfikowaniu odpowiednich użytkowników i tablic Miro powiązanych ze sprawą oraz zastosowaniu blokady, aby zapobiec wszelkim modyfikacjom. Administratorzy mogą zarządzać wieloma blokadami w obrębie jednej sprawy, co zapewnia grupowanie i zachowanie wszystkich niezbędnych danych w zorganizowany sposób. Proces ten pomaga utrzymać integralność danych i odpowiedzialność, gwarantując pełną zgodność organizacji i przygotowanie do procesu prawnego.

Tablice Miro pod prawnej blokadą danych mogą nadal być dostępne i edytowane, ale wszystkie wersje zostaną zachowane. Jeśli treść zostanie usunięta, nadal będzie dostępna w ramach prawnej blokady danych. Liczba elementów treści objętych blokadą może wzrosnąć na podstawie przyszłych działań użytkowników. Po nałożeniu na tablicę prawnej blokady danych wszystkie wersje tablicy są przechowywane na czas nieokreślony, aż do zwolnienia blokady.

Aby utworzyć prawną blokadę danych, wykonaj następujące kroki:

:::note
Musisz mieć [rolę eDiscovery Admin](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md), aby wykonać to zadanie. Aby ubiegać się o rolę eDiscovery Admin, skontaktuj się z administratorem firmy.
:::

1. Przejdź do swoich ustawień Miro.
2. W lewym panelu, w sekcji **Enterprise Guard**, kliknij **eDiscovery**.
3. Na stronie **eDiscovery** kliknij kartę **Sprawy**.
4. Na stronie **Utwórz sprawę** kliknij sprawę, do której chcesz dodać prawną blokadę danych.
5. Kliknij **Dodaj prawną blokadę danych**.
6. Na stronie **Dodaj prawną blokadę danych** wpisz lub wybierz odpowiednie informacje dla każdego pola. W poniższej tabeli wymieniono każde pole i jego opis.

   |  |  |
   | --- | --- |
   | **Pole** | **Opis** |
   | Nazwa prawnej blokady danych  **(wymagane)** | Nazwa prawnej blokady danych.  Maks. długość: 60 znaków. |
   | Kryteria  **(wymagane)** | Rodzaj zawartości uwzględniony w tej prawnej blokadzie danych. Ta wersja obsługuje tylko całą zawartość. |
   | **Użytkownicy, którzy są właścicielami, współwłaścicielami, uzyskali dostęp do treści, zmodyfikowali je lub je utworzyli**  **(wymagane)** | Dodaj użytkowników, których chcesz objąć prawną blokadą danych. Kliknij pole, aby wyszukać po nazwisku lub adresie e-mail. Możesz dodać jednocześnie do 200 użytkowników.    **Uwagi:**  - Gdy użytkownik objęty prawną blokadą danych otwiera, modyfikuje lub w jakikolwiek sposób oddziałuje na tablicę (zmienia nazwę lub dodaje treści), ta tablica zostaje oflagowana i zachowana. Na przykład, jeśli nazwa tablicy zostanie zmieniona lub dodana zostanie nowa treść, automatycznie zostanie objęta prawną blokadą danych. Dodatkowo, własność tablicy i jej utworzenie także zostaną wstrzymane.  - Gdy tworzy się prawną blokadę danych, dotyczy ona tablic utworzonych, posiadanych lub współposiadanych przez zarządców w momencie blokady. Ponadto, obejmuje także wszelkie tablice, do których zarządcy uzyskają dostęp i zmodyfikują je po nałożeniu blokady. Szczegóły dotyczące historycznego dostępu do tablic i ich aktualizacji nie są dostępne w tej wersji. |
7. Kliknij **Next**. Pojawi się strona **Przegląd skutków**.
8. Przejrzyj skutki utworzenia tej prawnej blokady danych, takie jak liczba istniejących tablic, które zostaną objęte blokadą, oraz użytkowników, którzy posiadali, współposiadali, uzyskali dostęp do tablic, modyfikowali lub je tworzyli.

   **Uwagi:**
   - Tablice objęte blokadą mogą być nadal dostępne i edytowane, ale wszystkie ich wersje zostaną zachowane. Jeśli treść zostanie usunięta, nadal będzie dostępna w ramach blokady. Liczba elementów treści objętych prawną blokadą danych może wzrosnąć na podstawie przyszłych działań użytkownika.

   - Gdy użytkownik objęty prawną blokadą danych otwiera, modyfikuje lub w jakikolwiek sposób wchodzi w interakcję z tablicą (zmieniając nazwę lub dodając treść), tablica zostanie oznaczona i zachowana. Na przykład, jeśli nazwa tablicy zostanie zmieniona lub treść zaktualizowana, zostanie automatycznie objęta blokadą prawną. Ponadto, własność tablicy i jej utworzenie są objęte blokadą.

   - Gdy tworzona jest prawna blokada danych, dotyczy ona tablic, które opiekunowie stworzyli, posiadali lub współposiadali w momencie wprowadzenia blokady. Dodatkowo, także wszystkie tablice, do których opiekunowie mają dostęp i które modyfikują po wprowadzeniu blokady, są do niej włączane. Historyczne dane dostępu do tablic i ich aktualizacji nie są dostępne w tej wersji.
9. Po przejrzeniu wpływu tworzonej prawnej blokady danych kliknij **Dodaj prawną blokadę danych**.
    Strona sprawy pojawi się, wyświetlając zawartą w niej prawna blokadę danych oraz informacje o każdej blokadzie, takie jak nazwa blokady, rodzaj treści objętej blokadą, liczba użytkowników objętych blokadą, data utworzenia blokady, status blokady oraz liczba tablic objętych blokadą.
