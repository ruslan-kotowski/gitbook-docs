---
title: "Como restaurar o conte\xFAdo do board"
article_id: 360019838260
translation_id: 360019838260
locale: pt-br
sidebar_position: 18
created_at: '2021-02-24T08:56:24Z'
updated_at: '2026-01-06T19:00:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
---

Com a funcionalidade de restauração de conteúdo do board , você pode ter certeza de que a exclusão acidental de conteúdo não prejudicará a produtividade da sua equipe. Os editores de board podem restaurar facilmente objetos excluídos recentemente de seus boards.

> **Configurado por:** editores que foram explicitamente convidados aos boards [por e-mail](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) ou que têm acesso ao board porque fazem parte de um [projeto](../sharing-boards/16-projects.md) ou [time](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) na Miro
> **Disponível em:** versão para navegador, [aplicativo para desktop](../../getting-started/apps-for-devices/05-desktop-app.md), [aplicativo para tablet](../../getting-started/apps-for-devices/11-tablet-app.md)

:::warning
A funcionalidade não está disponível para os **visitantes**.
:::

:::tip
Confira [este guia](../managing-boards/12-board-history-versions.md) para aprender como restaurar uma versão da board .
:::

### Que conteúdo pode ser restaurado

- Qualquer conteúdo excluído do board durante sua sessão ativa atual e 30 minutos após o conteúdo ter sido excluído, caso a sessão tenha terminado
- Os últimos 1000 objetos excluídos do board — se a restauração ocorrer mais de 30 minutos após o conteúdo ter sido excluído
- Qualquer conteúdo excluído do board se os objetos tiverem sido selecionados e excluídos simultaneamente por um período indefinido — até os próximos 1000 objetos forem excluídos

### Como restaurar conteúdo

Para restaurar objetos excluídos, faça o seguinte:

1. Clique no ícone **Abrir barra lateral** no canto inferior esquerdo.
2. Na visão geral do board aberto, clique no ícone **Histórico do board** .
3. Clique no ícone **Restaurar** em qualquer objeto que você deseja recuperar. Os objetos excluídos reaparecerão no board (exatamente onde estavam antes de serem excluídos) e o board ampliará essa parte do board.

![restore_board_content_restore_feature.jpg](../../../../../../docs/using-miro/working-on-the-board/images/21017592941586_restore_board_content_restore_feature.jpg)
Como restaurar um objeto excluído

### Restrições

> **⚠️** Observe que haverá casos extremos quando:

- o conteúdo será restaurado em uma parte diferente do board (por exemplo, quando uma [linha de conexão](../essential-tools/05-connection-lines.md) for restaurada e a [nota adesiva](../essential-tools/14-sticky-notes.md) à qual ela estava anexada for reposicionada no board)
- o conteúdo perderá sua conexão com o objeto ao qual estava vinculado inicialmente (por exemplo, quando um [cartão](../essential-tools/02-cards.md) é excluído de uma [mesa](../advanced-tools/05-grid.md)e depois restaurado – ele será restaurado na mesma parte do board , mas não será mais anexado à mesa)
- certos conteúdos não serão restaurados. As limitações atuais incluem:

- [linhas](../essential-tools/05-connection-lines.md) que foram conectadas a objetos excluídos do board posteriormente
- texto de uma célula da tabela se ele foi removido da tabela (se a tabela foi excluída junto com o texto, ele será restaurado)
- [mapa da história do usuário](../advanced-tools/07-user-story-mapping.md) (tanto a framework quanto os cartões)
- [comentários](../facilitation-tools/asynchronous-tools/01-comments.md) deletados separadamente

  ![mceclip0.png](../../../../../../docs/using-miro/working-on-the-board/images/21017605949842_mceclip0.png)
  *O banner que você obtém se algum conteúdo não foi restaurado*

Como regra, se os objetos forem excluídos e restaurados simultaneamente, todos os links dentro desse lote também serão restaurados, mas há uma chance de que os links para objetos externos fora do board não sejam restaurados.

Observe que [duplicatas de board](../managing-boards/03-how-to-duplicate-a-board.md) não suportam a opção de restaurar objetos que foram excluídos na board original.

### Perguntas frequentes

1. *Meu conteúdo desapareceu, mas não vejo a opção de restaurar objetos excluídos. O que faço?*
   - Observe que determinados conteúdos não podem ser restaurados (consulte as limitações acima). Se o seu conteúdo incluir outros tipos de widgets, por favor:
   - certifique-se de que você abriu a board correta
   - verifique a lista de seus [templates personalizados](../../getting-started/start-here/your-first-board/02-custom-templates.md) com um nome semelhante
   - verifique o [minimapa](21-work-smarter-not-harder.md#usar-minimapa) do board para ver se há conteúdo em diferentes partes do board
   - certifique-se de que você está autorizado no Miro com o endereço de e-mail correto caso tenha vários perfis no Miro .
