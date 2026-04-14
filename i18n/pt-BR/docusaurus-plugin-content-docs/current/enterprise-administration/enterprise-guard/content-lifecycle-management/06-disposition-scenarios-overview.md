---
title: "Vis\xE3o geral dos cen\xE1rios de disposi\xE7\xE3o"
article_id: 19596032332434
translation_id: 19596032332434
locale: pt-br
sidebar_position: 6
created_at: '2024-06-17T17:24:29Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

## Remoção automática de boards para a Lixeira

Os boards são movidos automaticamente para a Lixeira na data de disposição designada. Caso não haja nenhuma política de retenção ativa afetando o board, sua exclusão permanente será determinada pela política da Lixeira.
![disposition1.png](images/21019694995090_disposition1.png)

Por exemplo, considere um board de projeto designado a ser movido para a Lixeira em 1.° de julho de 2025, de acordo com a política de disposição e sem nenhuma política de retenção que o esteja afetando. Esse board será movido automaticamente para a Lixeira em 1.° de julho de 2025 e excluído permanentemente em 29 de setembro de 2025, de acordo com a política de 90 dias da Lixeira.

:::note
Uma política de retenção ativa substitui a política da Lixeira. Portanto, a data de exclusão permanente do board seguirá a política de retenção vigente.
:::

Se as notificações de disposição estiverem ativadas para a política, os usuários receberão uma notificação de acordo com o número de dias configurado, quando a notificação de disposição deve ser enviada antes da movimentação agendada do board para a Lixeira.

A notificação aparece no feed de notificações da Miro e se conecta diretamente ao board. Um banner também é exibido na parte superior do board, alertando o usuário sobre a ação de mover para a lixeira que está por vir. Os titulares e cotitulares do board têm a opção de manter o board.

## Exclusão de board iniciada pelo usuário

Quando a pessoa titular de um board o move para a Lixeira, a política de disposição não afeta mais o ciclo de vida desse board. Caso não haja políticas de retenção ativas aplicadas ao board, sua exclusão permanente seguirá a política da Lixeira.

![disposition2.png](images/21019706123922_disposition2.png)

Por exemplo, considere um board de plano operacional programado para disposição em 13 de outubro de 2024. Caso a pessoa titular do board o mova preventivamente para a Lixeira em 15 de maio de 2024, e não haja políticas de retenção ativas que afetem esse board, ele será submetido à política da Lixeira. O board será, assim, excluído permanentemente em 13 de agosto de 2024, de acordo com a política de 90 dias da Lixeira.

:::note
Caso haja uma política de retenção ativa afetando o board, essa política substituirá a política da Lixeira, definindo a data de exclusão permanente de acordo com a política de retenção.
:::

## Restauração de board iniciada pelo usuário

Quando um usuário restaura um board da Lixeira, qualquer política de disposição relevante é reaplicada automaticamente. Isso garante que o board retorne ao seu ciclo de vida com todas as configurações originais restauradas.

![disposition3.png](images/21019706125586_disposition3.png)

Por exemplo, caso um usuário restaure da Lixeira, em 20 de junho de 2024, um board de estratégia de marketing que estava sob uma política de disposição de 1 ano, esta política será reaplicada automaticamente após a restauração. A nova data de disposição do board será recalculada a partir da data de restauração, definindo sua data de disposição atualizada para 20 de junho de 2025 ou um ano a partir da data em que este board foi modificado pela última vez após a restauração.

## Notificações de disposição

As notificações de disposição alertam os usuários com antecedência quando um board está programado para ser movido automaticamente para a Lixeira devido à inatividade, com base em uma política de disposição ativa.

- Os admins podem habilitar notificações ao publicar uma política.
- O tempo de notificação é configurável de 1 a 30 dias antes do movimento agendado.
- As notificações são enviadas conforme o número de dias configurado quando a notificação de disposição deve ser enviada antes da data na Lixeira.

Quando um board entra no período de inspeção:

- Uma notificação aparece no feed de notificações do usuário.
- Ao clicar, o board é aberto com um banner no topo alertando sobre a próxima movimentação para a Lixeira.
- Os usuários podem optar por manter o board para retê-lo, o que reinicia o cronômetro de disposição.

