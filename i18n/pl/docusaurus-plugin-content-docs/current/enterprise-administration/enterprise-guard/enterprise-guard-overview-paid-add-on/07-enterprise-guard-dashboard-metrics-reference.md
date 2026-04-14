---
title: "Wska\u017Aniki pulpitu Enterprise Guard"
article_id: 26718144750610
translation_id: 26718144750610
locale: pl-pl
sidebar_position: 5
created_at: '2025-05-15T00:17:54Z'
updated_at: '2025-07-22T20:38:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: admin-analytics
---

:::note
Notatki o wskaźnikach:

- Wszystkie wskaźniki w Enterprise Guard wykluczają tablice zespołów znajdujących się w koszu.
- Wszystkie wskaźniki klasyfikacji wykluczają szablony i usunięte tablice.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Tytuł** | **Opis** | **Domena** | **Pojawia się na pulpicie Przegląd** | **Ma historyczny wskaźnik** |
| Łączna liczba sklasyfikowanych tablic | Liczba tablic, którym przypisano etykietę klasyfikacji | Klasyfikacja | ✅ | ❌ |
| Liczba tablic na klasyfikację | Liczba tablic na etykietę klasyfikacji (nazwa etykiety) | Klasyfikacja | ✅ | ❌ |
| Liczba nieklasyfikowanych tablic | Liczba tablic, którym nie przypisano żadnej etykiety klasyfikacji | Klasyfikacja | ✅ | ✅ |
| Liczba tablic sklasyfikowanych ręcznie | Liczba tablic, do których ręcznie przypisano etykietę klasyfikacji (nie przez automatyczną klasyfikację) | Klasyfikacja | ❌ | ✅ |
| Liczba tablic sklasyfikowanych automatycznie | Liczba tablic, które mają automatycznie przypisaną etykietę klasyfikacji przez automatyczną klasyfikację | Klasyfikacja | ❌ | ✅ |
| Liczba tablic zawierających dane wrażliwe | Liczba tablic, które mają co najmniej jedną przypisaną wbudowaną etykietę, etykietę słowa kluczowego lub etykietę prywatności | Wykrywanie danych | ✅ | ❌ |
| Liczba tablic zawierających poufne informacje biznesowe | Liczba tablic, które mają co najmniej jedną wbudowaną etykietę lub przypisaną etykietę słowa kluczowego | Wykrywanie danych | ✅ | ✅ |
| Liczba tablic zawierających wrażliwe dane związane z prywatnością | Liczba tablic, którym przypisano co najmniej jedną etykietę prywatności | Wykrywanie danych | ✅ | ✅ |
| Liczba tablic, do których przypisano etykietę (na etykietę) | Liczba tablic dla każdej etykiety (wbudowanej, słowa kluczowego lub prywatnej) | Wykrywanie danych | ❌ | ❌ |
| Liczba włączonych etykiet związanych z prywatnością | Liczba włączonych etykiet związanych z prywatnością | Wykrywanie danych | ❌ | ❌ |
| Liczba włączonych etykiet słów kluczowych | Liczba włączonych etykiet słów kluczowych | Wykrywanie danych | ❌ | ❌ |
| Liczba włączonych etykiet poufnych informacji biznesowych | Liczba włączonych etykiet poufnych informacji biznesowych | Wykrywanie danych | ❌ | ❌ |
| Łączna liczba tablic | Łączna liczba tablic we wszystkich stanach cyklu życia (aktywne, kosz, zatrzymane) | Zarządzanie cyklem życia treści | ✅ | ❌ |
| Liczba aktywnych tablic Zwróć uwagę, że nie chodzi tutaj o aktywność na tablicach, lecz o tablice znajdujące się w stanie aktywnym w cyklu życia | Łączna liczba tablic w stanie aktywnym cyklu życia | Zarządzanie cyklem życia treści | ✅ | ✅ |
| Liczba tablic w koszu | Łączna liczba tablic, których stan cyklu życia to „w koszu” | Zarządzanie cyklem życia treści | ✅ | ✅ |
| Liczba tablic w retencji | Łączna liczba tablic w stanie retencji w cyklu życia | Zarządzanie cyklem życia treści | ✅ | ✅ |
| Liczba tablic objętych retencją | Łączna liczba tablic z przypisaną co najmniej jedną niewygasłą zasadą retencji. | Zarządzanie cyklem życia treści | ❌ | ✅ |
| Liczba tablic podlegających usunięciu | Łączna liczba tablic z przypisaną co najmniej jedną niewygasłą zasadą usuwania. | Zarządzanie cyklem życia treści | ❌ | ❌ |
| Liczba tablic podlegających retencji pogrupowana według zasad polityki | Liczba tablic w dowolnym stanie cyklu życia, które mają przypisaną co najmniej jedną zasadę retencji | Zarządzanie cyklem życia treści | ✅ | ❌ |
| Liczba tablic do usunięcia zgodnie z zasadą usuwania pogrupowana według zasad | Liczba tablic w dowolnym stanie cyklu życia, które mają przypisaną co najmniej jedną zasadę usuwania | Zarządzanie cyklem życia treści | ✅ | ❌ |
| Liczba tablic utworzonych w danym dniu/tygodniu/miesiącu | Liczba tablic utworzonych w tym tygodniu | Zarządzanie cyklem życia treści | ❌ | ✅ |
| Liczba tablic usuniętych (przeniesionych do kosza) w tym dniu/tygodniu/miesiącu | Liczba tablic usuniętych (przeniesionych do kosza) w tym tygodniu | Zarządzanie cyklem życia treści | ❌ | ✅ |
| Liczba tablic podlegających zasadom usuwania pogrupowana według daty obowiązywania zasady usuwania na miesiąc |  | Zarządzanie cyklem życia treści | ❌ | ❌ |
| Liczba spraw | Łączna liczba spraw | eDiscovery | ✅ | ❌ |
| Liczba prawnych blokad danych | Całkowita liczba prawnych blokad danych | eDiscovery | ✅ | ❌ |
| Liczba prawnych blokad danych dla konkretnej sprawy | Łączna liczba prawnych blokad danych dla konkretnej sprawy | eDiscovery | ❌ | ❌ |
| Liczba tablic objętych prawną blokadą danych | Całkowita liczba tablic objętych prawną blokadą danych | eDiscovery | ❌ | ❌ |
| Użytkownicy objęci prawną blokadą danych i łączna liczba ich tablic | Lista użytkowników objętych prawną blokadą danych i łączna liczba ich tablic | eDiscovery | ❌ | ❌ |
