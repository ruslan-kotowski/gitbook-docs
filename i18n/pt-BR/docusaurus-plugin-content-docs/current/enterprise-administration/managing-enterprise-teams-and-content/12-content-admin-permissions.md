---
title: Permissões de admin de conteúdo
article_id: 360012777280
translation_id: 360012777280
locale: pt-br
sidebar_position: 13
created_at: '2020-03-26T12:31:39Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-admin-permissions
availability:
  notes: 'Disponível para: plano Enterprise'
---

Com as permissões de admin de conteúdo, você supervisiona todo o conteúdo da sua assinatura Enterprise. Como admin de conteúdo, você pode gerenciar perfeitamente o acesso a boards, Espaços, sessões e templates, e limpar o painel excluindo boards, Espaços e sessões que não estão sendo mais usados.

### Como atribuir uma função de admin de conteúdo

1. Navegue até suas [configurações](https://miro.com/app/settings/user-profile/).
2. Na seção **Usuários**, clique em **Funções de admin**.
3. Ao lado da função **Admin de conteúdo**, clique nos três pontos (**…**) e selecione **Atribuir função** no menu suspenso.
4. Selecione o usuário ou usuários aos quais você deseja conceder direitos de admin de conteúdo. Você pode selecionar até 50 usuários.
5. Clique no botão **Atribuir** para confirmar sua seleção.
6. Para visualizar todos os usuários aos quais foi atribuída a função de admin de conteúdo, clique nos três pontos (**…**) novamente e selecione **Visualizar usuários**. Alternativamente, clique em qualquer lugar na **barra de admin de conteúdo** para ver a lista de usuários.

Para visualizar as permissões atribuídas aos admins de conteúdo, clique na **barra de admin de conteúdo**, mude para a guia **Privilégios** e role para baixo para ver todas as permissões de **conteúdo**.

## Gerenciando boards e espaços

Para informações detalhadas sobre as permissões que os admins de conteúdo têm em boards e espaços, consulte a [seção de Gerenciamento de Conteúdo na documentação de funções de admin](../../administration/get-started-as-a-miro-admin/02-understand-admin-roles-and-their-privileges.md).

Além disso, os admins de conteúdo podem:

- abrir o diálogo Compartilhar e gerenciar as configurações de compartilhamento do board ([remover e alterar o acesso de usuários](../../using-miro/sharing-boards/01-board-access-rights.md), compartilhar o board [com um time](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)/um usuário/[empresa](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)/[publicamente](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartilhar-boards-por-meio-de-um-link-publico))
- alterar os detalhes do board (nome, descrição, capa)
- mover o board para um [espaço](../../using-miro/spaces/01-spaces.md)
- mover o board para uma seção
- [excluir o board](../../using-miro/managing-boards/07-how-to-delete-a-board.md)
- [baixar o backup do board](../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)
- configurar [as configurações de conteúdo do board](../../using-miro/sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)
- configurar [permissões avançadas de compartilhamento do board](../../using-miro/sharing-boards/02-who-can-share-a-miro-board.md)
- ver qual usuário criou a [senha para um board público](../../using-miro/sharing-boards/13-password-protection-for-public-boards.md), e definir, alterar ou remover senhas de boards compartilhados publicamente
- restaurar qualquer board da [lixeira](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md).

Admins de conteúdo e admins de conteúdo do time podem mover um board para outro time onde o titular do board é membro. Se o titular do board não for membro do time de destino, você pode [transferir a titularidade do board](../../using-miro/managing-boards/05-how-to-transfer-board-ownership.md) para um membro.

Caso você não veja um board no painel, significa que o board não foi compartilhado com você, mas ainda é possível encontrá-lo: [pesquise](../../getting-started/start-here/miro-dashboard/03-how-to-search-in-miro.md) no painel pelo nome do board, pelo titular do board ou pela localização (time). Os boards que não foram compartilhados com você aparecerão com um ícone de cadeado ao lado do nome. Para gerenciar um board, clique nos três pontos no canto superior direito.

Ao tentar abrir um board por meio de um link direto ou de um resultado de pesquisa, você receberá a mensagem **Sem acesso ao board**. Na parte inferior, você verá as opções para **visualizar os detalhes do board** e **gerenciar as permissões de acesso**.

:::note
Você não pode alterar as configurações de **privados** Espaços dos quais **não** é membro, nem os verá na lista de Espaços. Se você precisar alterar as configurações de um espaço privado, peça acesso ao titular do espaço ou use as [APIs públicas da Miro](https://developers.miro.com/reference/enterprise-update-project-settings). Você pode alterar as configurações dos Espaços que *vê* no dashboard*.*
:::

## Gerenciando templates

Você pode alterar as configurações de compartilhamento do seu template ([pessoal, time ou empresa](../../getting-started/start-here/your-first-board/02-custom-templates.md)), editar os detalhes do template (nome, descrição e imagem da capa) ou excluir um template por completo.

**Como gerenciar templates personalizados**

1. Vá para o seu painel e clique em **Explorar templates** no canto superior direito.
2. Vá para **templates personalizados** na navegação à esquerda e clique em **templates de [Nome da empresa]** ou **Pessoal**.
3. Passe o mouse sobre o template que deseja editar e clique nos três pontos (...).
4. Para excluir o template, clique em **Excluir**.
5. Para gerenciar outros detalhes do template, clique em **Editar**.
6. O board será aberto. Clique no nome do template no menu do board.
7. Adicione ou edite o **Nome do template** e a **Descrição**, **Selecione a área de visualização** para a imagem de capa e mude as configurações de compartilhamento para **Pessoal**, **Time** ou **Empresa**.
8. Clique em **Salvar alterações**.
