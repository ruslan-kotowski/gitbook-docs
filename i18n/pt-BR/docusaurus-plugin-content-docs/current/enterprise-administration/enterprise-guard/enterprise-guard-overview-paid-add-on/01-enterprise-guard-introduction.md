---
title: "Introdu\xE7\xE3o ao Enterprise Guard"
article_id: 15699815402514
translation_id: 15699815402514
locale: pt-br
sidebar_position: 0
created_at: '2023-12-11T23:40:22Z'
updated_at: '2025-11-25T15:40:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Na era digital atual, o crescimento exponencial de dados, especialmente informações confidenciais, tornou-se uma preocupação significativa para as empresas. A Miro, conhecida por seu espaço de trabalho para colaboração online de nível empresarial que promove a inovação e o trabalho em equipe, observou um aumento substancial na complexidade e na quantidade de conteúdo em seus boards. Um número notável de boards da Miro contém dados altamente confidenciais, como informações de identificação pessoal (PII), informações de saúde protegidas (PHI), informações de cartão de pagamento (PCI) e muito mais, apresentando desafios para gerenciar riscos e garantir a conformidade. Esta tendência destaca a importância da implementação de medidas avançadas de segurança e conformidade para ajudar a prevenir potenciais violações de dados e vazamentos de propriedade intelectual.

## Apresentamos o Enterprise Guard: uma solução abrangente de segurança e governança para a Miro

Reconhecendo esses desafios, a Miro apresenta **Enterprise Guard**, um complemento avançado de segurança e governança. O Enterprise Guard oferece um conjunto de recursos que capacitam as organizações a identificar, classificar, proteger e gerenciar com eficácia conteúdo confidencial nos boards da Miro. Esta solução é adaptada para garantir conformidade e proteção avançada de dados em escala.

Com a integração do Enterprise Guard ao ecossistema empresarial da Miro, as organizações podem usufruir de uma estrutura de segurança mais robusta, automatizada e abrangente. Este complemento não é apenas sobre proteger dados—é sobre permitir que as empresas continuem inovando e colaborando na Miro com segurança, sem impedir as operações comerciais.

## Lançamento de disponibilidade geral do Enterprise Guard: principais recursos

![Enterprise Guard General Availability release key features](images/21019706011410_Enterprise-Guard-Data-Security.png)

- **Descoberta de dados:** o Enterprise Guard permite um processo proativo e completo de [descoberta de dados](../../canvas-25-admin-features/data-discovery/01-data-discovery-overview.md), crucial para identificar dados confidenciais, como números de cartão de crédito, números de previdência social e outras informações críticas espalhadas por vários boards da Miro. Esta estratégia proativa é crucial para identificar e mitigar potenciais vulnerabilidades, ajudando a prevenir violações de dados e garantir a conformidade.
- **eDiscovery:** Habilitar a preservação segura, o rastreamento e a exportação de dados do board para atender aos requisitos legais, de conformidade e de segurança. O recurso eDiscovery no Enterprise Guard ajuda as organizações a cumprir suas obrigações regulatórias por meio das capacidades de [retenção legal](../../canvas-25-admin-features/ediscovery/02-legal-hold-overview.md), [logs de conteúdo](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md) e [exportação de boards](../../canvas-25-admin-features/ediscovery/13-board-export-api-overview.md).

  A retenção legal impede a exclusão permanente de conteúdo relevante para investigações ou assuntos legais, preservando todos os boards com os quais um usuário sob retenção interage, incluindo todas as suas versões. Os logs de conteúdo fornecem registros detalhados das atividades dos usuários, que podem ser exportados e integrados a ferramentas externas para auditoria ou revisão legal. Com as APIs de eDiscovery, os clientes Enterprise também podem exportar dados de board em grande escala, garantindo que informações críticas estejam acessíveis para fluxos de trabalho jurídicos e de conformidade.
- **Classificação automática**: Defina critérios para que a Miro [classifique automaticamente seus boards](../../canvas-25-admin-features/data-classification/03-auto-classification-overview-and-scenarios.md) com base no conteúdo sensível encontrado nos boards.
- **Proteções inteligentes****:** [Aplique regras de segurança em tempo real](../../canvas-25-admin-features/data-classification/01-intelligent-guardrails-overview.md) e defina o que os usuários podem fazer com um board, como restringir a replicação do conteúdo do board e os recursos de compartilhamento em vários níveis (público, time, organização), com base na classificação manual ou automatizada do board. Isso garante privacidade e conformidade sem prejudicar as operações comerciais.
- **Política de lixeira**: A [Política da Lixeira](https://help.miro.com/hc/articles/13860817985426) do Enterprise Guard oferece controle aprimorado sobre a exclusão e restauração de boards da Miro. As organizações podem definir prazos de exclusão automática (30, 60, 90, 180 dias) para manter a conformidade com os requisitos regulatórios, equilibrando a retenção de dados com a minimização do risco empresarial.
- **Retenção:** assegure a proteção e a conformidade dos dados, permitindo que os admins definam, editem e excluam políticas adaptadas às necessidades da sua organização. Essas políticas desempenham uma função crucial na proteção dos boards da Miro dentro da organização, permitindo que você retenha determinados boards por um período específico. [A retenção](https://help.miro.com/hc/articles/16855776325778) garante que os boards da Miro não sejam excluídos acidental ou intencionalmente até que o board deixe o período de retenção. Com as políticas de retenção, as organizações podem garantir a proteção de dados, a conformidade e a preservação de informações críticas para os negócios.
- ****Disposição:**** Ativar limpeza automática dos boards, arquivando-os e excluindo-os com base em políticas de retenção. [Disposição](../../canvas-25-admin-features/content-lifecycle-management/03-disposition-overview.md) garante que os boards sejam mantidos apenas pelo tempo necessário e sejam automaticamente movidos para a lixeira após um período de inatividade. A partir daí, as configurações padrão da lixeira determinam quem pode restaurar os boards e quando eles serão excluídos permanentemente—apoiando a conformidade, a eficiência operacional e a segurança dos dados.
- **Gerenciamento de Chaves de Criptografia****(EKM)****:** [EKM](../../canvas-25-admin-features/encryption-key-management/01-encryption-key-management-overview.md) concede controle centralizado sobre as chaves de criptografia, permitindo que as organizações monitorem atividades relacionadas às chaves e revoguem o acesso sempre que necessário, garantindo assim uma camada adicional de segurança de dados.
