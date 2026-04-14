---
title: Jak sprawdzić, czy WASM jest obsługiwany w Twojej przeglądarce
article_id: 33769132852498
translation_id: 33769132852498
locale: pl-pl
sidebar_position: 3
created_at: '2026-03-04T12:47:24Z'
updated_at: '2026-03-16T13:02:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Kto może to zrobić: Wszyscy użytkownicy Jakie abonamenty: Free, Starter,
    Business, Enterprise, Education Na jakich platformach: Przeglądarka'
---

WebAssembly (WASM) może być wyłączone z powodów, takich jak zgodność z polityką bezpieczeństwa ustanowioną przez Twoją organizację, lub braku wsparcia w starszych środowiskach, na przykład.

> **Wskazówka:** [Tabela porównawcza WebAssembly](https://webassembly.org/features/?categories=browsers) pokazuje, które funkcje WASM są obsługiwane w Twojej przeglądarce.

Możesz sprawdzić, czy Twoja przeglądarka obsługuje WASM.

Postępuj zgodnie z tymi krokami:

1. Otwórz Narzędzia dla programistów.
   - W swojej przeglądarce:
     - (MacOS) Chrome, Edge, Firefox: `⌘ + ⌥ + I`
     - (Linux, Windows) Chrome, Edge, Firefox: `Ctrl + Shift + I`, lub `F12`
     - (MacOS) Safari: Przejdź do **Ustawienia** > **Zaawansowane**. Włącz **Pokaż menu Rozwój w menu głównym** | **Pokaż funkcje dla programistów internetowych**. Otwórz **Rozwój** > **Pokaż konsolę JavaScript**.
   - W aplikacji komputerowej Miro:
     - W lewym górnym rogu kliknij **Pomoc** > **Otwórz narzędzia deweloperskie**.
2. W narzędziach deweloperskich kliknij kartę **Konsola**.
3. W wierszu wejściowym konsoli wpisz lub wklej `typeof WebAssembly`.
4. Na klawiaturze naciśnij **ENTER**.
5. Interpretuj wynik:
   - Jeśli konsola zwróci `undefined`, oznacza to, że WebAssembly nie jest obsługiwany lub został wyłączony.
   - Jeśli konsola zwróci `object`, oznacza to, że WebAssembly jest obsługiwane.![](../../../../../../../docs/using-miro/troubleshooting-technical-questions/technical-guidelines/images/33770259460626_image.png)
     *Konsola DevTools pokazuje* `object`*, gdy WASM jest dostępne w Twojej przeglądarce.*

     > **UWAGA:** Jeśli konsola zwróci `object`, a mimo to nie możesz uzyskać dostępu do Miro, możesz sprawdzić inne [możliwe problemy i porady dotyczące rozwiązywania problemów](../troubleshooting), lub skontaktować się z [Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).
