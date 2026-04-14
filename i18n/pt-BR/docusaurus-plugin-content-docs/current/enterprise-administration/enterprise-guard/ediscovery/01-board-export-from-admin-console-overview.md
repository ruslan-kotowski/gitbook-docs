---
title: "Vis\xE3o geral da exporta\xE7\xE3o de board do console de admin"
article_id: 26259747401362
translation_id: 26259747401362
locale: pt-br
sidebar_position: 0
created_at: '2025-04-24T14:18:00Z'
updated_at: '2025-11-25T15:50:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: discovery-board-export
---

Os admins de eDiscovery agora podem exportar diretamente boards sob retenção legal do console de admin.
Esta capacidade permite que os admins de eDiscovery:

- Iniciar exportações de board do console de admin.
- Monitore o progresso do trabalho de exportação em tempo real através da guia **Exportações** dentro de cada caso.
- Filtre os trabalhos de exportação por status e criador e veja quais boards estão incluídos.
- Obtenha um registro completo de conteúdo para cada board exportado.
- Visualize uma lista de boards exportados e seus metadados (classificação, titular, estado da exportação).
- Baixe boards exportados individualmente, diretamente do console de admin.
- Conclua o fluxo de trabalho de exportação sem depender de APIs ou integrações.
- Cancele trabalhos de exportação na fila ou em andamento.

:::note
Para exportar boards e gerenciar operações de trabalho de exportação, você deve ter a [função de admin de eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, entre em contato com seu Admin da empresa.
:::

## **Capacidades de exportação de board**

- Cada **trabalho de exportação** pode conter até **1.000 boards**.
- **Limites de exportação** por plano:

  - **Enterprise Guard:** Até **100** tarefas de exportação ativas.
  - **Enterprise:** Até **10** tarefas de exportação ativas.
- **Limites de processamento paralelo**:

  - **Enterprise Guard**: Até **5** tarefas de exportação processadas em paralelo.
  - **Enterprise**: Apenas **1** tarefa de exportação processada por vez.
- **Logs de conteúdo com tarefas de exportação:** As exportações podem incluir opcionalmente um log de conteúdo completo para cada board exportado.
- **Filtros para tarefas de exportação**: Filtre tarefas de exportação e veja quais boards estão incluídos.
- **Cancelar tarefas de exportação em andamento e em fila**: Gerencie a largura de banda de exportação de forma eficiente.
  > ✏️ Quando você cancela uma exportação, todos os boards em andamento serão concluídos e estarão disponíveis para baixar. Os boards não iniciados não serão exportados.

- **Acesso a Downloads**: Os resultados podem ser baixados por **14 dias.**
- **Escopo do Console de admin**: Somente exportações iniciadas pelo Console de admin aparecem na **guia Exports**. Os trabalhos de exportação baseados em API não estão incluídos na lista do Console de admin.
