---
title: Dependências para Azure DevOps
article_id: 15556757538450
translation_id: 15556757538450
locale: pt-br
sidebar_position: 6
created_at: '2023-12-05T11:50:18Z'
updated_at: '2025-11-25T15:39:53Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: dependencies
availability:
  notes: 'Disponível para: planos Business, Enterprise'
---

[Mapeie dependências entre cartões do Azure no seu planejador ou em qualquer lugar do seu board da Miro. Com o aplicativo Dependências, é possível identificar, visualizar, debater e registrar as dependências entre os times em tempo real durante os exercícios de planejamento.](../../integrations-apps/microsoft/09-planner-for-azure-devops.md)

:::note
Para usar dependências para o Azure DevOps, primeiro [configure sua integração com o Azure](../../integrations-apps/microsoft/03-azure-cards.md).
:::

## Como funcionam as dependências

As dependências aparecem como camadas de linhas de conexão e mostram as relações entre os cartões do Azure.

Elas só ficam visíveis quando você abre o aplicativo Dependências no board. Os participantes podem filtrar diferentes tipos de dependências para debater bloqueadores e relacionamentos.

![Mapping-dependencies-Azure.png](../../../../../../docs/using-miro/facilitation-tools/images/15603398527890_Mapping-dependencies-Azure.png)
*Dependências mapeadas no Azure*

## Como visualizar e filtrar as dependências

:::note
Você só pode visualizar e filtrar dependências que já criou no Azure. Em breve, você poderá criar e editar dependências entre cartões do Azure diretamente no Miro.
:::

1. Vá para a barra de ferramentas Criação no lado esquerdo do board.
2. Clique no ícone **Dependências**. Se o ícone Dependências não estiver na barra de ferramentas Criação, você precisará adicioná-lo em **Ferramentas, mídia e integrações** (**+**).
3. O painel Dependências será aberto e todas as dependências existentes aparecerão como linhas no board.
4. Clique no ícone **Filtro** na parte superior do painel Dependências.
5. Use os botões de alternância para filtrar por **Tipo de dependência, representado por cores de linha diferentes.**
6. **Use o menu suspenso Mostrar linhas para controlar quando as dependências são exibidas. Selecione **Sempre** para visualizar todas as dependências ativas. Escolha Na seleção para ver dependências somente quando clicar em um cartão específico do Azure ou tipo de dependência.**

![Mapping-dependencies-Azure-and-Jira.png](../../../../../../docs/using-miro/facilitation-tools/images/15603699800338_Mapping-dependencies-Azure-and-Jira.png)
*Como filtrar dependências mapeadas*

## Cartões Jira e Azure no mesmo board

Se seu time usa o Azure DevOps e o Jira, e você configurou ambas as integrações na Miro, poderá gerenciar cartões e dependências de ambos os sistemas em um único board.

As Dependências vinculam dois cartões Jira ou dois cartões Azure. Ao abrir o aplicativo de dependências em um board com cartões do Azure e do Jira que têm dependências, mostraremos todos os links existentes entre esses cartões.

**Para filtrar dependências de apenas um sistema, use as opções **Salvo no Jira** e Salvo no Azure.**

![Dependencies-mapped-between-Jira-and-Azure-cards.png](../../../../../../docs/using-miro/facilitation-tools/images/15603628660626_Dependencies-mapped-between-Jira-and-Azure-cards.png)
*Dependências do Jira e do Azure em um único board da Miro*
