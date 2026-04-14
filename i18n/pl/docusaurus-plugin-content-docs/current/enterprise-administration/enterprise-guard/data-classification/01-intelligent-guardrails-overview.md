---
title: "Przegl\u0105d Inteligentnych Zabezpiecze\u0144"
article_id: 14375998880018
translation_id: 14375998880018
locale: pl-pl
sidebar_position: 0
created_at: '2023-10-12T12:35:03Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Elementy tablic Miro mogą zawierać dane prywatne i podlegające regulacjom (takie jak informacje umożliwiające identyfikację osoby, chronione informacje zdrowotne, PCI) lub poufne dane kluczowe dla biznesu (takie jak informacje finansowe, informacje HR, własność intelektualna, tajemnice handlowe). Po wykryciu danych i klasyfikacji automatycznej organizacje muszą wdrożyć proaktywne zabezpieczenia, które są kluczowe dla utrzymania ciągłej prywatności, bezpieczeństwa i zgodności z obowiązującymi regulacjami.

- Dzięki zabezpieczeniom można teraz automatycznie egzekwować proaktywne zabezpieczenia, takie jak:
  Automatyczne ograniczanie możliwości udostępniania na różnych poziomach (publicznym, zespole, organizacji) w oparciu o zawartość tablicy i poziom klasyfikacji.
- Ograniczenie replikacji zawartości.
- Blokowanie użycia Miro AI, aby zapobiec interakcjom opartym na AI z danymi wrażliwymi lub sklasyfikowanymi.

Te proaktywne zabezpieczenia zapewniają trwałą prywatność i zgodność bez zakłócania działań biznesowych.

Administratorzy mają dwie opcje wdrażania zabezpieczeń w swojej organizacji:
- **Tryb domyślny:** Domyślnie zabezpieczenia nie wpływają na aktywne opcje udostępniania na tablicach, aby nie zakłócać bieżącej współpracy, nawet gdy tablice są ponownie klasyfikowane podczas automatycznej klasyfikacji.

- **Tryb rygorystyczny:** Kiedy przełącznik **Zastosuj zabezpieczenia w trybie rygorystycznym** jest włączony, zabezpieczenia zastępują wszystkie aktywne opcje udostępniania. To daje administratorom najwyższy poziom kontroli, ale może również spowodować, że niektórzy użytkownicy stracą dostęp do tablicy natychmiast.

Rozważ scenariusz, w którym skonfigurowałeś zabezpieczenia, aby użytkownikom tablic sklasyfikowanych jako POUFNE uniemożliwić udostępnianie tablicy publicznie, zespołom, organizacji lub replikowanie zawartości. Ktoś w Twojej organizacji utworzył nową tablicę o nazwie Plan finansowy, dodał kilka danych dotyczących przychodów i przypisał dla tej tablicy poziom klasyfikacji *POUFNE*. Ustawienia zabezpieczeń są stosowane automatycznie, co oznacza, że wszyscy użytkownicy nie mogą udostępniać tablicy, a wszyscy użytkownicy z wyjątkiem właściciela tablicy nie mogą replikować zawartości (Rysunek 2).

Więcej informacji o każdym z zabezpieczeń, ich opisach oraz użytkownikach, których dotyczą, znajdziesz w [dokumentacji referencyjnej dotyczącej zabezpieczeń](02-guardrails-reference.md).
