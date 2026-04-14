---
title: Selecione seu Próprio Modelo (Beta)
article_id: 29484232754578
translation_id: 29484232754578
locale: pt-br
sidebar_position: 10
created_at: '2025-09-15T12:50:30Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-sidekicks
availability:
  notes: 'Quem pode fazer: Membros do time Quais planos: Free, Starter, Business,
    Enterprise Quais plataformas: Navegador, Desktop, Mobile'
---

Ao realizar ações de IA com os [fluxos](04-flows-overview.md) e Assistente de IA da Miro, a opção "Selecione seu próprio modelo" permite especificar o modelo de linguagem de grande porte (LLM) mais apropriado para a tarefa.

Por exemplo, para geração de imagem, você pode decidir entre usar Stable Diffusion 3.5 Large ou Gemini 2.5 Flash Image (Nano Banana).

Sua escolha pode depender da complexidade ou especificidade da sua tarefa.

:::tip
Os Miro Flows e Assistentes de IA incluem um LLM padrão pré-selecionado para cada tarefa. Quando você não tem certeza de qual modelo escolher, utilizar o modelo padrão é o melhor início. O modelo padrão é exibido com uma etiqueta "Recomendado".
:::

O seletor de modelo está disponível apenas como parte dos Flows e Assistentes de IA nas seguintes situações:

- Documentos e formatos de imagem nos Assistentes de IA e Flows
- Lógica principal dos Assistentes de IA
- Bloco de instrução nos Flows

Este artigo explica como selecionar seu próprio modelo para os Flows e Assistentes de IA, além de fornecer informações para ajudá-lo a escolher um LLM para tarefas comuns.

## Selecionando seu próprio modelo

### Fluxos

Docs, imagens e Blocos de Instrução em um Fluxo, cada um possui uma caixa de prompt onde você pode selecionar seu próprio modelo.

Siga estes passos:

1. Adicione um Doc, imagem ou Bloco de Instrução ao canvas.
2. Para acessar a lista de modelos disponíveis, no canto superior direito da caixa de prompt, clique no nome do modelo padrão. Por exemplo, `AWS | Claude 3.5`.
3. Selecione um modelo.

Para saber mais sobre a criação de Fluxos e a experiência de usuário dos Fluxos, veja [Fluxos](05-flows.md).

### Assistentes de IA

Ao criar ou editar os Assistentes de IA, você verá a seção **Modelo (avançado)**, e poderá escolher qual modelo deseja usar para o processamento do Assistente de IA, geração de imagens e geração de documentos.

Para saber mais sobre os Assistentes de IA, consulte a [documentação do Assistente de IA](08-ai-sidekicks.md).

## Como os modelos diferem

Um grande modelo de linguagem (LLM) geralmente faz parte de uma família de modelos que inclui modelos capazes, mas com alta demanda de recursos, modelos ideais, e os modelos mais rápidos, porém menos capazes.

Por exemplo, a família GPT-5 inclui GPT-5, GPT-5-mini e GPT-5-nano.

Os modelos mais rápidos, mas menos capazes, são ideais para menor latência.

### Modelos de raciocínio e não raciocínio

Um principal diferencial entre LLMs é entre modelos de raciocínio e de não-raciocínio.

*Raciocínio* significa que o modelo leva mais tempo para fornecer uma resposta de maior qualidade.

:::note
*Raciocínio* nem sempre significa o resultado mais preciso. Se você precisar de muitas iterações de resultados, alta capacidade de raciocínio pode não ser a opção mais eficiente.
:::

Para tarefas complexas, como criação de documentos para clientes, priorização e tarefas que requerem processamento de um grande volume de informações, um modelo de raciocínio é a melhor escolha.

Para tarefas simples, como verificação de gramática, tradução ou reformatação de texto, um modelo de não-raciocínio é a escolha mais eficiente.

A tabela a seguir mostra alguns modelos de raciocínio e de não-raciocínio.

| Funcionalidade de raciocínio | Modelos |
| --- | --- |
| Raciocínio | GPT-5, GPT-5-mini, GPT-5-nano, Claude Sonnet 4, Claude Sonnet 4.5, Gemini 2.5, Gemini 2.5 Flash, o3, o4-mini |
| Sem raciocínio | GPT 4o, GPT-4o-mini, GPT-4.1, GPT-4.1-mini, Claude Sonnet 3.7, Claude Sonnet 3.5, Gemini 2.5 Flash Lite |

### Estilo

Cada LLM tem um "estilo" único. Ao experimentar diferentes modelos, você pode perceber que um determinado estilo de saída atende aos seus requisitos, seja em termos de marca, vibração ou preferência.

:::tip
Modelos mais antigos possuem um estilo mais distinto, especialmente para resultados criativos e inovadores.
:::

## Selecionando seu modelo de IA por tarefa

| Tarefa | Modelos | Descrição |
| --- | --- | --- |
| Brainstorming | GPT-4o, o3, o4-mini, Sonnet 3.7 | Ótimo para pensamento divergente, explosão de ideias para funcionalidades, tom lúdico e "toque criativo". Use para gerar texto, como manchetes alternativas e variantes de microtexto, por exemplo. |
| Priorização e pontuação | GPT-5, Claude Sonnet 4.5, Gemini 2.5 | Os melhores modelos de raciocínio para pontuação consistente e justificativas claras. Por exemplo, RICE/MoSCoW em backlog, análises de trade-off e níveis de roadmap. |
| Síntese e pesquisa | GPT-5, GPT-5-mini, Claude Sonnet 4.5, GPT-4.1, Claude Sonnet 3.7, Gemini 2.5 Flash | Use para tarefas de média a alta complexidade. Por exemplo, gerar personas a partir de notas e obter insights de dados e bases de conhecimento. |
| Esquema e transformação | GPT-5-mini, GPT-5-nano, GPT-4.1, Sonnet 3.7, Gemini 2.5 Flash, Gemini 2.5 Flash Lite | Mudança de formato geralmente não requer raciocínio complexo, então versões otimizadas darão resultados mais rápidos, mas mantenha-se às famílias de modelos mais recentes para garantir consistência ao lidar com grandes contextos. notas → documentos, documento → tabela, especificação → diagrama) |
| Edições rápidas de texto | GPT-4o-mini, Gemini 2.5 Flash Lite, GPT-5-nano, Claude 3.7 | Opções mais rápidas. Melhor para edições simples de texto, como gramática, tradução e reescritas para clareza. |

## Selecionando modelos para geração de imagens

Todos os modelos de linguagem ampla (LLM) que a Miro suporta podem processar texto e imagens. No entanto, a maioria não consegue gerar imagens.

Para a geração de imagens, o Gemini 2.5 Flash Image (Nano Banana) é excepcionalmente hábil em converter suas instruções gerais em uma imagem.

A maioria dos LLMs espera uma descrição da imagem e não instruções específicas. Por exemplo, "uma pintura de um cachorro com um chapéu engraçado" como descrição, em vez de "criar uma imagem engraçada de um cachorro" como instrução. O Nano Banana é capaz de gerar imagens com base em instruções específicas.

:::note
Use o Nano Banana para edições direcionadas em uma imagem existente. Outros modelos podem usar uma imagem existente como referência de estilo.
:::

Em termos de velocidade ou qualidade de saída, há pouca diferença entre os LLMs. Assim como em cada caso de uso, você pode experimentar diferentes modelos para encontrar o que melhor se adequa às suas preferências.
