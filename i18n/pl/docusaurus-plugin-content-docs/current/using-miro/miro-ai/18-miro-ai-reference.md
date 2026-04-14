---
title: Zasoby dotyczące Miro AI
article_id: 20970362792210
translation_id: 20970362792210
locale: pl-pl
sidebar_position: 18
created_at: '2024-08-26T09:34:26Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: 'Kto może to zrobić: Wszyscy użytkownicy Jakie abonamenty: Free, Starter,
    Business, Enterprise, Education Jakie platformy: Przeglądarka, Komputer, Urządzenie
    mobilne'
---

Ten artykuł referencyjny opisuje funkcjonalność Miro AI.

## Modele Miro AI

Modele są zazwyczaj hostowane na infrastrukturze dostawcy, usłudze Microsoft Azure AI lub AWS Bedrock. Dla klientów, którzy nabywają Miro poprzez AWS Marketplace, wszystkie modele są hostowane na AWS Bedrock.

### Tworzenie i iteracja z pomocą AI

| **Funkcja Miro AI** | **Opis** | **Model** |
| --- | --- | --- |
| Podsumowania rozmów | Generuje podsumowanie długich wątków komentarzy na Twojej tablicy Miro. | GPT 4o-mini |
| Tworzenie diagramu - Schemat blokowy | Tworzy schemat blokowy na podstawie promptu użytkownika i wybranej zawartości tablicy. | GPT-4o |
| Edytuj diagram - Przepływ | Edytuje przepływ na podstawie promptu użytkownika i wybranej treści z tablicy. | GPT-4o |
| Twórz diagram - Mapa myśli | Tworzy mapę myśli na podstawie promptu użytkownika i wybranej treści z tablicy. | GPT 4o-mini |
| Edytuj diagram - Mapa myśli | Edytuje mapę myśli na podstawie promptu użytkownika i wybranej treści z tablicy. | GPT-4o |
| Utwórz diagram - ERD | Tworzy diagram ERD na podstawie promptu użytkownika. Opcja **Stwórz z AI**. | GPT 4o-mini |
| Edytuj diagram - ERD | Edytuje ERD na podstawie promptu użytkownika i wybranej treści z tablicy. | GPT-4o |
| Zdigitalizuj diagram | Przekształca obrazy ręcznie rysowanych diagramów na w pełni edytowalne diagramy w Miro. | Claude 3.7 Sonnet (AWS Bedrock) |
| Tworzenie dokumentu | Tworzy dokument Miro na podstawie promptu użytkownika i wybranej treści z tablicy. Opcja **Tworzenie z AI**. | GPT-4o |
| Edycja dokumentu | Edytuje dokument Miro na podstawie promptu użytkownika i wybranej treści z tablicy. | GPT-4o |
| Tworzenie obrazu | Tworzy obraz na podstawie promptu użytkownika, uwzględniając obiekty na tablicy jako kontekst. Opcja **Tworzenie z AI**. | Segmind Stable Diffusion 1B (SSD-1B) + StabilityAI Diffusion XL Refiner 1.0 |
| Edycja obrazu | Edytuje obraz na podstawie promptu użytkownika, uwzględniając obiekty na tablicy jako kontekst. Opcja **Twórz z AI**. | GPT-4o |
| Konwersja obrazu na prototyp | Konwertuje szkic lub obraz prototypu na edytowalny Miro Prototype. | Model własny Miro + Claude 3.7 Sonnet |
| Tekst alternatywny obrazu | Generuje tekst alternatywny dla obrazu. Nie zużywa tokena na AI. | Własny model Miro |
| Tworzenie karteczek | Tworzy karteczki Miro na podstawie promptu użytkownika i wybranej treści z tablicy. | GPT-4o |
| Edycja karteczek | Edytuje karteczki Miro na podstawie tablicy użytkownika i wybranej treści z tablicy. | GPT-4o |
| Przechwytywanie karteczek | Konwertuje obraz fizycznych karteczek na karteczki Miro. | Miro proprietary model |
| Utwórz Prototyp | Tworzy Prototyp Miro na podstawie promptu użytkownika i wybranej zawartości tablicy. | GPT-4o + Claude 4.5 Sonnet + GPT 4o-mini + Gemini 2.5 Flash Image (nano-banana) |
| Edytuj ekran Prototypu | Edytuje ekran Prototypu Miro na podstawie promptu użytkownika i wybranej zawartości tablicy. | Claude 4.5 Sonnet + Gemini 2.5 Flash Image (nano-banana) |
| Usuń tło | Usuwa tło z obrazu. | Model własnościowy Miro |
| Inteligentne rysunki | Konwertuje szkic na linię, kształt lub karteczkę. | Model własnościowy Miro |
| Utwórz tabelę | Tworzy tabelę Miro na podstawie promptu użytkownika i wybranej treści z tablicy. | Claude 3.7 Sonnet |
| Edytuj tabelę | Edytuje tabelę Miro na podstawie promptu użytkownika i wybranej treści z tablicy. | Claude 3.7 Sonnet |

