---
title: Conectar times da organização às configurações padrão do Jira
article_id: 26438407676434
translation_id: 26441945811858
locale: pt-br
sidebar_position: 6
created_at: '2025-05-02T14:36:04Z'
updated_at: '2025-10-21T12:08:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Quem pode fazer: Admins da empresa Quais planos: Enterprise Quais plataformas:
    Navegador, Desktop'
---

Os Admins da empresa podem conectar vários times da sua organização de uma vez às configurações globais do Jira, o que substitui as configurações definidas no nível do time.

## Pré-requisitos

- Você deve ter a função de Admin da empresa na Miro.
- Assegure-se de ter uma conexão padrão com um [Conectar ao Jira Data Center usando OAuth 2.0](https://help.miro.com/hc/articles/25753304280466).

## Conectar times às configurações padrão do Jira

1. No seu painel da Miro, selecione seu avatar no canto superior direito e vá para **Console de Admin** | **Configurações**.
2. Na barra lateral à esquerda, vá para **Aplicativos e integrações ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)** > **Aplicativos** > guia **Gerenciar aplicativos**.
3. Verifique se **Permitir somente aplicativos da lista abaixo** está ativado.
4. Na coluna **Aplicativo**, para **Cartões Jira**, selecione **Configurações**.
5. Em **Adicionar times à instância padrão**, selecione cada time que deseja conectar ou clique em **Selecionar todos**.

   > ✏️ A lista só mostra os times que não usam as configurações da organização global.
6. Clique em **Adicionar <número de times> ao padrão**.

   > ✏️ Os usuários que ainda não usam a instância global do Jira na sua organização serão migrados e devem se reautenticar.

   > ✏️ Na primeira vez que tentarem realizar qualquer ação relacionada ao Jira na Miro, os usuários migrados de outra instância do Jira devem se autenticar novamente.

## Perguntas frequentes

**Os times continuarão usando a conexão global com o Jira por tempo indefinido?**

Não. Você pode alterar as configurações do Jira para um time quando quiser.

**Quais times devem usar a conexão global do Jira?**

Geralmente, é preferível usar as configurações da organização para facilitar seu trabalho. Se alguma das conexões do seu time compartilhar as mesmas configurações da organização, recomendamos integrar esses times às configurações padrão da organização.
