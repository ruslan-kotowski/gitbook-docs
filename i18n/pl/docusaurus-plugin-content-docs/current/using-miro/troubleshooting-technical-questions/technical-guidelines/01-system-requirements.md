---
title: Wymagania systemowe
article_id: 360017731553
translation_id: 360017731553
locale: pl-pl
sidebar_position: 1
created_at: '2019-02-11T10:14:54Z'
updated_at: '2026-03-06T14:57:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Ten artykuł przedstawia wymagania systemowe dotyczące korzystania z Miro, w tym urządzenie, GPU i WebAssembly.

Aby pracować w Miro, upewnij się, że Twoje urządzenie spełnia poniższe minimalne lub zalecane wymagania systemowe.

Jednak pamiętaj, że wymienione poniżej parametry nie są ostateczne, ponieważ wydajność Miro może być związana z wieloma innymi czynnikami, takimi jak:

- Zadania w tle
- Liczba kart w przeglądarce i jak często się pomiędzy nimi przełączasz
- Rozdzielczość monitora, na którym otwierasz Miro
- Stabilność połączenia Wi-Fi
- Liczba użytkowników na tablicy
- System chłodzenia urządzenia

Jeśli doświadczasz problemów z wydajnością/dostępem, sprawdź [przewodniki dotyczące rozwiązywania problemów](../troubleshooting) oraz [wskazówki dotyczące optymalizacji wydajności tablicy](../../tools/troubleshooting/04-board-performance-and-loading-issues.md).

|  |  |  |
| --- | --- | --- |
|  | **Minimalne** | **Zalecane** |
| **Procesor (CPU)** | 3 GHz (2 rdzenie/4 wątki) | 2,8 GHz (4 rdzenie/8 wątków) |
| **Pamięć RAM** | 8 GB | 16 GB (DDR4) |
| **Przepustowość sieci** | 8 Mb/s | 32 Mb/s |

**Proszę zauważyć, że uruchomienie Miro na wysokowydajnym sprzęcie, który znacznie przewyższa zalecane specyfikacje, może nie przynieść oczekiwanego wzrostu wydajności, ponieważ Miro to aplikacja internetowa działająca z wykorzystaniem silnika przeglądarki. Silnik przeglądarki nie jest w stanie w pełni wykorzystać możliwości urządzenia tak jak oprogramowanie zainstalowane lokalnie na komputerze, zaprojektowane pod konkretny system operacyjny i architekturę procesora CPU.*

Minimalne wymagania systemowe dla komfortowego korzystania z Miro na [tabletach](../../../getting-started/apps-for-devices/11-tablet-app.md) to 6 GB RAM.

Miro można używać na różnych typach urządzeń. Możesz otworzyć Miro w przeglądarce, pobrać [aplikację komputerową](../../../getting-started/apps-for-devices/05-desktop-app.md), [tabletową](../../../getting-started/apps-for-devices/11-tablet-app.md), [mobilną](../../../getting-started/apps-for-devices/08-mobile-app.md) lub [używać Miro na wyświetlaczu interaktywnym](../../../getting-started/apps-for-devices/07-interactive-displays.md).

**Tryb offline**

Ponieważ Miro opiera się na wizji bezproblemowego rozwiązania chmurowego do *online* współpracy, *offline* tryb narzędzia nie jest obecnie na naszym radarze. Jednakże udostępniamy kilka opcji eksportu. [Dowiedz się więcej](../../import-and-export/export/03-how-to-export-your-board.md).

## Wymagania dotyczące GPU i WebAssembly

Miro wykorzystuje przyspieszenie sprzętowe GPU i WebAssembly (WASM) do płynnego renderowania i obsługi niektórych zaawansowanych funkcji.

### Korzystanie z Miro bez GPU

Dla optymalnej wydajności Miro wymaga przyspieszenia sprzętowego GPU.

Jeśli brak jest przyspieszenia sprzętowego GPU, na przykład na niektórych maszynach wirtualnych lub gdy przyspieszenie sprzętowe jest wyłączone, Miro automatycznie przełącza się na renderowanie oparte na CPU.

:::tip
Dla najlepszych wrażeń w Miro, utrzymuj włączoną akcelerację sprzętową, kiedy to możliwe.
:::

Bez sprzętowej akceleracji GPU możesz doświadczyć następujących zmian w wydajności:

- Niektóre funkcje zależne od GPU mogą być niedostępne lub wyświetlane jako symbole zastępcze
- Wolniejsze przesuwanie i powiększanie, zwłaszcza w przypadku dużych tablic lub tablic z dużą ilością mediów
- Podstawowa funkcjonalność tablicy może nie działać zgodnie z oczekiwaniami
- Wyższe zużycie CPU

### Korzystanie z Miro bez WebAssembly (WASM)

Niektóre funkcje Miro polegają na modułach WebAssembly (WASM).

Większość nowoczesnych przeglądarek domyślnie włącza WASM. Jeśli WASM jest niedostępny, na przykład zablokowany zgodnie z zasadami przedsiębiorstwa, wyłączony w przeglądarce lub niewspierany w starszych środowiskach, Miro automatycznie przełącza się na ścieżki renderowania oparte na JavaScript, gdzie to możliwe.

**Więcej informacji:** Zobacz [Jak sprawdzić, czy WASM jest wspierany w twojej przeglądarce](https://help.miro.com/hc/articles/33769132852498).

:::tip
Aby zapewnić najlepsze wrażenia z korzystania z Miro, utrzymuj WebAssembly włączone. W zarządzanym środowisku, jeśli podejrzewasz, że WASM jest zablokowany, skontaktuj się z zespołem IT.
:::

Bez WASM mogą wystąpić następujące zmiany wydajności:

- Funkcje wymagające WASM mogą się nie inicjować, a zamiast nich mogą być wyświetlane jako ukryte lub w formie zastępczych elementów wizualnych
- Tablice zależne od funkcjonalności bazującej na WASM mogą się nie załadować w pełni lub wcale
