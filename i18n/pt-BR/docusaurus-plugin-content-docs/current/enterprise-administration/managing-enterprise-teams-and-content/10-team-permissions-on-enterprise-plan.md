---
title: "Permiss\xF5es de time no plano Enterprise"
article_id: 4402822899986
translation_id: 4402822899986
locale: pt-br
sidebar_position: 10
created_at: '2021-06-24T12:51:56Z'
updated_at: '2026-02-19T16:30:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
---

O plano Enterprise fornece configurações de permissão avançadas e permite que você configure facilmente o nível necessário de acesso e segurança para seus times. Você pode selecionar descoberta de time, configurações de convite, configurações de compartilhamento e configurações de conteúdo do board que atendam às necessidades e políticas da sua empresa. As configurações são definidas para cada time na assinatura Enterprise .

:::note
Ao [criar um nov time dentro de uma assinatura Enterprise](09-create-a-new-team-on-enterprise-plan.md), os Admins da empresa podem selecionar configurações de permissões padrão ou escolher um time para copiar as permissões do time. Saiba mais sobre as configurações padrão abaixo.
:::

> **Disponível para:** plano [Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Configurado por:** Admins da empresa, admins do time

## Como acessar permissões e configurações do time

No painel da Miro, no canto superior esquerdo, selecione seu avatar. Em seguida, selecione **Configurações** para abrir o console de admin .

No console de admin, selecione **Times**. Em seguida, selecione o time que deseja configurar. A visualização do time é aberta. Em seguida, selecione **Configurações**.

:::tip
Para encontrar seu time, você pode usar a barra de pesquisa na parte superior da visualização de **times**.
:::

A primeira configuração é **Configurações de descoberta de time**.

![Configurações de descoberta de Team no console de admin Enterprise](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)

*Configurações de descoberta de time no console de admin do Enterprise .*

Você pode tornar seu time aberto para outros usuários Enterprise participarem ou ocultá-lo — saiba mais no artigo [Gerenciar privacidade e descoberta do time no plano Enterprise](11-manage-team-privacy-and-discovery-on-enterprise-plan.md). A configuração pode ser alterada pelos Admins da empresa e admins do time se tiverem [permissão para convidar novos membros para o time](../user-management/05-manage-user-invitations-on-enterprise-plan.md).

**As configurações de convite do time** permitem que os Admins da empresa determinem quem pode convidar usuários para o time e escolham se você precisa [convidados](../../using-miro/sharing-boards/07-collaboration-with-guests.md) para o time.

![Configurações de convite de Team no console de admin do Enterprise](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)

*Configurações de convite de time no console de admin do Enterprise*

**Mais informações:** Consulte [Gerenciar convites de usuário no plano Enterprise](../user-management/05-manage-user-invitations-on-enterprise-plan.md).

Os Admins da empresa também podem definir as **configurações de compartilhamento**.

Primeiro, você pode definir quem pode criar novos conteúdos (boards, espaços e templates) no time e mover boards para o time. Isso é extremamente útil se você precisar configurar um time dedicado para [provisionamento automático](../user-management/13-user-provisioning-on-enterprise-plan.md) ou usar um time como armazenamento para determinados boards. Você pode permitir isso a todos os membros, somente aos Admins da empresa, ou aos Admins da empresa e admins do time.

![Compartilhando configurações no console de admin do Enterprise](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)*Compartilhando configurações no console de admin do Enterprise*

Você pode permitir ou proibir que membros do time compartilhem boards e espaços com todo o time, com toda a empresa ou por meio de links públicos. Se restringir esses tipos de compartilhamento, as opções serão removidas dos boards do time.

![Compartilhamento de board no console de admin Enterprise](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)
*Compartilhamento de board no console de admin Enterprise*

Também é possível definir [**configurações de compartilhamento** para os boards e espaços recém-criados pelo time](../../using-miro/sharing-boards/11-default-sharing-settings.md). Tanto os admins do time como os da empresa têm acesso à configuração.

:::warning
A opção **Qualquer pessoa na empresa pode encontrar e visualizar/comentar** não é exibida se [a privacidade do time](07-team-management-on-enterprise-plan.md) estiver ativada.
:::

**Mais informações:** consulte o artigo Política de compartilhamento no plano Enterprise.

Os Admins da empresa podem definir [domínios permitidos para um time.](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)

Os Admins da empresa podem ver a configuração para [restringir ou permitir a movimentação de boards de e para o time](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md). ![Domínios permitidos para time no console de admin Enterprise](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)
*Domínios permitidos para time no console de admin Enterprise*

Os admins do time podem definir as configurações de **segurança de conteúdo** para o time: escolher se os usuários externos ao time podem copiar o conteúdo do board (bem como duplicar os boards do time e baixar o conteúdo do board) e decidir para quem essa opção deve estar disponível nos boards recém-criados (a menos que o titular do board selecione outra opção).

![Segurança de conteúdo no console de admin Enterprise](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)
*Segurança de conteúdo no console de admin Enterprise*

Como parte das configurações de segurança de conteúdo, os admins do time também podem configurar uma etiqueta padrão para os boards recém-criados no time ou na **classificação do board**. A etiqueta padrão do time substituirá a etiqueta padrão da empresa definida nas [configurações de classificação do board](../canvas-25-admin-features/data-security/02-data-classification.md) da empresa.

Na parte inferior da página, você verá a seção **Configurações de colaboração**. Aqui, os admins do time e Admins da empresa podem habilitar a função de cotitular do board, que é desabilitada por padrão. Observe que a opção fica esmaecida se a função não for permitida no nível da empresa. [Saiba mais](../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md).

![Classificação do board e configurações de colaboração no console de admin Enterprise](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921781883666_image.png)
*Classificação do board e configurações de colaboração no console de admin Enterprise*

### Configurações padrão

Se você escolher Configurações de permissão **padrão** ao [criar um novo time Enterprise](09-create-a-new-team-on-enterprise-plan.md), as seguintes configurações serão escolhidas:

- **Configurações de descoberta de time**: os membros podem participar após aprovação
- **Configurações de convite**: todos os membros do time podem convidar novos usuários, e colaboradores convidados são permitidos
- **Configurações de** compartilhamento
  - Todos os membros do time podem criar **ativos neste time.**
  - **Compartilhamento do board**: os membros do time podem compartilhar seu conteúdo com o time para visualização, comentários e edição, compartilhar com toda a empresa para visualização e comentários e publicamente para visualização e comentários (se [o compartilhamento público for permitido no nível da empresa](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md))
  - **Configurações para compartilhamento de board**: somente titulares de board podem acessar
  - **Configurações de compartilhamento de espaços**: somente titulares de espaços podem acessar
  - **Domínios permitidos para o time**: a opção para restringir domínios permitidos está desativada. [Domínios permitidos configurados no nível da empresa](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) são aplicados
- **Mover boards para outros times**: permitido
- **Configurações do conteúdo do board**
  - **Copiar conteúdo do board**: permitido para membros do time e usuários que não fazem parte do time
  - **Cópia de board padrão**: membros do time com direitos de edição podem copiar o conteúdo do board em boards recém-criados
- **Classificação do board**: a opção de substituir o etiqueta padrão está desabilitada
- **Configurações de colaboração**: a função de cotitular está desabilitada
