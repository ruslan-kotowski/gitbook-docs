---
title: "Prompt-Blockierung im \xDCberblick (Beta)"
article_id: 29332642230546
translation_id: 29332642230546
locale: de
sidebar_position: 4
created_at: '2025-09-09T07:58:00Z'
updated_at: '2026-01-12T11:23:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Prompt blocking ermöglicht es Admins für sensible Inhalte, zu verhindern, dass Nutzer AI-Prompts einreichen, die sensible Informationen enthalten. So kannst du sicherstellen, dass sensible Daten in deiner Organisation nicht in Miro AI gelangen. Miro scannt den Text, den ein Nutzer im Prompt-Feld eingibt, und jegliche textbasierte Inhalte, die er von dem Board hinzufügt. Falls dieser Inhalt mit den in der Prompt-blocking-Konfiguration ausgewählten Sensibilitätslabels oder Quellcode-Mustern übereinstimmt, blockiert Miro die Prompt-Einreichung.

:::note
Nur textbasierte Inhalte werden in der Beta-Version unterstützt.
:::

## So funktioniert‘s

- Du wählst aus, welche Label-Kategorien auf Orgebene blockiert werden sollen. Änderungen werden sofort für alle in deiner Organisation wirksam.
- Wenn sensible Daten in einem Prompt erkannt werden, zeigt Miro AI eine Richtliniennachricht im Einstiegspunkt des Nutzers an, der Prompt wird blockiert und kann nicht an Miro AI gesendet werden.
- Prompt-Blocking und die Board-Überprüfung sind unterschiedlich. Die Board-Überprüfung lokalisiert sensible Inhalte auf Boards und kann das Board automatisch klassifizieren. Das Prompt-Blocking überprüft, was Nutzer an Miro AI senden möchten.

## Was blockiert wird

- Datenschutzbezogene Labels: Wählen Sie aus all unseren integrierten Datenschutzlabels, wie SPII, HIPAA, Anmeldeinformationen, Finanzkennzahlen. Für weitere Informationen zu unseren integrierten Datenschutzlabels siehe [Sensitivity labels and infotypes reference](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md).
- Scannen von Code. Wenn aktiviert, blockiert Miro Prompts, die erkannten Quellcode enthalten. Siehe [Scannen von Code](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md) für weitere Details.

## Typische Ergebnisse für Nutzer

Wenn der Nutzer einen Prompt eingibt, der gemäß Ihrer Konfiguration sensible Informationen enthält:

- Nutzer sehen eine Nachricht wie: Wir können diesen Inhalt nicht erstellen, da er gegen die Richtlinien Ihrer Organisation verstoßen könnte.
- Der Prompt wird nicht an Miro AI gesendet. Nutzer können den Prompt bearbeiten und es erneut versuchen.

## Scannen von Code

Das Scannen von Code blockiert AI-Prompts, die erkennbaren Quellcode enthalten. Dafür sind mindestens 5 Codezeilen erforderlich, um die Blockierung auszulösen.

Beispiel:

```
function connect() {

  const token = "example-token";

  fetch("https://api.example.com/health");

  return true;

}
```

## Unterstützte Sprachen

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
- Shell-Skript
- SQL
- TypeScript
