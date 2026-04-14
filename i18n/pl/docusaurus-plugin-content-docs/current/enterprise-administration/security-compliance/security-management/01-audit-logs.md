---
title: Dzienniki audytu
article_id: 360017571434
translation_id: 360017571434
locale: pl-pl
sidebar_position: 1
created_at: '2019-02-11T10:09:04Z'
updated_at: '2026-03-12T09:21:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Dostępne dla: Enterprise Konfigurowane przez: administratorów firmy'
---

Dzienniki audytu umożliwiają administratorom organizacji, posiadającym odpowiednie uprawnienia, śledzenie aktywności użytkowników w organizacji Miro. Dzienniki są niezwykle przydatne podczas badania problemu lub uzyskiwania szczegółowego raportu na temat ważnych wydarzeń (na przykład zmiany ustawień globalnych zabezpieczeń, zaproszenia nowych użytkowników lub tworzenie nowych tablic).

:::note
Aktualnie wydarzenia są rejestrowane od momentu utworzenia subskrypcji Enterprise i przechowywane przez domyślnie 180 dni:
a) Jeśli dokonasz zmiany na wyższą wersję Enterprise z innego abonamentu, wydarzenia będą rejestrowane od chwili aktualizacji.
b) Jeśli przeniesiesz część zespołów do subskrypcji Enterprise, ich dane będą rejestrowane dopiero, gdy staną się częścią subskrypcji.
:::

## Dostęp do dzienników audytu

Aby uzyskać dostęp do dzienników audytu, wykonaj następujące kroki:

1. Przejdź do **Ustawień firmy**.
2. Na lewym panelu kliknij **Bezpieczeństwo** > **Dzienniki audytu**.
3. Możesz filtrować dzienniki audytu, wybierając **Zakres dat**, **Aktora**, **Kategorię zdarzeń** i określone **Zdarzenie**.

Kliknij przycisk Wyświetl zdarzenia, aby zobaczyć zdarzenia pasujące do Twoich kryteriów filtrowania. Czas jest wyświetlany w formacie **ISO 8601**, w **lokalnej** strefie czasowej. Możesz zobaczyć szczegóły określonego zdarzenia, klikając menu z 3 kropkami w kolumnie **Szczegóły**.

:::note
Tylko zdarzenia, które miały miejsce w ciągu ostatnich 90 dni, są dostępne do podglądu.
:::

## Eksportowanie dzienników audytu

Możesz eksportować dzienniki w formacie pliku **CSV**.

W pliku eksportu CSV data i godzina zdarzenia są podawane w formacie ISO 8601, w strefie czasowej UTC. Nie ma limitu liczby rekordów do wyeksportowania na raz, jednak im więcej danych eksportujesz, tym dłużej trwa przygotowanie pliku do pobrania. Pamiętaj również, że popularne aplikacje do pracy z tabelami mają swoje ograniczenia dotyczące ilości danych, które mogą otworzyć.

Aby eksportować dzienniki, kliknij przycisk **Export to CSV**.

Pasek z szczegółami pliku eksportu pojawi się poniżej. Gdy plik będzie gotowy do pobrania, możesz kliknąć przycisk Download CSV. Plik będzie dostępny do pobrania przez 24 godziny.

:::note
W danym momencie można pobrać tylko jeden plik eksportu na organizację. Kliknięcie przycisku **Eksportuj do CSV** zastąpi bieżący plik eksportu.
:::

## Dostęp do dzienników audytu przez API

