---
title: "Przegl\u0105d dziennik\xF3w audytu Enterprise Guard"
article_id: 17331872857746
translation_id: 17331872857746
locale: pl-pl
sidebar_position: 0
created_at: '2024-02-27T21:08:55Z'
updated_at: '2025-11-25T15:41:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Dzienniki audytu zapewniają administratorom kompleksowy zapis wszystkich zdarzeń związanych z Enterprise Guard. Te dzienniki są cennym źródłem do efektywnego rozwiązywania problemów i oferują szczegółowe wglądy w istotne zdarzenia, takie jak aktualizacje zasad czasu przechowywania w koszu i uprawnienia do tablic umieszczonych w koszu, tworzenie, aktualizację lub usunięcie zasad retencji dla organizacji, czy trwałe usunięcie tablicy z kosza. Systematyczne śledzenie tych działań wzmacnia monitorowanie, analizę i konserwację, zapewniając bezpieczny i dobrze zarządzany system.

## Zdarzenia Enterprise Guard w dziennikach audytu

Oprócz [istniejących rejestrowanych zdarzeń](../../security-integrations/security-management/01-audit-logs.md), dzienniki audytu zawierają wpisy dotyczące następujących kategorii zdarzeń i zdarzeń związanych z Enterprise Guard.

### Zasada dotycząca kosza

Poniższa tabela zawiera kategorię zdarzeń i działania zdarzeń rejestrowane dla komponentu zasady Kosza Organizacji.

|  |  |
| --- | --- |
| **Kategoria zdarzenia** | **Działanie zdarzenia** |
| Administracja | Zmieniono zasady dotyczące czasu przechowywania kosza dla organizacji |
| Administracja | Zmieniono zasady uprawnień do tablic umieszczonych w koszu dla organizacji. |

*Tabela 1: Kategorie zdarzeń i działania zdarzeń rejestrowane dla komponentu zasady Kosza organizacji*Więcej informacji na temat zasad kosza znajdziesz w [naszej dokumentacji](https://help.miro.com/hc/articles/13860817985426-Trash-Policy).

### Zasada retencji

Poniższa tabela przedstawia kategorie zdarzeń i działania zdarzeń rejestrowane dla komponentu Zasady Retencji Treści.

|  |  |
| --- | --- |
| **Kategoria zdarzenia** | **Działanie zdarzenia** |
| Administracja | Zasada retencji utworzona dla organizacji |
| Administracja | Zaktualizowano zasadę retencji dla organizacji |
| Administracja | Zasada retencji usunięta dla organizacji |

*Tabela 2: Kategorie zdarzeń i działania zdarzeń rejestrowane dla komponentu Zasady Retencji Treści*Więcej informacji na temat zasad retencji znajdziesz w [naszej dokumentacji](https://help.miro.com/hc/articles/16855776325778-Retention-Beta).

### Wykrywanie danych

Poniższa tabela zawiera kategorie zdarzeń i działania zdarzeń rejestrowane dla komponentu Content Discovery.

|  |  |
| --- | --- |
| **Kategoria zdarzenia** | **Akcja zdarzenia** |
| Administracja | Zmieniono wykrywanie informacji prywatnych dla organizacji  (włączone/wyłączone) |
| Administracja | Wykluczono dopasowanie wykrywania danych w organizacji |

*Tabela 3: Kategorie zdarzeń i akcje zdarzeń rejestrowane dla komponentu Content Discovery*

Więcej informacji o wykrywaniu danych można znaleźć w [naszej dokumentacji](../../canvas-25-admin-features/data-discovery/01-data-discovery-overview.md).

### Inteligentne zabezpieczenia

Poniższa tabela zawiera kategorie zdarzeń i działania związane ze zdarzeniami zarejestrowane dla komponentu Inteligentne zabezpieczenia.

|  |  |
| --- | --- |
| **Kategoria zdarzenia** | **Akcja zdarzenia** |
| Inteligentne zabezpieczenia | Inteligentne zabezpieczenia zmienione dla tablicy |

*Tabela 4: Kategorie zdarzeń i działania związane ze zdarzeniami zarejestrowane dla komponentu Inteligentne zabezpieczenia*

Więcej informacji o Inteligentnych zabezpieczeniach znajdziesz w [naszej dokumentacji](../../canvas-25-admin-features/data-classification/01-intelligent-guardrails-overview.md).

### eDiscovery

Poniższa tabela zawiera kategorie zdarzeń i działania związane ze zdarzeniami zarejestrowane dla komponentu eDiscovery.

|  |  |
| --- | --- |
| **Kategoria zdarzenia** | **Akcja zdarzenia** |
| Administracja | Sprawa utworzona dla organizacji |
| Administracja | Sprawa zamknięta dla organizacji |
| Administracja | Utworzono prawną blokadę danych dla organizacji |
| Administracja | Zamknięto prawną blokadę danych dla organizacji |
| Administracja | Zastosowano prawną blokadę danych na tablicę. Tablica zwolniona z prawnej blokady danych. |

*Tabela 3: Kategorie i akcje zdarzeń zarejestrowane dla komponentu eDiscovery*

Aby uzyskać więcej informacji o eDiscovery, zobacz [naszą dokumentację](https://help.miro.com/hc/sections/22049853357842-eDiscovery-Legal-Hold-Beta).
