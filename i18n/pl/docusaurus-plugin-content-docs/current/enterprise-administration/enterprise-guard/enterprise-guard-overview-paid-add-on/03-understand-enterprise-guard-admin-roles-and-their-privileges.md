---
title: Zrozum role administratora Enterprise Guard i ich uprawnienia
article_id: 15695755655954
translation_id: 15695755655954
locale: pl-pl
sidebar_position: 1
created_at: '2023-12-11T18:33:53Z'
updated_at: '2026-03-12T22:21:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Możliwości Enterprise Guard są kontrolowane poprzez uprawnienia administracyjne. Te uprawnienia mogą być nadane za pośrednictwem zdefiniowanych ról administratorów lub poprzez niestandardowe role administratorów skonfigurowane z wymaganymi uprawnieniami.

Poniższa tabela wymienia dostępne uprawnienia dla każdej funkcji i pokazuje, które zdefiniowane role administratorów zawierają je domyślnie. Podczas tworzenia niestandardowych ról administratorów, administratorzy firmy mogą przypisać te uprawnienia, aby zapewnić dostęp do konkretnych możliwości Enterprise Guard.

Poniższa tabela wymienia szczegółowe uprawnienia i matrycę ról administratorów dla każdej funkcji.

|  |  |  |  |
| --- | --- | --- | --- |
| **Zarządzanie cyklem życia treści** | | | |
| **Uprawnienie** | **Administrator zarządzania danymi** | **Administrator treści wrażliwych** | **Administrator eDiscovery** |
| Wyświetlanie ustawień kosza | ✅ | ❌ | ❌ |
| Edycja ustawień kosza | ✅ | ❌ | ❌ |
| Dodaj zasadę retencji | ✅ | ❌ | ❌ |
| Edytuj zasadę retencji | ✅ | ❌ | ❌ |
| Usuń zasadę retencji | ✅ | ❌ | ❌ |
| Dodaj zasadę usuwania | ✅ | ❌ | ❌ |
| Edytuj zasadę usuwania | ✅ | ❌ | ❌ |
| Usuń zasadę usuwania | ✅ | ❌ | ❌ |
| **Klasyfikacja danych** | | | |
| **Uprawnienia** | **Administrator zarządzania danymi** | **Administrator treści wrażliwych** | **Administrator eDiscovery** |
| Wyświetlanie ustawień klasyfikacji danych | ❌ | ✅ | ❌ |
| Edytowanie poziomów klasyfikacji | ❌ | ✅ | ❌ |
| Edytowanie ustawień automatycznej klasyfikacji | ❌ | ✅ | ❌ |
| Edytowanie ustawień zabezpieczeń klasyfikacji | ❌ | ✅ | ❌ |
| Edytowanie domyślnego poziomu klasyfikacji | ❌ | ✅ | ❌ |
| **Odkrywanie danych** | | | |
| **Uprawnienie** | **Administrator zarządzania danymi** | **Administrator treści wrażliwych** | **Administrator e-odkrywania** |
| Wyświetlanie etykiet prywatności | ❌ | ✅ | ❌ |
| Włączanie/wyłączanie wykrywania prywatności danych | ❌ | ✅ | ❌ |
| Wyświetlanie liczby dopasowań – etykiety prywatności | ❌ | ✅ | ❌ |
| Wyświetlanie zredagowanych dopasowań – etykiety prywatności | ❌ | ✅ | ❌ |
| Wyświetlanie pełnych dopasowań – etykiety prywatności | ❌ | ✅ | ❌ |
| **eDiscovery** | | | |
| **Uprawnienia** | **Administrator ds. Zarządzania Danymi** | **Administrator Treści Wrażliwych** | **Administrator eDiscovery** |
| Zarządzanie ustawieniami prawnych blokad danych | ❌ | ❌ | ✅ |
| Wyświetlanie ustawień prawnych blokad danych | ❌ | ❌ | ✅ |

*Szczegółowa macierz uprawnień i predefiniowanych ról administratora dla każdej funkcji*

> **UWAGA:** Możliwości Enterprise Guard można przydzielić za pośrednictwem predefiniowanych ról administratora lub poprzez niestandardowe role administratora skonfigurowane z wymaganymi uprawnieniami.

## Przypisywanie roli administratora Enterprise Guard

:::note
Aby przypisać użytkownikowi rolę administratora Enterprise Guard, musisz być **administratorem firmy**.
:::

1. Przejdź do **ustawień profilu**:

   - Z tablicy: **Menu główne > Preferencje > Ustawienia profilu**.
   - Z pulpitu: Kliknij swoją **awatar** w prawym górnym rogu i kliknij **Ustawienia**.
   - Z adresu URL: Przejdź do `https://miro.com/app/settings`, a następnie wybierz swoją **firmę** z listy w lewym górnym rogu.
