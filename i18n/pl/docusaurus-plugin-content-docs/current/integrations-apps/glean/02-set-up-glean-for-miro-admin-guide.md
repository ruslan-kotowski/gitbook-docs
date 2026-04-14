---
title: "Skonfiguruj Glean dla Miro (przewodnik dla administrator\xF3w)"
article_id: 27581463837330
translation_id: 27581463837330
locale: pl-pl
sidebar_position: 2
created_at: '2025-06-23T10:52:57Z'
updated_at: '2026-01-02T09:57:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Wymagania wstępne

1. Jesteś **administratorem organizacji Miro** oraz **administratorem Glean**.
2. W Glean **zarejestruj OAuth Client ID.** Przeczytaj [dokumentację Glean](https://developers.glean.com/api-info/client/authentication/oauth) po więcej szczegółów.
3. Włącz ustawienie prywatności na poziomie użytkownika **Zezwól na zapisanie historii czatu do 30 dni**.

## Zainstaluj aplikację Glean

Aby rozpocząć, zainstaluj aplikację Glean z Miro Marketplace do odpowiednich zespołów w swojej organizacji.

1. Przejdź do swoich ustawień **Firmy** i kliknij **Aplikacje i integracje**.
2. W karcie **Aplikacje** kliknij **Dodaj aplikacje**, aby otworzyć Marketplace.
3. Wyszukaj "Glean". Możesz również znaleźć ją, wklejając jej identyfikator klienta w pasku wyszukiwania: `1202342442818548396`.
4. Z profilu aplikacji wybierz, gdzie dodać aplikację: dla **Wszystkich zespołów** lub wybierz **Określone zespoły...**.
5. Przejrzyj stronę uprawnień. Aplikacja Glean jest rozwijana i utrzymywana przez Miro i nie wymaga specyficznych uprawnień.
6. Wybierz **Dodaj**, aby zakończyć instalację.

## Konfiguracja pojedynczego logowania (Okta)

Jeśli Twoja organizacja używa Okta jako swojego dostawcy usługi pojedynczego logowania (SSO), musisz utworzyć aplikację webową Okta OpenID Connect (OIDC) przed przejściem do kolejnych sekcji.

1. Utwórz nową aplikację Okta, korzystając z kroków opisanych w dokumentacji [tutaj](https://help.okta.com/en-us/content/topics/apps/apps_app_integration_wizard_oidc.htm).
   1. Wybierz **OIDC - OpenID Connect** jako metodę logowania.
   2. Wybierz **aplikację webową** jako typ aplikacji.
   3. Upewnij się, że **Token odświeżania** jest włączony w ustawieniach **Typu udzielenia dostępu** > **Podstawowe zezwolenia**.
   4. Dodaj `https://integrations.miro.com/api/external-auth/oauth2/callback` jako **URI do przekierowania logowania**.
   5. Wybierz **Zapisz**.
2. Skopiuj **ClientId** i **Client Secret** z sekcji danych dostępowych. Będą one potrzebne w kolejnych sekcjach, aby zakończyć konfigurację integracji.

## Konfiguracja pojedynczego logowania (SSO)

Postępuj zgodnie z tymi krokami, aby skonfigurować aplikację:

1. Na stronie **Aplikacje i integracje** przejdź do **Zarządzaj aplikacjami**.
2. Znajdź "Glean" na liście zainstalowanych aplikacji i kliknij jego **Ustawienia**. Jeśli nie widzisz aplikacji, wyszukaj ją za pomocą identyfikatora klienta (`1202342442818548396`) i najpierw zatwierdź.
Azure3. Kliknij **Zapisz**, aby zastosować konfigurację.

:::note
Jeśli używasz Azure, upewnij się, że administrator Microsoft Entra wybrał "Zgódź się w imieniu Twojej organizacji" dla aplikacji Glean w centrum administracyjnym Microsoft Entra, aby umożliwić użytkownikom poprawne uwierzytelnianie.
:::

## Konfiguracja konsoli administracyjnej Glean

Przed użyciem Glean w Miro musisz skonfigurować dostęp do tokena OAuth w swojej konsoli administracyjnej Glean.

1. Otwórz swoją **konsolę administracyjną Glean** i przejdź do **Ustawienia** > **Dostęp zewnętrzny (OAuth)**.
2. W sekcji **OAuth skonfigurowany przez IDP** włącz **Włącz IdP OAuth dla dostępu API**.
3. Kliknij **Zarządzaj ustawieniami**, wybierz swojego **dostawcę SSO**.
4. Wypełnij dane dostawcy na podstawie swojego dostawcy SSO.
   - **Okta**
     - URL serwera autoryzacji: `https://<subdomain>.okta.com`
     - Dopuszczalne ID klienta: ID klienta aplikacji Okta utworzonej w poprzedniej sekcji.
     - Pozostałe pola formularza można zostawić puste.
   - **Azure**
     - Subdomena wydawcy: `https://login.microsoftonline.com/<tenant-id>/v2.0`
     - Dozwolone ID klienta(-ów): `a49fdb25-3b5f-4d3b-bedf-6da7be2b4bf4`
   - **GSuite**
     - Dozwolone ID klienta(-ów): `1062019541050-pf2ndc9f3o4lrmkupj3cj0fep5hkecns.apps.googleusercontent.com`
5. Wybierz **Zapisz**, aby zastosować ustawienia.

> ⏰ **Uwaga:** Może minąć do 30 minut, zanim zmiany zaczną obowiązywać w konsoli administracyjnej Glean.

## Używanie aplikacji Glean

Po zainstalowaniu i skonfigurowaniu aplikacji użytkownicy w wyznaczonych zespołach mogą zacząć jej używać. Za pierwszym razem, gdy użytkownik otworzy aplikację Glean w Miro, pojawi się prośba o uwierzytelnienie.

1. Otwórz tablicę Miro i kliknij ikonę Glean na pasku narzędzi, aby otworzyć panel boczny.
2. Kliknij **Połącz Glean**, aby rozpocząć autoryzację.
3. Pojawi się okno dialogowe autoryzacji SSO.
4. Po pomyślnym uwierzytelnieniu pojawi się interfejs użytkownika Glean, gotowy do użycia.

## Bezpieczeństwo

Więcej informacji o danych i bezpieczeństwie znajdziesz w [tym dokumencie o bezpieczeństwie](https://docs.google.com/document/d/1lGLF7eASQb2uMRmMEAaH-GzFhyz4UKfwMeqSQOSYPdM/edit?tab=t.0#heading=h.gu9ng058yy7y).
