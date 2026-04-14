---
title: "Osadzanie tablic Miro w\_Microsoft Teams"
article_id: 360017572514
translation_id: 360017572514
locale: pl-pl
sidebar_position: 5
created_at: '2019-02-11T10:13:30Z'
updated_at: '2025-04-24T13:52:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ms-teams
---

Osadzaj tablice Miro na kanałach Microsoft Teams i płynnie udostępniaj je osobom należącym do zespołu. Miej tablice Miro pod ręką i upewnij się, że cały zespół znajduje się na tej samej stronie.

:::note
Jeśli chcesz otrzymywać powiadomienia Miro za pośrednictwem Microsoft Teams, zapoznaj się [z tym przewodnikiem](10-miro-notifications-in-microsoft-teams.md).
:::

:::note
Sprawdź, jak osadzać tablice Miro na spotkaniach Microsoft Teams: [Miro dla Microsoft Teams Meetings (przewodnik](01-miro-for-microsoft-teams-admin-guide.md) dla administratora), [Miro dla Microsoft Teams Meetings (przewodnik dla użytkownika)](02-miro-for-microsoft-teams-user-guide.md).
:::

> **Dostępne dla** wszystkich wersji Miro

### Instalowanie wtyczki

Najpierw musisz znaleźć **Miro** w **Microsoft Teams Store** lub po prostu kliknąć na [link](https://teams.microsoft.com/l/app/8216e453-3db5-48ee-a3d6-5122f505c8a3).

:::warning
Pamiętaj, że administrator dzierżawy po stronie Microsoft Teams powinien włączyć aplikację Miro w katalogu aplikacji innych firm dla zespołów. Jeśli Miro nie zostanie zatwierdzone, nie będzie ono widoczne na liście wraz z aplikacjami w Microsoft Teams Store.
:::

Kliknij **Dodaj,** aby zainstalować wtyczkę.

![Miro_plugin_installation.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790725266_Miro%20plugin%20installation.jpg)
*Instalacja wtyczki Miro*

Po zainstalowaniu wtyczki Miro przekierujemy Cię na czat, na którym będziesz mógł skonfigurować otrzymywanie powiadomień Miro. Aby dowiedzieć się więcej, zapoznaj się z [tym](10-miro-notifications-in-microsoft-teams.md) artykułem.

Jednak w tym momencie możesz już rozpocząć osadzanie tablic Miro na kanale Microsoft Teams bez dodatkowej konfiguracji.

### Osadzanie tablic na kanałach Microsoft Teams

> **Konfiguracja przez:** [właścicieli](../../../using-miro/sharing-boards/01-board-access-rights.md) tablicy i [edytujących,](../../../using-miro/sharing-boards/01-board-access-rights.md) którzy są członkami zespołu, w którym znajduje się tablica.

Możesz osadzać swoje tablice na kanałach Microsoft Teams, tworząc nową kartę. Kliknij ikonę plusa. Otrzymasz selektor z różnymi aplikacjami. Znajdź Miro na liście aplikacji i wybierz je. Jeśli nie masz uprawnień w Miro w tej samej przeglądarce lub w aplikacji komputerowej, musisz się zalogować. Kliknij **Rozpocznij** i zaloguj się lub [zarejestruj](../../../getting-started/start-here/02-how-to-register-with-miro.md) się w Miro.

![embed_in_MS_teams.gif](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734975122_embed%20in%20MS%20teams.gif)
*Tryb wyświetlający monit o autoryzację profilu Miro*

Po autoryzacji zobaczysz selektor z tablicami Miro – selektor pokaże te tablice, do których masz dostęp po stronie Miro. Pamiętaj, że możesz uzyskać autoryzację w Miro i w Microsoft Teams pod różnymi adresami e-mail.

Umieść tablicę, którą chcesz dodać do swojego kanału Microsoft Teams.

![MS_teams_embed_picker.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734978322_MS%20teams%20embed%20picker.jpg)
*Selektor z tablicami Miro*

Pamiętaj, że tylko właściciele tablic i edytujący, którzy są członkami zespołu, mogą osadzać tablice Miro. Jeśli wybierzesz tablicę, na której nie masz potrzebnego poziomu dostępu, zobaczysz komunikat ostrzegawczy.

![unable_to_embed_boards.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790732690_unable%20to%20embed%20boards.jpg)
*Komunikat o tym, że poziom dostępu nie pozwala na osadzenie tablicy*

Następnie możesz ustawić uprawnienia dla pozostałych uczestników spotkania i przyznać lub ograniczyć dostęp do tablicy. Możesz wybrać spośród tych typów uprawnień:

- **Każdy może edytować** (logowanie nie jest wymagane)
- **Każdy może komentować** (logowanie nie jest wymagane)
- **Każdy może wyświetlać** (logowanie nie jest wymagane)
- **Prywatny**

![sharing_level.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790733586_sharing%20level.jpg)
*Uzyskaj dostęp do ustawień osadzonej tablicy*

:::note
Pamiętaj, że ustawienia udostępniania skonfigurowane dla tablicy w Miro mogą również definiować dostęp do tablicy w ramach Microsoft Teams. Jeśli tablica jest udostępniana publicznie w Miro, będzie dostępna dla wszystkich osób w zespołach Microsoft Teams, nawet jeśli osadzona jest na tablicy jako **prywatna**. Jeśli jednak Twoja tablica jest [prywatna](../../../using-miro/sharing-boards/15-make-a-miro-board-private.md) po stronie Miro i osadzasz ją w aplikacji **Każdy może przeglądać/komentować/edytować** dostęp, nie wpłynie to na dostęp do tablicy w Miro. [Dowiedz się więcej](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).
:::

:::note
Dla użytkowników [abonamentu Enterprise](../../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md) Miro ustawienia dostępu będą zgodne z ustawieniami dostępu dla całej organizacji, co może oznaczać, że niektóre opcje udostępniania mogą być ograniczone. Dowiedz się więcej: [Zarządzanie zasadami udostępniania Enterprise dla integracji osadzania](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

:::warning
**Każda osoba może komentować** opcja nie jest obsługiwana, jeśli osadzasz tablicę znajdującą się w [bezpłatnym zespole](../../../plans-billing/miro-plans/09-free-plan.md).
:::

Po osadzeniu tablicy możesz od razu rozpocząć interakcję z nią.

![Miro_embed_in_MS_teams.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734972562_Miro%20embed%20in%20MS%20teams.jpg)
*Tablica osadzona na kanale Microsoft Teams*

:::note
Użytkownicy Microsoft Teams, którzy korzystają z Miro w aplikacji mobilnej Microsoft Teams, mogą *wyświetlać i komentować* tablice w zależności od ustawionych uprawnień. Zalecamy użytkownikom zainstalowanie naszej natywnej [aplikacji](../../../getting-started/apps-for-devices/08-mobile-app.md) mobilnej, dla której zoptymalizowaliśmy interfejs użytkownika.
:::

![Miro_in_MS_Team_on_mobile.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734976146_Miro%20in%20MS%20Team%20on%20mobile.jpg)
*Tablica Miro w MS Teams na urządzeniach mobilnych – naciśnij **Otwórz w** aplikacji, aby zainstalować natywną aplikację mobilną Miro.*

### Często zadawane pytania

1. *Czy każdy uczestnik zespołu musi mieć profil Miro, aby wyświetlać osadzone tablice w Microsoft Teams?*
   - Jeśli wybierzesz **Każdy może** wyświetlać/komentować/edytować podczas osadzania tablicy, nawet niezarejestrowani użytkownicy będą mogli ją przeglądać/komentować. Ponadto, jeśli tablica jest [udostępniana publicznie](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#udostepnianie-tablic-za-pomoca-linku-publicznego) po stronie Miro, będzie dostępna dla wszystkich osób w zespołach Microsoft Teams.
2. *Kto po osadzeniu tablicy ma możliwość zmiany dostępu do tablicy w zespołach MS (np. z „Każdy może wyświetlać” na „Prywatny”)?*- Nikt nie może zmienić dostępu do dołączonej tablicy, nawet ta osoba, która ją dołączyła. Jednak każdy może kliknąć **Ustawienia** na karcie, a następnie wybrać inną (lub tę samą tablicę) dla tej samej karty i wybrać inny poziom dostępu dla wybranej tablicy.
3. *Jestem zarejestrowany w Miro pod dwoma adresami e-mail i chcę osadzić tablicę Miro z mojego drugiego profilu Miro. Jak przełączyć profil Miro?*- Selektor pokazuje tablice użytkownika, do którego masz autoryzację w Miro w tej samej przeglądarce. Otwórz Miro w innej karcie przeglądarki, wyloguj się i zaloguj się na swój drugi profil Miro.
   Jeśli korzystasz z aplikacji komputerowej Microsoft Teams, wyloguj się z aplikacji -  spowoduje to również wylogowanie Cię z Miro w aplikacji. Następnie zaloguj się do aplikacji i spróbuj [osadzić tablicę](#h_5af20ae6-78c0-4e6c-ab20-e4968c89c97f). Zostaniesz poproszony o zalogowanie się do Miro i będziesz mógł zalogować się do innego profilu Miro.
