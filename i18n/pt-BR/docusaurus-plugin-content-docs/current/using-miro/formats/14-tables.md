---
title: Tabelas
article_id: 22760922335506
translation_id: 22760922335506
locale: pt-br
sidebar_position: 11
created_at: '2024-11-20T17:33:53Z'
updated_at: '2026-03-13T12:26:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

A ferramenta Tabelas é interativa e permite estruturar seu conteúdo na Miro, transformando ideias em planos acionáveis.

> ***Disponível em:** Todos os dispositivos*
> ***Disponível para:** Todos os planos da Miro*
> ***Quem pode fazer:** Titulares e editores do board*

## Principais funcionalidades

As Tabelas incluem as seguintes funcionalidades principais:

- **Crie campos personalizados**
  Organize e estruture suas informações com campos personalizados.
- **Crie registros a partir de cartões da Miro**
  Arraste e solte os cartões da Miro no widget Tabela para criar novos registros.
- **Crie registros a partir de notas adesivas**
  Veja Adicionar um cartão da Miro ou nota adesiva a uma Tabela.
- **Crie registros sincronizados a partir de cartões do Jira**
  Veja Adicionar um cartão do Jira a uma Tabela.
- **Funcionalidades avançadas de filtro e ordenação**
  Filtre e ordene Tabelas para organizar e priorizar registros.
- **Agrupar registros**
  Organize os registros em uma Tabela por campo para agrupar informações logicamente.
- **Criar Tabelas sincronizadas em múltiplos boards**
  Copie e cole uma Tabela para criar uma visualização sincronizada dos mesmos registros
- **Visualização de Timeline**
  Mude para a visualização de linha do tempo para ver seus dados em um novo layout.
- **Cálculos por coluna**
  Calcule agregados como soma, média e mais para campos numéricos para analisar seus dados rapidamente.
- **Formatação visual de números**
  Formate números como barras de progresso com exibição de porcentagem ou moeda e use regras de formatação condicional para destacar valores que atendem a critérios específicos. Veja [Números visuais em Tabelas](04-visual-numbers-in-tables.md).
- **Dependências**
  Mapeie e visualize dependências entre registros usando os campos "bloqueado por" e "bloqueando" entre projetos.
- **Ações em massa**
  Execute ações como editar, mover, duplicar e excluir em vários registros de uma vez, ou arraste vários registros para o canvas como cartões.

## Adicionar uma Tabela ao seu board

:::warning
Editores convidados não têm permissão para adicionar ou editar Tabelas.
:::

1. Abra um board da Miro.
2. Clique no ícone de **Ferramentas, Mídia e Integrações** (**+**) na barra de ferramentas de criação.
   O painel de Ferramentas, Mídia e Integrações será aberto.
3. Procure e selecione **Tabelas**.
   Seu cursor agora mostra o ícone de Tabelas.
4. Clique em qualquer lugar no board da Miro para posicionar seu widget Tabelas.

## Converter um arquivo do Excel em uma Tabela

1. Abra um board da Miro.
2. Clique no ícone de **Ferramentas, mídia e integrações** (**+**) na barra de ferramentas de criação.
   O painel de Ferramentas, mídia e integrações será aberto.
3. Pesquise e selecione **Carregar**.
   O painel de Carregar será aberto.
4. Selecione **Meu dispositivo**.
5. Navegue e selecione o arquivo do Excel (.xlsx) que deseja carregar.
6. Será aberto um modal com as opções:
   1. Converter para tabela.
   2. Converter para grade.
   3. Adicionar como arquivo.
7. Selecione **Converter para tabela** e escolha se deseja **Usar a primeira linha como cabeçalhos**.
8. Clique em **Selecionar**.
9. Uma tabela será criada no board com os dados do arquivo Excel.

:::warning
Ao carregar um arquivo Excel, há um limite de 500 linhas e 30 colunas.
:::

## Copiar e colar Tabelas

Você basicamente tem duas opções ao copiar e colar Tabelas, seja dentro de um board ou entre boards. A primeira opção é criar uma Tabela sincronizada que mostrará as atualizações em cada local. A segunda opção é criar uma Tabela não sincronizada, que funciona como um template.

