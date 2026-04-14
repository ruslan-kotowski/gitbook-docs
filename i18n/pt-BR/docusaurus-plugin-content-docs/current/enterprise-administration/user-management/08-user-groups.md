---
title: Grupos de usuários
article_id: 30658859384594
translation_id: 30658859384594
locale: pt-br
sidebar_position: 8
created_at: '2025-10-30T13:00:25Z'
updated_at: '2026-01-20T13:17:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: groups
availability:
  notes: 'Quem pode fazer: (Configuração) Admins da empresa, Membros do Team Quais
    planos: Enterprise Quais plataformas: Navegador, Desktop, Mobile'
---

Como Admin da empresa, Grupos de Usuários permitem que você gerencie o acesso ao conteúdo para grupos de usuários, em vez de compartilhar com cada membro individualmente. Todos os membros da sua organização podem ver e compartilhar seu conteúdo com os Grupos de Usuários que você cria.

Este artigo explica como criar, gerenciar e compartilhar conteúdo com Grupos de Usuários. Para mais informações gerais sobre essa funcionalidade, consulte a [visão geral de Grupos de Usuários](07-user-groups-overview.md).

:::note
Para saber mais sobre como gerenciar Grupos de Usuários via SCIM, contate seu Gerente de Sucesso do Cliente da Miro ou Suporte.
:::

## Guia do Admin da empresa

### Criar um Grupo de Usuários

1. Como Admin da empresa, vá para o Console de Admin.
2. Vá para **Usuários** > **Grupos**.
3. No canto superior direito, clique em **+ Criar grupo**.
   O modal **Criar novo grupo** será aberto.
4. Dê um nome ao seu grupo.
5. (Opcional) Adicione uma descrição para o seu novo grupo. Você pode adicionar ou editar sua descrição mais tarde.
6. Clique em **Criar grupo**.
   O seu novo grupo é adicionado à visualização de **Grupos**.

### Adicionar usuários a um grupo de usuários

1. No console de admin, vá para **Usuários** > **Grupos**.
2. Para o grupo de usuários que você deseja gerenciar, selecione os três pontos (**...**) no final da linha.
3. Clique em **Adicionar usuários**.
   O modal **Adicionar usuários** será aberto.
4. Para localizar seu(s) usuário(s), pesquise por nome ou e-mail.
5. Marque cada usuário que deseja adicionar.
6. Clique em **Adicionar usuários selecionados**.
   Cada usuário selecionado é adicionado ao seu grupo de usuários.

### Adicionar grupo de usuários aos times

1. No console de admin, vá para **Usuários** > **Grupos**.
2. Para o grupo de usuários que deseja gerenciar, selecione os três pontos (**...**) no final da linha.
3. Clique em **Adicionar a times**.
   O modal **Adicionar grupo a times** é aberto.
4. Para localizar seu(s) time(s), busque pelo nome.
5. Marque cada time ao qual deseja que seu grupo de usuários se junte.
6. Clique em **Adicionar**.
   Seu grupo de usuários se juntou a cada time selecionado.

   > ✏️ Os membros do grupo de usuários têm acesso de edição a todo o conteúdo em cada time selecionado.

### Editar um grupo de usuários

1. No console de admin, vá para **Usuários** > **Grupos**.
2. Para o grupo de usuários que você quer gerenciar, selecione os três pontos (**...**) no final da linha.
3. Clique em **Editar grupo**.
   A modal **Editar grupo** abre.
4. (Opcional) Renomeie seu grupo.
5. (Opcional) Adicione uma descrição para o seu novo grupo.
6. Clique em **Salvar**.

### Excluir um grupo de usuários

:::warning
A exclusão de um grupo de usuários não pode ser desfeita. Ao excluir um grupo de usuários, alguns usuários podem ser removidos de alguns times.
:::

1. No console de admin, vá para **Usuários** > **Grupos**.
2. Para o grupo de usuários que você deseja gerenciar, selecione os três pontos (**...**) no final da linha.
3. Clique em **Excluir grupo**.
   O modal **Excluir \{nome do grupo de usuários\}** será aberto.
4. Clique em **Excluir**.
   O grupo de usuários é excluído permanentemente.

## Guia do usuário

### Compartilhar um board com um grupo de usuários

Os membros do time podem compartilhar um board com qualquer Grupo de Usuários na organização. O board é compartilhado com todos os membros desse Grupo de Usuários.

Siga estes passos:

1. No board do Miro, clique em **Compartilhar** no canto superior direito.
   Um modal será aberto.
2. Insira o nome do seu Grupo de Usuários alvo.
3. Selecione o Grupo de Usuários das opções auto-populadas.
4. (Opcional) Atualize as permissões. Padrão: **Pode editar**.
5. (Opcional) Adicione uma mensagem personalizada.
6. Clique em **Enviar convites**.
   Cada usuário no Grupo de Usuários receberá um e-mail de convite para acessar o seu board.

### Compartilhar um Espaço com um Grupo de Usuários

Os membros do time podem compartilhar um Espaço com qualquer Grupo de Usuários em sua organização e especificar permissões. O Espaço é compartilhado com todos os membros daquele Grupo de Usuários.

Siga estes passos:

1. No painel da Miro, para o Espaço que você deseja compartilhar, clique nos três pontos verticais para abrir o menu **Opções**.

   > 💡 Alternativamente, na barra lateral de Espaços, clique nos três pontos verticais no topo para abrir o menu **Opções**.
2. Clique em **Compartilhar**.
   A modal **Compartilhar Espaço '\{Space Name\}'** será aberta.
3. Insira o nome do Grupo de Usuários.
4. (Opcional) Atualize as permissões. Padrão: **Pode editar**.
5. (Opcional) Adicione uma mensagem personalizada.
6. Clique em **Enviar convites**.
   Cada membro do Grupo de Usuários receberá um convite por e-mail para acessar seu Espaço.

:::note
Os membros adicionados ao Grupo de Usuários têm acesso automaticamente aos Espaços compartilhados. Para os membros removidos do Grupo de Usuários, o acesso é automaticamente revogado.
:::
