---
title: Aplicativo Estimativa
article_id: 5651786248210
translation_id: 5651786248210
locale: pt-br
sidebar_position: 8
created_at: '2022-05-20T11:28:11Z'
updated_at: '2025-11-25T16:08:42Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: estimation
---

As estimativas são uma parte vital do desenvolvimento e do planejamento ágeis. Elas ajudam a alinhar os membros do time ao escopo do trabalho, a identificar falhas na análise ou entendimento e a definir expectativas claras para a entrega.

Durante as estimativas, os membros do time atribuem um número a uma tarefa para indicar a quantidade de trabalho necessária. Para fazer estimativas realistas, é usado um sistema de numeração que soma os números anteriores. Os membros do time podem debater e se alinhar sobre o número escolhido.

Use nosso aplicativo Estimativa para realizar sessões de estimativa com vários participantes em um board da Miro com [cartões](../essential-tools/02-cards.md), [notas adesivas](../essential-tools/14-sticky-notes.md) e [cartões do Jira](../../integrations-apps/atlassian/03-jira-cards.md).

> **Disponível para:** planos Starter, Business e Enterprise
> **Configurado por**: membros do time com direitos de edição do board

Para iniciar a estimativa:

1. Acesse o aplicativo Estimativa na barra de ferramentas Criação e selecione **Iniciar nova sessão**. Pode ser necessário adicionar o aplicativo Estimativa no ícone **Ferramentas, Mídia e Integrações** (**+**):
   ![estimation-entry-point.png](../../../../../../docs/using-miro/facilitation-tools/images/21537436002962_estimation-entry-point.png)*aplicativo Estimativa na barra de ferramentas*
2. Selecione a escala de estimativa: no menu suspenso, escolha **T-shirt** (disponível apenas para [cartões](../essential-tools/02-cards.md) da Miro) ou a técnica de estimativa **Fibonacci**.
3. Arraste a área para selecionar os objetos que deseja estimar. Você pode selecionar cartões, notas adesivas ou [cartões do Jira](../../integrations-apps/atlassian/03-jira-cards.md) para a estimativa. Se quiser excluir objetos específicos da estimativa, basta clicar nos pontos azuis.
4. Caso sua seleção inclua os cartões do Jira, você será solicitado a selecionar o board do Jira ao qual esses cartões estão vinculados. Isso garante que suas estimativas sejam salvas no Jira com precisão e previsibilidade. Sem esta etapa, o Jira pode não salvar tais estimativas.
5. Clique em **Estimativa para X cartões/notas adesivas/itens** quando estiver tudo pronto para iniciar a estimativa.![estimation_launch.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016786471186_estimation%20launch.gif)*Iniciando a sessão de estimativa*![estimation_app_jira_cards.png](../../../../../../docs/using-miro/facilitation-tools/images/21016786474514_estimation_app_jira_cards.png)*Usando o aplicativo Estimativa com Jira Cards*

Todas as pessoas que estão no board (e aquelas que participam do board enquanto a sessão de estimativa estiver em andamento) poderão participar da sessão de estimativa. Todos os participantes devem ter acesso de edição do board e permissões do Jira. As estimativas podem ser feitas de forma presencial ou assíncrona. Todas as estimativas são anônimas.

![join_estimation.jpg](../../../../../../docs/using-miro/facilitation-tools/images/21016751234578_join%20estimation.jpg)
*Janela pop-up para participar da sessão de estimativa*

Os usuários serão redirecionados para o primeiro item para adicionar suas estimativas depois de clicar em **Participar da estimativa**. Os usuários podem votar em todos os itens ou ignorar alguns e votar apenas em alguns específicos. Para editar uma estimativa, clique no ícone da caneta.

![adding_estimates.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751237010_adding%20estimates.gif)
*Sessão de estimativas em andamento*

A pessoa responsável pela condução da sessão pode ver, durante a sessão, uma pesquisa das estimativas fornecidas para cada item e os avatares de quem forneceu uma estimativa. Quando todos os itens tiverem recebido as estimativas de todos os participantes necessários, a pessoa que facilita a sessão pode “Escolher a estimativa final” para cada item. E também pode editar as estimativas acordadas.

![agreed_estimates.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751238162_agreed%20estimates.gif)
*Estimativa concluída*

Após todos os participantes aprovarem as estimativas para todos os itens, a pessoa que estiver conduzindo a sessão verá a janela pop-up com a opção para encerrar a sessão e compartilhar os resultados. Ela também pode clicar em **Encerrar para todos** a fim de concluir a sessão a qualquer momento. Fazendo isso, o número total de pontos será exibido. Clique em **Encerrar e compartilhar os resultados** na janela pop-up e os resultados da sessão serão salvos.

![end_session.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751242386_end%20session.gif)
*Acordo de estimativa*

Se você estimar as notas adesivas ou cartões da Miro, as estimativas são salvas como tags nos cartões ou notas adesivas.

![estimate_tags.jpg](../../../../../../docs/using-miro/facilitation-tools/images/21016786489362_estimate%20tags.jpg)
*As tags mostram as estimativas dos cartões*

Se você estimar os cartões do Jira usando a técnica de estimativa **Fibonacci**, as estimativas são salvas no Jira (no momento, a sincronização só funciona para as estimativas Fibonacci). Observe que a pessoa que organiza a sessão deve autorizar com suas credenciais do Jira antes de dar as estimativas finais. Os resultados da estimativa serão sincronizados automaticamente com os itens do Jira correspondentes.

**Para que as estimativas de Fibonacci apareçam nos cartões do Jira e nas tarefas do Jira:**

1. Certifique-se de que o campo de pontos da história esteja configurado no Jira.
2. Verifique se você tem a permissão correspondente no Jira para atualizar o valor do campo de pontos da história.
