---
title: "Vis\xE3o geral do painel do Enterprise Guard"
article_id: 26707467343890
translation_id: 26707467343890
locale: pt-br
sidebar_position: 4
created_at: '2025-05-14T13:14:06Z'
updated_at: '2025-11-25T15:51:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: admin-analytics
---

## Visão centralizada de segurança e governança

O painel do Enterprise Guard oferece uma visão centralizada e de alto nível dos insights de segurança e governança da informação da sua organização em uma visão unificada. Desenhado para admins do Enterprise Guard, este painel reúne métricas-chave em domínios centrais — incluindo descoberta de dados, classificação, ciclo de vida do conteúdo e eDiscovery — em uma única interface consolidada. Ele permite uma rápida visibilidade da exposição atual, cobertura de políticas e prontidão legal — capacitando os admins a detectar riscos potenciais precocemente, tomar medidas proativas e temporais, e abordar áreas que necessitem de atenção.

## Métricas acionáveis e em tempo real

Cada métrica no painel do Enterprise Guard reflete dados em tempo real, atualizados diariamente. Todas as métricas são acionáveis e se conectam diretamente aos seus respectivos painéis de domínio, permitindo que os admins explorem insights detalhados e configurem as definições conforme necessário. Quer você esteja monitorando a sensibilidade do board, o status da classificação, as políticas de retenção ou as retenções legais, este painel oferece um ponto de partida centralizado. Esta abordagem em camadas garante consistência em todo o produto Enterprise Guard e simplifica a navegação para admins ocupados.

## Suporte para governança em grande escala

O painel do Enterprise Guard é especialmente útil para admins do Enterprise Guard que gerenciam implantações em grande escala no plano Enterprise. Ele traz clareza para configurações complexas de governança da informação e apoia a tomada de decisões informadas, consolidando os sinais mais importantes em um só lugar. Como parte do nosso compromisso com uma experiência mais intuitiva no Enterprise Guard, o painel do Enterprise Guard ajuda os admins não apenas a entenderem o que está acontecendo, mas também o que fazer a seguir, com links para agir diretamente dos dados. Quer você esteja reportando à liderança ou gerenciando a governança de dados do dia a dia, este painel garante que você possa acessar rapidamente informações relevantes, priorizar ações e demonstrar o valor da estratégia de segurança e conformidade da sua organização.

## Painéis específicos do domínio relacionados

Além do painel do Enterprise Guard, os admins podem explorar um conjunto de painéis específicos de domínio, projetados para fornecer insights mais profundos e controle sobre as principais áreas de governança. Cada um desses painéis possibilita a tomada de decisões focada em sua área respectiva, enquanto mantém o alinhamento com a estrutura mais ampla do Enterprise Guard. Eles incluem:

- **Painel de descoberta de dados:** descubra e analise onde informações sensíveis estão localizadas nos seus boards.
- **Painel de classificação:** acompanhe e gerencie a cobertura de classificação em nível de board e etiquetas de sensibilidade.
- **Painel do ciclo de vida do conteúdo:** monitore políticas de retenção de dados e automatize ações de gerenciamento do ciclo de vida.
- **Painel de eDiscovery:** obtenha visibilidade sobre retenções legais e simplifique os fluxos de trabalho de preparação de eDiscovery.

## Entenda as métricas do painel

Os painéis do Enterprise Guard incluem dois tipos de métricas: métricas atuais e métricas históricas. Para garantir clareza e consistência, cada métrica apresentada nos painéis do Enterprise Guard está definida na [documentação de métricas do painel do Enterprise Guard](07-enterprise-guard-dashboard-metrics-reference.md).

:::note
Notas sobre métricas:

- Todas as métricas no Enterprise Guard excluem boards de times na lixeira e boards sob retenção legal.
- Todas as métricas de classificação excluem templates e boards na lixeira.
:::

## Entenda os erros, os estados vazios e as alterações históricas

Compreender como interpretar estados vazios e mensagens de erro é essencial para ler com precisão as métricas do painel do Enterprise Guard.

### Entenda o comportamento de dados históricos quando as configurações são alteradas

Se uma funcionalidade, como a classificação, for desabilitada após a coleta dos dados, as métricas históricas ainda exibirão valores do período ativo. Por exemplo, se você desabilitar a classificação em maio e a classificação estava ativa em abril com 20 boards classificados:

- Os valores de abril continuarão aparecendo no painel.
- O gráfico de maio exibirá **sem dados disponíveis**, pois a coleta de dados foi interrompida.
