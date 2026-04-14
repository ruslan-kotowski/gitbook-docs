---
title: "Enterprise Guard i Microsoft Purview DSPM dla AI \u2013 przegl\u0105d integracji\
  \ (wersja beta)"
article_id: 28617278171154
translation_id: 28617278171154
locale: pl-pl
sidebar_position: 0
created_at: '2025-08-07T15:17:38Z'
updated_at: '2026-01-12T11:27:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Dla organizacji korzystających z Microsoft Entra ID (dawniej Azure AD) jako dostawcy tożsamości, Enterprise Guard bezpiecznie przesyła prompty i odpowiedzi AI do Microsoft Purview Data Security Posture Management (DSPM) dla AI. Zespoły ds. bezpieczeństwa i zgodności mogą wówczas monitorować, audytować i kontrolować użycie generatywnej AI z jednego, zaufanego miejsca, zmniejszając obciążenie operacyjne, minimalizując ryzyka takie jak wyciek i nadużycie danych oraz wzmacniając nadzór AI o jakości korporacyjnej Miro.

:::note
Wersja beta obsługuje formaty Miro AI, w tym diagramy, mapy myśli, dokumenty, prototypy, karteczki i tabele, ale nie obrazy. Pracujemy nad dodaniem obsługi obrazów i większej liczby funkcji AI w nadchodzących wydaniach.
:::

## **Dla kogo jest to przeznaczone**

Ta funkcja jest dostępna w wersji beta dla klientów Enterprise Guard, którzy zarządzają Miro i Microsoft Entra ID (dawniej Azure AD)/Microsoft Purview.

## **Co zyskujesz**

- **Scentralizowana widoczność:** Przeglądaj korzystanie z Miro AI w centrum AI Microsoft Purview.
- **Audytowalność:** Prompty (dane wejściowe użytkownika) i odpowiedzi (wyniki AI) są rejestrowane do przeglądu.
- **Wyrównanie zasad zarządzania:** Używaj istniejących przepływów pracy Purview do monitorowania, alarmowania i retencji.

## **Wymagania**

### **Miro**

- Wersja Enterprise z włączonym **Enterprise Guard**.
- Jesteś **administratorem firmy**.
- Microsoft **Entra ID** skonfigurowany jako dostawca SSO w Miro.
- Dostęp do strony **Integracje Enterprise** (jeśli jej nie widzisz, poproś **administratora firmy** o przyznanie dostępu).
- Aby włączyć tę funkcję w wersji beta, skontaktuj się z Twoim managerem ds. sukcesu klienta.

### **Microsoft**

- Aktywna licencja **Microsoft Purview**.
- Twój **Microsoft Entra ID tenant ID** (ten sam tenant używany dla SSO Miro; GUID, który identyfikuje Twoją organizację/tenant Microsoft).
- Rola Entra, która może **udzielać zgody administracyjnej na poziomie tenantu** aplikacji.

## **Jak to działa**

1. Administrator Miro łączy tenanta Microsoft Entra ze strony **Integracje Enterprise** w Miro.
2. To instalacja aplikacji **Miro AI governance** w Twoim tenantcie Microsoft (za zgodą administracyjną na poziomie tenantu).
3. Gdy użytkownicy logują się do Miro za pośrednictwem tego tenantu i korzystają z Miro AI, Miro przesyła prompt/odpowiedź do Microsoft Purview.
4. Działania pojawiają się w **DSPM dla AI → Eksploratorze działań** (widok Purview, który listuje działania AI) w Microsoft Purview (należy uwzględnić czas przetwarzania).

## **Widoczność danych i opóźnienia**

- Zalogowane dane: **Prompty i odpowiedzi AI** generowane w Miro przez użytkowników logujących się za pomocą pojedynczego logowania (SSO) dla skonfigurowanego dzierżawcy.
- Gdzie to zobaczyć: **Microsoft Purview → DSPM dla AI → Eksplorator aktywności** (widok Purview, który wyświetla działania AI). Możesz również wyświetlić informacje w dziennikach audytu.
  **Uwaga:** Wszystkie tekstowe prompty i odpowiedzi w funkcjach Miro AI są przesyłane do Purview. Obecnie zawartość obrazów nie jest przesyłana do Microsoft Purview.
- Opóźnienie: Rekordy zazwyczaj pojawiają się **w ciągu 10–30 minut** po akcji AI w Miro.

## **Znane ograniczenia**

- Wersja beta obsługuje formaty Miro AI, w tym diagramy, mapy myśli, dokumenty, prototypy, karteczki i tabele, ale nie obrazy. Pracujemy nad dodaniem obsługi obrazów i większej liczby funkcji AI w nadchodzących wersjach.
- Możesz skonfigurować **jeden identyfikator dzierżawcy Microsoft Entra** w Miro naraz.
- W środowiskach multi-IdP lub multi-tenant **tylko** aktywność użytkowników logujących się do Miro przez **skonfigurowanego dzierżawcę** jest rejestrowana w Microsoft Purview.

## **Bezpieczeństwo i prywatność**

Miro przekazuje prompty i odpowiedzi AI do **Twojego dzierżawcy Microsoft**, aby mogły być monitorowane w Purview. **Zarządzanie, retencja i kontrola dostępu** są zarządzane w Twoim środowisku Microsoft.

##

## **FAQ**

- **P: Które funkcje Miro AI są rejestrowane?**
  **O:** Wszystkie prompty i odpowiedzi tekstowe w funkcjach Miro AI są przekazywane do Purview. Obecnie zawartość obrazów nie jest przekazywana do Microsoft Purview.
- **P: Czy dotyczy to wszystkich użytkowników?**
  **O:** Tylko użytkownicy, którzy uwierzytelniają się w Miro przy użyciu skonfigurowanego dzierżawcy Microsoft Entra, są objęci.
- **P: Czy mogę eksportować logi z Miro?**
  **Odpowiedź:** Użyj Microsoft Purview do eksportu i retencji. Miro przekazuje aktywność do Twojego dzierżawcy Microsoft, gdzie podlega ona Twoim zasadom.
- **Pytanie: Co z bezpieczeństwem i prywatnością?**
  **Odpowiedź:** Miro przekazuje zapytania i odpowiedzi AI do **Twojego dzierżawcy Microsoft**, aby mogły być monitorowane w Purview. **Zarządzanie, retencja i kontrola dostępu** są zarządzane w Twoim środowisku Microsoft.

## **Pomoc i zasoby**

- Aby uzyskać informacje o wymaganiach wstępnych dotyczących zgody Entra, zapoznaj się z dokumentacją Microsoft dotyczącą **udzielania zgody administratora dzierżawy** dla aplikacji.
- Aby uzyskać instrukcje dotyczące konfiguracji Enterprise Guard, zobacz [tę dokumentację](../../enterprise-subscription-management/integrations/03-set-up-microsoft-purview-dspm-for-miro-ai.md).