Este mecanismo de notificação se aplica a todos os cenários onde:

- Uma política de disposição com notificações está ativa.
- O board está entrando em seu período de inspeção (conforme o número de dias configurado antes da data de disposição).

### Cenário 1: Boards que atendem a uma política de disposição

Esses boards estão sob uma política e serão movidos para a lixeira após o período definido de inatividade.

Se as Notificações de Disposição estiverem ativadas para a política, uma notificação será enviada conforme o número de dias configurado para que a notificação de disposição seja enviada antes da data programada para o board ser movido para a lixeira. O board também exibirá um banner permitindo que os usuários o revisem ou mantenham.

### Cenário 2: Boards com uma etiqueta de classificação que foi adicionada após o board ter sido modificado pela última vez

Esses boards são retroativamente incluídos no escopo e ainda seguem a mesma data de disposição baseada na última modificação.

Se as Notificações de Disposição estiverem habilitadas, os usuários receberão uma notificação conforme o número de dias configurado para que a notificação de disposição seja enviada antes da data programada para o board ser movido para a lixeira, mesmo se a etiqueta foi aplicada após a última edição.

### Cenário 3: Boards com uma etiqueta de classificação que foi removida antes da publicação da política

Esses boards não estão mais sob a política e são excluídos da avaliação de disposição.

Como estão fora de escopo, nenhuma Notificação de Disposição será enviada.

### Cenário 4: Boards modificados recentemente e ainda não dentro do limite de disposição.

Esses boards foram editados recentemente e ainda não estão elegíveis para disposição.

Uma notificação será enviada apenas se o board entrar no período de inspeção — ou seja, conforme o número de dias configurado para que a notificação de disposição seja enviada antes da data de disposição. Até lá, nenhuma notificação é acionada.

### Cenário 5: Boards modificados após entrar em inspeção

Assim que um board entra no período de inspeção, sua data de disposição é fixada. Isso significa que, a menos que o titular do board escolha explicitamente manter o board, ele será movido automaticamente para a Lixeira na data agendada.

Modificar ou acessar o board durante o período de inspeção não afeta o cronograma de disposição. As seguintes ações não mudarão o resultado da disposição: editar ou visualizar o board, alterar sua etiqueta de classificação ou time, ou mesmo excluir a política associada.

Se as Notificações de Disposição estiverem ativadas, uma notificação será enviada conforme o número de dias configurado antes da data agendada para mover o board para a Lixeira, e o board exibirá um banner permitindo que o usuário o revise ou mantenha.

### Cenário 6: Boards que já foram excluídos ou movidos manualmente para a Lixeira

Esses boards já foram removidos do espaço de trabalho e não são mais geridos por políticas de disposição.

Nenhuma Notificação de Disposição é enviada para boards que já estão na Lixeira ou foram excluídos permanentemente.

### Cenário 7: Boards sob múltiplas políticas

Boards podem estar sob mais de uma política de disposição ativa ao mesmo tempo, especialmente se várias políticas tiverem como alvo a mesma etiqueta de classificação ou time.

Se mais de uma política com notificações ativadas se aplicar a um board, o usuário receberá apenas uma notificação quando o board entrar em inspeção. A notificação é baseada na política com a data de disposição mais precoce e é enviada de acordo com o número de dias configurado para o envio da notificação de disposição antes dessa data.

## Cenário 8: Boards já em estado de inspeção e a política de disposição é excluída posteriormente

Se um board já entrou no período de inspeção e as notificações de disposição foram enviadas (se ativadas), a data de disposição agendada é confirmada. Mesmo que a política de disposição associada seja posteriormente excluída ou modificada, o board ainda será movido automaticamente para a lixeira na data original de disposição — a menos que o titular do board opte por mantê-lo.

Em contraste, se a política for excluída antes de um board entrar no período de inspeção, o board é considerado fora de escopo e não será movido para a lixeira.
Isso garante que, uma vez que os usuários tenham sido notificados, a ação de disposição permaneça consistente e previsível, independentemente das alterações de política feitas posteriormente.
