---
title: "Zarz\u0105dzanie niestandardowymi warunkami korzystania z us\u0142ugi"
article_id: 27621616452882
translation_id: 27621616452882
locale: pl-pl
sidebar_position: 3
created_at: '2025-06-24T23:29:13Z'
updated_at: '2025-11-04T14:10:40Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

## Tworzenie niestandardowych warunków korzystania z usługi

:::note
Notatki:

- Administratorzy muszą mieć następujące uprawnienia Enterprise Guard, aby wyświetlać i zarządzać niestandardowymi warunkami korzystania z usługi:
  - Administrator treści wrażliwych ma wbudowane uprawnienia.
  - Niestandardowe role administratora muszą obejmować:
    - Wyświetl niestandardowe warunki korzystania z usługi
    - Zarządzaj niestandardowymi warunkami korzystania z usługi
- Goście i użytkownicy zewnętrzni są wyłączeni.
- Miro nie przechowuje warunków, tylko link i metadane.
:::

1. Przejdź do **Ustawienia** > **Enterprise Guard** > **Niestandardowe warunki usługi**.
2. Jeśli tworzysz niestandardowe warunki usługi po raz pierwszy, kliknij **Dodaj warunki usługi**.
   Jeśli masz już istniejącą konfigurację i chcesz dodać kolejną, kliknij **Utwórz nowe** w widoku listy.
3. W **Konfiguracja** → **Warunki**:
   - **Wyzwalacz**: Wybierz pomiędzy **Udane logowanie** lub **Użycie AI**.
     **Udane logowanie**

     - Okno dialogowe pojawia się natychmiast po logowaniu.
     - Użytkownicy mogą kliknąć **Kontynuuj** aby zaakceptować i przejść dalej, lub **Wyloguj się**.

     **Użycie AI**

     - To okno dialogowe pojawia się, gdy użytkownik wchodzi w interakcję z Miro AI, na przykład przełącza układ AI, otwiera panel boczny AI lub uruchamia narzędzie AI lub akcję (na przykład współpracownik AI).
     - Użytkownicy mogą kliknąć **Kontynuuj**, aby zaakceptować i korzystać z funkcji AI. Jeśli użytkownicy klikną **Anuluj**, pozostają zalogowani i mogą nadal korzystać ze wszystkich funkcji nie związanych z AI.
   - **Zakres**: **Wszyscy użytkownicy i administratorzy w organizacji**.
   - **Okres powtarzania**: wprowadź liczbę i wybierz **Dni**, **Tygodnie** lub **Miesiące**. Domyślnie: dwa tygodnie.
     Użytkownicy nie będą ponownie pytani, dopóki nie zakończy się okno powtarzania lub nie zostaną zaktualizowane warunki.
4. W **Skonfiguruj** → **Zawartość**:
   - **Tytuł** (maks. 32 znaki)
   - **Opis** (maks. 200 znaków)
   - **Link:** Linki do polityk (hostowane zewnętrznie). Aby dodać dodatkowe linki, kliknij +Dodaj link. Obsługiwane są maksymalnie trzy linki. Każdy adres URL linku musi być unikalny.
   - **Tekst linku** (maks. 60 znaków). Każdy tekst linku musi być unikalny.
5. Kliknij **Pokaż podgląd** (w prawym górnym rogu), aby przejrzeć zawartość okna dialogowego warunków usługi. W razie potrzeby dostosuj zawartość warunków usługi.
6. Gdy będziesz gotowy z treścią niestandardowych warunków korzystania z usługi, kliknij **Dalej**.
7. Przejrzyj niestandardowe warunki korzystania z usługi, potwierdź swoje ustawienia i treść, a następnie kliknij **Opublikuj**.
   Wymuszenie jest natychmiastowe dla wybranego wyzwalacza.

## Edycja niestandardowych warunków korzystania z usługi

1. Otwórz **Ustawienia** > **Enterprise Guard** > **Warunki usługi**.
2. Na liście wybierz konfigurację warunków usługi, którą chcesz zaktualizować, a następnie kliknij **Edytuj**.
3. Zaktualizuj pola zgodnie z potrzebą w **Warunki** i **Zawartość**.
4. Jeśli chcesz zaktualizować warunki usługi i natychmiast zresetować wszystkie akceptacje użytkowników, kliknij **Opublikuj natychmiast.**
   Jeśli chcesz zaktualizować warunki usługi i ponownie poprosić użytkowników po zakończeniu skonfigurowanego okresu odnawiania, kliknij strzałkę w dół, wybierz **Opublikuj w następnym cyklu**, a następnie kliknij **Opublikuj w następnym cyklu**.

## Usuwanie niestandardowych warunków korzystania z usługi

Usunięcie wyłącza niestandardowe warunki korzystania z usługi natychmiast i nie może zostać cofnięte.

1. Otwórz **Ustawienia** > **Enterprise Guard** > **Niestandardowe warunki korzystania z usługi**.
2. Na liście wybierz konfigurację niestandardowych warunków korzystania, którą chcesz usunąć, a następnie kliknij **Usuń**.
3. Aby trwale usunąć wybrane niestandardowe warunki korzystania z usługi, kliknij **Usuń warunki**.
