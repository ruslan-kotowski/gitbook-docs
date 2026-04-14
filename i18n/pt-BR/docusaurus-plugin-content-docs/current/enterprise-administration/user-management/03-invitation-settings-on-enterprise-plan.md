---
title: "Configura\xE7\xF5es de convite no plano Enterprise"
article_id: 4412315533842
translation_id: 4412315533842
locale: pt-br
sidebar_position: 3
created_at: '2021-12-13T04:56:26Z'
updated_at: '2026-02-19T10:56:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
---

Configure suas configurações de convite do plano Enterprise para gerenciar quem pode convidar novos usuários para participar do seu plano. Você pode personalizar suas configurações de convite para atender aos requisitos dos seus times e da empresa como um todo.

> **Disponível para**: plano Enterprise
> **Quem pode fazer:** Admins da empresa

:::tip
Se você é novo na Miro, saiba mais sobre [Configurações do time e da empresa](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md).
:::

## Configurações de convite do time

Para uma colaboração mais eficaz, permita que **todos os membros do time** convidem novos membros para o time. Se preferir ter mais controle sobre os convites do time, você pode restringir essa opção para Admins da empresa e/ou Admins do time, de modo que todas as solicitações de convite sejam enviadas via [Gestão de Solicitações](09-request-management-on-enterprise-plan.md). Você também pode controlar se os usuários podem convidar [convidados](../../using-miro/sharing-boards/07-collaboration-with-guests.md) para os times.

### Como configurar configurações de convite do time

Para gerenciar suas configurações de convite do time, no console de admin, acesse **Times** e selecione seu time. Seu painel do time será aberto. Em **Convite**, selecione uma das seguintes opções:

- **Somente Admins da empresa**
  Apenas Admins da empresa podem adicionar novos membros ao time.
- **Admins da empresa e do time**
  Admins da empresa e do time podem convidar novos membros para o time.
- **Todos os membros do time**
  Todos os membros do time podem convidar novos membros para o time.

:::note
Nas [assinaturas do Programa de Licenças Flexíveis (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md), as configurações de convite de time são complementadas pelas configurações de convite de empresa.
:::

### Como configurar convites para convidados

Admins da empresa podem permitir ou restringir a opção para que os Membros convidem [Convidados](../../using-miro/sharing-boards/07-collaboration-with-guests.md). Convidados só podem acessar boards para os quais foram convidados e não precisam de uma licença.

Atualize as configurações de convite para Convidados em **Times** > selecione seu time > **Configurações** > **Permitir Convidados para o time [Nome].**

:::note
Admins da empresa podem ativar a desativação automática de convidados após 30 dias de inatividade.
:::

## Cenários de convite

:::tip
Dependendo das [configurações de Gerenciamento de Solicitações](09-request-management-on-enterprise-plan.md), as solicitações para compartilhar um board ou convidar um usuário para um time podem ser enviadas diretamente para Admins da empresa, para pessoas específicas via e-mail, ou um ticket de suporte pode ser criado.
:::

**Convidar novos Membros para um time**

Se Convidados não são permitidos e os Membros não têm permissão para convidar novos Membros, ao tentarem compartilhar um board, eles verão a notificação abaixo e precisarão enviar uma solicitação.

**Atribuir a função de titular ou cotitular**

Se os Membros não têm permissão para convidar novos Membros e tentarem atribuir a função de titular ou cotitular a um Convidado ou a um Membro [Free Restrito](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) em um board específico, eles verão a notificação abaixo e precisarão enviar uma solicitação.

**Convidando um usuário externo ou convidado para editar um board**

:::note
Convidados externos são convidados fora do domínio da sua empresa. Eles terão um e-mail de uma empresa externa.
:::

Se os membros não estão autorizados a convidar novos membros para o time, e convidados com acesso de edição não foram ativados para o time, ao tentar convidar um usuário externo para editar um board, os usuários verão a notificação abaixo e precisarão enviar uma solicitação. Após enviar a solicitação, o convidado será adicionado ao board com acesso de comentário, permitindo que ele adicione comentários no board, mas não edite seu conteúdo.

## Configurações de convite da empresa

As configurações de convite da empresa controlam quem pode convidar novos membros para sua assinatura Enterprise. Todos os novos membros recebem uma licença Advanced, Standard, Full (legado), Free ou Free Restricted, dependendo do seu [modelo de licença](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md) e [licença padrão](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

### Como configurar as configurações de convite da empresa

> **Disponível para**: [Programa de licenças flexíveis (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)

Para gerenciar as configurações de convite da sua empresa, acesse as configurações da **empresa** > **Segurança** > **Compartilhamento** > **Convite** e selecione uma das seguintes opções:

**Apenas Admins da empresa**
Apenas Admins da empresa podem conceder licenças a novos Membros. Admins do time e Membros podem apenas convidar Membros já existentes na empresa para seus times e não podem ativar novas licenças.

**Admins da empresa e admins do time**
Admins da empresa e admins do time podem convidar novos Membros e adicionar novas licenças. Admins do time podem apenas convidar novos Membros para os times nos quais são admin do time.

**Todos os membros**
Cada membro da assinatura Enterprise pode adicionar novas licenças ao convidar pessoas para o seu time, desde que as convites sejam permitidos para **Todos os membros do time** nas configurações de convite do time.

## Como as configurações de Empresa e Time funcionam juntas

As configurações de Empresa complementam as configurações de convite do Time. Os Admins da empresa podem configurar quem pode convidar usuários para um time específico nas configurações do time. Isso significa que os Admins da empresa podem permitir que Membros e Admins do time gerenciem suas próprias convites e colaborações, mas as licenças ainda são controladas pelos Admins da empresa nas configurações da empresa.

## Desativação automática de Convidados

Configure a desativação automática de convidados após 30 dias de inatividade. Use esta funcionalidade para remover convidados e manter sua assinatura segura.

Quando a funcionalidade está ativada, qualquer convidado (independentemente do seu domínio) que não tenha estado ativo nos times do seu Enterprise em 30 dias será automaticamente desativado. Não é possível customizar o período de 30 dias.

Essa configuração é aplicada a todos os times dentro da organização.

Vá para as configurações da **Empresa** > **Segurança** > **Compartilhamento** e ative **Desativar convidados automaticamente**.

:::tip
Assim que a configuração é ativada, a ação é registrada em [logs de auditoria](../security-integrations/security-management/01-audit-logs.md) como **Configuração de expiração de usuários externos habilitada/desabilitada**. Os eventos de desativação também serão registrados nos [logs de auditoria](../security-integrations/security-management/01-audit-logs.md). O autor será exibido como **Automação Miro**.
:::
