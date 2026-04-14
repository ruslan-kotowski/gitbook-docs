---
title: "Przegl\u0105d eksportu tablic z konsoli administracyjnej"
article_id: 26259747401362
translation_id: 26259747401362
locale: pl-pl
sidebar_position: 0
created_at: '2025-04-24T14:18:00Z'
updated_at: '2025-11-25T15:50:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: discovery-board-export
---

Administratorzy eDiscovery mogą teraz bezpośrednio eksportować tablice objęte prawną blokadą danych z konsoli administracyjnej.
Ta funkcja umożliwia administratorom eDiscovery:

- Rozpocznij eksportowanie tablic z konsoli administracyjnej.
- Monitoruj postęp zadania eksportu w czasie rzeczywistym za pośrednictwem karty **Eksporty** w każdej sprawie.
- Filtruj zadania eksportu według statusu i twórcy oraz sprawdź, które tablice są uwzględnione.
- Uzyskaj pełny dziennik zawartości dla każdej wyeksportowanej tablicy.
- Wyświetl listę wyeksportowanych tablic i ich metadane (klasyfikacja, właściciel, stan eksportu).
- Pobierz wyeksportowane tablice indywidualnie, bezpośrednio z konsoli administracyjnej.
- Zakończ przepływ pracy eksportu bez korzystania z API lub integracji.
- Anuluj zadania eksportu w kolejce lub w toku.

:::note
Aby eksportować tablice i zarządzać operacjami związanymi z eksportem, musisz mieć [rolę administratora eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby poprosić o rolę administratora treści wrażliwych, skontaktuj się z administratorem firmy.
:::

## **Możliwości eksportu tablic**

- Każde **zadanie eksportu** może zawierać do **1000 tablic**.
- **Limity eksportu** dla wersji:

  - **Enterprise Guard:** Do **100** aktywnych zadań eksportu.
  - **Enterprise:** Do **10** aktywnych zadań eksportu.
- **Limity przetwarzania równoległego**:

  - **Enterprise Guard**: Do **5** zadań eksportu przetwarzanych równolegle.
  - **Enterprise**: **1** zadanie eksportu przetwarzane na raz.
- **Dzienniki treści z zadaniami eksportu:** Eksporty mogą opcjonalnie zawierać pełny dziennik treści dla każdej wyeksportowanej tablicy.
- **Filtry dla zadań eksportu**: Filtruj zadania eksportu i sprawdź, które tablice są uwzględnione.
- **Anuluj trwające i oczekujące zadania eksportu**: Efektywne zarządzanie przepustowością eksportu.
  > ✏️ Jeśli anulujesz eksport, wszystkie tablice w toku zostaną ukończone i będą dostępne do pobrania. Tablice, które nie zostały rozpoczęte, nie zostaną wyeksportowane.

- **Dostęp do pobrania**: Wyniki można pobrać przez **14 dni.**
- **Zakres konsoli administracyjnej**: Tylko eksporty zainicjowane poprzez konsolę administracyjną pojawiają się w karcie **Eksporty**. Prace eksportowe oparte na API nie są uwzględniane na liście w konsoli administracyjnej.
