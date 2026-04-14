---
title: "Przegl\u0105d niestandardowych warunk\xF3w us\u0142ugi"
article_id: 27375760557330
translation_id: 27375760557330
locale: pl-pl
sidebar_position: 2
created_at: '2025-06-13T08:24:28Z'
updated_at: '2025-11-04T14:10:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Funkcja niestandardowych warunków usługi pozwala administratorom wyświetlać niestandardowe okno dialogowe warunków usługi dla wszystkich wewnętrznych członków organizacji Miro. Zapewnia to, że użytkownicy przeglądają i akceptują warunki i zasady Twojej organizacji przed rozpoczęciem korzystania z Miro. Użyj tej funkcji, aby poinformować użytkowników o zasadach dopuszczalnego użytkowania funkcji Miro, w tym Miro AI. Administratorzy mogą dodać wiele linków do zasad zamieszczonych na zewnętrznych serwerach oraz skonfigurować częstotliwość, tak aby użytkownicy byli przypominani w harmonogramie zgodnym z wewnętrznymi wymaganiami. Wszystkie działania związane z niestandardowymi warunkami usługi są zapisywane w dzienniku audytu w celu śledzenia.

:::note
Niestandardowe Warunki Usługi są obecnie dostępne tylko w aplikacji internetowej i przeglądarkach.
:::

## Kluczowe korzyści

- Wyświetlaj warunki usługi w całej organizacji.
- Prezentuj dialog z dostosowanymi warunkami usługi w odpowiednich momentach: po pomyślnym logowaniu lub przy interakcji z Miro AI.
- Egzekwuj akceptację użytkowników według harmonogramu, który konfigurujesz (dni, tygodnie lub miesiące) lub po aktualizacjach.
- Linkuj do trzech wewnętrznych lub zewnętrznych zasad w preferowanym języku lub formacie.
- Zachowaj audytowalność w dziennikach audytu.

## Zakres

- Dotyczy: tylko użytkowników wewnętrznych, wszystkich członków organizacji oraz administratorów.
- Wykluczeni: goście i współpracownicy zewnętrzni.
- Wyzwalacze:
  - Udane logowanie: wyświetlane bezpośrednio po zalogowaniu.
  - Użycie Miro AI: wyświetlane, gdy użytkownik wchodzi w interakcję z Miro AI (na przykład, przełączając układ AI, otwierając panel boczny AI lub rozpoczynając akcję AI, taką jak współpracownik AI).
- Częstotliwość: konfigurowana przez administratora w dniach, tygodniach lub miesiącach. Każde własne Warunki usługi mają swoje własne statusy i częstotliwości. Domyślnie: dwa tygodnie.
- Formaty warunków: treść musi być hostowana zewnętrznie. Miro odwołuje się do linków i nie przechowuje pełnego tekstu zasad.
- Linki: do trzech linków do zasad, każdy z wyraźną etykietą.
- Konfiguracja: możesz skonfigurować jeden własny warunek usługi dla każdego wyzwalacza (pomyślne logowanie i użycie Miro AI). Każdy własny warunek usługi ma swój status oraz częstotliwość występowania.

## Kto może używać tej funkcji?

Administratorzy muszą posiadać następujące uprawnienia Enterprise Guard, aby wyświetlać i zarządzać własnymi warunkami usługi:

- **Administrator wrażliwych treści:** ma wbudowane uprawnienia.
- **Niestandardowe role admina**, muszą zawierać:
  - Wyświetl niestandardowe warunki korzystania z usługi
  - Zarządzaj niestandardowymi warunkami korzystania z usługi

## Jak to działa

1. **Skonfiguruj warunki:** wybierz wyzwalacz (udane logowanie lub użycie AI), zakres (wewnętrzni członkowie) i częstotliwość.
2. **Dodaj treść:** podaj zwięzły tytuł, krótki opis oraz do trzech oznaczonych linków do zewnętrznie hostowanych zasad.
3. **Przejrzyj i włącz:** przejrzyj dialog dla użytkownika końcowego i włącz konfigurację.
4. **Egzekwowanie:**

- **Pomyślne logowanie:** dialog nie może być zamknięty. Użytkownicy muszą zaakceptować, aby kontynuować lub się wylogować.
- **Użycie AI:** dialog pozwala na **kontynuowanie** lub **anulowanie**. Anulowanie utrzymuje użytkownika w stanie zalogowanym, ale wyłącza funkcje AI.

5. **Rejestracja:** zmiany konfiguracji i akceptacje użytkowników są zapisywane w dziennikach audytu.

### Doświadczenie użytkownika

- **Pomyślne logowanie**

  - Okno dialogowe pojawia się natychmiast po zalogowaniu.
  - Użytkownicy mogą kliknąć **Kontynuuj**, aby zaakceptować i kontynuować, lub **Wyloguj się**.
- **Użycie Miro AI**

  - Okno dialogowe pojawia się, gdy użytkownik wchodzi w interakcję z Miro AI, na przykład zmieniając układ AI, otwierając panel boczny AI lub uruchamiając narzędzie lub akcję AI (na przykład współpracownika AI).
  - Użytkownicy mogą kliknąć **Kontynuuj**, aby zaakceptować i korzystać z funkcji AI. Jeśli użytkownicy klikną **Anuluj**, pozostają zalogowani i mogą nadal korzystać ze wszystkich funkcji niezwiązanych z AI.
- Użytkownicy nie są ponownie powiadamiani aż do zakończenia okresu powtarzania lub aktualizacji warunków.

## Zachowanie przy akceptacji

- **Wyzwalacz logowania:** użytkownicy muszą zaakceptować zgodnie z ustalonym harmonogramem lub się wylogować. Dialog nie może być pominięty.
- **Wyzwalacz użycia AI:** użytkownicy mogą zaakceptować, aby włączyć funkcje AI, lub anulować, aby pozostawić funkcje AI wyłączone. Anulowanie pozostawia użytkownika zalogowanego i z możliwością korzystania z funkcji nie-AI.
- **Powtarzanie się i wersje:** użytkownicy nie są ponownie pytani, dopóki nie minie okres powtarzania lub nie zostanie opublikowana nowa wersja, zgodnie z ustalonym wyzwalaczem.

##

###
