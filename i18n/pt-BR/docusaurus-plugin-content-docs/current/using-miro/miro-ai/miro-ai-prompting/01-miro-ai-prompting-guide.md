---
title: Guia de prompts da Miro AI
article_id: 30226743358226
translation_id: 30226743358226
locale: pt-br
sidebar_position: 1
created_at: '2025-10-14T17:24:22Z'
updated_at: '2025-11-25T15:54:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Prompts melhores produzem resultados melhores ao trabalhar com qualquer modelo de IA. Prompts mais detalhados geralmente criam saídas mais alinhadas ao que você tem em mente. Prompts mais curtos e menos detalhados dão ao modelo de IA mais liberdade para interpretar o que você deseja, o que pode resultar em saídas surpreendentes.

Este guia de prompts irá ajudá-lo a criar prompts melhores ao trabalhar com as funcionalidades de Miro AI.

## Framework RISEN

O framework RISEN para criação de prompts de IA é uma abordagem estruturada para gerar melhores resultados desde o início. Inclui:

- **Função:** A IA é uma criadora, consultora ou solucionadora de problemas? Está desempenhando algum papel específico no seu time? *Exemplos: "Você é uma designer de produto sênior criando..." ou "Você é um especialista em redação técnica aconselhando..."*
- **Entrada:** Aqui você fornece as informações que a IA precisará para realizar sua tarefa. No Miro, isso pode incluir informações escritas ou contextos do board. Por exemplo, ao criar um protótipo, você poderia incluir as funcionalidades do produto ou quais páginas devem ser incluídas.
- **Passos:** Aqui você diz ao AI o que deseja que ele faça. Embora você possa dar instruções gerais, detalhar exatamente o que você quer que ele faça trará melhores resultados. *Exemplo: “1. Resuma o material fornecido no contexto da board. 2. Crie uma nota adesiva para cada ponto importante do material. 3. Organize as notas adesivas em termos de quais provavelmente terão mais impacto.”*
- **Expectativa:** Se você não especificar o que deseja que o output seja, o AI irá decidir por você, e nem sempre acertará. Seja específico aqui; em vez de dizer “crie um deck de slides”, diga para “criar um deck de slides com doze slides” e, em seguida, defina quais tópicos cada slide deve abordar.
- **Restringir:** Se houver elementos que você *não* deseja incluir no resultado final, especifique isso no final. Por exemplo, você pode criar um protótipo de IA para um processo de checkout online que *não* inclua uma página de iniciar sessão no fluxo.

Ao definir cada um desses parâmetros, a Miro AI saberá exatamente o que você espera de sua saída, criando resultados gerais melhores.

## Adicionando contexto do seu board Miro

Uma das funcionalidades mais poderosas da [Miro AI](../01-miro-ai-overview.md) é a capacidade de adicionar contexto a partir do board atual. Isso permite que você adicione um grande volume de informações de maneiras estruturadas para melhorar a saída da sua IA.

Aqui estão algumas dicas para aproveitar ao máximo o contexto do board:

- **Não selecione tudo no board.** Embora possa parecer mais fácil selecionar tudo como contexto, restringir-se apenas às informações mais relevantes gerará os melhores resultados.
- **Adicione contexto específico da indústria ao board.** Embora o Miro AI seja poderoso, ele também é construído em um modelo de linguagem amplo como a maioria dos outros modelos de IA. Adicionar documentação específica da indústria relevante para o seu prompt ajuda a produzir melhores resultados na primeira tentativa. Isso pode incluir coisas como um glossário de termos da indústria, um exemplo de um resultado específico que você deseja que ele crie, ou outro conhecimento da indústria que alguém de fora provavelmente não saberia.
- **Use o Miro AI para criar contexto.** Se você precisar de algo como um resumo de design de produto baseado em anotações de uma reunião, pode usar o Miro AI para criar isso em um Documento no seu board. Faça as edições necessárias e, em seguida, inclua isso como contexto em vez de incluir notas de reunião dispersas que podem ser confusas.

## Prompts iniciais do Miro AI

Começando na Miro AI? Não tem problema. Criamos prompts iniciais prontos para fluxos de trabalho populares. Basta substituir os espaços reservados entre colchetes (por exemplo, [função], [artefato], [tom]) por seu contexto e depois executar o prompt. Explore nossos prompts iniciais por fluxo de trabalho:

