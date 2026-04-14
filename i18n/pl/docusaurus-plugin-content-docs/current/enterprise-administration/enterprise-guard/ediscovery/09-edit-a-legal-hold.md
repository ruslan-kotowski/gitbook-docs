---
title: "Edytuj prawn\u0105 blokad\u0119 danych"
article_id: 27968005251090
translation_id: 27968005251090
locale: pl-pl
sidebar_position: 8
created_at: '2025-07-09T17:31:49Z'
updated_at: '2025-11-25T15:52:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Edycja prawnej blokady danych umożliwia administratorom eDiscovery dostosowywanie i udoskonalanie bieżących działań w zakresie zachowania danych w miarę zmieniających się wymagań spraw. Niezależnie od tego, czy identyfikowani są nowi opiekunowie, dodatkowe tablice Miro stają się istotne, czy też istniejące tablice lub użytkownicy przestają być ważni, edycja prawnej blokady danych zapewnia, że właściwe dane pozostają zachowane i możliwe do obrony przez cały proces prawny.

Administratorzy mogą aktualizować nazwę lub opis prawnej blokady danych oraz dodawać lub usuwać użytkowników i tablice według potrzeb. Ta elastyczność wspiera dynamiczne przepływy pracy prawnej i zapewnia, że zachowanie jest precyzyjne, aktualne i zgodne z zakresem sprawy prawnej, utrzymując zgodność przy jednoczesnym unikaniu niepotrzebnej retencji danych.

Gdy edytowana jest prawna blokada danych:

- Nowo dodane do zatrzymania tablice będą miały zachowywane swoje wersje od tego momentu.
- Tablice lub użytkownicy usunięci z prawnej blokady danych przestaną być zachowywani, a ich wersje nie będą już przechowywane jako część tej prawnej blokady danych.
- Tablice objęte blokadą będą miały zachowane wszystkie wersje, łącznie z tymi, które zostały usunięte po nałożeniu blokady.

Takie podejście zapewnia organizacjom możliwość reagowania na potrzeby prawne z dokładnością i odpowiedzialnością w miarę postępu sprawy.

Aby edytować prawną blokadę danych, wykonaj następujące kroki:

:::note
Musisz mieć [rolę Administratora eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md), aby wykonać to zadanie. Aby poprosić o rolę administratora eDiscovery, skontaktuj się z administratorem firmy.
:::

1. Przejdź do swoich ustawień Miro.
2. W panelu po lewej stronie, w sekcji **Enterprise Guard**, kliknij **eDiscovery**.
3. Na stronie **eDiscovery** kliknij kartę **Sprawy**.
4. Kliknij sprawę, w której chcesz edytować prawną blokadę danych.
   Lista prawnych blokad danych w ramach sprawy jest wyświetlana.
