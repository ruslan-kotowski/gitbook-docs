---
title: Configurações de convite
article_id: 360022258119
translation_id: 360022258119
locale: pt-br
sidebar_position: 3
created_at: '2021-06-03T10:01:33Z'
updated_at: '2025-06-02T11:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
availability:
  notes: 'Quem pode fazer isso: (Free, Starter, Education) Admins do time, (Business,
    Enterprise) Admins da empresa, Admins do time'
---

Admins podem configurar permissões de convite para um time e restringir a capacidade de usuários não-admins de [convidar novos membros](01-invite-users.md) e alterar o tamanho da assinatura.

Acesse o console de admin clicando no seu avatar de perfil no canto superior direito e depois clicando em **console de admin**.

Na guia **Segurança** > **Permissões**, role para baixo até **Configurações de convite**. A configuração parece diferente em diferentes planos da Miro.

Nos planos Free, Starter e Education, você também pode ativar ou desabilitar o link de convite do time, que permite que os usuários entrem no seu time seguindo um link especial que pode ser copiado nos modais de Compartilhamento e Convite dos boards. [Saiba mais](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

![invitation-settings.png](../../../../../../docs/administration/user-management/images/25007070132626_invitation-settings.png)
*Configurações de convite no plano Starter*

Nos planos Starter e Education, apenas membros podem editar boards. Assim, se um usuário que não tem permissão para convidar membros tentar compartilhar um board com um editor que não é membro do time, verá o pop-up.

## Configurações de convite para Business e Enterprise

Nos planos Business e Enterprise, os Admins da empresa podem adicionalmente permitir ou proibir [convidados](../../using-miro/sharing-boards/07-collaboration-with-guests.md).

![inv-settings-invitation.png](../../../../../../docs/administration/user-management/images/21855329470994_inv-settings-invitation.png)
*Configurações de convite no plano Enterprise*

Os [Admins da empresa](../get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md) do plano Business e do plano Enterprise podem configurar as configurações de convite para cada time dentro da assinatura.

Siga estas etapas:

1. Vá para **Console de admin**.
   No seu painel da Miro, clique no seu avatar no canto superior direito e selecione **Console de admin**.
2. Clique em **Times**.
3. Em **Team name**, selecione um time.
   O painel de configurações do time abre.
4. Clique em **Configurações**.
5. Em **Convite**, selecione quem pode convidar usuários para este time.
   > ⚠️ (Business) Suas licenças são automaticamente aumentadas quando um novo usuário é adicionado. Se você permitir que qualquer pessoa convide novos usuários, então qualquer um pode incorrer em novas licenças adicionadas à sua assinatura.
6. Selecione **Permitir** ou **Não permitir** para convidados.
7. No canto superior direito, clique no **X** para fechar o painel de configurações do time.
   Suas configurações foram salvas.

Se os usuários não tiverem permissão para convidar novos membros, eles não verão a opção em seus painéis. Um pop-up é mostrado para usuários nos planos Business se convidados não forem permitidos.

Para saber mais sobre como funcionam as configurações de convite no plano Enterprise, confira [este artigo](../../enterprise-administration/user-management/03-invitation-settings-on-enterprise-plan.md).
