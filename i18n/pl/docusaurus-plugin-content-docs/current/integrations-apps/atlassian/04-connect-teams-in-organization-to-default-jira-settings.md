---
title: Połącz zespoły w organizacji z domyślnymi ustawieniami Jira
article_id: 26438407676434
translation_id: 26441941690514
locale: pl-pl
sidebar_position: 6
created_at: '2025-05-02T14:34:57Z'
updated_at: '2025-10-21T12:07:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Kto może to zrobić: administratorzy firmy Jakie abonamenty: Enterprise Jakie
    platformy: Przeglądarka, Desktop'
---

Administratorzy firmy mogą zbiorczo połączyć zespoły w swojej organizacji, aby używały globalnych ustawień Jira, co nadpisuje ustawienia określone na poziomie zespołu.

## Wymagania wstępne

- Upewnij się, że masz rolę administratora firmy w Miro.
- Upewnij się, że masz domyślne połączenie z [Połącz z Jira Data Center za pomocą OAuth 2.0](https://help.miro.com/hc/articles/25753304280466).

## Połącz zespoły z domyślnymi ustawieniami Jira

1. Z pulpitu Miro wybierz swój awatar w prawym górnym rogu i przejdź do **Konsola administracyjna** | **Ustawienia**.
2. W lewym pasku bocznym przejdź do **Aplikacje i integracje ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Aplikacje** > karta **Zarządzaj aplikacjami**.
3. Upewnij się, że **Zezwól tylko aplikacjom z poniższej listy** jest włączone.
4. Pod kolumną **Aplikacja**, dla **Jira Cards** wybierz **Ustawienia**.
5. W sekcji **Dodaj zespoły do instancji domyślnej**, wybierz każdy zespół, który chcesz połączyć, lub kliknij **Wybierz wszystkie**.

   > ✏️ Lista pokazuje jedynie zespoły niekorzystające z globalnych ustawień organizacji.
6. Kliknij **Dodaj <liczba zespołów> do domyślnych**.

   > ✏️ Użytkownicy, którzy nie korzystają z globalnej instancji Jira w Twojej organizacji, zostaną przeniesieni i muszą się ponownie uwierzytelnić.

   > ✏️ Użytkownicy przeniesieni z innej instancji Jira są proszeni o ponowną autoryzację przy pierwszej próbie akcji związanej z Jira w Miro.

## FAQ

**Czy zespoły będą na stałe korzystać z globalnego połączenia z Jira?**

Nie. Możesz później zmienić ustawienia Jira dla danego zespołu.

**Jakie zespoły powinny korzystać z globalnego połączenia z Jira?**

Korzystanie z ustawień organizacji jest generalnie preferowane, ponieważ wymaga mniej pracy administracyjnej z Twojej strony. Jeśli jakiekolwiek połączenia zespołów mają te same ustawienia co organizacja, zalecamy wdrażanie zespołów do domyślnych ustawień organizacji z tego powodu.
