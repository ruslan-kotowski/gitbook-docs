---
title: "Cen\xE1rios de reten\xE7\xE3o"
article_id: 19205103343506
translation_id: 19205103343506
locale: pt-br
sidebar_position: 9
created_at: '2024-05-28T17:58:22Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

## o board é descartado durante o período de retenção

**As políticas de retenção sobrepõem as políticas de lixeira.** Se um board sob retenção for movido para a lixeira durante a fase inicial ou intermediária de seu período de retenção, ele permanecerá na lixeira pelo período configurado na Política de lixeira (padrão de 90 dias). Após esse período, o board não aparece mais na lixeira. No entanto, o board será mantido e retido até a conclusão do período de retenção, após o qual o board será automaticamente eliminado. A Figura 1 ilustra esse cenário.

![Figure 1: Board is trashed during retention period](images/21019706071570_board_trashed_during_retention_period.png)*Figura 1: o board é descartado durante o período de retenção*

## o board é descartado quando o período de retenção termina

**A Política de lixeira permanece ativa após o término do período de retenção.** Se um board sob retenção for movido para a lixeira quando o período de retenção estiver terminando, ele permanecerá na lixeira pelo período configurado na Política de lixeira (padrão de 90 dias). Após esse período, o board não aparece mais na lixeira. Após o término do período de retenção, o board poderá ser manualmente excluído permanentemente e será automaticamente eliminado ao fim do período estabelecido na Política de lixeira. A Figura 2 ilustra esse cenário.

![Figure 2: Board is trashed when the retention period is ending](images/21019706073874_board_trashed_when_retention_period_is_ending.png)*Figura 2: o board é descartado quando o período de retenção termina*

## o time é excluído durante o período de retenção

**Quando um time é eliminado, todos os boards que pertencem a esse time são excluídos permanentemente.** Quando um time é movido para a lixeira, todos os boards desse time são excluídos permanentemente após 90 dias, incluindo os boards sob uma política de retenção. Se um time na lixeira for manualmente excluído permanentemente por um admin, o mesmo resultado se aplica: todos os boards do time serão excluídos permanentemente, mesmo que esses boards estejam sob retenção. A Figura 3 ilustra esse cenário.

![Figure 3: Team is trashed during retention period](images/21019694949138_team_trashed_during_retention_period.png)*Figura 3: o time é excluído durante o período de retenção*
