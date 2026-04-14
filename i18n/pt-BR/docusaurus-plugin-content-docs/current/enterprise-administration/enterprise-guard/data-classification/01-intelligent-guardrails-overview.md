---
title: "Vis\xE3o geral das Prote\xE7\xF5es Inteligentes"
article_id: 14375998880018
translation_id: 14375998880018
locale: pt-br
sidebar_position: 0
created_at: '2023-10-12T12:35:03Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Os itens do board da Miro podem conter dados de privacidade e regulamentares (como PII, PHI, PCI) ou conteúdos confidenciais essenciais para os negócios (como informações financeiras, informações de RH, propriedade intelectual, segredos comerciais). Após a descoberta e classificação automática dos dados, as organizações devem implementar controles proativos que são cruciais para manter a privacidade, a segurança e a conformidade com as regulamentações relevantes.

- Com as proteções, agora é possível aplicar automaticamente controles proativos, tais como:
  Restringir automaticamente as funcionalidades de compartilhamento em vários níveis (público, time, organização) com base no conteúdo do board e no nível de classificação.
- Restringir a replicação de conteúdo.
- Bloquear o uso do Miro AI para impedir interações com dados sensíveis ou classificados.

Essas proteções proativas garantem a privacidade e a conformidade sem prejudicar as operações comerciais.

Os admins têm duas opções para implementar as Proteções Inteligentes em sua organização:
- **Modo padrão:** Por padrão, as proteções não afetam as opções de compartilhamento ativas nos boards para evitar interrupções na colaboração em andamento, mesmo quando os boards são reclassificados durante a autoclassificação.

- **Modo rígido:** Quando a alternância **Aplicar proteções em modo rígido** está ativada, as proteções substituem todas as opções de compartilhamento ativas. Isso proporciona aos admins os níveis mais rígidos de controle, mas também pode resultar na perda imediata de acesso aos boards por parte de alguns usuários.

Considere um cenário em que você configurou proteções para garantir que os usuários de boards classificados como CONFIDENCIAL não possam compartilhar o board com o público, compartilhar com times, compartilhar com a organização ou replicar conteúdo. Alguém na sua organização criou um novo board chamado Financial Plan, adicionou alguns números de receita e atribuiu o nível de *classificação* CONFIDENCIAL a esse board. As configurações de proteção são aplicadas automaticamente e todos os usuários não conseguem compartilhar o board e todos os usuários, exceto o titular do board, não podem replicar conteúdo (Figura 2).

Para mais informações sobre cada uma das proteções, suas descrições e usuários afetados, consulte a [documentação de referência das proteções](02-guardrails-reference.md).
