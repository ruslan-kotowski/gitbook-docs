---
title: Logs de conteúdo
article_id: 17774729839378
translation_id: 17774729839378
locale: pt-br
sidebar_position: 5
created_at: '2024-03-19T13:00:06Z'
updated_at: '2026-03-15T21:32:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
availability:
  notes: 'Configurado por: Admins da empresa, Admins de segurança'
---

Os logs de conteúdo permitem que clientes empresariais coletem registros detalhados de atividades de usuários nos boards e os utilizem para investigações ou arquivamento regulatório.

Os logs de conteúdo podem ser integrados em várias ferramentas especializadas para fins legais, de conformidade e segurança. Ao fornecer uma solução para exportar dados de atividades de usuários em larga escala, a Miro mitiga o risco do cliente e desbloqueia oportunidades para mais trabalhadores do conhecimento em toda a empresa experimentarem o poder colaborativo da Miro, enquanto observam requisitos rigorosos de segurança e conformidade.

## Dados de logs de conteúdo

Quando um usuário atualiza um widget no board, uma entrada de log é criada com informações como o horário da ação do usuário, detalhes do usuário, tipo de ação (criação, atualização, exclusão), IDs do board e do widget, e outras informações relevantes sobre o status do widget como resultado das ações dos usuários. Os logs de conteúdo *não* registram atualizações na posição, tamanho ou rotação do widget.

## Coletar logs de conteúdo

Os eventos são registrados a partir do momento em que um admin habilita a coleta de logs de conteúdo. Os eventos coletados são armazenados por 30 dias, por padrão.

Para habilitar a coleta de logs de conteúdo, execute as seguintes etapas:

1. Acesse as Configurações da Empresa.
2. No painel à esquerda, clique em **Segurança** > **Logs de auditoria**.
3. Em **Logs de auditoria**, clique na guia **Configurações**.
4. Na seção **Logs de conteúdo**, clique para ativar o botão de alternância para **Coletar logs de conteúdo**.
   ![content_logs.png](images/24936962977554_content_logs.png)
   *Ativando a coleta de logs de conteúdo*

## Acessar logs de conteúdo via API

Os Admins podem usar a [API de Logs de Conteúdo](https://developers.miro.com/reference/board-content-logs) para acessar programaticamente os dados de logs de conteúdo dentro de sua organização. Os Admins também podem coletar dados de logs de conteúdo usando integrações suportadas, como Smarsh ou Theta Lake.

Para autenticar o acesso à API, os admins podem escolher entre as seguintes opções:

- Ativar a alternância de eDiscovery em Integrações Enterprise.
- Criar um aplicativo de Plataforma e conceder a ele acesso ao escopo Content log:read.
- Instalar e autorizar uma das integrações de eDiscovery no Marketplace.

## Exclusão de logs de conteúdo

Os admins podem definir uma política de retenção para os logs de conteúdo, escolhendo entre 30, 90, 180 ou 365 dias. Por padrão, o período de retenção é definido para 30 dias.

:::note
Uma vez que os logs de conteúdo são excluídos, eles não podem ser recuperados.
:::

Para definir um período de exclusão, execute as seguintes etapas:

1. Vá para as Configurações da empresa.
2. No painel esquerdo, clique em **Segurança** > **Registros de auditoria**.
3. Em **Registros de auditoria**, clique na guia **Configurações**.
4. Em **Registros de conteúdo**, escolha uma opção na lista suspensa. Você será solicitado a confirmar sua escolha.
   ![content_logs_duration.png](images/24936976103442_content_logs_duration.png)
   *Definindo política de retenção de registros de conteúdo*