2. W sekcji **Zarządzanie użytkownikami** kliknij **Role administratorów**.
3. W prawym panelu znajdź rolę administratora, którą chcesz przypisać (na przykład **administrator zarządzania danymi**, **administrator treści wrażliwych** lub **administrator eDiscovery**).
4. Kliknij **wielokropek (…)** obok roli i wybierz **Przypisz rolę**.
5. Wybierz użytkownika, któremu chcesz przypisać rolę.
6. Przewiń na dół okna i kliknij **Przypisz**.

## Niestandardowe role administratorów dla Enterprise Guard

Niestandardowe role administratorów pozwalają administratorom firmy na przyznawanie dostępu do poszczególnych funkcji Enterprise Guard bez konieczności przypisywania szerszych ról administracyjnych. Dzięki temu organizacje mogą dostosować dostęp na podstawie wewnętrznych wymagań dotyczących zarządzania, bezpieczeństwa lub zgodności.

Podczas tworzenia lub edytowania niestandardowej roli administratora, administratorzy firmy mogą wybrać uprawnienia, które określają, do jakich funkcji Enterprise Guard dana rola ma dostęp i którymi może zarządzać. Te uprawnienia obejmują wiele domen Enterprise Guard, takich jak: klasyfikacja danych, wykrywanie danych, zarządzanie cyklem życia treści, eDiscovery.

Przyznając tylko niezbędne uprawnienia, organizacje mogą delegować zadania administracyjne, takie jak przeglądanie wyników dotyczących wrażliwych treści, zarządzanie ustawieniami klasyfikacji, konfigurowanie polityk zarządzania cyklem życia oraz dostęp do narzędzi eDiscovery do odpowiednich zespołów. Poniższa tabela wymienia uprawnienia, które można przydzielić przy konfigurowaniu niestandardowych ról administratora.

|  |  |  |
| --- | --- | --- |
| **Możliwość** | **Uprawnienie** | **Opis** |
| **Klasyfikacja danych** | Wyświetlanie ustawień klasyfikacji danych | Administrator może wyświetlać ustawienia klasyfikacji w organizacji. |
| Edycja ustawień automatycznej klasyfikacji | Administrator może edytować ustawienia automatycznej klasyfikacji w organizacji. |
| **Wykrywanie danych** | Wyświetlanie ustawień wykrywania danych | Administrator może wyświetlać ustawienia wykrywania danych w organizacji. |
| Zarządzanie ustawieniami wykrywania danych | Administrator może zarządzać ustawieniami wykrywania danych w organizacji. |
| Wyświetlanie wyników wykrywania danych | Administrator może wyświetlać wyniki wykrywania danych. |
| Zarządzanie wynikami wykrywania danych | Administrator może zarządzać wynikami wykrywania danych. |
| **eDiscovery** | Wyświetlanie ustawień prawnych blokad danych | Administrator może wyświetlać blokady danych ze względów prawnych na stronie z ustawieniami spraw eDiscovery. |
| Zarządzanie ustawieniami prawnych blokad danych | Administrator może zarządzać prawnymi blokadami danych na stronie z ustawieniami spraw eDiscovery. |
| Wyświetlanie eksportów tablic | Administrator może wyświetlać eksporty tablic w ramach eDiscovery. |
| Zarządzanie eksportami tablic | Administrator może zarządzać eksportami tablic w ramach eDiscovery. |
| **Zarządzanie cyklem życia treści** | Wyświetlanie ustawień kosza | Administrator może wyświetlać ustawienia kosza tablic organizacji. |
| Zarządzanie ustawieniami kosza | Administrator może zarządzać uprawnieniami i czasem przechowywania tablic organizacji w koszu. |
| Wyświetlanie ustawień retencji cyklu życia treści | Administrator może wyświetlać stronę ustawień retencji w ramach cyklu życia treści. |
| Zarządzanie ustawieniami retencji cyklu życia treści | Administrator może zarządzać stroną ustawień retencji w ramach cyklu życia treści. |
| Wyświetlanie ustawień usuwania cyklu życia treści | Administrator może wyświetlać stronę ustawień usuwania w ramach cyklu życia treści. |
| Zarządzanie ustawieniami usuwania cyklu życia treści | Administrator może zarządzać stroną ustawień usuwania w ramach cyklu życia treści. |
| Wyświetlanie treści podlegających retencji lub usuwaniu | Umożliwia użytkownikowi wyświetlanie treści podlegających zasadom retencji lub usuwania. |
