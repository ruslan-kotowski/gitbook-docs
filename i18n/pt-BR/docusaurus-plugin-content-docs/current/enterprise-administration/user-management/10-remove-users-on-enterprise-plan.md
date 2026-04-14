---
title: "Remover usu\xE1rios do plano Enterprise"
article_id: 360017730193
translation_id: 360017730193
locale: pt-br
sidebar_position: 10
created_at: '2019-02-11T10:09:21Z'
updated_at: '2025-11-04T11:30:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-management
---

O gerenciamento avançado de usuário no Miro permite que os admins filtrem e gerenciem facilmente todos os usuários em um só lugar. Como admin, você pode remover usuários extras a qualquer momento.

> **Disponível para:** Plano Enterprise

### Excluir um usuário de um time

Para excluir um usuário de uma time específica na sua assinatura Enterprise , abra as Configurações da Team passando o mouse sobre o nome da time no painel e clicando no ícone **Membros da Team** .

A aba **Usuários** será aberta. Encontre o membro do time que você gostaria de excluir e selecione **Excluir da time** no menu de **três pontos** (**...**).

![delete-users-from-team.png](../../../../../../docs/enterprise-administration/user-management/images/23921781390482_delete-users-from-team.png)

*Excluir um usuário de um time*

Observe que excluir um usuário de um time não o exclui completamente da organização Enterprise e não libera uma licença. Para excluir um usuário da organização (Empresa), siga os passos abaixo.

Você também pode selecionar vários usuários ou até 50 usuários da time de uma só vez e excluí-los em massa.

### Excluir um usuário da empresa

:::warning
Antes de excluir usuários, verifique se você habilitou a configuração [Bloquear usuários desativados](02-block-deactivated-users.md) . Usuários excluídos são tratados de forma diferente de usuários desativados.
:::

Para remover completamente um usuário do seu plano Enterprise , primeiro você precisa [desativá-](01-deactivated-users.md) lo na seção **Usuários ativos**da**empresa** configurações. Depois disso abra Aba**Usuários desativados** e escolha **Excluir** no menu de **três pontos** (**...**) na linha do usuário.

Você também pode selecionar até 50 usuários em massa e excluí-los todos de uma vez.

Se o usuário for o titular de alguns boards/[templates](../../getting-started/start-here/your-first-board/04-templates.md)/[projetos](../../using-miro/sharing-boards/16-projects.md) criados no plano Enterprise , você poderá escolher a quem o conteúdo será reatribuído (você pode selecionar um admin ou um usuário não administrador). Se você escolher **Excluir usuário e conteúdo**, o conteúdo do usuário será removido. Os admins poderão [restaurar os boards excluídos](../../using-miro/managing-boards/08-how-to-restore-a-deleted-board.md) dentro de 90 dias após a exclusão.

O usuário excluído perderá todo o acesso aos ativos do seu plano imediatamente (sem ser notificado). Observe que eles manterão o acesso aos boards que foram compartilhados [com um link público](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartilhar-boards-por-meio-de-um-link-publico) se o usuário salvou os links para esses boards específicos.

Se você estiver removendo um usuário gerenciado da sua assinatura Enterprise , ele será contado como [não capturado](../canvas-25-admin-features/domain-control/01-domain-control.md) nas configurações de controle do seu domínio.
