---
title: "Przegl\u0105d pulpitu klasyfikacji"
article_id: 26886219054354
translation_id: 26886219054354
locale: pl-pl
sidebar_position: 3
created_at: '2025-05-22T11:26:15Z'
updated_at: '2025-08-18T09:36:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Pulpit klasyfikacji zapewnia scentralizowany widok dla administratorów do śledzenia i zarządzania klasyfikacją tablic w całej organizacji. Pulpit zapewnia przejrzysty podział na sklasyfikowane i nienazwane jeszcze tablice, pomagając zapewnić kompleksowy przegląd oraz zidentyfikować obszary wymagające uwagi.

Administratorzy mogą również monitorować metodę klasyfikacji używaną — czy to manualną, automatyczną, czy nieklasyfikowaną — aby zrozumieć, jak tablice są kategoryzowane. Dodatkowo historia metody klasyfikacji wizualizuje zmiany w czasie, oferując wgląd w trendy i skuteczność bieżącej klasyfikacji tablic.

:::note
Notatki do wskaźników:

- Wszystkie wskaźniki w Enterprise Guard wykluczają tablice zespołów w koszu oraz tablice objęte prawną blokadą danych.
- Wszystkie wskaźniki klasyfikacji wykluczają szablony i kosze tablic.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Tytuł** | **Opis** | **Domena** | **Pojawia się na pulpicie Przegląd** | **Ma historyczny wskaźnik** |
| Łączna liczba sklasyfikowanych tablic | Liczba tablic, którym przypisano etykietę klasyfikacji | Klasyfikacja | ✅ | ❌ |
| Liczba tablic na klasyfikację | Liczba tablic na etykietę klasyfikacji (nazwa etykiety) | Klasyfikacja | ✅ | ❌ |
| Liczba nieklasyfikowanych tablic | Liczba tablic, którym nie przypisano żadnej etykiety klasyfikacji | Klasyfikacja | ✅ | ✅ |
| Liczba tablic sklasyfikowanych ręcznie | Liczba tablic, do których ręcznie przypisano etykietę klasyfikacji (nie przez automatyczną klasyfikację) | Klasyfikacja | ❌ | ✅ |
| Liczba tablic sklasyfikowanych automatycznie | Liczba tablic, które mają automatycznie przypisaną etykietę klasyfikacji przez automatyczną klasyfikację | Klasyfikacja | ❌ | ✅ |

## Zrozumienie błędów, pustych stanów i zmian historycznych

Zrozumienie, jak interpretować puste stany i komunikaty o błędach, jest kluczowe dla dokładnego odczytywania wskaźników pulpitu Enterprise Guard.

### Zrozumienie zachowania danych historycznych przy zmianie ustawień

Jeśli funkcja, taka jak klasyfikacja, zostanie wyłączona po zebraniu danych, historyczne wskaźniki nadal będą pokazywać wartości z okresu aktywnego. Na przykład, jeśli wyłączysz klasyfikację w maju, a klasyfikacja była aktywna w kwietniu z 20 tablicami sklasyfikowanymi:

- Kwietniowe wartości nadal będą pojawiać się na pulpicie.
- Wykres z maja pokaże **brak danych**, ponieważ gromadzenie danych zostało zatrzymane.
