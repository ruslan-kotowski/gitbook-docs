---
title: Referência da Miro AI
article_id: 20970362792210
translation_id: 20970362792210
locale: pt-br
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
  notes: 'Quem pode fazer: Todos os usuários Quais planos: Free, Starter, Business,
    Enterprise, Education Em quais plataformas: Navegador, Desktop, Mobile'
---

Este artigo de referência descreve a funcionalidade do Miro AI.

## Modelos de IA da Miro

Os modelos são geralmente hospedados na infraestrutura do provedor, ou no serviço Azure AI da Microsoft ou no AWS Bedrock. Para clientes que adquirem o Miro através do AWS Marketplace, todos os modelos são hospedados no AWS Bedrock.

### Criação e iteração impulsionada por IA

| **Funcionalidade da Miro AI** | **Descrição** | **Modelo** |
| --- | --- | --- |
| Resumos de conversas | Gera um resumo de longas conversas no seu board da Miro. | GPT 4o-mini |
| Criar diagrama - Fluxograma | Cria um fluxograma a partir de um prompt do usuário e do conteúdo selecionado do board. | GPT-4o |
| Editar diagrama - Fluxograma | Edita um fluxograma a partir de um prompt do usuário e do conteúdo selecionado do board. | GPT-4o |
| Criar diagrama - Mapa mental | Cria um mapa mental a partir de um prompt do usuário e do conteúdo selecionado do board. | GPT 4o-mini |
| Editar diagrama - Mapa mental | Edita um mapa mental a partir de um prompt do usuário e conteúdo do board selecionado. | GPT-4o |
| Criar diagrama - ERD | Cria um diagrama de entidades e relacionamentos (ERD) a partir de um prompt do usuário. Uma opção de **Criar com IA**. | GPT 4o-mini |
| Editar diagrama - ERD | Edita um ERD a partir de um prompt do usuário e do conteúdo selecionado do board. | GPT-4o |
| Digitalizar diagrama | Transforma imagens de diagramas desenhados à mão em diagramas totalmente editáveis na Miro. | Claude 3.7 Sonnet (AWS Bedrock) |
| Criar Documento | Cria um Miro Doc a partir de um prompt do usuário e do conteúdo selecionado do board. Uma opção **Criar com IA**. | GPT-4o |
| Editar Documento | Edita um Miro Doc a partir de um prompt do usuário e do conteúdo selecionado do board. | GPT-4o |
| Criar imagem | Cria uma imagem a partir de um prompt do usuário, incluindo objetos do board para contexto. Uma opção **Criar com IA** . | Segmind Stable Diffusion 1B (SSD-1B) + StabilityAI Diffusion XL Refiner 1.0 |
| Editar imagem | Edita uma imagem a partir de um prompt do usuário, incluindo objetos do board para contexto. Uma opção **Criar com IA**. | GPT-4o |
| Converter imagem em Protótipo | Converte uma imagem de esboço ou protótipo em um Protótipo Miro editável. | Modelo proprietário da Miro + Claude 3.7 Sonnet |
| Texto alternativo da imagem | Gera texto alternativo para uma imagem. Não consome crédito de IA. | Modelo proprietário da Miro |
| Criar notas adesivas | Cria notas adesivas da Miro a partir de um prompt do usuário e do conteúdo selecionado do board. | GPT-4o |
| Editar notas adesivas | Edita notas adesivas da Miro de um board do usuário e do conteúdo selecionado do board. | GPT-4o |
| Captura de notas adesivas | Converte uma imagem de notas adesivas físicas em notas adesivas da Miro. | Modelo proprietário da Miro |
| Criar protótipo | Cria um protótipo Miro a partir de um prompt do usuário e conteúdo do board selecionado. | GPT-4o + Claude 4.5 Sonnet + GPT 4o-mini + Gemini 2.5 Flash Image (nano-banana) |
| Editar tela do protótipo | Edita uma tela do protótipo Miro a partir de um prompt do usuário e conteúdo do board selecionado. | Claude 4.5 Sonnet + Gemini 2.5 Flash Image (nano-banana) |
| Remover fundo | Remove o fundo de uma imagem. | Modelo proprietário da Miro |
| Desenhos inteligentes | Converte um desenho a lápis em uma linha, forma ou nota adesiva. | Modelo proprietário da Miro |
| Criar Tabela | Cria uma Tabela Miro a partir de um prompt de usuário e do conteúdo selecionado do board. | Claude 3.7 Soneto |
| Editar Tabela | Edita uma Tabela Miro a partir de um prompt de usuário e do conteúdo selecionado do board. | Claude 3.7 Soneto |

