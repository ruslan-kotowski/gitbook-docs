---
title: "Vis\xE3o geral dos logs de auditoria do Enterprise Guard"
article_id: 17331872857746
translation_id: 17331872857746
locale: pt-br
sidebar_position: 0
created_at: '2024-02-27T21:08:55Z'
updated_at: '2025-11-25T15:41:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Os logs de auditoria fornecem aos admins um registro abrangente de todos os eventos associados ao Enterprise Guard. Esses logs são um recurso valioso para solução eficiente de problemas e oferecem insights detalhados sobre eventos críticos, como atualizações na política de tempo de vida da lixeira e política de permissão de board na lixeira, a criação, atualização ou exclusão de políticas de retenção para a organização, ou a exclusão permanente de um board da lixeira. O acompanhamento sistemático dessas atividades fortalece o monitoramento, a análise e a manutenção, garantindo um sistema seguro e bem gerenciado.

## Eventos do Enterprise Guard nos logs de auditoria

Além dos [eventos registrados existentes](../../security-integrations/security-management/01-audit-logs.md), os logs de auditoria incluem registros sobre as seguintes categorias de eventos e eventos associados ao Enterprise Guard.

### Política de lixeira

A tabela a seguir lista as categorias de eventos e ações de eventos registradas para o componente de Política de Lixeira da organização.

|  |  |
| --- | --- |
| **Categoria de evento** | **Ação de evento** |
| Administração | Política de tempo de permanência na lixeira alterada para a organização |
| Administração | Política de permissão de board na lixeira alterada para a organização |

*Tabela 1: Categorias de eventos e ações de eventos registradas para o componente de política de Lixeira da organização*Para mais informações sobre políticas de lixeira, consulte [nossa documentação](https://help.miro.com/hc/articles/13860817985426-Trash-Policy).

### Política de retenção

A tabela a seguir lista as categorias de eventos e ações de eventos registradas para o componente de Políticas de Retenção de Conteúdo.

|  |  |
| --- | --- |
| **Categoria de evento** | **Ação de evento** |
| Administração | Política de retenção criada para a organização |
| Administração | Política de retenção atualizada para a organização |
| Administração | Política de retenção excluída para a organização |

*Tabela 2: Categorias de eventos e ações de eventos registradas para o componente de Políticas de Retenção de Conteúdo*Para mais informações sobre políticas de retenção, consulte [nossa documentação](https://help.miro.com/hc/articles/16855776325778-Retention-Beta).

### Descoberta de dados

A tabela a seguir lista as categorias de eventos e as ações de evento registradas para o componente Descoberta de Conteúdo.

|  |  |
| --- | --- |
| **Categoria do evento** | **Ação do evento** |
| Administração | Alterou a detecção de informações privadas da organização  (habilitado/desabilitado) |
| Administração | Suprimiu uma correspondência de descoberta de dados na organização |

*Tabela 3: Categorias de eventos e ações de eventos registradas para o componente Descoberta de Conteúdo*

Para mais informações sobre a descoberta de dados, consulte [nossa documentação](../../canvas-25-admin-features/data-discovery/01-data-discovery-overview.md).

### Proteções inteligentes

A tabela a seguir lista as categorias de eventos e ações de eventos registrados para o componente de Proteções Inteligentes.

|  |  |
| --- | --- |
| **Categoria de evento** | **Ação do evento** |
| Proteções inteligentes | Proteções inteligentes alteradas para um board |

*Tabela 4: Categorias de eventos e ações de eventos registradas para o componente de Proteções Inteligentes*

Para mais informações sobre Proteções Inteligentes, consulte [nossa documentação](../../canvas-25-admin-features/data-classification/01-intelligent-guardrails-overview.md).

### eDiscovery

A tabela a seguir lista as categorias de eventos e ações de eventos registradas para o componente de eDiscovery.

|  |  |
| --- | --- |
| **Categoria de evento** | **Ação do evento** |
| Administração | Caso criado para a organização |
| Administração | Caso fechado para a organização |
| Administração | Retenção legal criada para a organização |
| Administração | Retenção legal fechada para a organização |
| Administração | Retenção legal aplicada ao board Board liberado da retenção legal |

*Tabela 3: Categorias de eventos e ações de eventos registradas para o componente eDiscovery*

Para mais informações sobre eDiscovery, consulte [nossa documentação](https://help.miro.com/hc/sections/22049853357842-eDiscovery-Legal-Hold-Beta).
