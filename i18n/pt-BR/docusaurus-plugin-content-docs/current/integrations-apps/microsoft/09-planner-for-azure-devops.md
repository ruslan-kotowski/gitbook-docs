---
title: Planner para Azure DevOps
article_id: 15280547945618
translation_id: 15280547945618
locale: pt-br
sidebar_position: 10
created_at: '2023-11-23T14:12:19Z'
updated_at: '2025-11-25T15:39:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: program-board-widget
availability:
  notes: 'Disponível para: plano Education , plano Enterprise , plano de Business'
---

Durante eventos de planejamento de times e empresas, como Incrementos de Programas (PI), Big Room, Roadmapping e Sprints, os times de desenvolvimento debatem e se alinham.

Com o planejador para Azure, facilitadores e times podem executar e participar de eventos de planejamento em um board da Miro, além de sincronizar atualizações com seu board Azure em tempo real, economizando horas de trabalho manual.

## Como criar um planejador para o Azure DevOps

:::note
Para usar o planejador para o Azure DevOps, primeiro [configure sua integração com o Azure](03-azure-cards.md).
:::

1. Navegue até a [barra de ferramentas de criação](../../getting-started/start-here/your-first-board/05-toolbars.md) no lado esquerdo do seu board.
2. Clique em ****Mais aplicativos**** (+) e pesquise por "Planner".
3. Clique em **Planner.**
4. Um cursor de mouse aparecerá no board. Clique em qualquer lugar para colocar um planner em branco.
5. A fonte de dados do seu planejador será definida como padrão para a integração que você autorizou. Se você ainda não autorizou uma integração, o padrão será o Jira. Você pode facilmente alterar isso para Azure DevOps clicando no menu suspenso **Jira**e selecionando **Azure DevOps**.
6. Se você ainda não autorizou sua conta do Azure DevOps no Miro, será solicitado que você faça login.
7. Depois de efetuar login, clique no menu suspenso**Projeto do Azure**e selecione um projeto para conectar ao planejador.
8. Em seguida, clique no menu suspenso **Equipes** e selecione um time.
9. O primeiro campo ***Colunas*** corresponde ao seu tipo de coluna. **A iteração** é selecionada automaticamente. Mais campos do Azure estarão disponíveis em breve.
10. Use o segundo menu suspenso **Colunas** para refinar ainda mais quais iterações você deseja exibir.

## Como trabalhar com o planner

Arraste os cartões do Azure pelas colunas para atualizá-los. Por exemplo, arrastar um cartão do Azure da Iteração 1 para a Iteração 2 no planejador o atualizará no Miro e no Azure.

Os participantes podem comentar nos cartões do Azure para acompanhar discussões e notas em andamento.

![Comment-on-an-Azure-Planner.png](../../../../../../docs/integrations-apps/microsoft/images/21016020674450_Comment-on-an-Azure-Planner.png)*Comentando sobre o planejador*

## Sincronização do planner

### De Miro a Azure

Quando você arrasta um cartão entre campos personalizados no Miro, o Azure é atualizado automaticamente. Isso pode levar alguns segundos.

### Do Azure ao Miro

Para garantir que seu planejador permaneça atualizado com as alterações feitas no Azure, selecione o planejador e clique no botão **Sincronizar** no menu de contexto.

![Sincronizando o planejador com o Azure.png](../../../../../../docs/integrations-apps/microsoft/images/21016020674962_Syncying-the-planner-with-Azure.png)*Sincronizando o planejador com o Azure*

Os campos suportados atualmente pelo Azure são:

- Iteração (também conhecida como sprint).
- Atribuído a
- Todos os outros campos que atendem aos seguintes critérios:
  - Editável (ou seja, não somente leitura).
  - Valores de string (texto).
  - Uma lista de valores predefinidos que podem ser definidos (ou seja, não texto de fluxo livre).
  - Válido para itens de trabalho do Azure (alguns campos do Azure têm outros usos).

# Não está vendo os sprints da sua equipe?

Certifique-se de que suas iterações no Azure sejam mapeadas de volta para sua time para que você possa visualizá-las no planejador.

1. Acesse seu **Projeto** no Azure.
2. Na parte inferior do menu do lado direito, clique no ícone **Configurações do projeto** .
3. Vá para a seção **boards** e clique em **Configuração da Team**.
4. Clique na aba **Iterações** na parte superior da tela.
5. Clique em **+ Selecionar iteração**. Certifique-se de ter adicionado todas as iterações relacionadas à sua time.

![Adicionando-iterações-Azure-Devops.png](../../../../../../docs/integrations-apps/microsoft/images/21016020675858_Adding-iterations-Azure-Devops.png)*Adicionando iterações ao Azure*

## Mapeamento de dependência

Os participantes podem mapear visualmente as dependências entre as tarefas no planner. Saiba mais sobre [Dependências do Azure](../../using-miro/facilitation-tools/08-dependencies-for-azure-devops.md).