### Assistentes de IA

|  |  |  |
| --- | --- | --- |
| **Funcionalidade da Miro AI** | **Descrição** | **Modelo** |
| Assistentes de IA: Agile Coach | Identifica os principais temas em uma retrospectiva e sugere as próximas etapas. | GPT-4o |
| Assistente de IA - Líder de Produto | Fornece feedback e sugestões como comentários em quadros, notas adesivas ou texto. Também fornece ideias de soluções como notas adesivas. | GPT-4o |
| Assistente de IA - Aliança de Marketing de Produto | Fornece feedback e sugestões como comentários em quadros, notas adesivas ou texto. | GPT-4o |

### Agrupamento otimizado pela IA

| **Funcionalidade da Miro AI** | **Descrição** | **Modelo** |
| --- | --- | --- |
| Agrupamento de notas adesivas por palavras-chave | Agrupa notas adesivas por palavras-chave, atribuindo um título a cada grupo. | Claude 3.5 Haiku + Amazon Nova Micro |
| Agrupamento de notas adesivas por sentimento | Agrupa notas adesivas por sentimento, como opiniões e pontos de vista, em grupos positivos, neutros e negativos. | Claude 3.5 Haiku |

### Edição de texto otimizada pela IA

A tabela a seguir mostra a edição de texto otimizada pela Miro AI:

|  |  |  |
| --- | --- | --- |
| **Funcionalidade da Miro AI** | **Descrição** | **Modelo** |
| Alterar o tom | Modifica o tom do texto selecionado para transmitir uma mensagem amigável, profissional, empresarial ou divertida. | GPT-5 nano |
| Corrigir gramática e ortografia | Corrige a gramática e a ortografia do texto selecionado. | GPT-5 |
| Reescrever para dar clareza | Reescreve o texto selecionado para mais clareza. | GPT-5 Chat |
| Encurtar texto | Reformula o texto selecionado em uma versão mais curta sem perder a clareza e a legibilidade. | GPT-5 mini |
| Traduzir | Traduz o texto selecionado para inglês, espanhol, alemão, francês, japonês, português, coreano, polonês, italiano, turco, árabe, russo, dinamarquês, finlandês, norueguês, holandês, sueco ou tailandês. É possível traduzir um ou vários objetos ao mesmo tempo. | GPT-5 mini |

### Mapas mentais desenvolvidos com IA

| **Funcionalidade da Miro AI** | **Descrição** | **Modelo** |
| --- | --- | --- |
| Gerar mapa mental | Gera um mapa mental a partir de um nó central selecionado. | GPT 4o-mini |
| Mapa mental - Expandir com ideias | Gera ideias a partir de um nó central ou nó filho selecionado. | GPT 4o-mini |
| Mapa mental - Expandir com tópicos | Gera tópicos a partir de um nó central ou nó filho selecionado. | GPT 4o-mini |
| Mapa mental - Expandir com perguntas | Gera uma pergunta a partir de um nó central ou nó filho selecionado. | GPT 4o-mini |

### Slides com tecnologia IA

Os Slides do Miro utilizam os seguintes modelos:

- Amazon Titan
- Claude 4 Soneto
- Claude 3.7 Soneto
- Claude 3.5 Soneto
- GPT-5
- GPT-4o
- Stable Diffusion 3.5 Large
- Stability Image Core

### Miro Insights