- [Prompts de starter para geração e ideação de conteúdo](02-content-generation-and-ideation-starter-prompts.md)
- [Prompts de starter para análise e organização de conteúdo](03-content-analysis-and-organization-starter-prompts.md)
- [Prompts de starter para otimização de fluxo de trabalho](04-workflow-optimization-starter-prompts.md)

## Dicas de prompts específicas para funcionalidades

A Miro AI oferece Assistentes de IA gerais e especializados, modo de IA, fluxos e ferramentas de IA específicas de formato para melhor focar no resultado desejado. Se você estiver tentando criar um protótipo, por exemplo, abra o Miro Prototypes em vez de tentar criar um a partir do Assistente de uso geral.

### Miro Prototypes

[Miro Prototypes](../../miroverse/prototyping/07-miro-prototypes-add-on.md) permite criar fluxos de protótipos de uma ou várias telas com IA. Siga estas dicas para obter melhores resultados de prototipagem:

- Especifique as telas que deseja incluir no protótipo, especialmente se alguma delas estiver fora de um padrão típico de UX para a jornada do usuário que você está projetando.
- Se você tiver alguns requisitos de produto ou design (ou seja, códigos hexadecimais para cores específicas), inclua isso como contexto no seu board.
- Inclua capturas de tela de páginas ou designs semelhantes que você deseja usar como inspiração no seu board.
- Inclua informações sobre seu usuário-alvo no prompt (por exemplo, "estudantes universitários" ou "líderes de equipe de design").

### Slides da Miro

Use o AI para criar [Slides](../../formats/02-create-miro-slides-with-ai.md) e acelerar a preparação da sua apresentação. Siga estas dicas para gerar melhores decks de slides:

- Defina a paleta de cores ou outras considerações de estilo em seu prompt. Caso tenha especificado uma paleta de cores na Central da marca da Miro, inclua isso no seu prompt.
- Inclua conteúdo para slides específicos como um Documento ou notas adesivas como contexto no board.
- Especifique quem é seu público-alvo no prompt (por exemplo, "executivos C-level" ou "investidores de risco").

### Imagens

Use o Miro AI para criar imagens em seus boards. Aqui estão algumas dicas para criar melhores imagens:

- Especifique o estilo da imagem (por exemplo, "fotorrealista", "pintura digital", "impressionista").
- Inclua o contexto relevante do board, como uma descrição do que a imagem deve incluir (você pode também incluir isso na caixa de prompt, mas se já existir no board, inclua como contexto).
- Inclua quaisquer detalhes específicos que a imagem deve conter (por exemplo, "a pessoa está carregando um laptop" ou "uma pilha de livros está sobre a mesa").
- Quanto mais específico for o seu prompt, melhor será o resultado inicial.

## Editando e iterando com a Miro AI

A Miro AI é uma ferramenta para auxiliar o seu trabalho, não um substituto para insights e conhecimento humano. Editar e iterar é uma etapa importante para criar melhores resultados, tanto utilizando a IA quanto manualmente.

Ao criar Formatos com a Miro AI, você terá a opção de fazer edições antes de adicionar o conteúdo ao seu board. Nos Prototypes da Miro e nos Slides da Miro, você pode editar uma tela ou slide por vez, mas pode fazer quantas rodadas de edição forem necessárias. Você também pode reverter para versões anteriores a qualquer momento antes de adicionar o conteúdo ao board.

Aqui estão algumas dicas para editar com a Miro AI:

- Especifique uma edição de cada vez ao ajustar os resultados. Inserir muitas instruções de uma só vez pode fornecer resultados inesperados.
- Concentre-se no conteúdo, e não no estilo, já que você só pode editar uma tela ou slide por vez.
- Tente usar diferentes frases ou palavras-chave se o resultado não for o esperado.

Se você criou um formato que deseja iterar mas já o adicionou ao board, você pode usar esse objeto como contexto para a próxima iteração. Esta é uma boa opção se decidir que quer fazer algo tão simples quanto mudar o estilo de um deck de slides ou adicionar telas adicionais em um fluxo de protótipo.

:::note
Embora usar trabalhos anteriores gerados por IA como contexto para iterar novas versões seja um bom ponto de partida, a IA pode mudar aspectos do trabalho com base em outros elementos de prompt ou contexto adicional. Certifique-se de verificar todas as saídas.
:::
