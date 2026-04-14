---
title: "Vis\xE3o geral do painel do ciclo de vida do conte\xFAdo"
article_id: 26894063726482
translation_id: 26894063726482
locale: pt-br
sidebar_position: 2
created_at: '2025-05-22T16:02:58Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

O painel do ciclo de vida do conteúdo oferece uma visualização centralizada para que os admins monitorem e gerenciem o ciclo de vida completo dos boards — desde a criação até a exclusão — enquanto se alinham com as políticas de retenção de dados da organização. Ele fornece visibilidade sobre a fase atual do ciclo de vida de cada board, ajudando a garantir o manejo adequado do conteúdo.

Os admins também podem acompanhar boards regidos por políticas de retenção e disposição, e visualizar tendências históricas para aplicação de políticas. O painel inclui uma previsão de disposição, permitindo o planejamento proativo para ações automatizadas do ciclo de vida futuras. Isso permite a governança de conteúdo consistente e guiada por políticas em toda a organização.

:::note
Todas as métricas no Enterprise Guard excluem boards de times na lixeira e boards sob retenção legal.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Título** | **Descrição** | **Domínio** | **Aparece no painel de visão geral** | **Tem métrica histórica** |
| Total de boards | Total de boards em todos os estados do ciclo de vida (ativo, lixeira, retido). | Gerenciamento do ciclo de vida do conteúdo | ✅ | ❌ |
| Número de boards ativos. Observe que isto NÃO é atividade de board, mas boards que estão no estado do ciclo de vida "ativo". | Total de boards no estado de ciclo de vida "ativo". | Gerenciamento do ciclo de vida do conteúdo | ✅ | ✅ |
| Quantidade de boards na lixeira | Total de boards no estado de ciclo de vida "lixeira" | Gestão do ciclo de vida do conteúdo | ✅ | ✅ |
| Número de boards retidos | Total de boards no estado de ciclo de vida "retido" | Gestão do ciclo de vida do conteúdo | ✅ | ✅ |
| Número de boards sob retenção | Total de boards que têm ao menos uma política de retenção não expirada atribuída. | Gestão do ciclo de vida do conteúdo | ❌ | ✅ |
| Quantidade de boards sob disposição | Total de boards com ao menos uma política de disposição não expirada atribuída. | Gestão do ciclo de vida do conteúdo | ❌ | ❌ |
| Número de boards seguindo uma política de retenção agrupados por políticas | Número de boards em qualquer status do ciclo de vida que tenham pelo menos uma política de retenção atribuída por política | Gestão do ciclo de vida do conteúdo | ✅ | ❌ |
| Quantidade de boards sob uma política de disposição agrupados por políticas | Quantidade de boards em qualquer estado do ciclo de vida que tenham ao menos uma política de disposição atribuída por política. | Gestão do ciclo de vida do conteúdo | ✅ | ❌ |
| Quantidade de boards criados neste dia/semana/mês | Quantidade de boards criados esta semana. | Gestão do ciclo de vida do conteúdo | ❌ | ✅ |
| Quantidade de boards excluídos (movidos para a lixeira) neste dia/semana/mês | Quantidade de boards excluídos (movidos para a lixeira) esta semana. | Gestão do ciclo de vida do conteúdo | ❌ | ✅ |
| Número de boards sob políticas de disposição agrupados por mês com base na data de vigência da política de disposição. |  | Gestão do ciclo de vida do conteúdo | ❌ | ❌ |

## Entenda os erros, os estados vazios e as alterações históricas

Compreender como interpretar estados vazios e mensagens de erro é essencial para ler com precisão as métricas do painel do Enterprise Guard.

### Entenda o comportamento de dados históricos quando as configurações são alteradas

Se a descoberta de dados for desabilitada após a coleta dos dados, as métricas históricas ainda exibirão valores do período ativo. Por exemplo, se você desabilitar a descoberta de dados em maio e a descoberta de dados estava ativa em abril:

- Os valores de abril continuarão aparecendo no painel.
- O gráfico de maio exibirá **sem dados disponíveis**, pois a coleta de dados foi interrompida.

###
