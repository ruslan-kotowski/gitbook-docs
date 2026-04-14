---
title: "Recurso de Exporta\xE7\xE3o de Board do eDiscovery no Console de Admin"
article_id: 26529264912146
translation_id: 26529264912146
locale: pt-br
sidebar_position: 16
created_at: '2025-05-06T17:01:06Z'
updated_at: '2025-05-26T08:55:18Z'
draft: false
outdated: false
user_segment_id: 16307853619090
user_segment: Enterprise Company Admins
backstage_link:
  entity_kind: capability
  entity_id: content-explorer
---

Os admins do Enterprise Guard agora podem usar o console de admin para apoiar os fluxos de trabalho de eDiscovery de forma mais eficaz. Eles podem:

- Exporte todos os boards sob retenção legal (exportação seletiva não suportada).
- Visualizar uma lista de trabalhos de exportação (concluídos, em andamento e planejados) dentro de cada caso de eDiscovery.
- Ver o status de exportação de boards individuais em um trabalho.
- Baixar boards exportados individualmente, disponíveis por 14 dias após a exportação.

**Limites e comportamento de exportação:**

- Cada tarefa de exportação pode incluir até **1000 boards**. Os trabalhos não iniciarão se uma retenção legal incluir mais de 1000 boards.
- Um máximo de **100 trabalhos de exportação** pode estar ativo na organização.
- Até **5 jobs** são processados em paralelo (inalterado).

**Limites da API (API de exportação de board):**

- Até **100 exportações de trabalhos** para organizações Guard e **10 exportações** para organizações Enterprise.
- Limite de tamanho do trabalho de exportação: **1000 boards**.

Essas atualizações ajudam a otimizar os processos de retenção legal enquanto asseguram transparência e controle sobre as atividades de exportação de boards.
