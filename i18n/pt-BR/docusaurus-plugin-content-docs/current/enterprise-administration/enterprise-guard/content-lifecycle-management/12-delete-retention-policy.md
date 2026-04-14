---
title: "Excluir a pol\xEDtica de reten\xE7\xE3o"
article_id: 19205219887762
translation_id: 19205219887762
locale: pt-br
sidebar_position: 12
created_at: '2024-05-28T18:02:52Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

A exclusão de uma política de retenção libera os boards retidos associados à política de retenção. Esses boards podem então ser excluídos permanentemente, sem restrições.

:::note
Para excluir políticas de retenção, você deve ter a função de [Data Governance Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)admin de governança de dados. Para solicitar a função de admin de governança de dados, entre em contato com o Admin da empresa.
:::

Para excluir uma política de retenção, siga os seguintes passos:

1. Vá para as suas [configurações da Miro](https://miro.com/app/settings).
2. No painel esquerdo, em **Enterprise Guard,** clique em **Ciclo de vida do conteúdo**.
3. Clique na guia **Retenção**.
4. Na página de **políticas** de **retenção**, clique na política de retenção que deseja excluir.
   A página que exibe informações relacionadas à política é exibida.
5. Clique em **Excluir** no canto superior direito da página.
6. Revise o impacto da exclusão da política de retenção. A página de revisão do impacto fornece as seguintes informações:
   - **Resumo:** configuração da política de retenção, como o nome da política, o período de retenção e o escopo.
   - **Impacto da política:** número de boards que serão liberados da retenção e poderão ser excluídos permanentemente, sem restrições. A política de retenção também se aplica a boards na lixeira e eles estão incluídos no cálculo da revisão de impacto.
7. Para excluir a política de retenção, clique em **Excluir política**.

:::note
Criar, atualizar ou excluir uma política aciona o processo de políticas de retenção, que pode levar até 24 horas para ser concluído. No entanto, a atualização do nome ou da descrição de uma política ocorre imediatamente, pois essas ações não acionam o processo de políticas de retenção.
:::