1. Selecione a tabela que você deseja copiar.
2. Clique no menu de contexto (![icon-main.svg](../../../../../../docs/using-miro/formats/images/22916604338834_icon-main.svg)) e selecione Copiar. Alternativamente, use o atalho Ctrl + C (no Windows) ou Command + C (no Mac).
3. Navegue até o local no board onde você deseja colar a tabela.
4. Clique com o botão direito e selecione Colar. Alternativamente, use o atalho Ctrl + V (no Windows) ou Command + V (no Mac).
   Um pop-up será aberto.
5. Selecione se você deseja criar uma Tabela sincronizada ou uma nova Tabela no pop-up.

## Gerenciar permissões para Tabelas

Se você criar uma ou mais visualizações sincronizadas de uma tabela em diferentes boards da Miro, precisará gerenciar permissões para garantir que, ao adicionar uma visualização sincronizada de uma Tabela a um novo board, possa ver e gerenciar quem tem acesso de edição e visualização a essa Tabela. As permissões para visualizações sincronizadas de tabelas são gerenciadas pelo board de origem — o board em que a tabela original foi criada.

Ao colar uma Tabela em um novo board como visualização sincronizada, será exibido um pop-up caso nem todos os usuários do board tenham permissões de visualização ou de edição para a Tabela. Se você desejar visualizar ou editar as permissões da tabela, será direcionado para o board original onde está a Tabela para fazer as alterações.

Se um usuário em um board não tiver acesso ao board de origem onde a Tabela original foi criada, a Tabela aparecerá em um estado sem acesso para ele. Se o usuário tiver apenas acesso de visualização no board de origem, poderá ver a Tabela no novo board, mas não poderá editar nenhum dos registros ou alterar a visualização aplicando filtros, ordenações, grupos, etc.

## Interação com Tabelas

O widget de Tabela oferece flexibilidade para criar o conteúdo que você deseja e estruturá-lo e organizá-lo da maneira mais eficaz para o seu caso de uso.

Ao criar uma nova Tabela no seu board da Miro, um conjunto de campos padrão será fornecido que mapeia para os campos existentes encontrados em cartões da Miro. Você pode excluir, editar ou ocultar esses campos ou criar seus próprios novos campos.

### Criar um campo

Siga estas etapas para criar um novo campo:

1. Clique no ícone de + na parte superior da coluna mais à direita da Tabela.
   Um menu será aberto.
   ![tables-adding-fields.png](../../../../../../docs/using-miro/formats/images/25142699942930_tables-adding-fields.png)
   *Como adicionar um novo campo a uma Tabela*
2. Clique no tipo de campo que você deseja criar no menu. Há opções para campos da Miro e tipos de campo personalizados.
   Um diálogo de opções será aberto.
3. Insira as informações do campo (Nome do campo e, no caso do campo Selecionar, as Opções para o menu suspenso) no diálogo e clique em Salvar.

:::note
O tipo de campo Link está disponível apenas para os planos Business e Enterprise.
:::

### Editar o nome de um campo ou opções

1. Passe o mouse sobre o nome do campo.
   Um ícone de três pontos (...) irá aparecer.
2. Clique no ícone de **três pontos** (**...**).
   Um menu será aberto.
3. Clique em **Editar campo**.
   Uma caixa de diálogo com opções de edição será aberta.
4. Edite o nome do campo e/ou as opções e clique em **Salvar**.

### Excluir um campo

1. Passe o mouse sobre o nome do campo.
   Um ícone de três pontos (...) irá aparecer.
2. Clique no ícone de **três pontos** (**...**).
   Um menu será aberto.
3. Clique em Excluir.

:::warning
Um campo excluído não pode ser desfeito. Ele será removido da Tabela atual e de todas as versões sincronizadas imediatamente.
:::

### Ocultar ou exibir um campo

Siga estas etapas para ocultar ou exibir um único campo:

1. Passe o mouse sobre o nome do campo.
   Um ícone de três pontos (...) irá aparecer.
2. Clique no ícone **três pontos** (**...**).
   Um menu será aberto.
3. Clique em **Ocultar campo**.
   O campo será ocultado.
4. Para exibir o campo, repita as mesmas etapas acima, mas clique em **Exibir campo**.

Você também pode ocultar ou exibir vários campos de uma vez.

Siga estas etapas para ocultar ou exibir vários campos:

