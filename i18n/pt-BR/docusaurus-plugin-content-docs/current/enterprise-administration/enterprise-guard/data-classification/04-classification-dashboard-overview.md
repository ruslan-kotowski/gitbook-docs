---
title: "Vis\xE3o geral do painel de classifica\xE7\xE3o"
article_id: 26886219054354
translation_id: 26886219054354
locale: pt-br
sidebar_position: 3
created_at: '2025-05-22T11:26:15Z'
updated_at: '2025-08-18T09:36:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

O painel de classificação fornece uma visão centralizada para que os admins acompanhem e gerenciem a classificação dos boards em toda a organização. O painel oferece uma análise clara dos boards classificados e ainda não classificados, ajudando a garantir uma cobertura abrangente e a identificar áreas que precisam de atenção.

Os admins também podem monitorar o método de classificação utilizado—se manual, automático ou não classificado—para entender como os boards estão sendo categorizados. Além disso, o histórico do método de classificação visualiza as mudanças ao longo do tempo, oferecendo insights sobre tendências e a eficácia da classificação contínua do board.

:::note
Notas sobre métricas:

- Todas as métricas no Enterprise Guard excluem boards de times na lixeira e boards sob retenção legal.
- Todas as métricas de classificação excluem templates e boards na lixeira.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Título** | **Descrição** | **Domínio** | **Aparece no painel de visão geral** | **Tem métrica histórica** |
| Total de boards classificados | Número de boards com uma etiqueta de classificação atribuída | Classificação | ✅ | ❌ |
| Número de boards por classificação | Número de boards por etiqueta de classificação (nome da etiqueta) | Classificação | ✅ | ❌ |
| Número de boards não classificados | Número de boards que não têm etiqueta de classificação atribuída | Classificação | ✅ | ✅ |
| Número de boards classificados manualmente | Número de boards que receberam manualmente uma etiqueta de classificação (não identificados por classificação automática). | Classificação | ❌ | ✅ |
| Número de boards classificados automaticamente | Número de boards que receberam automaticamente uma etiqueta de classificação pela classificação automática | Classificação | ❌ | ✅ |

## Entenda os erros, os estados vazios e as alterações históricas

Compreender como interpretar estados vazios e mensagens de erro é essencial para ler com precisão as métricas do painel do Enterprise Guard.

### Entenda o comportamento de dados históricos quando as configurações são alteradas

Se uma funcionalidade, como a classificação, for desabilitada após a coleta dos dados, as métricas históricas ainda exibirão valores do período ativo. Por exemplo, se você desabilitar a classificação em maio e a classificação estava ativa em abril com 20 boards classificados:

- Os valores de abril continuarão aparecendo no painel.
- O gráfico de maio exibirá **sem dados disponíveis**, pois a coleta de dados foi interrompida.
