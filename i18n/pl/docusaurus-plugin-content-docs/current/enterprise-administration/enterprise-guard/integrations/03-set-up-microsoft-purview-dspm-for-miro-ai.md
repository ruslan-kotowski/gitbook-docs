---
title: Konfiguracja Microsoft Purview DSPM dla Miro AI (wersja beta)
article_id: 28698434922386
translation_id: 28698434922386
locale: pl-pl
sidebar_position: 8
created_at: '2025-08-11T19:20:50Z'
updated_at: '2026-01-12T11:28:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Skorzystaj z tej procedury, aby skonfigurować Microsoft Purview Data Security Posture Management (DSPM) dla Miro AI, aby prompty AI i odpowiedzi z Miro pojawiały się w DSPM dla AI w Microsoft Purview. Po konfiguracji zweryfikujesz zdarzenia i nauczysz się, jak zarządzać integracją.

## **Wymagania wstępne**

### **Miro**

- Wersja Enterprise z włączoną funkcją **Enterprise Guard**.
- Jesteś **administratorem firmy**.
- **Microsoft Entra ID** jest skonfigurowany jako **dostawca SSO** w Miro.
- Aby włączyć tę funkcję w wersji beta, skontaktuj się ze swoim managerem ds. sukcesu klienta.

### **Microsoft**

- Aktywna licencja Microsoft Purview z obsługą DSPM dla AI.
- Identyfikator dzierżawy Microsoft Entra ID używany do SSO w Miro (GUID identyfikujący Twoją organizację/tenant Microsoft).
- Rola w Entra, która umożliwia nadanie zgody na poziomie dzierżawy dla aplikacji.

## **Konfiguracja integracji w Miro**

1. W Miro otwórz **Ustawienia Enterprise → Integracje Enterprise**.
2. Przewiń w dół, a następnie kliknij, aby przełączyć **Microsoft Purview DSPM dla AI.**
3. W polu Identyfikator Tenanta wprowadź swój **identyfikator tenanta Microsoft Entra**.
4. Kliknij **Połącz**.
5. Gdy zostaniesz poproszony, zaloguj się do Microsoft Entra przy użyciu konta, które może udzielić **zgody administratora dla całego tenanta**.
6. Przejrzyj zgodę dla aplikacji **Zarządzanie Miro AI** i kliknij **Akceptuj**.
7. Wróć do Miro i potwierdź, że integracja pokazuje **Połączono.**

## **Sprawdzanie aktywności w Microsoft Purview**

1. W Miro wykonaj proste działanie AI (na przykład **podsumuj** karteczki na tablicy).
2. Poczekaj **do 10–30 minut** na zaimportowanie danych.
3. W Microsoft Purview przejdź do **Microsoft Purview → DSPM for AI → Eksplorator działania** (widok Purview, który wyświetla działania AI). Możesz także sprawdzić informacje w dziennikach audytu.
   Uwaga: Wszystkie polecenia tekstowe i odpowiedzi we wszystkich funkcjach Miro AI są przesyłane do Purview. Obecnie zawartość obrazów nie jest przesyłana do Microsoft Purview.
4. Filtruj **najnowsze** zdarzenia i zlokalizuj działania z Miro (na przykład polecenie i odpowiedź).

## **Zarządzanie integracją**

- **Rozłączenie**: W Miro przejdź do **Integracje dla przedsiębiorstw → Microsoft Purview dla AI → Rozłącz**.
- **Zmień tenant**: Najpierw **rozłącz**, a następnie **połącz** ponownie, używając innego **identyfikatora tenant**.

## **Rozwiązywanie problemów**

- **Brak opcji integracji**: Upewnij się, że Twoja organizacja ma **Enterprise Guard**, a Twoje konto ma dostęp do **integacji dla przedsiębiorstw**. Poproś **administratora firmowego** o przyznanie dostępu.
- **Niezgodność identyfikatora tenant lub błąd połączenia**: Identyfikator tenant musi **dokładnie odpowiadać** tenantowi Microsoft Entra używanemu do Miro **SSO**.
- **Błąd zgody lub pętla logowania**: Zaloguj się na konto, które może udzielać **zgody administracyjnej dla całego tenantu** (skontaktuj się z Twoim administratorem Microsoft).
- **Brak widocznej aktywności**: Upewnij się, że użytkownik wykonał testową akcję AI, logując się do Miro przez **skonfigurowany tenant**; poczekaj **10–30 minut**; zweryfikuj swoją **licencję Purview**; i sprawdź **DSPM for AI → Activity explorer**.
- **Wiele tenantów/dostawców tożsamości**: Tylko **jeden tenant** może być skonfigurowany w Miro. Aktywność użytkowników logujących się przez SSO z innymi tenantami/dostawcami tożsamości **nie** jest przesyłana.

## **Znane ograniczenia**

Aby uzyskać więcej informacji, zobacz [sekcję znanych ograniczeń w dokumentacji przeglądowej](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).
