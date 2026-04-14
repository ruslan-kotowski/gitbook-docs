---
title: "Gerenciar an\xFAncios do admin"
article_id: 31013703080722
translation_id: 31013816591762
locale: pt-br
sidebar_position: 6
created_at: '2025-11-12T21:54:12Z'
updated_at: '2026-03-19T07:59:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: in-app-notifications
---

Use a página Anúncios para visualizar todos os anúncios, acompanhar seu status e gerenciá-los ao longo de seu ciclo de vida.

## Visualizar e entender anúncios

Acesse **Console de Admin > Organização > Anúncios**. A tabela de anúncios oferece uma visão geral de todos os anúncios, incluindo o nome, status, datas, público-alvo e criador.

## Status dos anúncios

| Status | Descrição |
| --- | --- |
| **Rascunho** | Salvo, mas ainda não publicado. |
| **Agendado** | Publicado e programado para aparecer em uma data futura. |
| **Ativo** | Atualmente visível para os usuários. |
| **Encerrado** | Não está mais ativo após a data de término. |
| **Cancelado** | Parado antes da data de início. |

## Atualizar anúncios

### Editar um anúncio

1. Vá para **Anúncios**.
2. Selecione o anúncio.
3. Clique em **Editar**.
4. Atualize os detalhes do anúncio.
   Você pode atualizar a mensagem, texto do link, URL do link, público-alvo, agendamento ou prioridade.
5. Clique em **Publicar**.
   As mudanças são aplicadas imediatamente, incluindo para anúncios ao vivo.

### Publicar um anúncio

1. Abra o anúncio.
2. Revise os detalhes.
3. Clique em **Publicar**.
   O anúncio se torna **Programado** se a data de início for no futuro, ou **Disponível** se a data de início for no presente ou no passado.

## Reutilizar anúncios

### Duplicar um anúncio

1. Na lista de anúncios, abra o menu **Ações**.
2. Clique em **Duplicar**.
3. Atualize os detalhes do anúncio.
   Altere o nome, datas, público ou outros campos, conforme necessário.
4. Clique em **Salvar rascunho** ou **Publicar**.
   **Salvar rascunho** armazena o anúncio sem publicar.
   **Publicar** torna o anúncio ativo ou o agenda, com base nas datas selecionadas.

## Controlar o ciclo de vida do anúncio

### Cancelar um anúncio

1. Na lista de anúncios, abra o menu **Ações**.
2. Clique em **Cancelar**.

Você pode cancelar um anúncio em qualquer status. O anúncio não é mais exibido para os usuários.

### Excluir um anúncio

1. Na lista de anúncios, abra o menu **Ações**.
2. Clique em **Excluir**.

O anúncio é removido permanentemente e não pode ser recuperado.

## Rastrear alterações

Cada anúncio inclui uma seção de histórico que mostra eventos de ciclo de vida e atualizações.

O histórico inclui ações como:

- Criado
- Publicado ou lançado
- Editado
- Cancelado

Essas ações também são registradas nos logs de auditoria.
