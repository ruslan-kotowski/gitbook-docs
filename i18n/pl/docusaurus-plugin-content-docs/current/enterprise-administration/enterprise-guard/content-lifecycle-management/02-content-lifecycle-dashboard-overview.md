---
title: "Przegl\u0105d pulpitu cyklu \u017Cycia tre\u015Bci"
article_id: 26894063726482
translation_id: 26894063726482
locale: pl-pl
sidebar_position: 2
created_at: '2025-05-22T16:02:58Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

Pulpit cyklu życia treści zapewnia scentralizowane wyświetlanie, umożliwiające administratorom monitorowanie i zarządzanie pełnym cyklem życia tablic — od ich tworzenia po usuwanie — zgodnie z zasadami retencji danych organizacji. Zapewnia wgląd w bieżący etap cyklu życia każdej tablicy, co pomaga w odpowiednim zarządzaniu treściami.

Administratorzy mogą również śledzić tablice objęte zasadami retencji i usuwania oraz analizować historyczne trendy stosowania zasad. Pulpit obejmuje prognozę usuwania, co umożliwia proaktywne planowanie nadchodzących zautomatyzowanych działań w ramach cyklu życia. To umożliwia konsekwentne zarządzanie treściami opartymi na zasadach w całej organizacji.

:::note
Wszystkie wskaźniki w Enterprise Guard wykluczają tablice zespołów w koszu oraz tablice objęte prawną blokadą danych.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Tytuł** | **Opis** | **Domena** | **Pojawia się na pulpicie Przegląd** | **Ma historyczny wskaźnik** |
| Łączna liczba tablic | Łączna liczba tablic we wszystkich stanach cyklu życia (aktywne, kosz, zatrzymane) | Zarządzanie cyklem życia treści | ✅ | ❌ |
| Liczba aktywnych tablic Zwróć uwagę, że nie chodzi tutaj o aktywność na tablicach, lecz o tablice znajdujące się w stanie aktywnym w cyklu życia | Łączna liczba tablic w stanie aktywnym cyklu życia | Zarządzanie cyklem życia treści | ✅ | ✅ |
| Liczba tablic w koszu | Łączna liczba tablic, których stan cyklu życia to „w koszu” | Zarządzanie cyklem życia treści | ✅ | ✅ |
| Liczba tablic w retencji | Łączna liczba tablic w stanie retencji w cyklu życia | Zarządzanie cyklem życia treści | ✅ | ✅ |
| Liczba tablic objętych retencją | Łączna liczba tablic z przypisaną co najmniej jedną niewygasłą zasadą retencji. | Zarządzanie cyklem życia treści | ❌ | ✅ |
| Liczba tablic podlegających usunięciu | Łączna liczba tablic z przypisaną co najmniej jedną niewygasłą zasadą usuwania. | Zarządzanie cyklem życia treści | ❌ | ❌ |
| Liczba tablic podlegających retencji, pogrupowana według zasad polityki | Liczba tablic w dowolnym stanie cyklu życia, które mają przypisaną co najmniej jedną zasadę retencji na każdą z zasad | Zarządzanie cyklem życia treści | ✅ | ❌ |
| Liczba tablic do usuwania zgodnie z zasadą usuwania pogrupowana według zasad | Liczba tablic w dowolnym stanie cyklu życia, które mają przypisaną co najmniej jedną zasadę usuwania na każdą z zasad | Zarządzanie cyklem życia treści | ✅ | ❌ |
| Liczba tablic utworzonych w danym dniu/tygodniu/miesiącu | Liczba tablic utworzonych w tym tygodniu | Zarządzanie cyklem życia treści | ❌ | ✅ |
| Liczba tablic usuniętych (przeniesionych do kosza) w tym dniu/tygodniu/miesiącu | Liczba tablic usuniętych (przeniesionych do kosza) w tym tygodniu | Zarządzanie cyklem życia treści | ❌ | ✅ |
| Liczba tablic podlegających zasadom usuwania pogrupowana według daty obowiązywania zasady usuwania na miesiąc |  | Zarządzanie cyklem życia treści | ❌ | ❌ |

## Zrozumienie błędów, pustych stanów i zmian historycznych

Zrozumienie, jak interpretować puste stany i komunikaty o błędach, jest kluczowe dla dokładnego odczytywania wskaźników pulpitu Enterprise Guard.

### Zrozumienie zachowania danych historycznych przy zmianie ustawień

Jeśli wykrywanie danych zostanie wyłączone po zebraniu danych, historyczne wskaźniki nadal będą pokazywać wartości z okresu aktywnego. Na przykład jeśli wyłączysz wykrywanie danych w maju, a było ono aktywne w kwietniu:

- Kwietniowe wartości nadal będą pojawiać się na pulpicie.
- Wykres z maja pokaże **brak danych**, ponieważ gromadzenie danych zostało zatrzymane.

###
