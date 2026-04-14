---
title: "Przegl\u0105d pulpitu Enterprise Guard"
article_id: 26707467343890
translation_id: 26707467343890
locale: pl-pl
sidebar_position: 4
created_at: '2025-05-14T13:14:06Z'
updated_at: '2025-11-25T15:51:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: admin-analytics
---

## Centralne bezpieczeństwo i widok zarządzania

Pulpit Enterprise Guard oferuje scentralizowany, ogólny wgląd w bezpieczeństwo i zarządzanie informacjami w Twojej organizacji w jednym zjednoczonym widoku. Pulpit Enterprise Guard, zaprojektowany z myślą o administratorach Enterprise Guard, łączy kluczowe wskaźniki z głównych domen — takich jak wykrywanie danych, klasyfikacja, cykl życia treści i eDiscovery — w jednej, zintegrowanej interfejsie. Zapewnia szybki wgląd w obecne zagrożenia, pokrycie zasadami i gotowość prawną, co pozwala administratorom wcześnie wykrywać potencjalne ryzyka, podejmować w porę proaktywne działania i zajmować się obszarami wymagającymi uwagi.

## Wskaźniki w czasie rzeczywistym, na podstawie których można działać.

Każdy wskaźnik na pulpicie Enterprise Guard odzwierciedla dane w czasie rzeczywistym, aktualizowane codziennie. Wszystkie wskaźniki są wykonalne i bezpośrednio łączą się z odpowiednimi pulpitami domen, umożliwiając administratorom eksplorację szczegółowych wglądów i konfigurowanie ustawień według potrzeb. Niezależnie od tego, czy monitorujesz wrażliwość tablic, status klasyfikacji, zasady retencji czy prawne blokady danych, ten pulpit zapewnia scentralizowany punkt wyjścia. Takie warstwowe podejście zapewnia spójność w całym produkcie Enterprise Guard i upraszcza nawigację dla zajętych administratorów.

## Wsparcie dla zarządzania na dużą skalę

Pulpit Enterprise Guard jest szczególnie przydatny dla administratorów Enterprise Guard zarządzających dużymi wdrożeniami w wersji Enterprise. Przynosi jasność do skomplikowanych konfiguracji zarządzania informacjami i wspiera podejmowanie świadomych decyzji poprzez konsolidację najważniejszych sygnałów w jednym miejscu. W ramach naszego zobowiązania do stworzenia bardziej intuicyjnego doświadczenia z Enterprise Guard, pulpit Enterprise Guard pomaga administratorom nie tylko zrozumieć, co się dzieje, ale także co należy zrobić dalej — z linkami do bezpośredniego podjęcia działań na podstawie danych. Niezależnie od tego, czy raportujesz przed kierownictwem, czy zarządzasz codziennym zarządzaniem danymi, ten pulpit zapewnia szybki dostęp do odpowiednich informacji, priorytetyzację działań i demonstrowanie wartości strategii bezpieczeństwa i zgodności Twojej organizacji.

## Powiązane pulpity domen-specyficzne

Oprócz pulpitu Enterprise Guard, administratorzy mogą korzystać z pakietu pulpitów domen-specyficznych, zaprojektowanych w celu zapewnienia głębszych wglądów i kontroli w kluczowych obszarach nadzoru. Każdy z tych pulpitów umożliwia ukierunkowane podejmowanie decyzji w odpowiednim obszarze, utrzymując jednocześnie zgodność z szerszą strukturą Enterprise Guard. Obejmują one:

- **Pulpit wykrywania danych:** analizuj, gdzie informacje wrażliwe znajdują się na Twoich tablicach.
- **Pulpit klasyfikacji:** śledź i zarządzaj zakresem klasyfikacji na poziomie tablicy oraz etykietami poufności.
- **Pulpit cyklu życia treści:** monitoruj polityki retencji danych i automatyzuj działania zarządzania cyklem życia.
- **Pulpit eDiscovery:** zyskaj wgląd w prawne blokady danych i usprawnij przepływy pracy przygotowawcze eDiscovery.

## Zrozum wskaźniki pulpitu

Pulpity Enterprise Guard zawierają dwa rodzaje wskaźników: bieżące i historyczne. Aby zapewnić przejrzystość i spójność, każdy wskaźnik przedstawiony na pulpitach Enterprise Guard jest zdefiniowany w [dokumentacji wskaźników pulpitu Enterprise Guard](07-enterprise-guard-dashboard-metrics-reference.md).

:::note
Notatki dotyczące wskaźników:

- Wszystkie wskaźniki w Enterprise Guard wykluczają tablice z kosza zespołów i tablice objęte prawną blokadą danych.
- Wszystkie wskaźniki klasyfikacji wykluczają szablony i tablice w koszu.
:::

## Zrozumienie błędów, pustych stanów i zmian historycznych

Zrozumienie, jak interpretować puste stany i komunikaty o błędach, jest kluczowe dla dokładnego odczytywania wskaźników pulpitu Enterprise Guard.

### Zrozumieć zachowanie danych historycznych przy zmianie ustawień.

Jeśli funkcja, taka jak klasyfikacja, zostanie wyłączona po zebraniu danych, historyczne wskaźniki nadal będą pokazywać wartości z okresu aktywnego. Na przykład, jeśli wyłączysz klasyfikację w maju, a w kwietniu klasyfikacja była aktywna z 20 sklasyfikowanymi tablicami:

- Kwietniowe wartości nadal będą pojawiać się na pulpicie.
- Wykres z maja pokaże **brak danych**, ponieważ gromadzenie danych zostało zatrzymane.
