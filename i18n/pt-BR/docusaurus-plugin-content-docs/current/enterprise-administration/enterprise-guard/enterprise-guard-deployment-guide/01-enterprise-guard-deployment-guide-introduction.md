---
title: "Guia de implanta\xE7\xE3o do Enterprise Guard : Introdu\xE7\xE3o"
article_id: 17120515162386
translation_id: 17120515162386
locale: pt-br
sidebar_position: 0
created_at: '2024-02-19T09:17:20Z'
updated_at: '2025-11-25T15:40:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Este documento orientará você na implantação do produto de segurança avançado da Miro, o Enterprise Guard, detalhando as práticas recomendadas para configuração e habilitação do usuário final. Caso tenha alguma dúvida relacionada ao conteúdo deste guia, entre em contato com sua time de conta da Miro .

## Como usar este guia

- Navegue de seção para seção usando o contorno no lado esquerdo da tela
- Use o guia em conjunto com a documentação do recurso vinculada ao longo
- Personalize os templates fornecidos para economizar tempo, permitindo que seus usuários

## Esboço do guia

- [Parte 1 | Configurar funções de admin](02-enterprise-guard-deployment-guide-part-1-configure-admin-roles.md)
- [Parte 2 | Implantar Segurança de Dados](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md)
- [Parte 3 | Gerenciar o ciclo de vida do conteúdo](04-enterprise-guard-deployment-guide-part-3-manage-content-lifecycle.md)

## Por que você precisa do Enterprise Guard

O Miro é o espaço de trabalho on-online pronto para empresas para inovação que transforma a maneira como times distribuídas de qualquer tamanho realizam seu trabalho.

Observamos um aumento na quantidade de trabalho estratégico sendo feito no Miro e, com esse crescimento, há ainda mais conteúdo que precisa ser protegido e governado.

Dados confidenciais estão aparecendo onde os clientes menos esperam. Com base em uma amostra de 100 clientes empresariais opt-in, descobrimos que 62% deles tinham boards que continham dados confidenciais, como informações de identificação pessoal, informações pessoais de saúde e informações de cartão de crédito. Essa superfície de risco só aumenta à medida que o número de boards para nossos clientes empresariais cresce 250% a cada ano.

Esse crescimento de conteúdo torna ainda mais desafiador tentar gerenciar riscos estritamente por meio de ferramentas tradicionais existentes ou contando com a adesão dos funcionários às políticas da empresa.

O Enterprise Guard é o complemento avançado de segurança e governança de dados para o Miro. As organizações podem encontrar e proteger conteúdo confidencial e gerenciar os ciclos de vida do conteúdo, automaticamente e em escala.

## Apresentamos o Enterprise Guard: uma solução abrangente de segurança e governança para a Miro

Reconhecendo esses desafios, a Miro apresenta o **Enterprise Guard**, um complemento avançado de segurança e governança. O Enterprise Guard oferece um conjunto de recursos que capacitam as organizações a identificar, classificar, proteger e gerenciar com eficácia conteúdo confidencial nos boards da Miro. Esta solução é adaptada para garantir conformidade e proteção avançada de dados em escala.

Com a integração do Enterprise Guard ao ecossistema empresarial da Miro, as organizações podem usufruir de uma estrutura de segurança mais robusta, automatizada e abrangente. Este complemento não apenas protege os dados, como também permite que as empresas continuem inovando e colaborando na Miro com segurança, sem bloquear as operações comerciais.

## Lançamento de disponibilidade geral do Enterprise Guard: principais recursos

![Principais recursos de lançamento do Enterprise Guard – disponibilidade geral](images/26240565578898_Enterprise-Guard-Data-Security.png)

- **Descoberta de dados:** o Enterprise Guard permite um processo proativo e completo de descoberta de dados, crucial para identificar dados confidenciais, como números de cartão de crédito, números de previdência social e outras informações críticas espalhadas por vários boards da Miro. Esta estratégia proativa é crucial para identificar e mitigar potenciais vulnerabilidades, ajudando a prevenir violações de dados e garantir a conformidade.
- **eDiscovery**. Permita a preservação segura, o rastreamento e a exportação de dados do board para dar suporte a requisitos legais, de conformidade e segurança. O recurso eDiscovery no Enterprise Guard ajuda as organizações a cumprir obrigações regulatórias por meio de funcionalidades de [retenção legal](../../canvas-25-admin-features/ediscovery/02-legal-hold-overview.md), [registros de conteúdo](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md)e [exportação do board](../../canvas-25-admin-features/ediscovery/13-board-export-api-overview.md) .

  As retenções legais impedem a exclusão permanente de conteúdo relevante para investigações ou questões legais, preservando todos os boards com os quais um usuário retido interage, incluindo todas as suas versões. Os Logs de Conteúdo fornecem registros detalhados da atividade do usuário , que podem ser exportados e integrados a ferramentas externas para auditoria ou revisão legal. Com as APIs do eDiscovery, os clientes Enterprise também podem exportar dados do board em escala, garantindo que informações críticas sejam acessíveis para fluxos de trabalho legais e de conformidade .
- **Classificação automática** defina critérios para que a Miro classifique automaticamente seus boards com base no conteúdo confidencial encontrado.
- ****Proteções inteligentes:**** aplique regras de segurança em tempo real e defina o que os usuários podem fazer com um board, como restringir a replicação do conteúdo do board e os recursos de compartilhamento em vários níveis (público, time, organização), com base na classificação manual ou automatizada do board. Isso garante privacidade e conformidade sem prejudicar as operações comerciais.
- **Política da lixeira:** a Política da lixeira do Enterprise Guard oferece controle aprimorado sobre a exclusão e restauração de boards da Miro. As organizações podem definir prazos de exclusão automática (30, 60, 90, 180 dias) para manter a conformidade com os requisitos regulatórios, equilibrando a retenção de dados com a minimização do risco empresarial.
- **Retenção:** assegure a proteção e a conformidade dos dados, permitindo que os admins definam, editem e excluam políticas adaptadas às necessidades da sua organização. Essas políticas desempenham um papel crucial na proteção dos boards da Miro dentro da organização, permitindo que você retenha boards específicos por um período determinado. A retenção garante que os boards da Miro não sejam excluídos acidental ou intencionalmente até que o board deixe o período de retenção especificado. Com as políticas de retenção, as organizações podem garantir a proteção de dados, a conformidade e a preservação de informações críticas para os negócios.
- Disposição Habilite a limpeza automática de boards arquivando-os e excluindo-os com base em políticas de retenção . [A disposição](../../canvas-25-admin-features/content-lifecycle-management/03-disposition-overview.md) garante que os boards sejam retidos apenas pelo tempo necessário e sejam movidos automaticamente para a lixeira após um período de inatividade. A partir daí, as configurações de lixo padrão determinam quem pode restaurar os boards e quando eles serão excluídos permanentemente, dando suporte à conformidade, à eficiência operacional e à segurança dos dados.
- ****Gerenciamento de chave de criptografia** **(EKM):**** o EKM concede controle centralizado sobre as chaves de criptografia, permitindo que as organizações monitorem atividades relacionadas às chaves e revoguem o acesso sempre que necessário, garantindo assim uma camada adicional de segurança de dados.