1. Clique no **ícone de Ocultar** no topo da Tabela.
   Uma lista de campos na Tabela aparecerá.
2. Selecione os campos que você gostaria de ocultar ou exibir na lista.

### Editar um registro

1. Dê um duplo clique no registro que deseja editar.
   O registro se tornará editável.
2. Edite o registro e pressione enter.

Para aplicar formatação ou adicionar um link ao texto dentro de um registro:

1. Dê um duplo clique no registro que deseja editar.
   O registro se tornará editável.
2. Destaque o texto que deseja formatar.
   Um menu de contexto aparecerá.
3. Aplique formatação ou adicione um link ao texto a partir do menu de contexto ou usando [atalhos do teclado](../working-on-the-board/06-shortcuts-and-hotkeys.md).
4. Pressione Enter para salvar o registro.

A formatação de texto também pode ser aplicada no painel lateral ao editar um registro.

### Editar múltiplos registros em massa

1. Passe o mouse sobre a linha para revelar a caixa de seleção à esquerda.
2. Selecione os registros para editar usando as caixas de seleção em cada linha relevante.
   Uma barra de ferramentas aparecerá com opções para edição.
3. Edite, mova ou duplique esses registros simultaneamente na barra de ferramentas.

### Excluir um registro

1. Passe o mouse sobre o registro que deseja excluir.
2. Clique no ícone de seis pontos para abrir o menu.
3. Selecione **Excluir**.

### Excluir múltiplos registros

1. Passe o mouse sobre a linha para revelar a caixa de seleção à esquerda.
2. Selecione os registros para editar usando as caixas de seleção em cada linha relevante.
   Uma barra de ferramentas aparecerá com opções de edição.
3. Clique no ícone **Excluir** na barra de ferramentas para excluir todos os registros selecionados.

### Adicionar comentários às Tabelas

Facilite a colaboração adicionando comentários diretamente às partes de uma Tabela que você deseja discutir.

1. Passe o cursor sobre a linha à qual deseja adicionar um comentário.
   Um ícone de Adicionar comentário aparecerá à direita da primeira célula.
2. Clique no ícone de **Adicionar comentário**.
   Um painel lateral se abrirá à esquerda.
3. No painel, adicione seu comentário e pressione enter.

Uma vez que novos comentários foram adicionados, uma contagem de comentários aparecerá ao lado do ícone de Adicionar comentário para cada linha. Clique no ícone para abrir o painel de comentários.

Do painel de comentários, você pode:

- Responder aos comentários.
- Adicionar reações aos comentários.
- Resolver um tópico de comentários.
- Copiar um link para o comentário.
- Seguir o tópico de comentários para receber notificações.
- Excluir o tópico de comentários.
- Editar um comentário que você fez.

### Adicionar um cartão da Miro ou nota adesiva a uma Tabela

Você pode criar registros em uma tabela usando cartões da Miro ou notas adesivas.

1. Selecione o cartão ou nota adesiva que deseja copiar para a tabela.
2. Arraste e solte o cartão ou nota adesiva sobre a tabela.
   Uma linha azul aparecerá no local onde o novo registro será inserido.
3. Um novo registro é criado, com o conteúdo do cartão mapeado para os campos apropriados.
   No caso de uma nota adesiva, o conteúdo será inserido no primeiro campo.

### Adicionar um cartão do Jira a uma tabela

Você pode arrastar e soltar cartões do Jira em uma tabela para criar registros sincronizados do Jira. Isso significa que você pode consolidar o trabalho da Miro e do Jira para visualizá-los em uma tabela ou linha do tempo, podendo gerenciar e acompanhar o trabalho do time todo em um só lugar.

1. Encontre o cartão relevante do Jira no canvas.
2. Arraste o cartão para a Tabela.
3. Solte o cartão na linha da Tabela que desejar.

Qualquer alteração feita na Miro será refletida no Jira e vice-versa. Os seguintes campos dentro da Tabela serão sincronizados com o Jira:

- Título
- Descrição
- Estimativa
- Data de início
- Data final
- Responsável (Beta)
- Status (Beta)

Todos os outros campos da Tabela são armazenados somente na Miro e não sincronizam com o Jira.

**Mais informações:** Consulte as [perguntas frequentes sobre cartões do Jira](../../integrations-apps/atlassian/17-jira-cards-faq.md).

