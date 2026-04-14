---
title: "Przegl\u0105d pulpitu wykrywania danych"
article_id: 26806897106834
translation_id: 26806897106834
locale: pl-pl
sidebar_position: 1
created_at: '2025-05-19T11:10:19Z'
updated_at: '2025-11-25T15:51:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Pulpit wykrywania danych zapewnia scentralizowany widok informacji wrażliwych wykrytych na tablicach Twojej organizacji. Umożliwia administratorom monitorowanie, klasyfikowanie i zarządzanie ryzykiem danych poprzez identyfikację treści związanych z prywatnością lub poufnych informacji biznesowych. Pulpit wykrywania danych zawiera następujące wskaźniki:

:::note
Wszystkie wskaźniki w Enterprise Guard wykluczają tablice należące do usuniętych zespołów oraz tablice objęte prawną blokadą danych.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Tytuł** | **Opis** | **Domena** | **Pojawia się na pulpicie Przegląd** | **Ma historyczny wskaźnik** |
| Liczba tablic zawierających dane wrażliwe | Liczba tablic, które mają co najmniej jedną przypisaną wbudowaną etykietę, etykietę słowa kluczowego lub etykietę prywatności | Wykrywanie danych | ✅ | ❌ |
| Liczba tablic zawierających poufne informacje biznesowe | Liczba tablic, które mają co najmniej jedną wbudowaną etykietę lub przypisaną etykietę słowa kluczowego | Wykrywanie danych | ✅ | ✅ |
| Liczba tablic zawierających wrażliwe dane związane z prywatnością | Liczba tablic, którym przypisano co najmniej jedną etykietę prywatności | Wykrywanie danych | ✅ | ✅ |
| Liczba tablic, do których przypisano etykietę (na etykietę) | Dla każdej indywidualnej etykiety w trzech kategoriach (wbudowane, słowo kluczowe lub prywatność) policz liczbę tablic, którym przypisano tę etykietę. | Wykrywanie danych | ❌ | ❌ |
| Liczba włączonych etykiet związanych z prywatnością | Liczba włączonych etykiet związanych z prywatnością | Wykrywanie danych | ❌ | ❌ |
| Liczba włączonych etykiet słów kluczowych | Liczba włączonych etykiet słów kluczowych | Wykrywanie danych | ❌ | ❌ |
| Liczba włączonych etykiet poufnych informacji biznesowych | Liczba włączonych etykiet poufnych informacji biznesowych | Wykrywanie danych | ❌ | ❌ |

## Zrozumienie błędów, pustych stanów i zmian historycznych

Zrozumienie, jak interpretować puste stany i komunikaty o błędach, jest kluczowe dla dokładnego odczytywania wskaźników pulpitu Enterprise Guard.

### Zrozumienie zachowania danych historycznych przy zmianie ustawień

Jeśli wykrywanie danych zostanie wyłączone po zebraniu danych, historyczne wskaźniki nadal będą pokazywać wartości z okresu aktywnego. Na przykład jeśli wyłączysz wykrywanie danych w maju, a było ono aktywne w kwietniu:

- Kwietniowe wartości nadal będą pojawiać się na pulpicie.
- Wykres z maja pokaże **brak danych**, ponieważ gromadzenie danych zostało zatrzymane.

## Wyświetlanie wyników wykrywania danych

Cykl wykrywania danych uruchamia się co najmniej raz na godzinę i skanuje wszystkie aktualizacje tablic pod kątem informacji związanych z prywatnością, poufnych danych biznesowych lub niestandardowych poufnych danych biznesowych, zgodnie z Twoją konfiguracją wykrywania danych. Obejmuje to tablice, które zostały już zeskanowane w poprzednim cyklu wykrywania danych.

Wyniki wykrywania danych pojawiają się poniżej wykresów wskaźników. Możesz wyświetlić informacje, takie jak nazwa etykiety, stan, typ, klasyfikacja, liczba tablic itp.

Aby uzyskać więcej informacji na temat przeglądania tablic z dokumentacją związaną z prywatnością, [przeczytaj ten artykuł](16-review-boards-with-privacy-related-information.md).

Aby uzyskać więcej informacji na temat przeglądania tablic zawierających poufne i niestandardowe dane biznesowe, [zobacz ten artykuł](14-review-boards-with-business-sensitive-and-custom-business-sensitive-information-beta.md).

Aby uzyskać więcej informacji na temat przeglądania tablic z niestandardowymi etykietami poufnych informacji biznesowych, [zobacz ten artykuł](15-review-custom-business-sensitive-labels-and-data-discovery-results.md).

:::note
- Aby wyświetlić wyniki wykrywania danych, musisz mieć [rolę administratora treści wrażliwych](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby poprosić o rolę administratora treści wrażliwych, skontaktuj się z administratorem firmy.

- Choć nieustannie współpracujemy z naszym partnerem technologicznym i klientami nad poprawą systemu wykrywania danych wrażliwych, nie możemy zagwarantować, że wykryje i oznaczy 100% danych wrażliwych na Twoich tablicach. Nasz system wykrywania treści wrażliwych używa wzorców i innych kryteriów do określenia prawdopodobieństwa dopasowania. Czasami system może błędnie oznaczać dane na Twoich tablicach jako prawdopodobnie wrażliwe (fałszywy pozytyw) lub nie oznaczać danych jako wrażliwe (fałszywy negatyw). Różne czynniki przyczyniają się do tych zdarzeń, w tym bliskość powiązanych terminów lub formatowanie danych wrażliwych.

Aby uzyskać więcej informacji o sposobach eliminowania fałszywych dopasowań, zobacz [Eliminowanie dopasowań treści wrażliwych](11-suppress-a-sensitive-content-match.md).
:::

##

##
