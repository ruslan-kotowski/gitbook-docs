---
title: Połącz z Centrum danych Jira za pomocą OAuth 2.0
article_id: 25753304280466
translation_id: 26513350378386
locale: pl-pl
sidebar_position: 8
created_at: '2025-05-06T09:04:28Z'
updated_at: '2025-05-21T09:27:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Kto może to zrobić: Administratorzy firmy z uprawnieniami administratora
    systemu Jira Które wersje: Przedsiębiorstwo Które platformy: przeglądarka, aplikacja
    komputerowa'
---

> Łączenie z Jira Data Center za pomocą OAuth 2.0 jest włączone tylko na poziomie organizacji.

## Wymagania wstępne

- Upewnij się, że masz następujące uprawnienia:
  - Uprawnienia administratora systemu Jira
  - Rola administratora firmy Miro
- Utwórz link do aplikacji OAuth 2.0 na Centrum danych Jira. Aby dowiedzieć się, jak to zrobić, zobacz (Zewnętrzne) [pomoc dotyczącą aplikacji Atlassian Jira](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Create%20an%20incoming%20link%20using%20application%20links).
  - Użyj następującego adresu URL przekierowania, gdy pojawi się monit:
    https://integrations.miro.com/api/external-auth/oauth2/callback
  - Aby używać automatycznych webhooków, upewnij się, że wybierasz **Administratora** jako swój zakres.

## Połącz Miro z Centrum danych Jira przy użyciu OAuth 2.0

1. Na pulpicie Miro kliknij swój awatar w prawym górnym rogu i przejdź do (Enterprise) **Konsola administratora** lub(Starter i Business) **Ustawienia**.
2. Na pasku po lewej stronie przejdź do **Aplikacje i integracje ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Aplikacje** > **karta Zarządzaj aplikacjami** .
3. Upewnij się, że **Zezwalaj tylko na aplikacje z poniższej listy** jest włączone.
4. W kolumnie **Aplikacja**, wybierz **Ustawienia** dla **kart Jira**.
5. Wybierz **Dodaj nowe połączenie**.
6. W sekcji **Jira setup** wybierz **Centrum danych Jira**.
7. W sekcji **Metoda uwierzytelniania** wybierz **OAuth 2.0**.
8. Dla **adresu URL Jira** wprowadź adres URL swojej instancji Jira.
9. (Opcjonalnie) Aby ustawić to połączenie jako domyślne połączenie dla wszystkich zespołów w organizacji, kliknij **Ustaw jako domyślne**.
10. Wpisz ID klienta **Jira**.
    **Więcej informacji**: Zobacz (Zewnętrzny) [Skonfiguruj przychodzące połączenie](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
11. Wpisz klucz tajny **klienta** Jira.
    **Więcej informacji**: Zobacz (Zewnętrzny) [Konfiguruj połączenie przychodzące](https://confluence.atlassian.com/adminjiraserver/configure-an-incoming-link-1115659067.html#:~:text=Copy%20OAuth%20credentials%20to%20the%20application).
12. Wybierz zakres.
    Aby korzystać z automatycznych webhooków, wybierz **Administrator** lub **Administrator systemu**.
13. (Opcjonalne) Aby otrzymywać aktualizacje w czasie rzeczywistym z Jira w Miro, zaznacz **Utwórz webhook automatycznie**.
    > Opcjonalnie, możesz ręcznie dodać webhook później.
14. Wybierz **Połącz**.
    > Po raz pierwszy, gdy użytkownik próbuje wykonać akcję związaną z Jira, zostaje poproszony o uwierzytelnienie. Nie trzeba ponownie uwierzytelniać.

## Co dalej?

Aby wyświetlić i zarządzać połączonymi instancjami Jira, przejdź do **Konsola Administratora** | **Ustawienia** >  **Aplikacje i integracje ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** >  **Zarządzaj aplikacjami**. Następnie w kolumnie **Aplikacja** dla **kart Jira** wybierz **Ustawienia**.

Aby dowiedzieć się, jak połączyć swoje zespoły z domyślną instancją Jira, zobacz [Łączenie zespołów w organizacji z domyślnymi ustawieniami Jira.](https://help.miro.com/hc/articles/26438407676434)

## FAQ

**Czy wybór administratora jako zakresu wymaga, aby wszyscy użytkownicy mieli uprawnienia administratora w Jira?**

Nie. Zakres administratora oznacza, że administrator ma najwyższy zakres, jaki może mieć użytkownik w Miro. Zakres jest i tak ograniczony na użytkownika, w zależności od ich uprawnień w Jira.

**Czy mogę połączyć Centrum danych Jira z OAuth 2.0 na poziomie zespołu?**

Nie. Tylko na poziomie organizacji.
