---
title: "Depend\xEAncias para Jira"
article_id: 10649083010834
translation_id: 10649083010834
locale: pt-br
sidebar_position: 7
created_at: '2023-03-22T10:22:08Z'
updated_at: '2025-11-25T16:22:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

Mapeie as dependências existentes ou crie novas entre os cartões do Jira no seu [Planner](../../integrations-apps/atlassian/21-planner-for-jira.md) ou em qualquer lugar do seu board da Miro, e elas serão sincronizadas instantaneamente no Jira. Com o aplicativo Dependências, é possível identificar, visualizar, debater e registrar as dependências entre os times em tempo real durante os exercícios de planejamento.

> ****💡**** Esta funcionalidade está agora disponível para [Azure DevOps](08-dependencies-for-azure-devops.md).

> **Disponível para:** planos Business e Enterprise
>
> **Disponível em:** navegador para desktop, aplicativo para desktop

## Como funcionam as dependências

As dependências aparecem como camadas de linhas de conexão e mostram as relações entre os cartões do Jira.

Elas são visíveis apenas quando você abre as dependências no board. Os participantes podem filtrar diferentes tipos de dependências para debater bloqueadores e relacionamentos.

![Dependencies-app.png](../../../../../../docs/using-miro/facilitation-tools/images/13244544218258_Dependencies-app.png)
*Dependências mapeadas entre os cartões do Jira em um widget do Planner*

## Como criar uma nova dependência

1. Vá para a barra de ferramentas de criação no lado esquerdo do board.
2. Clique no **ícone de Dependências**. Se o ícone de Dependências não estiver na sua barra de ferramentas de Criação, você precisará adicioná-lo em **Ferramentas, mídia e integrações** (**+**).
3. O painel de Dependências será aberto.
4. Clique em **Nova dependência**.
5. Clique em **Primeiro cartão** e selecione um item do Jira no menu suspenso ou por pesquisa.
6. Selecione o **Tipo de dependência** com base nas opções disponíveis na sua instância do Jira (por exemplo, blocos, clones, duplicatas ou relacionados a).
7. Clique em **Segundo cartão** e selecione um item do Jira no menu suspenso ou por pesquisa.
8. Clique em **Salvar rascunho**, ou **Salvar no Jira**diretamente.

:::tip
As dependências provisórias são salvas somente na Miro. É possível criar dependências provisórias como sugestões para outros participantes e times durante os exercícios de planejamento. Após elas terem sido revisadas e discutidas, você pode salvá-las no Jira ou excluí-las.
:::

![dependencies-entry-point.png](../../../../../../docs/using-miro/facilitation-tools/images/21537435953426_dependencies-entry-point.png)
*Criando uma nova dependência e salvando-a no Jira*

## Como visualizar e filtrar as dependências

1. Vá para a barra de ferramentas de criação no lado esquerdo do seu board.
2. Clique no **ícone Dependências**. Se o ícone Dependências não estiver na barra de ferramentas Criação, você precisará adicioná-lo em **Ferramentas, Mídia e Integrações** (**+**).
3. O painel Dependências será aberto e quaisquer dependências existentes aparecerão como linhas no board.
4. Clique no ícone **Filtro** na parte superior do painel Dependências.
5. Use os botões de alternância para filtrar por **Tipo de dependência** e **Status de sincronização**.
6. Use o menu suspenso **Mostrar linhas** para controlar quando as dependências são exibidas. Selecione **Sempre** para visualizar todas as dependências ativas. Escolha **Na seleção** para ver dependências somente quando clicar em um cartão específico do Azure ou tipo de dependência.

As linhas pontilhadas mostram as dependências provisórias, e as linhas sólidas mostram as dependências que foram sincronizadas com o Jira. A cor da linha representa o tipo de dependência.

![Filtering-dependencies.gif](../../../../../../docs/using-miro/facilitation-tools/images/13245295619730_Filtering-dependencies.gif)
*Filtrando a visualização de dependências* *no widget do Planner*

## Como editar, salvar, reverter ou excluir uma dependência

1. Vá para a barra de ferramentas de criação no lado esquerdo do board.
2. Clique no ícone **Dependências**.
3. O painel Dependências será aberto.
4. Clique no ícone **Editar** ao lado de uma dependência.

![The_option_to_edit_a_Dependency.jpg](../../../../../../docs/using-miro/facilitation-tools/images/10866625733778_The%20option%20to%20edit%20a%20Dependency.jpg)
*Editando uma dependência*

Você pode alterar o **Primeiro cartão** e o **Segundo cartão** de uma dependência, bem como o **tipo de dependência.**

*![Editing_a_dependency.gif](../../../../../../docs/using-miro/facilitation-tools/images/10866808392722_Editing%20a%20dependency.gif)**Alterando o Primeiro cartão e o Tipo de dependência*

Clique em **Salvar no Jira** para salvar e sincronizar um rascunho de dependência com o Jira.

![Save_to_Jira.png](../../../../../../docs/using-miro/facilitation-tools/images/10868740630034_Save%20to%20Jira.png)
*Salvando um rascunho de dependência no Jira*

Clique em **Reverter para rascunho** para reverter uma dependência sincronizada de volta ao rascunho.

![Revert_to_draft.png](../../../../../../docs/using-miro/facilitation-tools/images/10868741500690_Revert%20to%20draft.png)
*Revertendo uma dependência sincronizada no Jira de volta ao rascunho*

Clique no ícone **Lixeira** para excluir uma dependência.
![Delete_dependency.png](../../../../../../docs/using-miro/facilitation-tools/images/10868804195986_Delete%20dependency.png)*Como excluir uma dependência*
