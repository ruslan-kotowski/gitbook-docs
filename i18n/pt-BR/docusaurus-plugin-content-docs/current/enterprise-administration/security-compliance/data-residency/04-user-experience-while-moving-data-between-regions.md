---
title: Experiência do usuário ao mover dados entre regiões
article_id: 25075857856658
translation_id: 25075857856658
locale: pt-br
sidebar_position: 4
created_at: '2025-03-04T08:51:38Z'
updated_at: '2025-05-09T08:47:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Quem pode fazer isso: Todos os usuários Quais planos: Enterprise Quais plataformas:
    navegador, desktop, dispositivo móvel'
---

Este artigo descreve a experiência do usuário durante uma migração de dados entre regiões, tanto para processos com [exportação e importação manual](../../canvas-25-admin-features/data-residency/05-move-data-between-regions-–-automated-migration.md) como [automática](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md).

## Experiência do usuário durante a migração automática (BETA)

As seções a seguir descrevem o que esperar antes, durante e depois de uma transferência automática de dados entre regiões.

### Antes da migração automática

Duas semanas antes da migração, todos os usuários da sua organização Enterprise recebem as seguintes notificações:

- **Banner no produto**
  Exibe a data e a duração prevista da migração no fuso horário local.
- **Notificação por e-mail**
  Descreve a próxima manutenção programada para todos os usuários da sua organização Enterprise.

:::note
Se você for membro de várias contas da Miro, suas outras contas permanecerão acessíveis durante a migração.
:::

### Durante a migração automática

Uma migração automática requer cerca de oito horas de inatividade.

Durante uma migração automática, não é possível acessar os dados da sua organização Enterprise, nem boards, times e configurações.

O painel da Miro mostra um aviso informando que uma migração de dados da sua organização está em andamento. Durante o processo de migração, você não terá acesso aos boards, times ou configurações da organização.

:::tip
Se você for membro de várias organizações, poderá trocar a organização no seu painel para continuar usando a Miro.
:::

### Após a migração automática

Assim que a migração for concluída, você recebe um e-mail de confirmação. Uma mensagem aparece no seu painel da Miro confirmando a migração.

Se ocorrer uma falha durante a migração, você receberá uma notificação por e-mail. Você pode continuar usando a Miro na região da UE, entrando em [miro.com](https://miro.com).

### Redirecionamentos de boards após a migração automática

Os boards marcados como favoritos na sua região anterior serão automaticamente redirecionados para a nova região, com um URL atualizado.

## Experiência do usuário durante a exportação e importação manual

Os usuários devem exportar manualmente os backups dos boards da sua região de origem e importá-los para a região de destino.

**Mais informações:** Veja [Mover dados entre regiões: exportação e importação manual](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md).

## Colaboração entre regiões

Os usuários da Miro são regionais. Para colaborar com usuários de organizações em outras regiões, é necessário ter um perfil de usuário em cada uma delas.

Por exemplo, se você é um usuário da região da UE e quer colaborar com usuários de uma organização da região da Austrália, deve criar um perfil de usuário à parte em [au.miro.com](https://au.miro.com/).
