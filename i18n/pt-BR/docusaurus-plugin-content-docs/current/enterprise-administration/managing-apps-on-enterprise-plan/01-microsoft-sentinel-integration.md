---
title: "Integra\xE7\xE3o com Microsoft Sentinel"
article_id: 31325908249362
translation_id: 31325908249362
locale: pt-br
sidebar_position: 1
created_at: '2025-11-24T18:16:15Z'
updated_at: '2025-12-16T15:49:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: audit-logs
---

## Visão geral

O conector [Miro](https://miro.com/) ingere logs de auditoria e logs de atividade de conteúdo das [APIs REST da Miro](https://developers.miro.com/reference/overview) no Microsoft Sentinel usando o Codeless Connector Framework (CCF). Isso centraliza o monitoramento de atividades no espaço de trabalho do Miro no Microsoft Sentinel para detecção de ameaças de segurança, investigação de incidentes e relatórios de conformidade.

## Conectores de dados

Esta solução inclui dois conectores de dados.

| Conector | Requisitos do plano | O que captura | Referências |
| --- | --- | --- | --- |
| **Logs de Auditoria da Miro (Plano Enterprise)** | Plano Enterprise | Eventos de auditoria de toda a organização, incluindo autenticação de usuários, acesso a conteúdo, mudanças de time e ações administrativas. | [Documentação da API](https://developers.miro.com/reference/enterprise-get-audit-logs) | [Visão geral dos logs de auditoria](https://developers.miro.com/reference/audit-logs) |
| **Logs de Conteúdo da Miro (Enterprise Plan + Enterprise Guard)** | Enterprise Plan + complemento Enterprise Guard | Rastreamento de atividades de conteúdo, incluindo criação, atualizações e exclusões de itens para conformidade e eDiscovery. | [Documentação da API](https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch) | [Visão geral dos logs de conteúdo](https://developers.miro.com/reference/board-content-logs) |

## Pré-requisitos

### Requisitos gerais

- Espaço de trabalho ativo do Microsoft Sentinel.
- Função de Admin da empresa na sua organização Miro.
- Token de acesso OAuth da Miro (que não expira).

### Requisitos específicos do conector

#### Para o conector de logs de auditoria

- Plano Enterprise da Miro.
- Escopo OAuth: `auditlogs:read`.
- Token de acesso.

#### Para o conector de logs de conteúdo

- Plano Miro Enterprise + complemento Enterprise Guard.
- Escopo OAuth: `contentlogs:export`.
- Token de acesso.
- ID da organização Miro.

## Instalação

Existem duas maneiras de configurar os conectores da Miro.

- **Opção 1 (recomendada):** use integrações enterprise. Configuração mais simples com geração automática de token.
- **Opção 2 (alternativa):** crie um aplicativo OAuth personalizado. Mais controle sobre a configuração do aplicativo OAuth.

**Nota:** Ao usar a Opção 1, a integração é automaticamente vinculada ao time com o maior número de usuários na sua organização. Ao usar a Opção 2, você pode escolher em qual time instalar o aplicativo. No entanto, a seleção do time não afeta quais logs são coletados. Ambas as opções fornecem acesso a logs em toda a organização. Todos os eventos relevantes para a integração de todos os times estão incluídos nos seus logs.

### Opção 1: Use as integrações enterprise (recomendado)

Esta é a opção mais simples para a maioria dos usuários. Ela cria automaticamente um aplicativo OAuth e gera um token de acesso para você através das configurações de integrações enterprise da Miro.

#### Para o conector de logs de auditoria

1. Abra as [configurações da empresa na Miro](https://miro.com/app/settings/).
2. Expanda a seção **Apps e integrações**.
3. Clique em **Integrações Enterprise**.
4. Ative a opção **SIEM**.
5. Copie o valor do **Token de Acesso** que aparece.
6. Armazene o token de forma segura.

#### Para o conector de logs de conteúdo

1. Abra as [configurações da empresa Miro](https://miro.com/app/settings/).
2. Expanda a seção de **Apps e integrações**.
3. Clique em **Integrações Enterprise**.
4. Ative a opção **eDiscovery**.
5. Copie o valor do **Access Token** que aparece.
6. Obtenha o seu **ID da Organização** a partir da URL do navegador:
   - Verifique a URL do navegador para encontrar o seu ID de organização.
   - O formato da URL é: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - Copie o seu ID de organização da URL (o valor numérico).
7. Armazene ambos, o token e o ID da organização, de forma segura.

### Opção 2: Use uma aplicação OAuth personalizada (alternativa)

Esta opção lhe dá mais controle sobre a configuração da aplicação OAuth. Use esta opção se precisar personalizar escopos, gerenciar múltiplas integrações ou preferir a gestão manual de apps OAuth.

#### Passo 1: Criar aplicação OAuth da Miro

1. Faça login na sua conta da Miro.
2. Vá para [configurações de aplicativos da Miro](https://miro.com/app/settings/user-profile/apps).
3. Clique em **Criar novo aplicativo**.
4. Selecione a opção **Token de acesso não expirável** durante a criação do aplicativo ([saiba mais sobre tokens OAuth](https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens)).
5. Habilite os escopos OAuth necessários:
   - `auditlogs:read` para o conector de logs de auditoria.
   - `contentlogs:export` para o conector de logs de conteúdo (requer Enterprise Guard).
6. Clique em **Instale o aplicativo e obtenha o token OAuth**.
7. Copie o **Token de Acesso** e armazene-o seguramente.

Para instruções detalhadas sobre a configuração do OAuth, consulte [Introdução ao OAuth](https://developers.miro.com/docs/getting-started-with-oauth).

#### Passo 2: Obter ID da organização (somente para logs de conteúdo)

1. Acesse as [Configurações de empresa da Miro](https://miro.com/app/settings/).
2. Observe a URL do navegador para encontrar o ID da sua organização:
   - O formato da URL é: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - Copie o ID da sua organização a partir da URL (o valor numérico).

### Implantar solução no Microsoft Sentinel

1. No Microsoft Sentinel, vá para **Hub de Conteúdo**.
2. Procure por **"Miro"** e clique na solução.
3. Clique em **Instalar** e siga o assistente de implantação.
4. Selecione o seu espaço de trabalho do Log Analytics.
5. Conclua a instalação.

### Configurar conectores de dados

#### Conector de logs de auditoria da Miro

1. No Microsoft Sentinel, vá para **Conectores de dados**.
2. Encontre **Miro Audit Logs (Enterprise Plan)** e clique em **Abrir página do conector**.
3. Clique em **Conectar**.
4. Insira seu **Token de Acesso**.
5. Clique em **Conectar** para ativar o conector.

#### Conector de logs de conteúdo do Miro

1. No Microsoft Sentinel, vá para **Conectores de dados**.
2. Encontre **Miro Content Logs (Plano Enterprise + Enterprise Guard)** e clique em **Abrir página do conector**.
3. Clique em **Conectar**.
4. Insira seu **ID da Organização**.
5. Insira seu **Token de Acesso**.
6. Clique em **Conectar** para ativar o conector.

A ingestão de dados começa entre 5 e 10 minutos após a ativação do conector.

## Tabelas de dados

### MiroAuditLogs_CL

Eventos de auditoria em nível de organização, incluindo:

- Autenticação e acesso de usuário.
- Operações de conteúdo.
- Mudanças em times e na organização.
- Modificações de perfil de usuário.
- Ações administrativas.

**Principais colunas**

| Coluna | Descrição |
| --- | --- |
| `TimeGenerated` | Timestamp do evento. |
| `event` | Nome do evento identificando a ação ou atividade específica. |
| `logType` | Tipo de entrada de log. |
| `category` | Categoria do evento que agrupa eventos relacionados. |
| `createdBy_email` | Usuário que acionou o evento. |
| `context_ip` | Endereço IP do evento. |
| `details` | Informações adicionais específicas do evento (JSON). |

### MiroContentLogs_CL

Logs de atividade em nível de conteúdo incluem:

- Operações em nível de item com atribuição de usuário e marcação de tempo.
- Transições de estado e modificações.
- Rastreamento de atividades para conformidade e e-Discovery.

**Colunas principais**

| Coluna | Descrição |
| --- | --- |
| `TimeGenerated` | Carimbo de tempo do evento. |
| `actionType` | Tipo de ação realizada no conteúdo. |
| `actor_email` | Usuário que realizou a ação. |
| `itemType` | Tipo do item de conteúdo afetado. |
| `contentId` | Identificador único do conteúdo. |
| `state` | Informações de estado do item (JSON). |

## Consultas de exemplo

### Visualizar eventos recentes de auditoria

```
MiroAuditLogs_CL
| sort by TimeGenerated desc
| project TimeGenerated, event, category, createdBy_email, context_ip
| take 20
```

### Atividade por usuário e tipo de evento

```
MiroAuditLogs_CL
| summarize EventCount = count() by createdBy_email, event, category
| order by EventCount desc
```

### Mudanças de conteúdo por usuário

```
MiroContentLogs_CL
| where TimeGenerated > ago(7d)
| summarize Changes = count() by actor_email, actionType
| order by Changes desc
```

### Tendências de eventos ao longo do tempo

```
MiroAuditLogs_CL
| summarize count() by event, bin(TimeGenerated, 1h)
| render timechart
```

### Usuários mais ativos (mudanças de conteúdo)

```
MiroContentLogs_CL
| where TimeGenerated > ago(30d)
| summarize TotalActions = count() by actor_email
| top 10 by TotalActions desc
```

## Solução de problemas

### Nenhum dado aparecendo

- Verifique se o access token é válido e tem os escopos corretos.
- Para logs de conteúdo, confirme se sua organização possui o complemento Enterprise Guard.
- Confirme se o ID da organização está correto (para logs de conteúdo).
- Aguarde de 5 a 10 minutos para a ingestão inicial dos dados.
- Verifique o status do conector na página **Data connectors**.

### Erros de autenticação

#### Se estiver usando a Opção 1 (alternância de integrações empresariais)

- Acesse as [Configurações da empresa no Miro](https://miro.com/app/settings/), expanda **Aplicativos e integrações** e clique em **Integrações empresariais**.
- Verifique se a alternância (SIEM para logs de auditoria, eDiscovery para logs de conteúdo) ainda está ativada.
- Se outro admin desativou a alternância, o token será invalidado.
- Reative a alternância para gerar um novo token e atualize a configuração do conector.
- Verifique se você tem a função de Admin da empresa no Miro.

#### Se usar a Opção 2 (aplicativo OAuth personalizado)

- Verifique se o token não foi revogado nas [configurações do aplicativo Miro](https://miro.com/app/settings/user-profile/apps).
- Certifique-se de que o aplicativo OAuth tenha as permissões necessárias ativadas.
- Regere o token, se necessário, e atualize-o na configuração do conector.
- Verifique se você possui a função de Admin da empresa na Miro.

### Logs de conteúdo não funcionam

- Verifique se o seu plano Miro inclui o complemento **Enterprise Guard** (não disponível no plano Enterprise básico).
- Confirme se a permissão OAuth `contentlogs:export` está habilitada.
- Verifique se o ID da organização está correto.
- Entre em contato com o gerente de conta da Miro se precisar atualizar para o Enterprise Guard.

## Recursos

### Recursos da Central de ajuda da Miro

- **Logs de Auditoria da Miro:** `../security-integrations/security-management/01-audit-logs.md
- **Logs de Conteúdo da Miro:** `../canvas-25-admin-features/ediscovery/06-content-logs-overview.md
- **Guia de integração do Miro com o Sentinel:** `01-microsoft-sentinel-integration.md`.

### Documentação para desenvolvedores da Miro

- **Introdução à API Enterprise:** `https://developers.miro.com/docs/getting-started-with-enterprise-api`.
- **Introdução ao OAuth:** `https://developers.miro.com/docs/getting-started-with-oauth`.
- **Autorização de token OAuth:** `https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens`.
- **API de Logs de Auditoria:** `https://developers.miro.com/reference/enterprise-get-audit-logs`.
- **API de Logs de Conteúdo:** `https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch`.
- **Referência da API:** `https://developers.miro.com/reference`.

### Microsoft Sentinel

- **Documentação do Microsoft Sentinel:** `https://docs.microsoft.com/azure/sentinel/`.
