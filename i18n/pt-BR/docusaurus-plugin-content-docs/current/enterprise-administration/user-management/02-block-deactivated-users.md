---
title: "Usu\xE1rios desativados perdem todo o acesso \xE0 Miro"
article_id: 11846063620882
translation_id: 11846063620882
locale: pt-br
sidebar_position: 2
created_at: '2023-06-06T12:47:53Z'
updated_at: '2025-11-04T11:30:33Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-deactivation
---

Quando um Admin da empresa [desativa um usuário](01-deactivated-users.md), ele perde o acesso à assinatura Enterprise e não consegue mais efetuar login com SSO. Usuários desativados podem continuar acessando outras assinaturas do Miro com o mesmo e-mail.

Você pode bloquear ainda mais [usuários gerenciados](06-managed-users-on-enterprise-plan.md) desativados para impedir que eles acessem outras assinaturas do Miro .

> **Disponível para:** plano Enterprise
> **Quem pode fazer isso:** Admins da empresa

## Bloqueando usuários desativados

**Quando a configuração estiver ativada:** usuários gerenciados desativados serão bloqueados do acesso a qualquer assinatura do Miro . Esta configuração se aplica a todos os usuários que estão atualmente desativados na sua assinatura e a todos os usuários que você desativar no futuro.

**Quando a configuração é desativada:** usuários gerenciados desativados podem continuar acessando outras assinaturas do Miro com seu e-mail e senha corporativos.

:::tip
Habilitar a configuração **Bloquear usuários desativados** afetará todos os usuários desativados anteriormente na sua assinatura. Antes de habilitar a configuração ou verificar novos domínios enquanto a configuração estiver habilitada, recomendamos primeiro revisar sua lista de usuários desativados para entender quem será bloqueado.
:::

### Como bloquear usuários desativados

1. Vá para **Configurações** > **Segurança** > **Domínios gerenciados**
2. Ativar/ **desativar bloqueio de usuários**
   *![Bloquear usuários desativados no console de admin do Enterprise](../../../../../../docs/enterprise-administration/user-management/images/23921780232082_image.png)*
   *Bloqueie usuários desativados no console de admin do Enterprise .*

## O que os usuários bloqueados veem?

Usuários gerenciados desativados e bloqueados serão imediatamente desconectados. Quando tentarem efetuar login na próxima vez, verão uma das seguintes mensagens:

![Conta](../../../../../../docs/enterprise-administration/user-management/images/21017430794898_Account%20deactivated.png)*O usuário tentou efetuar login com e-mail e senha*

![E-mail](../../../../../../docs/enterprise-administration/user-management/images/21017417753746_Email%20not%20associated%20with%20an%20SSO%20account.png)*O usuário tentou efetuar login com SSO*

## Desbloqueando usuários desativados

Os Admins da empresa podem desbloquear usuários de três maneiras:

**Reativar ou convidar novamente o usuário**

Reative ou convide novamente o usuário para sua assinatura Enterprise onde o domínio é verificado. Este usuário obtém acesso a todas as assinaturas das quais faz parte. Se eles não estiverem usando ativamente sua assinatura Enterprise , você pode atribuir a eles uma licença [Free restrita](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) . Saiba mais sobre como convidar membros em [Gerenciar convites no plano Enterprise](05-manage-user-invitations-on-enterprise-plan.md).

**Desative a configuração Bloquear usuários desativados**

Isso desbloqueará todos os usuários gerenciados desativados, e eles poderão efetuar login no Miro com seu e-mail corporativo. Isso não lhes dará acesso à sua assinatura Enterprise . Esta opção só funciona se o usuário não tiver sido excluído da assinatura. Acesse as configurações **de Domínios gerenciados** e desative **Bloquear usuários desativados.**

**Excluir o domínio**

Você pode excluir o domínio da sua lista de domínios verificados. Isso desbloqueará todos os usuários gerenciados daquele domínio, a menos que eles tenham sido excluídos da assinatura. Para excluir um domínio, nas configurações da sua empresa, vá para **Segurança e conformidade**> **Colaboração** > clique em **Remover** ao lado do nome do domínio.