### Współpracownicy AI

|  |  |  |
| --- | --- | --- |
| **Funkcja Miro AI** | **Opis** | **Model** |
| Współpracownik AI - Trener Agile | Identyfikuje kluczowe tematy w retrospektywie i sugeruje kolejne kroki. | GPT-4o |
| Współpracownik AI - Lider Produktu | Daje opinie i sugestie jako komentarze na ramkach, karteczkach lub tekście. Dostarcza również pomysły na rozwiązania w formie karteczek. | GPT-4o |
| Współpracownik AI - Sojusz Produktowego Marketingu | Daje opinie i sugestie jako komentarze na ramkach, karteczkach lub tekście. | GPT-4o |

### Kategoryzacja wspomagana AI

| **Funkcja Miro AI** | **Opis** | **Model** |
| --- | --- | --- |
| Kategoryzacja karteczek według słów kluczowych | Organizuje karteczki w grupy według słów kluczowych, z tytułem dla każdej grupy. | Claude 3.5 Haiku + Amazon Nova Micro |
| Kategoryzacja karteczek według odczuć | Organizuje karteczki według odczuć, takich jak opinie i punkty widzenia, w grupy pozytywne, neutralne i negatywne. | Claude 3.5 Haiku |

### Edycja tekstu oparta na sztucznej inteligencji

Poniższa tabela pokazuje edytowanie tekstu napędzane przez Miro AI:

|  |  |  |
| --- | --- | --- |
| **Funkcja Miro AI** | **Opis** | **Model** |
| Zmień ton | Zmienia ton wybranego tekstu, aby był bardziej przyjazny, profesjonalny, biznesowy lub zabawny. | GPT-5 nano |
| Poprawia pisownię i gramatykę | Poprawia pisownię i gramatykę dla zaznaczonego tekstu. | GPT-5 |
| Przepisz dla jasności | Przepisuje wybrany tekst, aby był bardziej zrozumiały. | GPT-5 Chat |
| Skróć tekst | Tworzy krótszą wersję wybranego tekstu, zachowując jasność i czytelność. | GPT-5 mini |
| Tłumacz | Tłumaczy wybrany tekst na angielski, hiszpański, niemiecki, francuski, japoński, portugalski, koreański, polski, włoski, turecki, arabski, rosyjski, duński, fiński, norweski, niderlandzki, szwedzki lub tajski. Możesz tłumaczyć pojedyncze obiekty lub wiele obiektów jednocześnie. | GPT-5 mini |

### Mapy myśli zasilane przez AI

| **Funkcja Miro AI** | **Opis** | **Model** |
| --- | --- | --- |
| Generowanie mapy myśli | Generuje mapę myśli z wybranego węzła głównego. | GPT 4o-mini |
| Mapa myśli - rozszerzanie o pomysły | Generuje pomysły z wybranego węzła głównego lub elementu podrzędnego. | GPT 4o-mini |
| Mapa myśli - Rozwijaj z tematami | Generuje tematy z wybranego węzła głównego lub elementu podrzędnego. | GPT 4o-mini |
| Mapa myśli - Rozwijaj z pytaniami | Generuje pytanie z wybranego węzła głównego lub elementu podrzędnego. | GPT 4o-mini |

### Slajdy wspomagane przez AI

Miro Slajdy używają następujących modeli:

- Amazon Titan
- Claude 4 Sonnet
- Claude 3.7 Sonnet
- Claude 3.5 Sonnet
- GPT-5
- GPT-4o
- Stable Diffusion 3.5 Large
- Stability Image Core

### Miro Insights

