---
title: Como excluir seu perfil
article_id: 360017571354
translation_id: 360017571354
locale: pt-br
sidebar_position: 7
created_at: '2019-02-11T10:08:54Z'
updated_at: '2026-01-07T13:30:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
availability:
  notes: 'Configurado por: titular do perfil'
---

Excluir seu perfil da Miro resultará na remoção de suas informações do nosso sistema. Observe que um perfile um time são duas coisas diferentes.

- Seu perfil representa seus dados conectados ao seu registro e endereço de e-mail.
- Um time é um espaço do qual você faz parte junto com outros membros do time, onde vocês podem criar conteúdo e armazenar seus boards.

Cada perfil pode ser associado a vários times. Se deseja excluir um time, siga o passo a passo [aqui](../../administration/team-management/06-delete-and-restore-teams.md).
:::warning
A exclusão do perfil **não pode** ser desfeita.
:::

:::warning
Observe que a exclusão do perfil não cancela suas assinaturas ativas. Para interromper futuras renovações, [cancele sua assinatura nas configurações](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md).
:::

### Como excluir seu perfil

1. Abra as [configurações do seu perfil](https://miro.com/app/settings/user-profile/).

2. Role até o final da página e escolha **Excluir meu perfil.**

![Excluir_perfil.png](../../../../../../docs/using-miro/managing-your-profile/images/21017429126546_Delete%20profile.png)
*Como excluir seu perfil*

3. Neste ponto, sugerimos salvar [backups](../import-and-export/export/05-how-to-save-board-backup.md) ou [exportar](../import-and-export/export/03-how-to-export-your-board.md) seus boards antes de excluí-los.

![profile_removal_modal.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017429125778_profile%20removal%20modal.jpg)*Mensagem de confirmação de remoção de perfil*

4. Logo depois, você receberá um e-mail com um link de confirmação. Clique no link para finalizar. Observe que você precisa estar conectado ao seu perfil da Miro no navegador ao clicar em **Excluir perfil** para concluir a exclusão do perfil.

![Profile_deletion_email.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017416055186_Profile%20deletion%20email.jpg)
*E-mail de confirmação para excluir o perfil*

### O que acontece com seu conteúdo após a remoção do perfil

Assim que seu perfil é excluído, seus boards são excluídos.

Se você for o único admin do seu time, o conteúdo será *totalmente* excluído. Os direitos de admins serão concedidos ao membro convidado primeiro, em ordem cronológica.

Se houver outros admins no time da qual você é membro, o conteúdo será excluído e reatribuído a um dos admins. Isso significa que o admin poderá [restaurar seus boards em até 90 dias](../managing-boards/08-how-to-restore-a-deleted-board.md) (usuários pagos os encontrarão na lixeira, usuários gratuitos poderão restaurá-los por meio de um link).

### Perguntas frequentes

1. *Posso excluir meu perfil se fizer login na Miro com [Single Sign-On (SSO)](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)?*
   - Sim, você pode. No entanto, se sua organização usa [SCIM](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md), seu perfil será recriado imediatamente, desde que seu e-mail seja provisionado na Miro via SCIM.
2. *Como posso alterar meu endereço de e-mail vinculado ao perfil da Miro?*
   - Use este guia: [Como alterar seu e-mail](04-how-to-change-your-email.md).
3. *Não recebo o e-mail com o link de confirmação. O que eu faço?*
   - Experimente seguir esses passos:

- Abra as caixas de **Spam, Promoções,****Lixo, Social** e **Atualizações** e verifique se o e-mail de confirmação da Miro está lá.
- Verifique se sua caixa de entrada está cheia para ter certeza de que você não atingiu o limite da sua caixa de entrada de e-mail. Se estiver cheio, talvez seja necessário excluir alguns e-mails existentes para receber novos. Após excluir os e-mails, solicite novamente a exclusão do perfil
- Também pode ser que um firewall esteja impedindo o e-mail de chegar à sua caixa de entrada. Peça ao *admin do sistema*  para incluir nossos domínios e subdomínios na lista de permissões: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) and [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). [Veja este artigo](../tools/troubleshooting/02-allowlist-miro-mailers.md) com mais informações sobre quais remetentes você deve permitir.
- Se nenhuma das soluções ajudar, [reporte o problema ao Suporte da Miro](../tools/troubleshooting/06-contacting-miro-support.md).