### Trabalhar com cartões do Jira em massa

Ao editar registros em lote sincronizados com o Jira, apenas ações e campos suportados pela integração com o Jira estarão disponíveis. Ações não suportadas serão ocultadas ou desabilitadas no menu de ações em lote.

### Filtrar uma Tabela

Você pode filtrar os conteúdos de uma Tabela por um ou mais campos para ajudar a restringir a exibição/registros com os quais deseja trabalhar.

1. Clique no **ícone de Filtro** no topo da Tabela.
   Uma caixa de diálogo se abrirá.
2. Selecione se deseja **Adicionar filtro** ou **Adicionar grupo de filtros**.
   Uma caixa de diálogo se abrirá.
3. Especifique os parâmetros do filtro: o campo a ser filtrado, a lógica do filtro e o conteúdo específico para o filtro.
   A Tabela é filtrada em tempo real.
4. Clique em qualquer lugar fora da caixa de diálogo do filtro para fechá-la.

### Ordenar uma Tabela

1. Passe o mouse sobre o nome do campo.
   Um ícone de três pontos (...) aparecerá.
2. Clique no **ícone de três pontos** (**...**).
   Um menu será aberto.
3. Clique em **Classificação crescente** ou **Classificação decrescente**.

Para remover a ordenação em uma Tabela:

1. Clique no **ícone de Ordenar** no topo da Tabela.
   Uma caixa de diálogo se abrirá.
2. Clique em **Excluir ordenação**.

### Pesquisa em uma Tabela

1. Clique no ícone de **Pesquisar** na barra de ferramentas superior da Tabela.
2. Digite sua consulta de pesquisa.
3. Os resultados relevantes aparecerão à medida que você digita.
4. Você pode navegar pelos resultados usando os ícones de seta na barra de pesquisa ou rolando pela Tabela.
5. Clique no ícone de **Limpar** (**X**) para retornar à Tabela completa.

### Agrupar registros por campo

1. Clique no ícone **Agrupar** no topo da Tabela.
   Um menu será aberto.
   ![table-group-records.png](../../../../../../docs/using-miro/formats/images/25142699944338_table-group-records.png)
   *Agrupando registros em uma Tabela*
2. Selecione o campo pelo qual você deseja agrupar os registros.
   Os registros na Tabela serão agrupados pelo campo escolhido.

:::note
Quando você arrasta um registro para um grupo existente, o valor relevante do campo será atualizado para corresponder a esse grupo.
:::

Para remover o agrupamento em uma Tabela, siga estas etapas:

1. Clique no ícone de **Agrupar** no topo da Tabela.
   Um menu será aberto.
2. Clique em **Limpar agrupamento**.

### Cartões sincronizados

Você pode arrastar e soltar registros da Tabela para o seu canvas para criar um cartão sincronizado.

1. Passe o mouse sobre o registro do qual deseja criar um cartão sincronizado.
   Ícones aparecem no lado esquerdo do registro.
2. Clique e segure o ícone dos pontos e arraste-o para o canvas.
   Um cartão é criado com as informações do registro.
3. O cartão será atualizado sempre que o registro na Tabela for atualizado e vice-versa.

O ícone do banco de dados, que aparece no canto inferior direito do cartão, indica se o cartão está sincronizado com uma Tabela.

Se você excluir um registro, o cartão sincronizado correspondente continuará no board, mas ficará em branco.

Se você excluir um cartão sincronizado no canvas, o registro permanecerá na Tabela.

Não dá certo arrastar um cartão sincronizado para a Tabela de origem, pois será tratado como um registro único nessa Tabela. No entanto, você pode arrastar um cartão sincronizado para uma nova Tabela, onde ele aparecerá como um novo registro não sincronizado.

### Visualizar uma Tabela como Linha do Tempo

Siga estas etapas para alternar para a visualização em Linha do Tempo:

1. Clique no ícone de **Tabela** no topo da Tabela.
   Uma caixa de diálogo se abrirá.
2. Selecione **Visão de Timeline** (ou mude de volta para **Visão de Tabela**).

Ao mudar para uma visão de linha do tempo, as datas de início e fim padrão, onde preenchidas, são usadas para traçar os registros em sua Tabela como barras correspondentes na sua linha do tempo. O campo de título e o campo de responsável são usados para exibir o nome do registro e o responsável na barra.

