---
title: Política de compartilhamento no plano Enterprise
article_id: 360017730133
translation_id: 360017730133
locale: pt-br
sidebar_position: 7
created_at: '2019-02-11T10:09:02Z'
updated_at: '2025-11-25T16:00:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponível para: plano Enterprise Função necessária: Admin da empresa'
---

A segurança e a confidencialidade dos dados são preocupações significativas para a maioria das empresas. É por isso que nosso plano Enterprise fornece ferramentas aplicadas para controlar os riscos de segurança da informação. Isso inclui o gerenciamento de acesso mais seguro com a opção de logon único baseada em SAML e um melhor controle de direitos e permissões do usuário com capacidades de admin aprimoradas. Além disso, introduzimos restrições opcionais: compartilhamento fora dos domínios permitidos e compartilhamento por meio de link público.

:::note
As configurações da política de compartilhamento também influenciam as configurações de acesso disponíveis ao inserir boards em um aplicativo específico. Saiba mais: [Como gerenciar a política de compartilhamento do plano Enterprise para integrações inseridas](../../managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

## Restringir o compartilhamento fora dos domínios permitidos

No nível da empresa No nível do time

Depois de definir os domínios permitidos no nível da empresa, a opção de compartilhar boards fora dos domínios ficará restrita para todos os membros e times da empresa.

1. Vá para **Configurações da empresa** > **Segurança** > **Compartilhamento**.
2. Ative a opção **Restringir domínios permitidos**.
3. Adicione a lista de domínios confiáveis usados no seu plano Enterprise.

Para habilitar o compartilhamento com [colaboradores convidados](../../../using-miro/sharing-boards/07-collaboration-with-guests.md) e ignorar a lista de permissões, marque a caixa **Permitir compartilhamento com convidados fora desses domínios**.

Quando **Permitir compartilhamento com convidados fora desses domínios** está ativado, usuários com domínios fora da lista de permissões podem ter boards compartilhados com eles, mas ainda assim não poderão encontrar times em [descoberta de times.](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)

![sharing-allowed-domains.png](https://help.miro.com/hc/article_attachments/23922129664914)
*A lista de domínios confiáveis e a opção para compartilhamento com convidados fora desses domínios*

Todos os usuários que foram convidados para a assinatura antes de a configuração ser habilitada permanecem no seu plano e mantêm o acesso ao conteúdo compartilhado. No entanto, não será possível compartilhar nenhum outro conteúdo com eles.

Além disso, você pode **verificar todos os usuários na lista de permissões**, no caso de haver usuários com domínio não permitido. Você pode removê-los na seguinte janela pop-up:

![validate_against_the_allowlist.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017004911250_validate%20against%20the%20allowlist.jpg)*Usuários com endereços de e-mail que não correspondem à lista de permissões*

Ao restringir o acesso no nível do time, os usuários fora dos domínios permitidos não poderão acessar os boards nem ser convidados para o time. A opção permite que você habilite as configurações para um time específico sem restringir as regras de compartilhamento para todos os usuários Enterprise. Também fornece a opção de permitir um domínio específico para um time sem a necessidade de permitir isso para toda a empresa.

:::note
Se os domínios listados com permissão não estiverem configurados no nível do time, as configurações da empresa serão eficazes. Se a lista de permissões no nível de time estiver configurada, isso substituirá as restrições no nível da empresa. Por exemplo, se o **Domínio 1** estiver listado no nível da empresa e o **Domínio 2** estiver listado no nível do time, o **Domínio 1** não será permitido no nível do time, a menos que seja adicionado à lista de permissões no nível do time.
:::

Para configurar os domínios permitidos para um time específico:

1. Vá para **Times** e selecione o time que deseja configurar.
2. Vá para **Configurações** e role para baixo até **Domínios permitidos para o time**.
3. Habilite a opção **Restringir domínios permitidos**.
4. Insira seus domínios permitidos e clique em **Adicionar**.
   Para permitir o compartilhamento com convidados fora dos domínios, marque a caixa **Habilitar compartilhamento com convidados fora dos domínios permitidos**.

![sharing-team-allowed-domains.png](https://help.miro.com/hc/article_attachments/23922115040018)
*A opção de restringir domínios permitidos para um time específico em uma assinatura Enterprise*

Depois de restringir o compartilhamento fora dos domínios permitidos, os usuários da empresa poderão compartilhar seus boards com usuários apenas dos domínios especificados. Com a configuração habilitada, se um usuário da empresa tentar compartilhar seu board com um domínio que não é permitido, ele recebe a seguinte mensagem:

![can_t_share_outside_the_allowlist.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956416146_can%27t%20share%20outside%20the%20allowlist.jpg)*O board não pode ser compartilhado com um usuário que não esteja na lista de permissões*

:::note
Se o compartilhamento por meio de link público for permitido na sua Empresa, [os boards públicos](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartilhar-boards-por-meio-de-um-link-publico) ainda podem ser acessados por *qualquer pessoa com o link do board* (e por senha, se estiver configurada).
:::

## Restringir o compartilhamento por meio de link público

Admins da empresa podem restringir todos os usuários da empresa ou membros de um time específico de [compartilhar boards da empresa publicamente](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartilhar-boards-por-meio-de-um-link-publico). Depois que a configuração for desativada, a opção **Qualquer pessoa com o link** desaparece do menu Compartilhar dos boards na empresa ou no time.

No nível da empresa No nível do time

Para restringir o compartilhamento público para todos os usuários da empresa:

1. Vá para **Configurações da empresa** **>** **Segurança > Compartilhamento**.
2. Desabilite a opção **Boards podem ser compartilhados publicamente**.

Ao fazer isso, removerá a opção "Qualquer pessoa com o link" do menu Compartilhar do board. Isso também significa que todos os boards que foram compartilhados anteriormente com um link público ou inseridos em sites ficarão indisponíveis para usuários públicos, e suas sessões ativas nos boards serão encerradas.

Se os admins habilitarem a capacidade de compartilhar boards publicamente de novo, os usuários precisarão reativar o compartilhamento público manualmente para cada board.

Se você quiser permitir a edição em boards compartilhados publicamente, marque a opção para **Permitir edição em boards compartilhados publicamente***.* Se você *desmarcar a caixa de seleção,* o acesso público a todos os boards compartilhados anteriormente para edição pública será restrito.

:::note
O compartilhamento por meio de um link público é habilitado por padrão no nível do time e definido como "Qualquer pessoa pode visualizar e comentar" para times recém-criados. No entanto, se isso estiver **desabilitado** no nível da empresa, os times não poderão compartilhar boards publicamente, mesmo que isso seja permitido no nível do time.
:::

Para restringir o compartilhamento de boards publicamente para um determinado time:

1. Vá para **Times** e selecione o time que deseja configurar.
2. Vá para **Configurações** e role para baixo até **Configurações de compartilhamento**.
3. Em **Compartilhamento de board** > **Por link público**, você verá três opções: você pode escolher se deseja permitir o compartilhamento público para visualização e comentários apenas, para visualização, comentários e edição, ou para restringir o compartilhamento público para o time.

![sharing-public-link.png](https://help.miro.com/hc/article_attachments/23922129675666)
*A opção de configurar o compartilhamento por link público para um time em uma assinatura Enterprise*

**Expiração do link público (nível da empresa)**

Para tornar os boards compartilhados publicamente mais seguros, habilite a expiração do link público. Isso significa que quaisquer links para o board compartilhados com visitantes deixarão de funcionar após um determinado período, se o board não tiver sido aberto. Isso se aplica a todos os boards, quando a expiração do link público estiver habilitada nas configurações da empresa.

Para habilitar a expiração do link público:

1. Vá para **Configurações da empresa > Segurança > Compartilhamento**.
2. Role para baixo até a seção **Conteúdo**.
3. Selecione a caixa de seleção para **Expirar link de compartilhamento público**.
4. Defina o número de dias antes que os links inativos expirem. Você pode escolher entre 30 e 999 dias.

:::warning
Se a senha de um board for redefinida, a data de expiração do board também será redefinida para esse board.
:::

## Exigir senhas para boards públicos (nível da empresa)

Você também pode requerer senhas obrigatórias para todos os boards compartilhados publicamente por link.

1. Vá para **Configurações da empresa > Segurança > Compartilhamento**.
2. Role para baixo até a seção **Conteúdo**.
3. Marque a caixa **Exigir senhas para boards compartilhados publicamente**.

Depois que esta funcionalidade for habilitada, isso se aplicará imediatamente a boards anteriormente acessíveis com um link público e todos os boards daqui para frente não poderão ser acessados publicamente sem uma senha.

- *Para boards anteriormente acessíveis por* [*link público*](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartilhar-boards-por-meio-de-um-link-publico) *sem senhas:*
  Se os boards eram acessíveis anteriormente por um link público sem senhas, as sessões abertas serão revogadas e os visitantes serão solicitados a inserir uma senha, se tentarem acessar um link anteriormente acessível.
- *Para todos os boards:*
  Para tornar um board acessível publicamente por link, uma senha deve ser definida pelo titular do board ou pelo [admin de conteúdo](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md). Se uma senha for removida, a opção **Qualquer pessoa com o link** no menu Compartilhar do board será convertida para **Sem acesso**. Os membros do time com direitos de edição podem compartilhar um board por meio de um link público se a senha já tiver sido definida. Caso contrário, eles devem entrar em contato com o titular do board para definir uma senha.
- Quando a opção "*Expirar quando o board estiver inativo por 'x' dias*" estiver definida, um ícone de relógio aparecerá na caixa de diálogo Compartilhar, com uma mensagem de que o acesso público desaparecerá após o número especificado de dias.
  ![1-2.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978811282_1-2.png)
*Opção de compartilhamento público no plano Enterprise com senhas obrigatórias*

Você também pode exigir que as senhas sejam complexas e especificar quais requisitos as senhas devem atender. Esses podem incluir:

- Comprimento mínimo de senha (de 6 a 14 caracteres; o padrão é 8).
- Letras maiúsculas e minúsculas.
- Números.
- Caracteres especiais.

![complex-board-password.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956422418_complex-board-password.png)
*Configurações para senhas complexas de boards*

## Restringir o compartilhamento em todos os times e em toda a empresa (nível de time)

:::note
O compartilhamento para todo o time e empresa é habilitado por padrão, se as configurações não tiverem sido personalizadas pelo Admin da empresa.
:::

Admins da empresa do plano Enterprise podem também habilitar/desabilitar o compartilhamento em toda a empresa ou em todo o time.

1. Vá para **Times** e selecione o time que deseja configurar.
2. Vá para **Configurações** e role para baixo até **Configurações de compartilhamento**.
3. Em **Compartilhamento do board,** escolha se o compartilhamento com um time é permitido ou não permitido. Para configurações em toda a empresa, escolha se a empresa pode visualizar e comentar em boards compartilhados, visualizar/comentar/editar ou se o compartilhamento não é permitido.![sharing-board-sharing.png](https://help.miro.com/hc/article_attachments/23922115056530)*Configurações de compartilhamento do board no plano Enterprise*

A habilitação do compartilhamento do board com um time permite que seus membros compartilhem facilmente seus boards e projetos com toda a equipe.

A desabilitação desta opção a removerá do menu Compartilhar de boards e projetos do time. Os boards e projetos compartilhados anteriormente não estarão mais disponíveis para os usuários do time, a menos que compartilhados por outros meios.

Se o admin reabilitar a capacidade de compartilhar com o time, os boards e projetos já compartilhados não serão compartilhados de forma automática com o time e os usuários deverão voltar a compartilhá-los manualmente.

![1-3.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978812178_1-3.png)
*A opção de compartilhar um board com o time pode ser ocultada no menu Compartilhar*

Os usuários dos planos Enterprise com a [Privacidade do Time](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) desabilitada também podem [compartilhar seus boards com toda a empresa para visualização, comentário ou edição com apenas um clique](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md). Você pode bloquear esta opção para um time específico ao selecionar **Não permitido** na configuração **Com toda a empresa**. Ou você pode permitir o compartilhamento no modo somente visualização e comentário ou também para edição.

Observe que, se a [Privacidade do Time](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) estiver habilitada na sua empresa, a opção de compartilhar boards com toda a empresa não estará disponível, mesmo que isso seja permitido no nível do time.

![1-4.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956423442_1-4.png)
*A opção de compartilhar o board com toda a empresa pode ser ocultada no menu Compartilhar*

## Restringir a capacidade de mover boards para outros times (nível de time)

:::note
A capacidade de mover boards para outros times é habilitada por padrão se a configuração não tiver sido personalizada pelo Admin da empresa.
:::

Quando um Admin da empresa não permite mover boards para um time, os membros desse time não poderão mover boards para outros times nem fora desse time. A configuração é definida para cada time em **Configurações do time > Permissões**.

:::note
Os usuários que não são admins não podem mover boards para um time se a [opção de criar boards estiver restrita](../../managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md) para eles no time de destino.
:::

![sharing-moving-boards.png](https://help.miro.com/hc/article_attachments/23922115059602)
*A opção de restringir a movimentação de boards dentro e fora do time*

## Restringir o compartilhamento de templates personalizados para toda a empresa

> **Disponível para:** plano Enterprise
> **Quem pode fazer isso:** Admins da empresa

Admins da empresa podem permitir ou restringir o compartilhamento de templates personalizados no nível da empresa. Quando o compartilhamento é restrito, os membros do time não poderão compartilhar um template personalizado com a empresa sem a aprovação do admin.

1. Vá para **Configurações da empresa** > **Segurança** > **Configurações**.
2. Role para baixo até **Funções e permissões**.
3. Habilite a opção **Restringir o compartilhamento de templates da empresa**.

![sharing-restrict-templates.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978813202_sharing-restrict-templates.png)
*A opção de restringir o compartilhamento de templates da empresa*

## Perguntas frequentes

Os membros recebem notificações quando Admins da empresa alteram as configurações de compartilhamento acima mencionadas no nível do time ou da empresa?

Não, não são enviadas notificações nesses casos. As regras são aplicadas imediatamente.

Existe algum painel onde podemos acompanhar todos os boards que estão sendo compartilhados com um link público?

Atualmente, não há esse tipo de painel.

Desabilitei a opção de restringir domínios permitidos, mas ainda não conseguimos compartilhar os boards com usuários fora dos domínios permitidos. Como posso resolver isso?

É possível que a configuração ainda esteja habilitada no nível da empresa/time. Verifique se a restrição está desabilitada nas configurações da empresa ou do time.
