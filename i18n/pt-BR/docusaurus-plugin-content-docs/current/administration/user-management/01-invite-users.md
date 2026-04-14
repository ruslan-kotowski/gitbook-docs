---
title: "Convidar usu\xE1rios"
article_id: 360017730013
translation_id: 360017730013
locale: pt-br
sidebar_position: 4
created_at: '2019-02-11T10:08:23Z'
updated_at: '2026-01-06T11:44:43Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
---

Convide pessoas para o seu time e boards com facilidade para começar a colaborar e criar juntos. Dependendo das [configurações de convite](02-invitation-settings.md), a opção de convidar novos usuários pode estar disponível apenas para admins ou para todos os membros.

:::note
Visite [este artigo](../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md) para saber como convidar usuários no plano Enterprise.
:::

## Convidar membros

Há várias maneiras de adicionar membros ao seu time.

- No seu painel. Clique em **Convidar membros** no canto superior direito
  ![invite-members-dashboard.png](../../../../../../docs/administration/user-management/images/25007019083026_invite-members-dashboard.png)
  *A opção de convidar membros a partir do painel*
- Do console de admin: Abra a guia **Todos os Usuários**. Lá você poderá ver todos os membros do time e usuários convidados.

  ![admin-invite-users.png](../../../../../../docs/administration/user-management/images/25007019084178_admin-invite-users.png)
  *A opção de convidar novos membros do console de admin*

  Clique em **Convidar novos membros** no canto superior direito e insira os e-mails dos seus convidados. Você pode inserir até 500 e-mails na janela de convite.

  ![invite_modal.jpg](../../../../../../docs/administration/user-management/images/21017416281746_invite%20modal.jpg)
  *Janela de convite*
- Neste menu, você também podecopiar[**link de convite do time**](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) - todos que seguirem o link poderão entrar no seu time (disponível nos planos [Free](../../plans-billing/miro-plans/09-free-plan.md), [Starter](../../plans-billing/miro-plans/08-starter-plan.md), [Education](../../plans-billing/miro-special-pricing/03-education-plan.md)). Os admins podem ativar ou desabilitar o link nas [configurações de convite](02-invitation-settings.md)
- No plano Free, **cada usuário** [**convidado para um board por e-mail**](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) é convidado para o time também e se torna membro do time
- No plano Starter, **cada editor** [**convidado para um board por e-mail**](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)se torna membro do time. Você verá a seguinte notificação e também terá a opção de convidar o usuário com acesso de comentarista sem adicioná-lo ao time
  ![only_members_can_edit.jpg](../../../../../../docs/administration/user-management/images/21017429340690_only%20members%20can%20edit.jpg)
  *Uma notificação que apenas membros podem editar boards neste tipo de plano*

A pessoa convidada receberá um convite por e-mail e poderá participar do trabalho imediatamente.

Se a pessoa convidada não estiver registrada na Miro, o convite ficará ativo por 30 dias. Também receberá uma notificação por e-mail no terceiro e no sétimo dia se não aceitá-lo imediatamente. Ao clicar no link do e-mail de notificação, será sugerido que ela [faça o cadastro](../../getting-started/start-here/02-how-to-register-with-miro.md). Se uma pessoa convidada não registrada não aceitar o convite em 30 dias, ele expirará e o usuário será excluído da lista de **usuários ativos**.

Os usuários registrados da Miro poderão encontrar seu time na barra lateral esquerda do seu [painel](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md) assim que você convidá-los.

Se você enviou acidentalmente um convite para um endereço de e-mail errado ou ocorreu um erro de digitação e agora quiser excluir o convite extra, clique nos três pontos ao lado do usuário convidado e escolha **Revogar convite.**

### Testes para membros convidados no plano Starter

:::note
Somente disponível para o [Starter Plan](../../plans-billing/miro-plans/08-starter-plan.md).
:::

Ao convidar membros para o time, em vez de adicioná-los imediatamente como uma licença paga, eles serão adicionados primeiro como **Membros** **gratuitos**.

A licença do usuário permanece gratuita até que o usuário convidado realize qualquer ação paga no time — abra um board/crie seu próprio board/projeto.

Uma vez que a ação paga é realizada, sua licença é convertida em teste por sete dias — nenhuma licença é consumida neste momento.

Os usuários podem ter acesso pago completo ao time gratuitamente por sete dias — isso permite a colaboração sem compromisso imediato de custo.