Administratorzy mogą używać [Audit Log API](https://developers.miro.com/reference/audit-logs) lub obsługiwanych [integracji SIEM](https://help.miro.com/hc/sections/4404757427090-Security-information-and-event-management-SIEM), aby programowo uzyskać dostęp do danych z dzienników audytu i je gromadzić.

## Usuwanie dzienników audytu

Administratorzy mogą ustalić zasadę retencji dla dzienników audytu. Można wybrać spośród 30, 90, 180 lub 365 dni.

:::warning
Po usunięciu dzienników audytu nie można ich odzyskać.
:::

:::note
Bezterminowa retencja dla dzienników audytu została wycofana.
:::

Aby ustawić okres usuwania, wykonaj następujące kroki:

1. Przejdź do **Ustawień firmy**.
2. Na lewym panelu kliknij **Bezpieczeństwo** > **Dzienniki audytu**.
3. Pod **Dziennikami audytu** kliknij kartę **Ustawienia**.
4. Wybierz opcję z listy rozwijanej. Zostaniesz poproszony(-a) o potwierdzenie wyboru.

## Wydarzenia w dziennikach audytu

Dzienniki audytu zawierają zapisy o następujących kategoriach wydarzeń:

**Administracja**

- Zmieniono nazwę firmy
- Zmieniono, usunięto logo firmy
- Utworzono prośbę o dostęp
- Odrzucono prośbę o dostęp
- Włączono, wyłączono wskaźniki aktywności użytkowników w Analizach
- Włączono, wyłączono lub zmieniono ustawienia SSO/SAML
- Włączono, wyłączono SCIM
- Wygenerowano token dla SCIM API
- Włącz zamówienia powiadomień SCIM
- Włącz, wyłącz, zmień [listę dozwolonych](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Włącz, wyłącz udostępnianie gościom poza dozwolonymi domenami
- Włącz, wyłącz udostępnianie [przez publiczny link](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Włącz, wyłącz udostępnianie [przez publiczny link do edycji](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- Włącz, wyłącz [ochronę prywatności zespołu](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Włącz, wyłącz, zaktualizuj [ustawienia zarządzania domeną](../../canvas-25-admin-features/domain-control/01-domain-control.md)
- Włącz, wyłącz [blokowanie dezaktywowanych użytkowników](../../user-management/02-block-deactivated-users.md)
- Zmień [ustawienia zarządzania prośbami](../../user-management/09-request-management-on-enterprise-plan.md) (w tym zmianę e-maila ServiceNow lub URL usługi pomocy technicznej)
- Utwórz, usuń zespół
- Zmień nazwę zespołu
- Zmień, usuń logo zespołu
- Zmień [ustawienia zapraszania do zespołu](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Zmień [widoczność zespołu](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- Włącz, wyłącz [gości w zespole](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- Zmień [domyślne ustawienia udostępniania tablicy](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Zmień [domyślne ustawienia udostępniania projektów](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- Zainstaluj lub odinstaluj aplikację
- [Zatwierdź lub ogranicz aplikację](../../../integrations-apps/integrations-basics/04-how-to-install-apps.md)
- [Moderacja Miro AI](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md)

**Zarządzanie użytkownikami**

- Zaproś nowego członka zespołu
- Przekształć członka w gościa
- Przekształć użytkownika w uczestnika z pełnym dostępem
- Awansuj użytkownika na administratora firmy, cofnij uprawnienia administratora firmy
- Awansuj użytkownika na administratora zespołu, cofnij uprawnienia administratora zespołu
- Usuń użytkownika z zespołu lub firmy (jeśli użytkownik opuszcza zespół, działa zarówno jako wykonawca, jak i obiekt dotknięty)
- Cofnij zaproszenie
- Dezaktywuj, reaktywuj użytkownika
- Użytkownik dołącza do zespołu/firmy

**Tablice**

- Otwórz tablicę
- Utwórz, usuń, przywróć tablicę
- Zmień nazwę tablicy
- Zmień opis tablicy
- Zmień okładkę tablicy
- Przenieś tablicę do innego zespołu
- Dodaj tablicę do projektu, usuń z projektu, przenieś do innego projektu
- Zmień właściciela tablicy
- Udostępnij tablicę wyświetlającemu/komentującemu/edytującemu
- Usuń użytkownika z tablicy
- Włącz, wyłącz, zmień [publiczny link do tablicy](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#udostepnianie-tablic-za-pomoca-linku-publicznego)
- Włącz, wyłącz, zmień [hasło do publicznej tablicy](../../../using-miro/sharing-boards/13-password-protection-for-public-boards.md)
- Włącz, wyłącz, zmień [udostępnianie tablicy firmie](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Włącz, wyłącz, zmień [udostępnianie tablicy zespołowi](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)
- Eksport tablicy, pobierz plik z tablicy.
- Utworzono stan
- Zaktualizowano stan
- Usunięto stan
- Przesłano plik (wycofany, dostępne w [Dzienniku treści](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md))

Należy pamiętać, że dziennik audytu **nie** zapisuje informacji dotyczących zmian na tablicach.

**Szablony**

- Otwórz szablon
- Utwórz, usuń, przywróć szablon
- Zmień nazwę szablonu
- Zmień właściciela szablonu
- Stan utworzony
- Stan zaktualizowany
- Stan usunięty

**Projekty**

- Utwórz, usuń projekt
- Zmień nazwę projektu
- Udostępnij projekt użytkownikowi, usuń uczestnika projektu
- Włącz, wyłącz udostępnianie projektu przez zespół
- Zmień właściciela projektu

**Logowania**

- Zaloguj się
- Logowanie nie powiodło się
- Wyloguj się
- Profil zablokowany, odblokowany

:::warning
Wydarzenia związane z logowaniem będą uwzględniać aktywność [dezaktywowanych użytkowników](../../user-management/01-deactivated-users.md).
:::

**Informacje profilowe**

- Zmień informacje profilowe
- Poproś o zmianę adresu e-mail
- Zmień adres e-mail

**Plany projektów**

- Utwórz plan projektu
- Usuń plan projektu
- Utwórz sekcję planu projektu
- Usuń sekcję planu projektu
- Zmień właściciela planu projektu

**Miro AI**

- Użyj funkcji Miro AI

### Często zadawane pytania

Czy istnieje sposób na automatyczne pobieranie dzienników audytu?

Tak, możesz skonfigurować [aplikację Miro dla Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md), aby uzyskać dostęp do dzienników Miro z Splunk.
