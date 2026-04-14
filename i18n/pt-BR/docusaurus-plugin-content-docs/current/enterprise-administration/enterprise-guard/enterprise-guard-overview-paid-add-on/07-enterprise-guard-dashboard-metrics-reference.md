---
title: "Refer\xEAncia de m\xE9tricas do painel do Enterprise Guard"
article_id: 26718144750610
translation_id: 26718144750610
locale: pt-br
sidebar_position: 5
created_at: '2025-05-15T00:17:54Z'
updated_at: '2025-07-22T20:38:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: admin-analytics
---

:::note
Observações sobre métricas:

- Todas as métricas no Enterprise Guard excluem boards de times na lixeira.
- Todas as métricas de classificação excluem templates e boards na lixeira.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Título** | **Descrição** | **Domínio** | **Aparece no painel de visão geral** | **Tem métrica histórica** |
| Total de boards classificados | Número de boards com uma etiqueta de classificação atribuída | Classificação | ✅ | ❌ |
| Número de boards por classificação | Número de boards por etiqueta de classificação (nome da etiqueta) | Classificação | ✅ | ❌ |
| Número de boards não classificados | Número de boards que não têm etiqueta de classificação atribuída | Classificação | ✅ | ✅ |
| Número de boards classificados manualmente | Número de boards que receberam manualmente uma etiqueta de classificação (não por classificação automática) | Classificação | ❌ | ✅ |
| Número de boards classificados automaticamente | Número de boards que receberam automaticamente uma etiqueta de classificação pela classificação automática | Classificação | ❌ | ✅ |
| Número de boards sensíveis | Número de boards que têm pelo menos uma etiqueta integrada, etiqueta de palavra-chave ou etiqueta de privacidade atribuída. | Descoberta de dados | ✅ | ❌ |
| Número de boards que têm itens sensíveis da empresa | Número de boards que têm pelo menos uma etiqueta integrada ou etiqueta de palavra-chave atribuída. | Descoberta de dados | ✅ | ✅ |
| Número de boards que possuem itens sensíveis relacionados à privacidade | Número de boards que têm pelo menos uma etiqueta de privacidade atribuída. | Descoberta de dados | ✅ | ✅ |
| Número de boards que têm uma etiqueta atribuída por etiqueta | Número de boards para cada etiqueta (integrada, palavra-chave ou privacidade) | Descoberta de dados | ❌ | ❌ |
| Quantidade de etiquetas relacionadas à privacidade habilitadas. | Número de etiquetas relacionadas à privacidade habilitadas | Descoberta de dados | ❌ | ❌ |
| Quantidade de etiquetas de palavras-chave habilitadas. | Número de etiquetas de palavras-chave habilitadas | Descoberta de dados | ❌ | ❌ |
| Quantidade de etiquetas Confidencial da empresa habilitadas. | Número de etiquetas sensíveis da empresa habilitadas | Descoberta de dados | ❌ | ❌ |
| Total de boards | Total de boards em todos os estados do ciclo de vida (ativo, lixeira, retido). | Gestão do ciclo de vida do conteúdo | ✅ | ❌ |
| Número de boards ativos. Observe que isto NÃO é atividade de board, mas boards que estão no estado do ciclo de vida "ativo". | Total de boards no estado de ciclo de vida "ativo". | Gestão do ciclo de vida do conteúdo | ✅ | ✅ |
| Quantidade de boards na lixeira | Total de boards no estado de ciclo de vida "lixeira" | Gestão do ciclo de vida do conteúdo | ✅ | ✅ |
| Número de boards retidos | Total de boards no estado de ciclo de vida "retido" | Gestão do ciclo de vida do conteúdo | ✅ | ✅ |
| Número de boards sob retenção | Total de boards que têm ao menos uma política de retenção não expirada atribuída | Gestão do ciclo de vida do conteúdo | ❌ | ✅ |
| Quantidade de boards sob disposição | Total de boards que têm ao menos uma política de disposição não expirada atribuída. | Gestão do ciclo de vida do conteúdo | ❌ | ❌ |
| Número de boards seguindo uma política de retenção agrupada por políticas | Número de boards em qualquer estado do ciclo de vida que tenham pelo menos uma política de retenção atribuída | Gestão do ciclo de vida do conteúdo | ✅ | ❌ |
| Quantidade de boards sob uma política de disposição agrupados por políticas | Número de boards em qualquer estado do ciclo de vida que tenham pelo menos uma política de disposição atribuída | Gestão do ciclo de vida do conteúdo | ✅ | ❌ |
| Quantidade de boards criados neste dia/semana/mês | Quantidade de boards criados esta semana. | Gestão do ciclo de vida do conteúdo | ❌ | ✅ |
| Quantidade de boards excluídos (movidos para a lixeira) neste dia/semana/mês | Quantidade de boards excluídos (movidos para a lixeira) esta semana. | Gestão do ciclo de vida do conteúdo | ❌ | ✅ |
| Número de boards sob políticas de disposição agrupados por mês com base na data de vigência da política de disposição. |  | Gestão do ciclo de vida do conteúdo | ❌ | ❌ |
| Número de casos | Total de casos. | Descoberta eletrônica (eDiscovery) | ✅ | ❌ |
| Quantidade de retenções legais | Total de retenções legais. | eDiscovery | ✅ | ❌ |
| Quantidade de retenções legais para um caso específico | Total de retenções legais para um caso específico. | eDiscovery | ❌ | ❌ |
| Quantidade de boards sob retenção legal | Total de boards sob retenção em todas as retenções legais. | eDiscovery | ❌ | ❌ |
| Usuários sob retenção legal e total de boards de sua titularidade | Lista usuários sob retenção legal e o número total de seus boards | eDiscovery | ❌ | ❌ |