> **✏️** Bloquear o acesso de um usuário ao Miro significa que ele não poderá fazer login em outras assinaturas do Miro com seu e-mail e senha corporativos, ou via SSO. O desbloqueio não concede ao usuário acesso à assinatura Enterprise, a menos que o acesso seja explicitamente concedido.

## Cenários de usuário bloqueados

Use esta tabela para entender mais sobre o que acontece em diferentes cenários de usuário bloqueados.

|  |  |
| --- | --- |
| Ação | Resultado |
| **O usuário está bloqueado** | |
| O admin da empresa desativa o usuário gerenciado | O usuário está bloqueado |
| Um membro da sua assinatura Enterprise tenta convidar um usuário gerenciado **desativado** para sua time | O usuário permanece bloqueado. O autor do convite verá uma mensagem informando que o usuário foi desativado. Eles não podem ser convidados. Os admins podem reativar usuários. |
| O admin da empresa desativa e exclui um usuário gerenciado | O usuário está bloqueado |
| O usuário gerenciado está desativado no IdP | O usuário está bloqueado |
| O usuário gerenciado é removido do aplicativo da Miro no IdP | O usuário está bloqueado |
| O admin da empresa adiciona e verifica um domínio enquanto a configuração está habilitada | Todos os usuários dos domínios recém-verificados na lista de desativados serão bloqueados. |
| Alguém de outra assinatura (qualquer outra assinatura além daquela em que o domínio é verificado) tenta convidar seu usuário gerenciado desativado para sua assinatura.   Isso também se aplica mesmo que o usuário gerenciado seja excluído da sua assinatura. | O usuário permanece bloqueado. Eles podem ser convidados para outras assinaturas e receberão notificações de convite, mas não poderão efetuar login no Miro. |
| **O usuário está desbloqueado** | |
| O admin da empresa reativa um usuário gerenciado desativado | O usuário está desbloqueado |
| O admin da empresa convida um usuário gerenciado desativado ou excluído de volta à assinatura. | O usuário é convidado e desbloqueado |
| O usuário gerenciado é reativado via SCIM | O usuário está desbloqueado |
| O usuário gerenciado é adicionado novamente ao aplicativo da Miro no IdP e sincronizado via SCIM | O usuário está desbloqueado |
| Um membro da sua assinatura Enterprise convida um usuário gerenciado **excluído** para sua time | Se o [As configurações de convite](03-invitation-settings-on-enterprise-plan.md) permitem que os membros convidem novos usuários para suas times, o usuário é convidado e desbloqueado. |
| **Cenários mistos** | |
| O domínio verificado é excluído do Controle de Domínio | Usuários desativados do domínio excluído são desbloqueados. Usuários excluídos permanecem bloqueados e precisam ser convidados novamente para a assinatura para serem desbloqueados. |
| A configuração é desabilitada após ser habilitada. | Todos os usuários desativados gerenciados são desbloqueados. Usuários excluídos permanecem bloqueados e precisam ser convidados novamente para a assinatura para serem desbloqueados. |

## Perguntas frequentes

**O que outras assinaturas podem ver sobre usuários desativados bloqueados?**

Desativar o usuário na sua assinatura irá desativá-lo apenas na sua assinatura Enterprise . O bloqueio afetará apenas a capacidade de efetuar login no Miro usando o e-mail corporativo. O usuário parece ativo em outras assinaturas, mas não consegue fazer login com seu endereço de e-mail corporativo.

**Se um usuário for desativado e excluído, ele será bloqueado do acesso ao Miro depois que a configuração for ativada?**

Os usuários permanecerão bloqueados após você [excluí-los da sua assinatura](01-deactivated-users.md). A exclusão do usuário terá algumas implicações - para mais informações, revise nossos cenários de usuário bloqueados e desativados. A única maneira de desbloquear um usuário excluído é convidá-lo novamente para a assinatura com o domínio verificado. Se o usuário for excluído da assinatura antes de habilitar a configuração, ela não se aplicará a ele.

**Esta configuração afeta usuários não gerenciados?**

Não. Somente usuários gerenciados são afetados por esta configuração.