Durante o período de teste, os novos membros podem ser promovidos a membros com acesso total ou alterados para convidados na seção **Todos os usuários** no console de admin.

Membros convidados se tornam membros pagos se nenhuma ação for tomada até o final do teste (sete dias). Se você não quiser adicionar membros convidados como **membros com acesso total** ao time após o término do teste, pode [removê-los](08-remove-users.md) do time ou convertê-los em usuários convidados (o que significa que eles poderão visualizar e comentar no board no qual foram convidados explicitamente) a qualquer momento durante o teste.

Observe que os testes para membros só estão disponíveis para novos membros uma única vez. Após o uso do teste, os membros adicionados novamente ocuparão uma licença paga imediatamente.

Se o plano Starter for [atualizado para o plano Business](https://help.miro.com/hc/articles/360011780620-How-to-Change-Your-Plan#h_8315f4f8-9f5b-4665-b271-e438aedaf289), todos os membros convidados atuais são convertidos em membros com acesso total no momento da atualização.

O custo da nova licença **é proporcional** ao tempo restante do seu período de assinatura atual (com precisão de até um dia), de modo que suas datas de renovação para novas licenças sempre coincidirão com suas licenças existentes. Se você tiver licenças disponíveis durante o período de assinatura e adicionar um novo membro, nenhuma cobrança será aplicada. Para saber mais sobre o sistema de cobrança proporcional, consulte nosso artigo — [Cobrança e pagamentos](../../plans-billing/billing-and-payments/04-miro-billing.md).

## Convidar convidados

Você pode compartilhar seus boards com usuários por e-mail sem adicioná-los ao seu time como membros. Esses usuários serão listados como convidados nas configurações do seu time.

:::warning
Note que convidados não estão disponíveis no [plano Free](../../plans-billing/miro-plans/09-free-plan.md).
:::

:::note
A opção de convidar convidados pode ser restrita nas [configurações de convite](02-invitation-settings.md) nos planos Business.
:::

Nos planos Starter e Education, você pode convidar convidados com acesso apenas para visualização ou comentário.

No plano Business, você pode convidar convidados como visualizadores, comentaristas ou editores para os seus boards.

Tais usuários são listados como **convidados** no console de admin. Os admins podem convertê-los em membros ou excluí-los do time/revogar o convite.

Os convidados não podem criar seus próprios boards no time e não podem acessar [boards compartilhados do time](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) e projetos. Se eles solicitarem participar do time, a notificação será enviada aos admins.

:::note
Aprenda a converter membros em convidados [nesta página](../../using-miro/sharing-boards/07-collaboration-with-guests.md).
:::

## Convidar visitantes

Você também pode compartilhar seus boards com visitantes — esses usuários não são adicionados ao seu time e podem visualizar/comentar/editar boards públicos sem serem usuários registrados. A opção está disponível em todos os planos pagos. Saiba mais: [Colaboração com visitantes](../../using-miro/sharing-boards/08-collaboration-with-visitors.md).

:::note
Veja a diferença entre membros, convidados e visitantes [nesta página](../../using-miro/sharing-boards/07-collaboration-with-guests.md).
:::

## Perguntas frequentes

1. *A pessoa que convidei não recebe um e-mail com o convite que enviei. Como podem fazer para acessar meu time?*
   - Peça ao usuário para se registrar na Miro ou fazer login se tiver um perfil da Miro. O usuário encontrará seu time na barra lateral esquerda do [painel](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md).
2. *Recebi o convite para um time da Miro, mas não o vejo quando faço login. Como posso acessar o time?*
   - Tente encontrar o time na barra lateral esquerda do seu [painel](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md) e alterne para ele. Se não houver time, certifique-se de que você esteja autorizado na Miro com o mesmo endereço de e-mail que foi convidado para o time.
3. *Não há um botão Convidar membros no meu painel. Por quê?*
   - Os admins restringiram a opção de convidar novos membros nas [Configurações de convite](02-invitation-settings.md). Observe que esta opção pode ser restrita para admins do time no plano Enterprise.
4. *Posso convidar usuários sem que eles se registrem na Miro?*
   - Sim, você pode [compartilhar seus boards por meio de links públicos](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartilhar-boards-por-meio-de-um-link-publico) com usuários não registrados sem custo.
5. *O que fazer se eu convidar novos membros pagos acidentalmente?*
   - Por favor, [siga estas etapas](../../plans-billing/billing-and-payments/04-miro-billing.md).