**Mais informações:** [Timeline](15-timeline.md)

## Cálculos de coluna

> **Quais planos:** Business, Enterprise

Os cálculos de coluna permitem realizar funções agregadas em campos numéricos na sua Tabela, ajudando a analisar e resumir seus dados. Você pode calcular a soma, média, contagem, valores mínimo, máximo e mediana para qualquer coluna numérica.

1. Abra o menu de opções do campo clicando no cabeçalho da coluna que contém os dados.
2. Selecione **Mostrar cálculo da coluna** no menu.
3. Escolha o tipo de cálculo que deseja aplicar:
   1. Soma: Adiciona todos os valores na coluna
   2. Média: Calcula a média de todos os valores
   3. Contagem: Conta o número de entradas
   4. Mínimo: Mostra o menor valor
   5. Máximo: Mostra o maior valor
   6. Mediana: Mostra o valor do meio
4. O resultado do cálculo aparecerá em uma linha de rodapé na parte inferior da Tabela.

Para remover um cálculo de coluna:

1. Clique na opção **Calcular** na linha de rodapé.
2. Selecione **Nenhum**.
3. Repita até que o último cálculo tenha sido definido como Nenhum.

:::note
Você pode aplicar um cálculo por coluna. Quando você filtra ou agrupa sua Tabela, os cálculos são atualizados automaticamente para refletir apenas os registros visíveis. Em visões agrupadas, os cálculos aparecem para cada grupo, bem como um total geral.
:::

Os cálculos de coluna funcionam perfeitamente com a formatação visual de números. Quando você aplica a formatação visual a uma coluna calculada, o resultado é exibido como uma barra de progresso seguindo suas regras de formatação. Veja [Números visuais em Tabelas](04-visual-numbers-in-tables.md).

## Fórmulas Multi-coluna

> **Quais planos:** Business, Enterprise

Além de cálculos de coluna, você pode criar campos para fórmulas em várias colunas. Os campos de fórmula calculam em várias colunas na mesma linha.

Para criar um campo de fórmula:

1. Clique no ícone **+** para adicionar um novo campo.
2. Selecione o tipo **Fórmula**.
3. Use o construtor visual de fórmulas para selecionar campos, constantes e operadores (+, -, ×, ÷, (,)).
4. Sua fórmula é automaticamente calculada para cada linha.

:::note
Os campos de fórmula atualmente suportam campos numéricos e constantes.
:::

## Relações (Dependências)

> **Quais planos:** Business, Enterprise

Esse tipo de campo de relação permite mapear dependências entre registros na sua Tabela usando os campos "bloqueado por" e "bloqueando". Isso ajuda a rastrear relações de projeto e entender como os itens de trabalho dependem uns dos outros.

### Criar campos de dependência

1. Clique no **ícone +** para adicionar um novo campo.
2. Escolha entre:
   1. **Bloqueado por** - Para mostrar quais registros devem ser concluídos antes deste.
   2. **Bloqueando** - Para mostrar quais registros estão aguardando este.
3. Dê um nome ao seu campo e clique em Criar.

### Adicionar dependências entre registros

Depois de criar campos de dependência, você pode vincular registros seguindo estas etapas:

1. Clique em uma célula na coluna **Bloqueado por** ou **Bloqueando**.
2. Selecione o(s) registro(s) que deseja vincular no menu suspenso.
3. Clique fora da célula para salvar.

:::note
Os registros podem ter múltiplas relações de bloqueio e bloqueado por. As dependências sincronizam entre todas as Tabelas sincronizadas, garantindo consistência entre suas visualizações e boards.
:::

:::warning
**Limitações atuais (Beta):**

- As dependências ainda não são suportadas para registros sincronizados com o Jira ou outras integrações de terceiros.
- Os indicadores visuais de dependências ainda não são mostrados em cartões sincronizados.
- Ajustes automáticos de datas com base em dependências ainda não estão disponíveis.
:::

## Relações (Aninhamento) (BETA)

> **Quais planos:** Business, Enterprise

O tipo de campo de relação de aninhamento permite criar hierarquia entre registros na sua Tabela usando campos de **Pai** e **Filho**.

### Criar campos hierárquicos

