---
title: Planner para Jira
article_id: 10648975837970
translation_id: 13808965391634
locale: pt-br
sidebar_position: 22
created_at: '2023-09-18T15:19:31Z'
updated_at: '2026-02-09T13:21:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Com o planner para Jira, os facilitadores e os times podem administrar e participar de eventos de planejamento em boards da Miro, enquanto sincronizam atualizações com o board do Jira em tempo real — economizando horas de trabalho manual.

> **Disponível para:** planos Business, Enterprise

Durante eventos de planejamento de times e empresas, como Program Increments (PI), Big Room, Roadmapping e Sprints, os times de desenvolvimento debatem e se alinham.

:::tip
O Planner está agora disponível para [Azure DevOps](https://help.miro.com/hc/articles/15280547945618).
:::

## Como criar um planner para o Jira

1. Navegue até a [barra de ferramentas de criação](https://help.miro.com/hc/articles/360017730553-Toolbars) à esquerda do seu board.
2. Clique em **Mais aplicativos** (**+**) e procure por ‘Planner’.
3. Clique em **Planner** para abrir o aplicativo.
4. Um cursor de mouse aparecerá no board. Clique em qualquer lugar para posicionar um planner em branco.
5. Clique no **menu suspenso do board do Jira** e selecione um board para conectá-lo ao planner. Caso ainda não tenha autorizado sua conta do Jira na Miro, será solicitado que faça login.
6. O primeiro campo de **Colunas** é seu *tipo de coluna*. Depois de selecionar o board do Jira, o tipo de coluna será padronizado em **Status** e mostrará até três colunas. Clique no primeiro campo de **Colunas** para selecionar um tipo de coluna diferente no menu suspenso (você pode escolher Sprint, Status, Prioridade, Corrigido na versão, Componentes ou um campo personalizado).
7. Use o segundo campo **Colunas** para refinar seu Planner. Por exemplo, se você escolheu 'Sprint' como o campo de Coluna, pode então selecionar quais sprints exibir.
8. Adicione **raias** ao seu planner, além de colunas, para organizar ainda mais as tarefas em um segundo campo do Jira (você pode escolher Sprint, Status, Prioridade, Versões de correção, Componentes, ou um campo personalizado).

:::note
Atualmente o planner só suporta um board do Jira. No entanto, você pode criar vários planners em um único board da Miro.
:::

![Creating-a-planner-widget.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696033042_Creating-a-planner-widget.gif)*Criando um planner*

## Como trabalhar com o planner

Arraste os cartões do Jira entre as colunas para atualizá-los. Por exemplo, arrastar um cartão do Jira do backlog para um sprint no planner o atualizará na Miro e no Jira.

![Dragging-stories-between-columns-planning-widget.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696028306_Dragging-stories-between-columns-planning-widget.gif)*Movendo cartões do Jira entre sprints*

Escolha um campo para **raias** para dividir seu trabalho em linhas e colunas. Mover cartões entre as raias atualizará os campos de *coluna* e *raia* do item do Jira.

![Choosing-a-swimlane.png](../../../../../../docs/integrations-apps/atlassian/images/21017725756946_Choosing-a-swimlane.png)*Como escolher um campo para raias*

Por padrão, o Planner mostra todos os itens no seu backlog. Para focar no sprint atual, no canto superior direito selecione o ícone de filtro e marque **Sprint**. Em seguida, selecione o filtro **Sprint** e ative o **Filtrar por sprint ativo**. Selecione **Aplicar** para aplicar o seu filtro de sprint.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Filtrar itens por sprint ativo.*

Você também pode usar o menu suspenso **Tipo de item** e selecionar quais tipos de itens exibir no seu planner. Por exemplo, você pode filtrar somente por História.

![Filtering-by-issue-type-planning-widget.png](../../../../../../docs/integrations-apps/atlassian/images/21017725749138_Filtering-by-issue-type-planning-widget.png)*Filtrar por tipo de item*

Os participantes podem comentar nos cartões do Jira para acompanhar discussões e notas em andamento.

![Commenting_on_a_story.png](../../../../../../docs/integrations-apps/atlassian/images/21017696024594_Commenting%20on%20a%20story.png)*Comentando em um cartão do Jira no planner*

:::note
Os cartões da Miro, notas adesivas e outros objetos não podem ser colocados dentro do Planner.
:::

## Capacidade e carga

Tome decisões informadas de priorização durante o planejamento de Sprint e PI visualizando o total de story points em colunas fáceis de ler. Aumente a eficiência do seu time e garanta a distribuição do trabalho ideal.

### Habilitar o campo de story points nos cartões do Jira

1. Vá para a [barra de ferramentas de criação](https://help.miro.com/hc/articles/360017730553-Toolbars#Creation_toolbar) no lado esquerdo do seu board.
2. Clique em **Mais apps** (**+**) e procure por ‘cartões do Jira’.
3. Clique em **cartões do Jira** para iniciar o aplicativo.
4. Clique em **Configurar cartões**.
5. Role para baixo e ative **Story Points**.

![Enabling-Story-Points-for-Jira-Cards.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696030866_Enabling-Story-Points-for-Jira-Cards.gif)
*Ativando story points para cartões do Jira*

### Como usar capacidade e carga

Depois de habilitar os story points, você pode criar um novo planner ou atualizar um board com um planner existente. Desde que pelo menos um item no board tenha story points atribuídos, você verá instantaneamente os campos **Capacidade** e **Carga** no topo de cada coluna do seu planner.

![Balancing-Capacity-and-Load.gif](../../../../../../docs/integrations-apps/atlassian/images/21017725755794_Balancing-Capacity-and-Load.gif)*Equilibrando capacidade e carga*

### Como funcionam a capacidade e a carga

**Capacidade**: Insira manualmente a capacidade de cada coluna no seu planner. Se a capacidade for menor do que a carga, a coluna ficará vermelha, sinalizando que você excedeu a capacidade do seu time. Tal sugestão visual alerta você a considerar realocar itens a fim de manter uma carga de trabalho equilibrada.

**Carga**: Representa a soma dos story points para todos os cartões em uma determinada coluna. A contagem dos cartões sem story points será nula neste cálculo.

## Configuração do Jira

Para configurar o planner, comece escolhendo um board do Jira para importar os itens. Pode ser a partir de um board do Jira de tipo Scrum ou Kanban.

Ao criar um planner, você pode escolher qual campo do Jira utilizar para suas colunas e linhas (raias), incluindo:

- Sprints
- Status
- Corrigido na versão
- Componente
- Prioridade
- Responsável
- Qualquer campo personalizado com uma seleção do menu suspenso em valor único
- Qualquer campo personalizado com uma seleção do menu suspenso em múltiplos valores

No momento, não oferecemos suporte a outros campos do Jira ou campos relacionados a datas.

A opção Sprint só aparecerá se o campo de sprint estiver disponível na tela de edição de itens no Jira. Geralmente, isso já é pré-configurado para o servidor e Data Center do Jira, mas muitas vezes o Cloud requer que o campo de sprint seja adicionado manualmente. Leia mais sobre [como configurar telas de itens](https://support.atlassian.com/jira-cloud-administration/docs/configure-issue-screens/).

:::note
Sprints fechados não podem ser exibidos no Planner.
:::

### Como criar um planner usando um JQL personalizado

Para criar um planner usando um JQL personalizado, comece criando um board do Jira com sua consulta JQL. Depois que o board do Jira for criado, siga as instruções acima para criar um planner. Ao chegar à etapa 5, lembre-se de escolher o board do Jira que você criou usando sua consulta JQL personalizada.

## Sincronização do planner

### Da Miro para o Jira

Ao arrastar um cartão entre campos personalizados na Miro, o Jira é atualizado automaticamente. Isso pode levar alguns segundos.

### Do Jira para a Miro

Se você fizer alterações em um sprint no Jira, uma notificação de **Atualizações disponíveis** aparecerá no menu de contexto do planner. Isso pode levar alguns segundos após fazer as alterações no Jira.

Clique no planner para abrir o menu de contexto e clique no ícone **Sincronizar com o Jira** para sincronizar as últimas alterações.

![Sync-planning-widget-with-jira.png](../../../../../../docs/integrations-apps/atlassian/images/21017696029970_Sync-planning-widget-with-jira.png)*Como sincronizar as atualizações do Jira para a Miro*

## Mapeamento de dependências

Os participantes podem mapear visualmente as dependências entre as tarefas no planner. Saiba mais sobre [Dependências para o Jira](https://help.miro.com/hc/articles/10649083010834).
