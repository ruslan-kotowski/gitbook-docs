---
title: "Usu\xE1rios desativados"
article_id: 360025025894
translation_id: 360025025894
locale: pt-br
sidebar_position: 1
created_at: '2019-06-19T22:16:18Z'
updated_at: '2026-02-19T10:44:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-deactivation
---

O gerenciamento avançado de usuários na Miro permite que os Admins da empresa desativem usuários ao invés de excluí-los. Usuários desativados permanecem no diretório do plano e podem ser reativados a qualquer momento.

> **Disponível para**: [Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Configuração por:** Admins da empresa

## Regras

- Usuários desativados não poderão acessar a sua conta Enterprise e suas funcionalidades.
- Se você ativou a configuração [Bloquear usuários desativados](02-block-deactivated-users.md), desativar um usuário gerenciado irá bloqueá-lo de acessar o Miro.
- Usuários desativados não poderão mais usar a opção de logon único da sua empresa para acessar, precisando voltar a métodos de autenticação padrão.
- Boards e Espaços compartilhados criados por usuários desativados *não* são atribuídos a mais ninguém e continuam disponíveis para colaboradores (a menos que durante a desativação você também remova o usuário do seu time. Nesse caso, os boards são atribuídos a um admin do time. Isso é geralmente relevante para operações de [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)).
- Todas as [notificações](../../using-miro/managing-your-profile/02-miro-notifications.md) para usuários desativados são bloqueadas.
- Outros usuários não podem compartilhar boards e Espaços com usuários desativados.
- Usuários desativados não podem ser adicionados a times dentro da sua assinatura Enterprise. Admins da empresa podem reativar usuários desativados ao convidá-los como membros, [saiba mais](05-manage-user-invitations-on-enterprise-plan.md).
- Usuários desativados não são cobrados. Suas licenças são liberadas e podem ser aplicadas a outro usuário ativo.
- Os seguintes atributos não podem ser atualizados para usuários desativados:

|  |
| --- |
| `nomeDeUsuário` |
| `tipoDeUsuário` |
| `funções.valor` |

## Desativar um usuário

Você pode desativar um usuário a qualquer momento. Ao desativar um usuário, ele é movido de um status **Ativo** para um status **Desativado** e para de consumir uma licença. Essa alteração também é refletida nas listas de usuários Ativos e Desativados nas configurações de **Usuários**.

Para desativar um usuário:

1. Abra as configurações da **Empresa**.
2. Selecione **Todos os Usuários** no menu **Usuários****.**
3. Clique no ícone de **três pontos** (**...**) à direita de um usuário que você gostaria de desativar.
4. Clique em **Desativar**.
   ![deactivate-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921781594002_deactivate-users.png)
   *A opção de desativar um usuário no plano Enterprise*

   Você também pode desativar usuários em massa. Selecione vários usuários marcando as caixas à esquerda ou aplique filtros e selecione até 50 usuários filtrados de uma vez, depois escolha **Desativar** em **Ações em massa.**
5. Marque a caixa **Reatribuir conteúdo do usuário** se você deseja transferir os boards, [templates](../../getting-started/start-here/your-first-board/02-custom-templates.md) e [Espaços](../../using-miro/spaces/01-spaces.md) do usuário. Um novo titular deve ser escolhido para cada time no qual o(s) usuário(s) selecionado(s) tinha(m) conteúdo. Reatribuir o conteúdo dos usuários não pode ser desfeito.
   ![deactivate-reassign-content.png](../../../../../../docs/enterprise-administration/user-management/images/23921804187154_deactivate-reassign-content.png)
   *A opção de reatribuir conteúdo do usuário ao desativá-los*
6. Selecione **Desativar.**

Desativar usuários não removerá seus dados na Miro. As permissões que eles possuem serão mantidas e serão restauradas assim que os usuários forem reativados.

:::note
Nota: para desativar um Admin da empresa, é necessário revogar primeiro as permissões de Admin da empresa.
:::

:::note
Se você vir uma notificação **O time deve ter pelo menos um admin** ao tentar desativar um usuário, isso significa que o usuário é o *único* admin em um time ou times no plano Enterprise. Para corrigir isso, [convidar você mesmo para esses times](05-manage-user-invitations-on-enterprise-plan.md) e [conceder direitos de admin do time a você mesmo](../../administration/user-management/06-how-to-manage-admin-roles.md). Clique no número de times do respectivo usuário para saber de quais times ele é membro.
:::

:::note
Se sua empresa usa a solução [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md), você também pode desativar usuários por meio do seu provedor de identidade. Quando um usuário é desativado pelo SCIM, seu conteúdo não é reatribuído - a opção de reatribuição é suportada apenas na interface do usuário para este cenário.
:::

### Desativação automática para convidados

Para convidados (usuários originalmente convidados para seus boards via e-mail), você pode ativar a [desativação automática](03-invitation-settings-on-enterprise-plan.md).

## Reativar um usuário

Para reativar um usuário:

1. Abra as configurações da sua **Empresa**.
2. Selecione **Todos os Usuários** no item de menu Usuários e, em seguida, a aba **Usuários Desativados****.**
3. Clique no ícone **três pontos** (...) à direita de um usuário que você gostaria de reativar.
4. Selecione **Reativar**.
5. Adicione o usuário aos times, se necessário.
6. Confirme **Reativar**.

![reactivate-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921804191762_reactivate-users.png)
*Reativando um usuário*

Quando você reativa um usuário:

- Os usuários podem iniciar sessão imediatamente
- Eles terão acesso aos boards compartilhados, aos boards do time e aos boards que criaram antes da desativação (a menos que os boards tenham sido realocados)

:::note
Nota: apenas Admins da empresa podem reativar usuários desativados.
:::

### Excluir permanentemente um usuário

Para excluir permanentemente um usuário desativado:

1. Abra as configurações da **Empresa**.
2. Clique em **Usuários** > **Todos os usuários** no menu.
3. Selecione a guia **Usuários desativados**.
4. Clique no ícone de **três pontos** (**...**) à direita de um usuário que você gostaria de excluir.
5. Selecione **Excluir**.
   ![delete-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921781612562_delete-users.png)
   *Excluindo um usuário desativado*
6. Escolha se deseja reatribuir o conteúdo do usuário ou removê-lo — escolha o novo titular e clique em **Excluir usuário** ou selecione **Excluir usuário e conteúdo**.

Você também pode excluir usuários usando ações em massa:

1. Na guia Usuários desativados, marque a caixa ao lado dos usuários que deseja excluir.
2. Clique no botão **Excluir da Empresa** no topo.

:::note
Nota: após a exclusão, os usuários podem ser convidados de volta ao seu plano como membros ou para um board como convidados por qualquer pessoa com permissão para [adicionar novos usuários](05-manage-user-invitations-on-enterprise-plan.md).
:::
