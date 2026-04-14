---
title: "Vis\xE3o geral da modera\xE7\xE3o com IA (Beta)"
article_id: 29491049430674
translation_id: 29491049430674
locale: pt-br
sidebar_position: 2
created_at: '2025-09-15T16:27:59Z'
updated_at: '2026-01-12T11:21:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Com a moderação do Miro AI, os Admins da empresa podem ajustar níveis de filtro para prompts que possam conter texto potencialmente prejudicial ou impróprio. Você pode definir a sensibilidade da moderação do Miro AI em toda a organização para filtrar conteúdo como ódio, conteúdo sexual, violência e autoagressão. Isso ajuda a alinhar o uso do Miro AI com os requisitos, políticas e tolerância ao risco da sua organização.

:::note
*Se a sua organização conectar seu próprio provedor de LLM (por exemplo, uma integração direta com OpenAI), o seletor de moderação será desabilitado e qualquer nível escolhido anteriormente será ignorado para essa integração.*
:::

## Níveis de moderação

Controle o conteúdo do Miro AI em toda a sua organização com a moderação do Miro AI. Defina o nível de filtro para Estrito, Padrão ou Mínimo para determinar quais prompts são bloqueados. Consulte a tabela abaixo para comparar rapidamente os níveis e, em seguida, mergulhe nas seções detalhadas para mais orientações.

| Nível | O que faz | Melhor para | Compromissos |
| --- | --- | --- | --- |
| Rigoroso | Bloqueia o nível Padrão + conteúdo de risco baixo a moderado. | Organizações altamente regulamentadas, educação. | Mais falsos positivos; potencial de sobre-filtragem. |
| Padrão (recomendado) | Bloqueia conteúdo moderadamente a altamente prejudicial. | Maioria dos casos de uso empresarial. | Algum conteúdo limítrofe pode passar. |
| Mínimo | Bloqueia apenas conteúdo gravemente prejudicial. | Contextos criativos/jogos/mídia. | Mais exposição a danos de baixo a moderado. |

:::note
*O padrão é recomendado para a maioria das organizações. Ele filtra o conteúdo que a maioria considera inapropriado ou prejudicial, mantendo uma boa usabilidade.*
:::

## Nível restrito

### O que ele filtra

Tudo no nível Padrão mais conteúdos de risco baixo a moderado (por exemplo, discurso de ódio sutil ou codificado, conteúdo sexualmente sugestivo, violência não gráfica ou menções não explícitas de autoagressão).

### Quando usar

- Indústrias reguladas ou políticas organizacionais avessas ao risco
- Programas focados em educação ou juventude
- Pilotos com baixa tolerância ao risco

### Compromissos

- Mais falsos positivos e bloqueio de prompts de fronteira
- Requer orientação para reduzir fricção do usuário

## Nível Padrão (recomendado)

### O que filtra

Conteúdo de moderado a severamente prejudicial (discurso de ódio explícito, conteúdo sexual explícito, violência gráfica, incentivo ao autoaumentação).

### Quando usar

- A maioria das organizações que buscam equilibrar segurança/usabilidade

### Compromissos

- Prompts contextuais ou limítrofes podem passar

## Nível mínimo

### O que filtra

Apenas conteúdo severamente prejudicial.

### Quando usar

- Times criativos que precisam de maior expressão (jogos, mídia)
- Ideação interna com caminhos claros de escalonamento

### Compromissos

- Maior exposição a conteúdo prejudicial de baixo a moderado nos resultados

## Auditoria e conformidade

As alterações no nível de moderação são registradas no log de auditoria da organização, incluindo o valor anterior, o novo valor, quem o alterou e quando foi alterado. Para mais informações, consulte nossa documentação sobre [Log de Auditoria](../security-management/01-audit-logs.md).

## Práticas recomendadas

- Comece com o padrão, depois ajuste com base no feedback do piloto e nas avaliações de escalonamento.
- Combine o rígido com uma orientação interna clara sobre prompts aceitáveis para reduzir falsos positivos.
- Se você precisar do mínimo, defina quando os times devem escalonar ou relatar saídas problemáticas.
- Revise sua configuração após grandes atualizações de políticas ou regulamentações.

- Visão geral da moderação com IA
- Níveis de moderação
- Nível restrito
- Nível padrão (recomendado)
- Nível mínimo
- Auditoria e conformidade
- Práticas recomendadas
