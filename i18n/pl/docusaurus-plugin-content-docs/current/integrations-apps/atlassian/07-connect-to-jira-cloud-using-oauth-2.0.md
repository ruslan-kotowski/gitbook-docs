---
title: Połącz z Jira Cloud przy użyciu OAuth 2.0
article_id: 8588617184402
translation_id: 26810590573970
locale: pl-pl
sidebar_position: 7
created_at: '2025-05-19T13:04:37Z'
updated_at: '2025-10-21T12:18:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Dostępne dla: Jira Cloud, w tym zabezpieczony przez LDAP Abonamenty: Starter,
    Business, Enterprise, Education Konfigurowane przez: (Enterprise) administratora
    firmy lub (inne abonamenty) administratora zespołu, z uprawnieniami administratora
    Jira'
---

:::warning
W przypadku problemów technicznych, zapoznaj się z naszym artykułem o [Możliwe problemy i ich rozwiązania](https://help.miro.com/hc/articles/360017572654).
:::

:::tip
Dowiedz się więcej o kartach Jira w artykułach [Często zadawane pytania o kartach Jira](https://help.miro.com/hc/articles/360013463739)
:::

## Łączenie Jira i Miro

### Instalowanie aplikacji

1. Aby włączyć integrację, na swoim [pulpicie](https://help.miro.com/hc/articles/360017571294-What-is-on-your-dashboard) w prawym górnym rogu kliknij swój awatar > **Integracje i aplikacje**:![mceclip0.png](../../../../../../docs/integrations-apps/atlassian/images/21017417672210_mceclip0.png)
   *Zarządzanie aplikacjami*
2. Znajdź "karty Jira" w linii **Wyszukiwania** i kliknij niebieski przycisk **Połącz** w prawym dolnym rogu menu podręcznego.
3. Zobaczysz okno do **Dodania "Kart Jira"**. Tutaj musisz potwierdzić instalację lub wybrać zespół, w którym chcesz zainstalować integrację (w przypadku, gdy jesteś członkiem kilku zespołów). Kliknij, aby **Dodać** integrację. Na górze pulpitu zobaczysz wiadomość potwierdzającą, że **Aplikacja została zainstalowana:**
   ![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)
   *Wiadomość potwierdzająca*

### Łączenie profilu Jira

1. Kliknij ponownie swój awatar na pulpicie i przejdź do **Ustawienia > Zespoły >** *Nazwa Twojego zespołu* **> Aplikacje & Integracje > Karty Jira**, a następnie kliknij **Połącz:
   ![mceclip2.png](../../../../../../docs/integrations-apps/atlassian/images/21017004818066_mceclip2.png)***Ustawienia integracji*
2. Zostaniesz skierowany na stronę Jira, aby autoryzować połączenie. Zaloguj się do Jira i kliknij **Akceptuj**.

### Łączenie instancji Jira z Twoim zespołem Miro

Dzięki OAuth 2.0 możesz teraz połączyć kilka instancji Jira z tym samym zespołem i tablicami. Po autoryzacji aplikacji w Ustawieniach zobaczysz opcję **Połącz inną instancję.**

1. Uruchom wybierak kart Jira z paska narzędzi tworzenia (możesz potrzebować dodać aplikację przyciskiem **Więcej aplikacji +**).
2. W wybieraku kliknij **Ustawienia**.
3. Zostaniesz przeniesiony do sekcji **Aplikacje i Integracje** w swoich ustawieniach. Poszukaj opcji **Połącz kolejną instancję** i wybierz dowolne dodatkowe instancje Jira, które chcesz połączyć.![mceclip0.png](../../../../../../docs/integrations-apps/atlassian/images/21017417672210_mceclip0.png)*Ustawienia kart Jira w koncie Miro*

Administratorzy zespołu mogą również zobaczyć wszystkie instancje połączone przez członków zespołu:

![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)

:::warning
Zwróć uwagę, że każdy użytkownik końcowy będzie musiał uwierzytelnić się z poziomu tablic Miro z każdą połączoną instancją Jira, jeśli spróbuje pracować z kartami tej instancji.
:::

> ✍️ Pamiętaj, że jednocześnie aktywna może być tylko jedna instancja, więc użytkownicy mogą pobierać z niej karty. Istniejące karty z nieaktywnych instancji nadal można edytować na tablicach Miro.

### Konfigurowanie aktualizacji w czasie rzeczywistym z Jira

Aby w pełni wykorzystać zalety naszego dwukierunkowego synchronizowania w czasie rzeczywistym, musisz skonfigurować webhooki dla dodanych instancji Jira. To zapewni, że wszelkie aktualizacje wprowadzone w Jira będą automatycznie odzwierciedlane w Miro.

1. Uruchom Wybór kart Jira z paska narzędzi (być może będziesz musiał dodać aplikację, używając przycisku **Więcej aplikacji +**).
2. W narzędziu Wybierania kliknij **Ustawienia**.
3. Zostaniesz przeniesiony do sekcji **Aplikacje i integracje** w swoich ustawieniach.
4. W sekcji **Połączone instance** powinieneś zobaczyć listę dodanych już instancji.
5. Obok każdej instancji znajduje się przycisk **Dodaj webhook.** Kliknięcie tego przycisku skonfiguruje aktualizacje w czasie rzeczywistym z Jira do Miro dla tej instancji.
6. Jeśli chcesz usunąć webhooki z tej instancji w przyszłości, możesz wykonać powyższe kroki i kliknąć przycisk **Usuń webhook**, który znajduje się obok połączonych instancji, do których dodałeś webhook.

:::note
Prosimy pamiętać, że musisz być administratorem w Miro *i* Jira, aby móc dodawać webhooki do swoich instancji.
:::

To wszystko! Teraz możesz dodawać zadania Jira jako karty na tablicy. Wszystkie zmiany dokonane w Jira są odzwierciedlane na kartach Jira na tablicy i odwrotnie.

## Odinstalowywanie wtyczki

Przejdź do **Ustawienia zespołu > Aplikacje i integracje > Karty Jira** i kliknij **Odinstaluj dla zespołu.**

:::tip
Nie zapomnij zapoznać się z głównym artykułem o [korzystaniu z kart Jira](https://help.miro.com/hc/articles/360017572434)!
:::