Para sintetizar feedbacks de clientes, o [Miro Insights](https://help.miro.com/hc/articles/25438311770770) utiliza GPT-4o.

### Clientes do AWS Marketplace

**Modelos do AWS Marketplace**

| **Funcionalidade da Miro AI** | **Modelo** |
| --- | --- |
| Resumos de conversas | Claude Haiku 3.7 (AWS Bedrock) |
| Criar diagrama – Fluxograma | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar diagrama – Fluxograma | Claude Sonnet 3.7 (AWS Bedrock) |
| Criar diagrama – Mapa mental | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar diagrama – Mapa mental | Claude Sonnet 3.7 (AWS Bedrock) |
| Criar diagrama – Diagrama ER | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar diagrama – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| Criar documento | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar documento | Claude Sonnet 3.7 (AWS Bedrock) |
| Criar notas adesivas | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar notas adesivas | Claude Sonnet 3.7 (AWS Bedrock) |
| Captura de notas adesivas | Claude Sonnet 3.7 (AWS Bedrock) + modelo proprietário da Miro |
| Criar imagem | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Editar imagem | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Texto alternativo da imagem | Claude Sonnet 3.7 (AWS Bedrock) |
| Criar protótipo | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| Editar tela do protótipo | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| Converter imagem em protótipo | Claude Sonnet 3.7 + modelo proprietário da Miro |
| Criar tabela | Claude Sonnet 3.7 (AWS Bedrock) |
| Editar tabela | Claude Sonnet 3.7 (AWS Bedrock) |
| Digitalizar diagrama | Claude Sonnet 3.7 (AWS Bedrock) |
| Agrupamento de notas adesivas por palavras-chave | Claude Sonnet 3.7 (AWS Bedrock) + modelo proprietário da Miro |
| Agrupamento de notas adesivas por sentimento | Modelo proprietário da Miro |
| Assistentes de IA | Claude Sonnet 3.7 (AWS Bedrock) |
| Edição de texto com IA | Claude Sonnet 3.7 (AWS Bedrock) |
| Mapas mentais com IA | Claude Sonnet 3.7 (AWS Bedrock) |

## Selecione Seu Próprio Modelo

As listas a seguir mostram quais modelos estão disponíveis com [Escolha Seu Próprio Modelo](10-select-your-own-model-beta.md), disponível para [fluxos](04-flows-overview.md) e Assistente de IA.

### Modelos de linguagem ampla

**Claude**

- Claude 3.7 Soneto
- Claude Soneto 4

**OpenAI**

- GPT-4o
- GPT-4o mini
- OpenAI o4-mini
- GPT-5
- GPT-5 mini
- GPT-4.1
- GPT-4.1 mini

### Modelos de imagem

**Stability AI**

- Stable Image Core
- Stable Image Ultra
- Stable Diffusion 3.5 Large

**Amazon**

- Gerador de Imagens Amazon Titan
- Canvas Amazon Nova

**Google**

- Imagem Flash Gemini 2.5 (Nano Banana)
- Vertex AI Imagegen 3
- Vertex AI Imagegen 3 Rápido
- Vertex AI Imagegen 4

## Créditos da Miro AI e complemento

A Miro aloca um número fixo de créditos de IA para sua conta a cada mês. A quantidade de créditos alocados depende do seu plano. Sua alocação é reiniciada no primeiro dia de cada mês do calendário.

Para cada ação de IA que você realiza, você consome créditos de IA. A maioria das ações de IA consome um (1) crédito por ação, no entanto, algumas funcionalidades podem consumir mais.

Para aumentar sua alocação de créditos da Miro AI, você pode optar por adquirir uma assinatura de complemento de crédito da Miro AI. Para saber mais, consulte [Miro AI credits and AI add-on](../../plans-billing/billing-and-payments/03-miro-ai-credits.md).

## Miro AI privacidade e segurança

A partir de 3 de fevereiro de 2025, a Miro coleta dados de interação com IA dos usuários do plano Free para melhorar funcionalidades da Miro AI como resumos de IA, diagramas e Assistente de IA.

Para saber mais sobre como a Miro utiliza as interações de IA para melhorar a Miro AI e como você pode controlar suas preferências de dados, consulte [Melhorias de qualidade da Miro AI](19-miro-ai-quality-improvements.md).
