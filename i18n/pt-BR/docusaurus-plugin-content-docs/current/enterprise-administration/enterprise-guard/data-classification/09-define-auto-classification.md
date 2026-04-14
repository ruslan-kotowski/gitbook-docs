---
title: "Definir a classifica\xE7\xE3o autom\xE1tica"
article_id: 16494707596050
translation_id: 16494707596050
locale: pt-br
sidebar_position: 9
created_at: '2024-01-19T19:01:08Z'
updated_at: '2025-11-25T15:40:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Para proteger seu conteúdo sensível, o Enterprise Guard inclui a funcionalidade de classificação automática, um processo de classificação automática de dados, que categoriza os boards da Miro com base no seu nível de conteúdo sensível. A classificação automática representa um avanço importante na maneira como você gerencia e protege seus dados confidenciais. A automação do processo de classificação permite que sua organização reforce o nível de segurança dos dados, atenda aos requisitos regulatórios e forneça uma melhor experiência de admin de segurança. A transição da classificação manual para a automática é um passo estratégico em prol de uma estrutura de segurança de dados mais precisa, segura e eficiente.

Para obter mais informações sobre classificação automática e cenários de exemplo, consulte [Visão geral da classificação automática](03-auto-classification-overview-and-scenarios.md).

## Definir a classificação automática

Esta é a segunda etapa do fluxo de configuração de autoclassificação e guardrails. Nesta etapa do fluxo, você configurará o etiqueta de sensibilidade de classificação automática aplicável a cada nível de classificação. A classificação do board é aplicada automaticamente a todos os boards novos e existentes que correspondem aos critérios definidos. Isso é feito depois que você analisa o impacto e decide publicar atualizações.

## Pré-requisitos

- [Você deve habilitar a descoberta de dados](../data-discovery/13-activate-privacy-related-data-discovery.md).
- Você deve concluir a primeira etapa do fluxo de classificação automática e guardrails, [1: Definir os níveis de classificação](07-define-classification-levels.md)./a>
- Você deve conhecer os rótulos de sensibilidade que deseja atribuir a cada nível de classificação com base em seus requisitos de segurança e governança.
- Você deve ter a [função de admin de conteúdo Sensível](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Para solicitar a função de admin de conteúdo sensível, entre em contato com seu Admin da empresa.

## Atribuir rótulos de sensibilidade para classificação automática

Para atribuir rótulos de sensibilidade a um nível de classificação, execute as seguintes etapas:

1. Na página **Definir classificação automática** , clique no ícone **Editar** do nível de classificação para o qual você deseja atribuir os rótulos de sensibilidade. Por exemplo, se você quiser atribuir rótulos de sensibilidade de classificação automática para o nível de classificação **CONFIDENCIAL** , clique no ícone Editar na linha do nível de classificação **CONFIDENCIAL** .
2. Marque a caixa de seleção para cada etiqueta de sensibilidade que você deseja atribuir a este nível de classificação. Por exemplo, se você quiser classificar automaticamente todos os boards que contêm dados confidenciais relacionados ao GDPR, marque a caixa de seleção **Regulamento Geral de Proteção de Dados do GDPR** . Você pode atribuir um ou mais rótulos de sensibilidade por etiqueta de classificação.
3. Clique em Concluído
   A classificação do board é aplicada automaticamente a todos os boards novos e existentes que correspondem aos critérios definidos. Isso é feito depois que você analisa o impacto e decide publicar atualizações.
4. Quando terminar de atribuir rótulos de sensibilidade para vários níveis de classificação, prossiga para [Concluir configuração de classificação automática](09-define-auto-classification.md).

## Configuração completa de autoclassificação

Depois de terminar de atribuir rótulos de sensibilidade para classificação automática, clique em **Avançar**. Sua configuração será salva, mas só entrará em vigor depois que você clicar em **Publicar** na página [**Revisar impacto**](https://help.miro.com/hc/articles/16494764223378) .

Você pode então prosseguir com qualquer uma das seguintes etapas:

- Definir as proteções Isto é opcional. Se você quiser definir guardrails posteriormente, clique em **Avançar**.
- Revisar impacto Esta é a última etapa do fluxo de trabalho e é obrigatória.
