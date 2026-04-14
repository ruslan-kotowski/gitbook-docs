---
title: Dodawanie wielu dostawców tożsamości
article_id: 16287287497234
translation_id: 16287287497234
locale: pl-pl
sidebar_position: 1
created_at: '2024-01-10T10:51:24Z'
updated_at: '2026-02-18T08:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Dostępne dla: Enterprise Konfiguracja przez: administratorów firmy'
---

:::note
Dodanie wielu dostawców tożsamości jest funkcją dostępną wyłącznie dla klientów Enterprise. Aby uzyskać dostęp do tej funkcji i ją włączyć, skontaktuj się z swoim Miro Account Team Managerem lub managerem ds. sukcesu klienta. Pomoc Miro nie może włączyć tej funkcji.
:::

Użyj kilku dostawców tożsamości (IdP) do pojedynczego logowania (SSO). Jest to szczególnie użyteczne dla dużych organizacji posiadających różne oddziały lub filie, z których każdy ma swojego IdP, ale potrzebuje dostępu do tej samej subskrypcji Miro.

## Przygotowanie do dodania wielu dostawców tożsamości

Aby mieć pewność, że [SSO](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) nadal działa po dodaniu kilku aplikacji dostawcy tożsamości, musisz zaktualizować konfigurację istniejącej aplikacji IdP.

Entra ID i niektórzy inni dostawcy tożsamości nie będą wspierać nowego formatu konfiguracji, dopóki Twoja organizacja nie włączy funkcji prywatnej dla wielu dostawców tożsamości (multi-IdP). Aby uniknąć zakłóceń w logowaniu, zalecamy umówienie rozmowy z Twoim managerem ds. sukcesu klienta, który krok po kroku poprowadzi Cię po procesie włączenia funkcji prywatnej multi-IdP jednocześnie z aktualizacją konfiguracji.

### Jak skonfigurować ustawienia Enterprise

1. Wyłącz SCIM.
2. Zaktualizuj konfigurację SSO.
3. Zweryfikuj funkcjonowanie SSO.

#### Wyłącz obsługę SCIM

Obecnie nie obsługujemy [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) z wieloma dostawcami tożsamości. Aby wyłączyć obsługę SCIM w swoim Planie Enterprise, przejdź do ustawień **Firmy** > **Konta** > **Integracje Enterprise** i przełącz **Obsługę administracyjną SCIM** na "wyłączone".

#### Zaktualizuj konfigurację SSO

**Stara konfiguracja**

Podczas początkowej konfiguracji pojedynczego logowania (SSO) Miro w Twoim dostawcy tożsamości najprawdopodobniej użyto następujących wartości konfiguracyjnych:

- **Callback URL/ACS:** https://miro.com/sso/saml
- **ID jednostki:** https://miro.com

**Nowa konfiguracja**

Aby upewnić się, że dostawca tożsamości wie, do której konfiguracji w Miro się odnosi, poniższe wartości muszą zostać zaktualizowane. Przejdź do **Ustawienia** > **Bezpieczeństwo** > **Uwierzytelnianie**.

Te wartości są dostępne w ustawieniach SSO, gdy Twoja organizacja włączy funkcję prywatną multi-IdP i będą miały następujący format:

- **Callback URL/ACS:** https://miro.com/sso/saml/&lt;org_id&gt;/&lt;saml_settings_id&gt;
- **Entity ID:** "https://miro.com/&lt;org_id&gt;/&lt;saml_settings_id&gt;

![Callback URL and Entity ID in the Enterprise admin console](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/23763575205778_image.png)

*Callback URL i Entity ID w konsoli administracyjnej Enterprise*

#### Zweryfikuj działanie SSO

Po zakończeniu aktualizacji konfiguracji dostawcy tożsamości, przetestuj poprawność działania SSO poprzez wylogowanie się i ponowne zalogowanie.

## Dodawanie nowego dostawcy tożsamości (IdP)

Proces dodawania nowych dostawców tożsamości (IdP) jest podobny do istniejącej [konfiguracji SSO](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), ale uwzględnia kilka kluczowych zmian:

- **Nowe pola:** 'Nazwa dostawcy tożsamości' i 'Opis dostawcy tożsamości' (opcjonalne). Te pola pomagają użytkownikom i administratorom w identyfikacji odpowiedniego dostawcy tożsamości podczas logowania, zwłaszcza jeśli używane są różne dostawcy tożsamości.

  Ze względu na to, że te pola są wyświetlane w ustawieniach administratora i mogą być pokazywane użytkownikom podczas logowania przez SSO, zdecydowanie zalecamy celowe ustawienie tych nazw (na przykład jednostka biznesowa lub nazwa dostawcy tożsamości).

  ![idP-name-and-IdP description.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016020733970_idP-name-and-IdP%20description.png)
*Opcja dodania nazwy i opisu dostawcy tożsamości*
- **Pola tylko do odczytu:** 'Callback URL' (Dozwolony Callback URL, niestandardowy Assertion Consumer Service URL, Reply URL) i 'Entity ID' (Identyfikator, Relying Party Trust Identifier) są teraz automatycznie generowane w Twoich ustawieniach IdP w Miro, gdy Twoja organizacja włączyła prywatną funkcję multi-IdP.

  Wcześniej te wartości były statyczne, ponieważ były takie same dla wszystkich konfiguracji IdP. Po wygenerowaniu, będziesz musiał również skopiować i wkleić te wartości do odpowiednich pól w ustawieniach swojego dostawcy tożsamości IdP.

  ![Callback-ID-and-Entity-ID-fields.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034166290_Callback-ID-and-Entity-ID-fields.png)
*Pola Callback URL i Entity ID*

## Zarządzanie wieloma dostawcami tożsamości (IdP)

> **💡** Możesz dodać i włączyć do 20 dostawców tożsamości jednocześnie.

Po dodaniu dostawców każdą konfigurację można włączać lub wyłączać według potrzeb. Aby wyłączyć dostawcę tożsamości, przejdź do **Ustawienia** firmy > **Konto** > **Uwierzytelnianie** i wyłącz dostawcę tożsamości.

![Toggle-on-or-off-IdPs.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034165010_Toggle-on-or-off-IdPs.png)
*Opcja włączania lub wyłączania dostawców tożsamości*

## Widok logowania dla domen e-mail z wieloma dostawcami tożsamości

Jeśli domena e-mail użytkownika jest powiązana z kilkoma konfiguracjami dostawców tożsamości, użytkownik może wybrać jedną z nich podczas logowania. Jeśli te konfiguracje mają różne domeny, użytkownik jest automatycznie przekierowywany do odpowiedniego dostawcy tożsamości.

![sso-screenshot.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/22437449166610_sso-screenshot.png)
*Widok wielu dostawców tożsamości podczas logowania*
