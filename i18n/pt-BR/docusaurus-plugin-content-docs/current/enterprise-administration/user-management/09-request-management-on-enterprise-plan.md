---
title: Gerenciamento de solicitações no plano Enterprise
article_id: 360017237379
translation_id: 360017237379
locale: pt-br
sidebar_position: 9
created_at: '2020-10-27T12:09:40Z'
updated_at: '2026-02-19T11:00:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: access-request-management
availability:
  notes: 'Relevante para: plano Enterprise Quem pode fazer: Admin da empresa'
---

Na Miro, solicitações de licenças, acesso de time e organização e logon único (SSO) são enviadas aos Admins da empresa por e-mail por padrão. Com recursos avançados de gerenciamento de solicitações, os Admins da empresa podem personalizar como essas solicitações são recebidas e tratadas.

### Tipo de solicitação

Os tipos de solicitação se enquadram em quatro categorias:

- Solicitações para fazer parte de sua organização
- Solicitações para fazer parte de um time
- Solicitações para uma licença
- Solicitações relacionadas a problemas de logon único

Saiba mais sobre os diferentes cenários de solicitação para o plano Enterprise.

### Opções de gerenciamento de solicitações

Os Admins da empresa têm uma variedade de opções de gerenciamento de solicitações, permitindo que eles personalizem os processos de acordo com o tipo de solicitação:

:::note
As opções para enviar e-mail para todos os Admins da empresa ou para Admins específicos da empresa incluem admins do time.
:::

- Enviar um e-mail para todos os Admins da empresa
- Enviar um e-mail para Admins específicos da empresa
- Criar um ticket na central de atendimento
- Redirecionar para um URL personalizado

## Como configurar o gerenciamento de solicitações

:::note
Para [gerenciar as solicitações de licença diretamente na Miro](04-license-requests-on-enterprise-plan.md), selecione **Enviar um e-mail para todos os Admins da empresa** ou **Enviar um e-mail para admins específicos**. Você receberá todas as solicitações de licença futuras nas configurações de solicitação de licença.
:::

### Enviar um e-mail para todos os Admins da empresa

Todos os Admins da empresa receberão uma notificação por e-mail quando um usuário fizer uma solicitação de acesso.

1. Em **configurações** da empresa vá para **Usuários** > **Solicitações de acesso** > **Gerenciamento de solicitações**.
2. Clique no **Tipo de solicitação** que você deseja gerenciar.
3. Um pop-up será aberto. Clique no menu suspenso e selecione **Enviar e-mail para todos os Admins da empresa**.

:::note
As opções de envio de e-mail para todos os Admins da empresa, ou Admins específicos da empresa, incluem admins do time.
:::

### Enviar um e-mail para Admins específicos da empresa

Os Admins da empresa podem especificar até 5 endereços de e-mail. Somente os e-mails especificados receberão a solicitação. Os e-mails não precisam pertencer a usuários da Miro.

1. Vá para **Configurações da empresa** > **Usuários** > **Solicitações de acesso** > **Gerenciamento de solicitações**.
2. Clique no **Tipo de solicitação** que você deseja gerenciar.
3. Um pop-up será aberto. Clique no menu suspenso e selecione **Enviar e-mail para admins específicos da empresa**.
4. Adicione até 5 e-mails. Clique em **Adicionar** sempre que inserir um endereço de e-mail no campo de e-mail.

:::note
As opções de enviar e-mail para todos os Admins da empresa, ou para Admins específicos da empresa, incluem admins do time.
:::

### Criar um ticket na central de atendimento

Crie automaticamente um ticket do service desk toda vez que um usuário fizer uma solicitação de acesso. Esta funcionalidade atualmente é compatível com **ServiceNow** e **Jira Service Management**.

ServiceNow Jira Service Management

1. Defina as configurações de e-mail para o ServiceNow. Crie um item de catálogo para a Miro no ServiceNow. Abra o ServiceNow, vá para **Propriedades do sistema** > **Propriedades de e-mail** e habilite o recebimento de e-mails