Aby zsyntetyzować opinie klientów, [Miro Insights](https://help.miro.com/hc/articles/25438311770770) używa GPT-4o.

### Klienci AWS Marketplace

**Modele AWS Marketplace**

| **Funkcja Miro AI** | **Model** |
| --- | --- |
| Podsumowania rozmów | Claude Haiku 3.7 (AWS Bedrock) |
| Tworzenie diagramu – Diagram przepływu | Claude Sonet 3.7 (AWS Bedrock) |
| Edycja diagramu – Diagram przepływu | Claude Sonet 3.7 (AWS Bedrock) |
| Twórz diagram – mapa myśli | Claude Sonnet 3.7 (AWS Bedrock) |
| Edytuj diagram – mapa myśli | Claude Sonnet 3.7 (AWS Bedrock) |
| Twórz diagram – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| Edytuj diagram – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| Utwórz dokument | Claude Sonnet 3.7 (AWS Bedrock) |
| Edytuj dokument | Claude Sonnet 3.7 (AWS Bedrock) |
| Tworzenie karteczek | Claude Sonnet 3.7 (AWS Bedrock) |
| Edycja karteczek | Claude Sonnet 3.7 (AWS Bedrock) |
| Przechwytywanie karteczek | Claude Sonnet 3.7 (AWS Bedrock) + Miro proprietary model |
| Tworzenie obrazu | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Edycja obrazu | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Tekst alternatywny obrazu | Claude Sonnet 3.7 (AWS Bedrock) |
| Utwórz prototyp | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| Edytuj ekran prototypu | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| Konwertuj obraz na prototyp | Claude Sonnet 3.7 + własny model Miro |
| Stwórz tabelę | Claude Sonnet 3.7 (AWS Bedrock) |
| Edytuj tabelę | Claude Sonnet 3.7 (AWS Bedrock) |
| Dygitalizuj diagram | Claude Sonnet 3.7 (AWS Bedrock) |
| Kategoryzacja karteczek według słów kluczowych | Claude Sonnet 3.7 (AWS Bedrock) + autorski model Miro |
| Kategoryzacja karteczek według odczuć | Autorski model Miro |
| Współpracownik AI | Claude Sonnet 3.7 (AWS Bedrock) |
| Edycja tekstu wspomagana AI | Claude Sonnet 3.7 (AWS Bedrock) |
| Mapy myśli wspomagane AI | Claude Sonnet 3.7 (AWS Bedrock) |

## Wybierz swój model

Poniższe listy pokazują, które modele są dostępne w ramach opcji [Wybierz swój model](10-select-your-own-model-beta.md), dostępnej dla [przepływów](04-flows-overview.md) i współpracowników AI.

### Duże modele językowe

**Claude**

- Claude 3.7 Sonnet
- Claude Sonnet 4

**OpenAI**

- GPT-4o
- GPT-4o mini
- OpenAI o4-mini
- GPT-5
- GPT-5 mini
- GPT-4.1
- GPT-4.1 mini

### Modele obrazowe

**Stability AI**

- Stable Image Core
- Stable Image Ultra
- Stable Diffusion 3.5 Large

**Amazon**

- Amazon Titan Generator Obrazów
- Plansza Amazon Nova

**Google**

- Gemini 2.5 Flash Image (Nano Banana)
- Vertex AI Imagegen 3
- Vertex AI Imagegen 3 Fast
- Vertex AI Imagegen 4

## Tokeny na Miro AI i dodatek

Miro przydziela określoną liczbę tokenów na AI do Twojego konta każdego miesiąca. Ilość przydzielonych tokenów zależy od wersji. Przydział resetuje się pierwszego dnia każdego miesiąca kalendarzowego.

Za każdą akcję AI, którą wykonujesz, zużywasz tokeny na AI. Większość akcji AI zużywa jeden (1) token na akcję, jednak niektóre funkcje mogą zużywać więcej.

Aby zwiększyć liczbę przydzielonych tokenów na Miro AI, można opcjonalnie zakupić subskrypcję dodatku na tokeny na Miro AI. Aby dowiedzieć się więcej, zobacz [Tokkeny na Miro AI i dodatek AI](../../plans-billing/billing-and-payments/03-miro-ai-credits.md).

## Prywatność i bezpieczeństwo Miro AI

Od 3 lutego 2025 r. Miro zbiera dane dotyczące interakcji AI od użytkowników w wersji Free, aby udoskonalić funkcje Miro AI, takie jak podsumowania AI, diagramy czy współpracownicy AI.

Aby dowiedzieć się więcej o tym, jak Miro wykorzystuje interakcje AI do ulepszania Miro AI i jak można kontrolować swoje preferencje dotyczące danych, zobacz [Ulepszenia jakości Miro AI](19-miro-ai-quality-improvements.md).