1. Clique no ícone **+** para adicionar um novo campo.
2. Escolha entre:
   1. **Pai**: Use este campo para vincular um registro ao seu item de nível superior (por exemplo, uma funcionalidade vinculada a um épico).
   2. **Filho**: Use este campo para vincular um registro aos seus itens de nível inferior (por exemplo, uma iniciativa com subtarefas).
3. Dê um nome ao seu campo e clique em **Criar**.

### Vincular registros de pai e filho

1. Clique em uma célula na coluna **Pai** ou **Filho**.
2. Selecione o(s) registro(s) que deseja vincular no menu suspenso.
3. Clique fora da célula para salvar.

### Visualize sua hierarquia

1. Clique no ícone **Configurações de visualização** no cabeçalho das Tabelas.
2. Ative o **Aninhamento**.

Use o **sinal de expansão** ao lado dos registros Pai para revelar ou ocultar registros Filho.

:::note
*O aninhamento e a hierarquia estão ocultos por padrão. Você precisará ativá-los nessas configurações.*
:::

### Outras maneiras de criar hierarquias

1. Clique em **Adicionar sub-registro** através do **menu de 6 pontos** à esquerda de cada linha.
2. A hierarquia será ativada por padrão.

   > ✏️ Campos de Pai e Filho serão criados, mas ficarão ocultos. Para exibir esses campos, vá até o menu Ocultar campos no cabeçalho da Tabela.

   > ✏️ Para desativar a hierarquia, vá até Configurações de Visualização no cabeçalho da Tabela.
3. Você pode gerenciar hierarquias através dos campos de Pai e Filho.
4. Quando a hierarquia está ativada, você também pode arrastar e soltar para criar hierarquias.

:::warning
*Se você excluir um registro pai, todos os registros filhos desse registro também serão excluídos. Utilize a função Desfazer para reverter isso se necessário.*
:::

Se os campos Pai e Filho não estiverem ocultos, eles ficarão visíveis no painel lateral. Você pode alternar para a visualização de linha do tempo e observar seu portfólio se expandir ao longo do tempo.

:::warning
***Limitações atuais (Beta):***

- *Máximo de quatro níveis para hierarquia.*
- *A Nesting ainda não é suportada para registros sincronizados com o Jira ou outras integrações de terceiros.*
- *Indicadores visuais para Aninhamento ainda não são mostrados em cartões sincronizados.*
:::

## Modo foco

Você pode editar e visualizar sua Tabela no modo foco (tela inteira). Basta clicar no **ícone da seta diagonal** na parte superior do widget. Configurações como Filtro, Ordenar, Agrupar e Ocultar campos estão localizadas no canto superior direito.

Para voltar ao canvas, clique em **Voltar ao canvas** no topo.

## Limites do widget de Dados Estruturados

Cada board da Miro tem um limite máximo de 250 widgets de dados estruturados, que inclui a contagem total combinada de Tabelas, Linhas do Tempo e cartões sincronizados. Cada tabela é limitada a 1.000 linhas e 50 colunas. Quando você atingir o limite de linhas, verá uma mensagem impedindo a adição de mais linhas.

Para um desempenho ideal, recomendamos manter as tabelas com menos de 200 linhas quando usar muitas colunas, pois operações como agrupar, classificar e filtrar podem desacelerar além desse ponto. Esses limites ajudam a garantir um desempenho e uma confiabilidade ótimos para os boards da Miro.

### O que acontece quando você atinge o limite do widget de dados?

Quando um board atinge ou excede o limite de 250 widgets de dados estruturados, você pode experimentar:

- Uma mensagem de erro ao tentar adicionar mais widgets de dados estruturados.
- Carregamento inconsistente dos widgets de dados existentes.
- Problemas potenciais com a gravação de mudanças.
- Desaceleração de desempenho.

### Dicas para gerenciar limites de widgets de dados

Se você está se aproximando ou já ultrapassou o limite de widgets de dados estruturados, tente:

**Distribuir widgets em vários boards:**

- Agrupar conteúdos relacionados em boards separados.
- Usar nomes de board significativos para facilitar a navegação.
- Criar um board "mestre" com links para todos os boards relacionados.

**Consolidar dados semelhantes:**

- Mesclar tabelas com estruturas semelhantes.
- Usar filtros em vez de criar tabelas separadas para diferentes visualizações.
