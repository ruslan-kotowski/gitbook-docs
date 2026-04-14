---
title: "Definir ou atualizar o n\xEDvel de modera\xE7\xE3o do Miro AI (Beta)"
article_id: 30613174297618
translation_id: 30613174297618
locale: pt-br
sidebar_position: 3
created_at: '2025-10-29T01:15:35Z'
updated_at: '2026-01-12T11:22:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Com a moderação do Miro AI, os Admins da empresa podem ajustar os níveis de filtro de prompts que poderiam resultar em saídas potencialmente prejudiciais ou inadequadas. Você pode controlar a sensibilidade da moderação do Miro AI em toda a sua organização e filtrar categorias como ódio, conteúdo sexual, violência e automutilação. Isso ajuda a alinhar o uso do Miro AI com os requisitos, políticas e tolerância ao risco da sua organização.

**Nota**: Se a sua organização conecta seu próprio fornecedor de LLM (por exemplo, uma integração direta com OpenAI), o seletor de moderação é desabilitado e qualquer nível escolhido anteriormente é ignorado para essa integração.

## Pré-requisitos

- Certifique-se de ter o complemento Enterprise Guard.
- Certifique-se de que você é um **Admin da empresa** para a organização que deseja configurar.
- Revise seus requisitos de governança e política para escolher um nível inicial apropriado. O padrão é recomendado para a maioria das organizações.

## Defina ou atualize o nível de moderação da Miro AI

1. Abra as **Configurações** da sua organização na Miro.
2. Vá para **Miro AI** › **Moderação**.
3. Escolha um nível:
   - **Rigoroso:** Bloqueia tudo no padrão mais conteúdos de risco baixo a moderado (por exemplo, ódio sutil ou codificado, conteúdo sexualmente sugestivo, violência não gráfica, menções não explícitas de autolesão).
   - **Padrão (recomendado):** Bloqueia conteúdos moderadamente a severamente prejudiciais (por exemplo, ódio explícito, conteúdo sexual explícito, violência gráfica, incentivo à autolesão).
   - **Mínimo:** Bloqueia apenas conteúdos severamente prejudiciais.
4. Clique em **Confirmar**.
   A alteração se aplica imediatamente a todos na organização e é registrada no log de auditoria.

## Validar o nível de moderação (opcional)

- Peça a um grupo piloto para testar prompts típicos e relatar qualquer filtragem excessiva ou insuficiente.
- Monitore os canais de suporte ou escalonamento para falsos positivos ou omissões de danos durante a primeira semana após uma alteração.

## Dicas e melhores práticas

- Comece com **Padrão**, depois ajuste com base no feedback do piloto e nas revisões de escalonamento.
- Se os usuários relatarem prompts bloqueados em excesso, tente **Padrão** (de Rigoroso) ou **Mínimo** (de Padrão) e publique exemplos de prompts aceitáveis.
- Se conteúdos de limite passarem, mude para **Rigoroso** e adicione orientações internas para reduzir fricções.
- Revise o nível após mudanças de políticas, regulamentações ou casos de uso.

## Solução de problemas

**O controle de moderação está desabilitado**
Uma integração de LLM customizada está conectada. Desconecte-a para reabilitar o seletor. Enquanto estiver conectada, qualquer nível escolhido anteriormente será ignorado para essa integração.

**Muitos falsos positivos**
Considere alterar de **Estrito → Padrão** e compartilhe exemplos de uso aceitável. Revise as mudanças recentes no log de auditoria para confirmar o momento.

**Exposição a conteúdo nocivo**
Certifique-se de que o nível não esteja em **Mínimo**. Considere **Padrão** ou **Estrito** dependendo da sua tolerância ao risco.

**Usuários não sabem por que os prompts são bloqueados**
Publique orientações internas apontando para o nível escolhido, exemplos de prompts e caminhos de escalonamento.
