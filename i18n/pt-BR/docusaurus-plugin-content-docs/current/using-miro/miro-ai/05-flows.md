---
title: Fluxos
article_id: 29687970855442
translation_id: 29687970855442
locale: pt-br
sidebar_position: 5
created_at: '2025-09-23T12:18:02Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: template-picker
availability:
  notes: 'Quem pode fazer: Membros do time Quais planos: Free, Starter, Business,
    Enterprise, Educação Quais plataformas: Navegador, Desktop, Mobile'
---

Os fluxos permitem encadear formatos no canvas para construir fluxos de trabalho automatizados com IA. Cada formato atua como entrada para o próximo, transformando processos complexos e multietapas, como planejamento de sprints, redação de briefs ou aproveitamento de dados de clientes, em fluxos automatizados.

Para saber quais formatos suportam fluxos, consulte Formatos suportados.

Este artigo explica como usar fluxos. Para informações gerais sobre fluxos, acesse [Visão geral dos fluxos](04-flows-overview.md).

:::tip
Obtenha templates prontos no [seletor de templates](../../getting-started/start-here/your-first-board/04-templates.md).
:::

## Criar e executar um fluxo

O procedimento a seguir utiliza elementos básicos de UX dos fluxos para criar um fluxo do zero. Para garantir que você possa começar a criar fluxos mais rapidamente, veja Elementos de UX dos fluxos.

Siga estas etapas:

1. Adicione um formato suportado ou bloco de Instrução de IA ao canvas.
2. (Opcional) Conecte qualquer formato ou bloco de instrução existente ao formato que você acabou de adicionar. Use os conectores de IA em forma de diamante para conectar seu fluxo.
3. Acima do Formato, clique na barra **TASK**.
   Uma barra **TASK** se expande em uma caixa onde você pode especificar seu prompt para essa posição no seu fluxo.
4. Na caixa **TASK**, adicione seu prompt. Por exemplo, em um Documento, você pode gerar um Documento de Requisitos de Produto (PRD). Você pode usar a saída de qualquer Formato conectado ou bloco de instrução de IA.

   > 💡 A caixa **TASK** permite selecionar um modelo de linguagem grande (LLM), provedor de conhecimento ou busca na web. No canto inferior esquerdo, selecione um modelo de IA, base de conhecimento ou faça uma busca na web. As opções variam dependendo do Formato.
5. (Opcional) Para criar uma nova saída, à direita, clique no conector de diamante de IA.
   O menu **Criar nova saída** é aberto.
6. (Opcional) Para criar uma nova entrada, clique à esquerda no conector de diamante Miro AI.
   O menu **Criar nova entrada** será aberto.
7. Para completar o seu fluxo, repita as etapas de 1 a 6 conforme necessário.
8. Para executar o seu fluxo, na barra **TASK** clique em **Executar**.
   ![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)*O menu de contexto **Fluxo selecionado** mostra quantas etapas o fluxo inclui.*

## Utilize Conhecimento com fluxos

Conhecimento se integra com provedores como Glean, pesquisa na web e Miro Insights, para recuperar tudo o que sua empresa sabe, usando fontes internas e externas.

Para qualquer formato em seu fluxo, clique na barra **TASK**. A barra **TASK** se expande. No canto inferior esquerdo, selecione e conecte sua base de conhecimento.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Especifique uma base de conhecimento interna para seu fluxo*

Você pode converter dados de seus próprios recursos de conhecimento em formatos como Documentos, Tabelas, notas adesivas e Slides. Em seguida, conecte cada formato para usar seus dados como entrada ou saída em um fluxo.

**Mais informações:** Consulte [Conhecimento](09-knowledge.md).

## Reverter saída em um fluxo

Você pode reverter a saída de qualquer formato em seu fluxo. Por exemplo, você executa um fluxo acidentalmente e sobrescreve um documento.

Para reverter o status de um Formato no seu fluxo para um momento anterior, clique na barra **TASK** do Formato. A barra **TASK** se expandirá. No canto inferior direito, clique no ícone de seta em sentido anti-horário. Selecione qualquer versão nas últimas 24 horas para restaurar.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *A funcionalidade Reverter permite restaurar qualquer versão do seu Formato das últimas 24 horas.*

## Elementos UX dos fluxos

Compreender os seguintes elementos UX dos fluxos ajudará você a começar a criar fluxos mais rapidamente.

### Conector de Miro AI

Formatos suportados e Blocos de Instrução têm um conector de diamante Miro AI à esquerda que permite conectar a entrada, e à direita, que conecta a saída.

Clique no conector Miro AI de qualquer lado para abrir os menus **Criar nova entrada** ou **Criar nova saída**.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)

*Clique no conector Miro AI para abrir os menus de entrada e saída.*

:::tip
Você também pode arrastar o conector Miro AI para o conteúdo existente.
:::

### Destaque inteligente de conectores

Clique em qualquer objeto no seu fluxo para ver apenas aquelas conexões destacadas.

### Ocultar conectores de Fluxos

Para fluxos complexos com muitas conexões, você pode ocultar todos os conectores de fluxo para simplificar sua visualização.

Na barra do [board](../working-on-the-board/02-miro's-new-simplified-user-interface.md), clique nos três pontos verticais. Em seguida, selecione **Visualizar**. Ative o interruptor **Mostrar/Ocultar Conectores de Fluxo** na posição desativada. Para mostrar todos os conectores de fluxo, ative na posição ativada.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Mostrar ou ocultar todos os conectores de fluxo no seu board.*

:::note
**Mostrar/Ocultar Conectores de Fluxo** impacta apenas a visualização do seu board. Colaboradores podem ajustar seu próprio interruptor.
:::

### Prompt no formato

Você pode criar um prompt para qualquer Formato ou bloco de instrução no seu fluxo, garantindo que cada Formato na cadeia execute uma tarefa especializada de fluxo.

Clique na barra **TAREFA** acima de qualquer Formato no seu fluxo. A barra **TAREFA** se expande. Adicione seu prompt e descreva como você deseja que o Formato leia o conteúdo de entrada, ou qualquer conteúdo no board, e especifique regras e saídas para o próximo Formato no seu fluxo.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *A caixa de prompt no Formato aparece na barra **TAREFA** acima de cada Formato no seu fluxo.*

### Bloco de instrução para IA

Você pode selecionar um modelo de linguagem de grande porte (LLM) ou qualquer provedor de [conhecimento](09-knowledge.md) disponível para executar um prompt em um bloco independente em qualquer lugar do seu fluxo.

Para um determinado Formato, clique no conector em forma de diamante do Miro AI. No menu de entrada ou saída, selecione **Instrução** **de IA**.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Blocos de instrução permitem que você encadeie instruções, aceite entrada e passe a saída para o próximo Formato.*

### Botão global de execução

Você pode iniciar sua execução a partir de qualquer formato ou bloco de instrução de IA em seu fluxo. Clique para selecionar o formato ou bloco. O menu de contexto **Fluxo selecionado** aparece próximo à barra de Colaboração.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *O menu de contexto Fluxo selecionado*

O menu **Fluxo selecionado** mostra quantos passos ainda precisam ser executados. Para executar o fluxo, clique em **Executar**.

## Formatos compatíveis

Os fluxos suportam os seguintes formatos do Miro.

- Diagramas
- Documentos
- Imagens
- Inserir o código do iFrame
- Kanban
- Protótipos
- Slides
- Tabelas
- Linha do tempo