2. [Crie uma ação de e-mail de entrada](https://docs.servicenow.com/bundle/tokyo-servicenow-platform/page/administer/notification/task/t_CreatingAnInboundEmailAction.html). No campo **De**No campo **De** sob a linha **Somente emails deste remetente acionarão esta ação de entrada**, digite [notification@miro.com](mailto:notification@miro.com).

3. [Defina os valores dos campos a partir do corpo do e-mail](https://docs.servicenow.com/bundle/rome-servicenow-platform/page/administer/notification/reference/r_SetFieldValsFromTheEmailBody.html) para configurar definições adicionais e definir o processo de conversão de um e-mail da Miro em um ticket do ServiceNow. Por exemplo, você pode atribuir um ticket recém-criado a uma pessoa específica.

4. Acesse a Miro e abra as configurações da empresa > **usuários** > **Pedidos de acesso** > **Gerenciamento de pedidos**, e selecione **Criar um ticket no ServiceNow**. No campo de e-mail, insira seu endereço de e-mail do ServiceNow.

1. Configure as configurações de e-mail para o Jira Service Management. No seu projeto de serviço, selecione **Configurações do projeto** > **Solicitações de e-mail**. [Escolha seu provedor de e-mail e siga as instruções para vincular a Miro](https://support.atlassian.com/jira-service-management-cloud/docs/receive-requests-from-an-email-address/).

2. Vá para a Miro, abra as **configurações da empresa** > **Gestão de usuários**> **Solicitações de acesso** > **Gerenciamento de solicitações**, e selecione **Criar um ticket no Jira Service Management**. No campo de e-mail, insira seu endereço de e-mail do Jira Service Management.

### Redirecionar para um URL personalizado

O solicitante será redirecionado para uma URL de sua escolha para as próximas etapas.

1. Em **Configurações da empresa** vá para **Usuários** > **Solicitações de acesso** > **Gerenciamento de solicitações**.
2. Clique no **Tipo de solicitação**que você deseja gerenciar.
3. Um pop-up será aberto. Clique no menu suspenso e selecione **Redirecionar para um URL personalizado**.
4. Digite o link de redirecionamento no campo de **URL personalizado**.

## Cenários de solicitação

Os cenários abaixo descrevem como diferentes solicitações são acionadas na Miro. Revise os cenários para decidir como você gostaria de gerenciar cada tipo de solicitação.

|  |  |
| --- | --- |
| **Solicitações para fazer parte de sua organização** | - Quando um novo usuário solicita a entrada em um time que é uma assinatura gerenciada pela empresa com [controle de domínio](../canvas-25-admin-features/domain-control/01-domain-control.md) (a menos que o controle de domínio esteja configurado para capturar novos usuários). |
| **Solicitações de licença** | - Quando um [usuário com restrições Free](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) solicita uma licença Standard ou Full (legada). - Quando um membro solicita uma licença Standard ou Full (legada) para um usuário com licença gratuita limitada, a menos que os membros possam convidar novos usuários para a assinatura nas [configurações de convite](03-invitation-settings-on-enterprise-plan.md). - Quando um usuário com licença Standard ou Full (legada) solicita uma licença Avançada. - Quando um membro tenta convidar ou dar acesso de edição a um usuário com uma licença gratuita limitada. |
| **Solicitações para fazer parte de um time** | - Quando um usuário que não é admin tenta compartilhar um board com um usuário que *não* é membro do time, convites de convidados estão desativados nas [configurações de convite](03-invitation-settings-on-enterprise-plan.md), e somente admins podem convidar novos membros para o time. - Quando um membro que não tem permissão para convidar novos membros tenta atribuir uma função de titular ou [cotitular](../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) em um determinado board a um usuário que não é membro do time. - Quando um usuário Enterprise solicita para entrar em um time [descoberto para usuários na sua organização](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md). - Quando um [convidado](../../using-miro/sharing-boards/07-collaboration-with-guests.md) convidado para boards específicos em um time solicita participar do time |
| **Solicitações relacionadas a problemas de logon único** | - Quando um usuário não recebeu acesso à Miro no IdP e tem problemas para fazer login via logon único. |

## Perguntas frequentes

**Por que ainda estou recebendo e-mails mesmo tendo definido minhas configurações para criar tickets?**

Se os admins do time tiverem permissão para convidar novos usuários para um time nas [configurações de convite](03-invitation-settings-on-enterprise-plan.md), eles receberão solicitações de convite relacionadas a este time por e-mail, mesmo que as configurações de gerenciamento de solicitações sejam definidas de forma diferente. Admins da empresa que também são admins do time também continuarão recebendo esses e-mails.

**Como os admins do time sabem se há uma solicitação para ingressar no time?**

Se tiverem permissão para convidar usuários para seus times, os admins do time receberão um e-mail sobre as solicitações, independentemente das configurações de gerenciamento de solicitações.
