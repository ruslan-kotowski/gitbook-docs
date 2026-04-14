---
title: "Vis\xE3o geral do bloqueio de prompt (Beta)"
article_id: 29332642230546
translation_id: 29332642230546
locale: pt-br
sidebar_position: 4
created_at: '2025-09-09T07:58:00Z'
updated_at: '2026-01-12T11:23:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Prompt blocking permite que os Admins de Conteúdo Sensível impeçam usuários de enviar prompts para a IA que incluam informações confidenciais, ajudando a manter dados confidenciais fora do Miro AI em sua organização. O Miro analisa o texto que um usuário insere no campo de prompt e qualquer conteúdo baseado em texto que eles adicionem no board. Se esse conteúdo corresponder aos rótulos de sensibilidade ou padrões de código-fonte selecionados na configuração do Prompt blocking, o Miro bloqueia o envio do prompt.

:::note
Apenas conteúdo baseado em texto é suportado na versão Beta.
:::

## Como funciona

- Você escolhe quais categorias de etiquetas bloquear no nível da organização. As alterações entram em vigor imediatamente para toda a sua organização.
- Quando dados confidenciais são detectados em um prompt, a Miro AI mostra uma mensagem de política no ponto de entrada do usuário, o prompt é bloqueado e não pode ser enviado para a Miro AI.
- O bloqueio de prompts e a varredura de boards são diferentes. A varredura de boards localiza conteúdos confidenciais nos boards e pode classificar automaticamente o board. O bloqueio de prompts revisa o que os usuários tentam enviar para a Miro AI.

## O que é bloqueado

- Etiquetas relacionadas à privacidade: Selecione entre todas as nossas etiquetas de privacidade embutidas, como SPII, HIPAA, credenciais, números financeiros. Para mais informações sobre nossas etiquetas de privacidade embutidas, consulte [Referência de etiquetas de sensibilidade e infotypes](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md).
- Varredura de código. Quando ativada, a Miro bloqueia prompts que incluem códigos fonte reconhecidos. Veja [Varredura de código](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md) para mais detalhes.

## Resultados típicos para usuários

Quando o usuário insere um prompt que contém informações sensíveis de acordo com a sua configuração:

- Os usuários veem uma mensagem como "Não podemos gerar este conteúdo, pois ele pode violar a política da sua organização."
- O prompt não é enviado para o Miro AI. Os usuários podem editar o prompt e tentar novamente.

## Varredura de código

A varredura de código bloqueia prompts de IA que incluam código fonte reconhecível. É necessário um mínimo de 5 linhas de código para acionar o bloqueio.

Exemplo:

```
function connect() {

  const token = "example-token";

  fetch("https://api.example.com/health");

  return true;

}
```

## Idiomas disponíveis

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
- Shell script
- SQL
- TypeScript
