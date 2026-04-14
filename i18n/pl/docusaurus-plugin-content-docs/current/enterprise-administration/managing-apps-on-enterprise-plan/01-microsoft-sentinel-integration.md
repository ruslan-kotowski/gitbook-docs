---
title: Integracja z Microsoft Sentinel
article_id: 31325908249362
translation_id: 31325908249362
locale: pl-pl
sidebar_position: 1
created_at: '2025-11-24T18:16:15Z'
updated_at: '2025-12-16T15:49:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: audit-logs
---

## Przegląd

Łącznik [Miro](https://miro.com/) wprowadza dzienniki audytu oraz dzienniki aktywności z [Miro REST API](https://developers.miro.com/reference/overview) do Microsoft Sentinel za pomocą Codeless Connector Framework (CCF). Konsoliduje to monitorowanie aktywności w przestrzeni roboczej Miro w Microsoft Sentinel, co umożliwia wykrywanie zagrożeń bezpieczeństwa, analizę incydentów oraz raportowanie zgodności.

## Łączniki danych

To rozwiązanie obejmuje dwa łączniki danych.

| Łącznik | Wymagania dotyczce abonamentu | Co rejestruje | Odnośniki |
| --- | --- | --- | --- |
| **Dzienniki audytu Miro (abonament Enterprise)** | Enterprise | Zdarzenia audytu na poziomie całej organizacji, w tym uwierzytelnianie użytkowników, dostęp do treści, zmiany zespołowe i działania administracyjne. | [Dokumentacja API](https://developers.miro.com/reference/enterprise-get-audit-logs) | [Przegląd dzienników audytu](https://developers.miro.com/reference/audit-logs) |
| **Rejestry Zawartości Miro (abonament Enterprise + dodatek Enterprise Guard)** | Abonament Enterprise + dodatek Enterprise Guard | Śledzenie aktywności zawartości, w tym tworzenie, aktualizacje i usuwanie elementów dla zgodności i eDiscovery. | [Dokumentacja API](https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch) | [Przegląd rejestrów zawartości](https://developers.miro.com/reference/board-content-logs) |

## Wymagania wstępne

### Ogólne wymagania

- Aktywna przestrzeń robocza Microsoft Sentinel.
- Rola administratora firmy w Twojej organizacji Miro.
- Token dostępu OAuth Miro (bezterminowy).

### Wymagania specyficzne dla łączników

#### Dla łącznika dzienników audytu

- Wersja Miro Enterprise.
- Zakres OAuth: `auditlogs:read`.
- Token dostępu.

#### Dla łącznika dzienników treści

- Abonament Miro Enterprise + dodatek Enterprise Guard.
- Zakres OAuth: `contentlogs:export`.
- Token dostępu.
- Identyfikator organizacji Miro.

## Instalacja

Istnieją dwa sposoby konfiguracji łączników Miro.

- **Opcja 1 (zalecana):** Użyj integracji przedsiębiorstwa. Najprostsza konfiguracja z automatycznym generowaniem tokenów.
- **Opcja 2 (alternatywna):** Utwórz niestandardową aplikację OAuth. Więcej kontroli nad konfiguracją aplikacji OAuth.

**Uwaga:** Korzystając z opcji 1, integracja jest automatycznie powiązana z zespołem o największej liczbie użytkowników w organizacji. Korzystając z opcji 2, możesz wybrać, do którego zespołu zainstalować aplikację. Jednak wybór zespołu nie wpływa na to, które dzienniki są gromadzone. Obie opcje zapewniają dostęp do dzienników na poziomie całej organizacji. Wszystkie wydarzenia istotne dla integracji ze wszystkich zespołów są uwzględnione w twoich dziennikach.

### Opcja 1: Użyj integracji Enterprise (zalecane)

Jest to najprostsza opcja dla większości użytkowników. Automatycznie tworzy aplikację OAuth i generuje token dostępu dla Ciebie poprzez ustawienia integracji Enterprise w Miro.

#### Dla konektora dzienników audytu

1. Otwórz [ustawienia firmowe Miro](https://miro.com/app/settings/).
2. Rozwiń sekcję **Aplikacje i integracje**.
3. Kliknij **Integracje Enterprise**.
4. Włącz przełącznik **SIEM**.
5. Skopiuj wartość **Access Token**, która się pojawi.
6. Przechowuj token w bezpiecznym miejscu.

#### Dla konektora logów dotyczących treści

1. Otwórz [ustawienia firmy Miro](https://miro.com/app/settings/).
2. Rozwiń sekcję **Aplikacje i integracje**.
3. Kliknij **Integracje Enterprise**.
4. Włącz przełącznik **eDiscovery**.
5. Skopiuj wartość **Access Token**, która się pojawi.
6. Pobierz **ID organizacji** z adresu URL przeglądarki:
   - Spójrz na adres URL przeglądarki, aby znaleźć ID organizacji.
   - Format adresu URL to: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - Skopiuj ID organizacji z adresu URL (wartość numeryczna).
7. Przechowuj bezpiecznie zarówno token, jak i ID organizacji.

### Opcja 2: Użyj niestandardowej aplikacji OAuth (alternatywa)

Ta opcja daje Ci większą kontrolę nad konfiguracją aplikacji OAuth. Wybierz ją, jeśli potrzebujesz dostosować zakresy, zarządzać wieloma integracjami lub wolisz ręczne zarządzanie aplikacją OAuth.

#### Krok 1: Utwórz aplikację OAuth w Miro

1. Zaloguj się na swoje konto w Miro.
2. Przejdź do [ustawień aplikacji Miro](https://miro.com/app/settings/user-profile/apps).
3. Kliknij **Utwórz nową aplikację**.
4. Wybierz opcję **Token dostępu bez daty wygaśnięcia** podczas tworzenia aplikacji ([dowiedz się więcej o tokenach OAuth](https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens)).
5. Włącz wymagane zakresy OAuth:
   - `dziennika audytu:read` dla łącznika dzienników audytu.
   - `contentlogs:export` dla łącznika dzienników treści (wymaga Enterprise Guard).
6. Kliknij **Zainstaluj aplikację i uzyskaj token OAuth**.
7. Kopiuj **token dostępu** i przechowuj go bezpiecznie.

Po szczegółowe instrukcje dotyczące konfiguracji OAuth zobacz [Pierwsze kroki z OAuth](https://developers.miro.com/docs/getting-started-with-oauth).

#### Krok 2: Uzyskaj ID organizacji (tylko dla dzienników treści)

1. Przejdź do [ustawień firmy Miro](https://miro.com/app/settings/).
2. Spójrz na URL przeglądarki, aby znaleźć ID organizacji:
   - Format URL wygląda następująco: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - Skopiuj ID organizacji z URL (wartość numeryczna).

### Wdróż rozwiązanie w Microsoft Sentinel

1. W Microsoft Sentinel, przejdź do **Content Hub**.
2. Wyszukaj **„Miro”** i kliknij rozwiązanie.
3. Kliknij **Zainstaluj** i postępuj zgodnie z instrukcjami kreatora wdrażania.
4. Wybierz swoją przestrzeń roboczą Log Analytics.
5. Zakończ instalację.

### Skonfiguruj łączniki danych

#### Łącznik dzienników audytu Miro

1. W Microsoft Sentinel przejdź do **Złącza danych**.
2. Znajdź **Miro Audit Logs (Plan Enterprise)** i kliknij **Otwórz stronę złącza**.
3. Kliknij **Połącz**.
4. Wprowadź swój **Token dostępu**.
5. Kliknij **Połącz**, aby aktywować złącze.

#### Złącze logów treści Miro

1. W Microsoft Sentinel przejdź do **Łączniki danych**.
2. Znajdź **Miro Content Logs (Enterprise Abonament + Enterprise Guard)** i kliknij **Otwórz stronę łącznika**.
3. Kliknij **Połącz**.
4. Wprowadź swój **ID organizacji**.
5. Wprowadź swój **Token dostępu**.
6. Kliknij **Połącz**, aby aktywować łącznik.

Przetwarzanie danych rozpocznie się w ciągu 5–10 minut od aktywacji łącznika.

## Tabele danych

### MiroAuditLogs_CL

Wydarzenia audytu na poziomie organizacji obejmujące:

- Uwierzytelnianie użytkownika i dostęp.
- Operacje na treściach.
- Zmiany w zespole i organizacji.
- Modyfikacje profilu użytkownika.
- Działania administracyjne.

**Kluczowe kolumny**

| Kolumna | Opis |
| --- | --- |
| `TimeGenerated` | Znacznik czasu zdarzenia. |
| `event` | Nazwa zdarzenia identyfikująca konkretną akcję lub aktywność. |
| `logType` | Typ wpisu do dziennika. |
| `category` | Kategoria zdarzenia grupująca powiązane zdarzenia. |
| `createdBy_email` | Użytkownik, który wywołał zdarzenie. |
| `context_ip` | Adres IP zdarzenia. |
| `details` | Dodatkowe informacje specyficzne dla zdarzenia (JSON). |

### MiroContentLogs_CL

Dzienniki aktywności na poziomie treści, obejmujące:

- Operacje na poziomie elementów z przypisaniem użytkownika i znacznikami czasu.
- Przejścia stanów i modyfikacje.
- Śledzenie aktywności dla zgodności i eDiscovery.

**Kluczowe kolumny**

| Kolumna | Opis |
| --- | --- |
| `TimeGenerated` | Znacznik czasu zdarzenia. |
| `actionType` | Typ akcji wykonanej na treści. |
| `actor_email` | Użytkownik, który wykonał akcję. |
| `itemType` | Typ elementu treści, którego dotyczy zmiana. |
| `contentId` | Unikalny identyfikator treści. |
| `state` | Informacje o stanie elementu (JSON). |

## Przykładowe zapytania

### Wyświetlanie ostatnich zdarzeń audytu

```
MiroAuditLogs_CL
| sort by TimeGenerated desc
| project TimeGenerated, event, category, createdBy_email, context_ip
| take 20
```

### Aktywność według użytkownika i typu zdarzenia

```
MiroAuditLogs_CL
| summarize EventCount = count() by createdBy_email, event, category
| order by EventCount desc
```

### Zmiany treści według użytkownika

```
MiroContentLogs_CL
| where TimeGenerated > ago(7d)
| summarize Changes = count() by actor_email, actionType
| order by Changes desc
```

### Trendy zdarzeń w czasie

```
MiroAuditLogs_CL
| summarize count() by event, bin(TimeGenerated, 1h)
| render timechart
```

### Najbardziej aktywni użytkownicy (zmiany treści)

```
MiroContentLogs_CL
| where TimeGenerated > ago(30d)
| summarize TotalActions = count() by actor_email
| top 10 by TotalActions desc
```

## Rozwiązywanie problemów

### Brak danych

- Upewnij się, że token dostępu jest ważny i ma odpowiednie zakresy uprawnień.
- Sprawdź, czy Twoja organizacja posiada dodatek Enterprise Guard dla logów zawartości.
- Upewnij się, że identyfikator organizacji jest poprawny (dla logów zawartości).
- Poczekaj 5–10 minut na początkowe załadowanie danych.
- Sprawdź status złącza na stronie **Data connectors**.

### Błędy uwierzytelniania

#### Jeśli korzystasz z opcji 1 (przełącznik integracji Enterprise)

- Przejdź do [ustawień firmy Miro](https://miro.com/app/settings/), rozwiń **aplikacje i integracje** i kliknij **Integracje Enterprise**.
- Sprawdź, czy przełącznik (SIEM dla dzienników audytu, eDiscovery dla dzienników zawartości) jest wciąż włączony.
- Jeśli inny administrator wyłączył przełącznik, token zostanie unieważniony.
- Ponownie włącz przełącznik, aby wygenerować nowy token i zaktualizować konfigurację konektora.
- Zweryfikuj posiadanie roli administratora firmy w Miro.

#### Jeśli używasz opcji 2 (własna aplikacja OAuth)

- Zweryfikuj, czy token nie został unieważniony w [ustawieniach aplikacji Miro](https://miro.com/app/settings/user-profile/apps).
- Upewnij się, że aplikacja OAuth ma włączone wymagane zakresy.
- W razie potrzeby wygeneruj ponownie token i zaktualizuj go w konfiguracji konektora.
- Zweryfikuj, czy posiadasz rolę administratora firmy w Miro.

### Dzienniki treści nie działają

- Sprawdź, czy Twój abonament Miro obejmuje dodatek **Enterprise Guard** (niedostępny w podstawowej wersji Enterprise).
- Potwierdź, czy zakres OAuth `contentlogs:export` jest włączony.
- Dokładnie sprawdź, czy ID organizacji jest prawidłowe.
- Skontaktuj się z menedżerem konta Miro, jeśli potrzebujesz zmiany na wyższą wersję Enterprise Guard.

## Zasoby

### Zasoby centrum pomocy Miro

- **Dzienniki audytu Miro:** `../security-integrations/security-management/01-audit-logs.md
- **Dzienniki treści Miro:** `../canvas-25-admin-features/ediscovery/06-content-logs-overview.md
- **Przewodnik po integracji z Miro i Sentinel:** `01-microsoft-sentinel-integration.md`.

### Dokumentacja dewelopera Miro

- **Rozpoczęcie pracy z Enterprise API:** `https://developers.miro.com/docs/getting-started-with-enterprise-api`.
- **Rozpoczęcie pracy z OAuth:** `https://developers.miro.com/docs/getting-started-with-oauth`.
- **Autoryzacja tokenu OAuth:** `https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens`.
- **API dzienników audytu:** `https://developers.miro.com/reference/enterprise-get-audit-logs`.
- **API dzienników treści:** `https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch`.
- **Referencje API:** `https://developers.miro.com/reference`.

### Microsoft Sentinel

- **Dokumentacja Microsoft Sentinel:** `https://docs.microsoft.com/azure/sentinel/`.
