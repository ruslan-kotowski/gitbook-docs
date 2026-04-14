---
title: "Przegl\u0105d blokowania prompt\xF3w (wersja beta)"
article_id: 29332642230546
translation_id: 29332642230546
locale: pl-pl
sidebar_position: 4
created_at: '2025-09-09T07:58:00Z'
updated_at: '2026-01-12T11:23:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Funkcja blokowania promptów pozwala administratorom treści wrażliwych zapobiegać przesyłaniu przez użytkowników promptów AI, które zawierają informacje wrażliwe, pomagając w ten sposób utrzymać takie dane poza Miro AI w całej organizacji. Miro skanuje tekst, który użytkownik wpisuje w polu prompta oraz wszelkie treści tekstowe, które dodaje z tablicy. Jeśli ta treść odpowiada wybranym w konfiguracji blokowania promptów etykietom poufności lub wzorcom kodu źródłowego, Miro blokuje przesłanie prompta.

:::note
W wersji beta obsługiwane są tylko treści tekstowe.
:::

## Jak to działa

- Wybierasz, które kategorie etykiet blokować na poziomie organizacji. Zmiany wdrażane są natychmiast dla wszystkich w organizacji.
- Gdy w promcie wykryte zostaną dane wrażliwe, Miro AI pokazuje komunikat o zasadach w punkcie wejścia użytkownika, prompt jest blokowany i nie może być wysłany do Miro AI.
- Blokowanie promptów i skanowanie tablic to różne rzeczy. Skanowanie tablic lokalizuje wrażliwe treści na tablicach i może automatycznie klasyfikować tablicę. Blokowanie promptów przegląda to, co użytkownicy próbują wysłać do Miro AI.

## Co jest blokowane

- Etykiety prywatności: Wybierz spośród wszystkich naszych wbudowanych etykiet prywatności, takich jak SPII, HIPAA, dane dostępowe, numery finansowe. Więcej informacji na temat naszych wbudowanych etykiet prywatności znajdziesz w [Odnośnik do etykiet i typów informacji wrażliwych](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md).
- Skanowanie kodu. Po włączeniu Miro blokuje prompty, które zawierają rozpoznawalny kod źródłowy. Zobacz [Skanowanie kodu](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md) dla dalszych szczegółów.

## Typowe rezultaty dla użytkowników

Kiedy użytkownik wprowadza prompt, który zawiera informacje wrażliwe zgodnie z Twoją konfiguracją:

- Użytkownicy widzą komunikat taki jak "Nie możemy wygenerować tej treści, ponieważ może naruszać zasady Twojej organizacji."
- Prompt nie jest wysyłany do Miro AI. Użytkownicy mogą edytować prompt i spróbować ponownie.

## Skanowanie kodu

Skanowanie kodu blokuje prompty AI zawierające rozpoznawalny kod źródłowy. Proces ten wymaga minimum 5 linii kodu, aby zainicjować blokadę.

Przykład:

```
function connect() {

  const token = "example-token";

  fetch("https://api.example.com/health");

  return true;

}
```

## Obsługiwane języki

- C
- C#
- C++
- Go
- HTML
- Java
- JavaScript
- JSON
- PHP
- PowerShell
- Python
- Rust
- Skrypt powłoki
- SQL
- TypeScript