5. Kliknij menu z 3 kropkami w wierszu prawnej blokady danych, którą chcesz edytować, a następnie kliknij **Edycja prawnej blokady danych**.
6. Na stronie **Edycja prawnej blokady danych** wprowadź lub wybierz odpowiednie informacje dla poszczególnych pól. Poniższa tabela zawiera każde pole i jego opis.

   |  |  |
   | --- | --- |
   | **Pole** | **Opis** |
   | Nazwa prawnej blokady danych  **(wymagane)** | Nazwa prawnej blokady danych  Maksymalna długość: Pokaż {} długość cyklu{}: Przekroczono maksymalną długość: Nazwa tablicy przekracza maksymalną długość. Maks: Usuń {} simbol, aby nazwa mieściła się w limicie. Przekroczona maksymalna długość dokumentu: Max długość przekroczona: Podaj wymiary maksymalnej długości: Max: Usuń {} symbol, aby pasować do maksymalnej długości nazwy: Przekroczona maksymalna zawartość dokumentu: Maksymalna długość przekroczona: Przekroczona maksymalna długość dokumentu 60 znaków. |
   | Kryteria  **(wymagane)** | Rodzaj treści zawartych w tej prawnej blokadzie danych. To wydanie obsługuje tylko całą treść. |
   | **Użytkownicy, którzy są właścicielami, współwłaścicielami, uzyskali dostęp do treści, zmodyfikowali je lub je utworzyli**  **(wymagane)** | Dodaj użytkowników, których chcesz umieścić na prawnej blokadzie danych. Kliknij pole, aby wyszukać według nazwiska lub e-maila. Możesz mieć maksymalnie 200 użytkowników na prawnej blokadzie danych, w tym użytkowników dodanych w aktualizacjach prawnej blokady danych.  **Notatki:**  - Gdy użytkownik objęty prawną blokadą danych otwiera, modyfikuje lub w jakikolwiek sposób wchodzi w interakcję z tablicą (np. zmieniając jej nazwę lub dodając treści), tablica jest oznaczana i zachowywana. Na przykład, jeśli nazwa tablicy zostanie zmieniona lub jej zawartość zaktualizowana, zostanie ona automatycznie objęta prawną blokadą danych. Dodatkowo własność tablicy i tworzenie tablicy zostają wstrzymane.  - Gdy prawna blokada danych jest edytowana, dotyczy tablic, które opiekunowie stworzyli, posiadają lub są współwłaścicielami w momencie nałożenia blokady. Dodatkowo, wszystkie tablice, do których opiekunowie mają dostęp i które modyfikują po wprowadzeniu blokady, również są uwzględniane. Szczegóły dostępu i aktualizacji tablicy nie są dostępne w tej wersji.  - Tablice nowo dodane do blokady będą miały swoje wersje zachowywane od momentu zapisania aktualizacji prawnej blokady danych w kroku 9.  - Tablice lub użytkownicy usunięci z prawnej blokady danych przestaną być zachowywani, a ich wersje nie będą już dłużej przechowywane jako część tej blokady.  Tablice objęte blokadą będą nadal miały zachowane wszystkie wersje, w tym wszelkie usunięcia, które nastąpią po zastosowaniu blokady. |
7. Kliknij **Dalej**. Strona **Sprawdź wpływ** pojawia się.
8. Przeanalizuj wpływ utworzenia tej prawnej blokady danych, takie jak:
   - Liczba tablic, które pozostają objęte blokadą, zostaną zwolnione z blokady, oraz dodane do blokady.
   - Użytkownicy, którzy posiadali, współposiadali, uzyskali dostęp do tablic, zmodyfikowali je lub je utworzyli.
   Kryteria wstrzymania.
   - Lista tablic objętych blokadą.

   **Notatki:**
   Tablice objęte blokadą danych mogą być nadal dostępne i edytowane, ale wszystkie ich wersje zostaną zachowane. Jeśli treść zostanie usunięta, nadal będzie dostępna w ramach blokady. Liczba elementów treści objętych prawną blokadą danych może wzrosnąć na podstawie przyszłych działań użytkownika.

   - Kiedy użytkownik objęty prawną blokadą danych otwiera, modyfikuje lub w jakikolwiek sposób wchodzi w interakcję z tablicą (zmieniając jej nazwę lub dodając treść), ta tablica jest oznaczana i zachowywana. Na przykład, jeśli nazwa tablicy zostanie zmieniona lub zawartość zostanie zaktualizowana, zostanie ona automatycznie objęta prawną blokadą danych. Dodatkowo, własność tablicy oraz tworzenie tablicy zostają wstrzymane.

   - Gdy prawna blokada danych zostaje utworzona, ma zastosowanie do tablic, które opiekunowie utworzyli, posiadali lub współposiadali w momencie nałożenia blokady. Dodatkowo, wszystkie tablice, do których kustosze uzyskują dostęp i które modyfikują po wprowadzeniu blokady, również są uwzględnione. Dostęp do historii tablic i szczegóły aktualizacji nie są dostępne w tej wersji.
9. Po przejrzeniu wpływu tworzonej prawnej blokady danych, kliknij **Zapisz prawną blokadę danych**.
   Strona sprawy wyświetla zaktualizowaną prawną blokadę danych, takie jak nazwa blokady, rodzaj treści objętych blokadą, liczba użytkowników w tej blokadzie, data utworzenia blokady, status blokady oraz liczba tablic objętych blokadą.
