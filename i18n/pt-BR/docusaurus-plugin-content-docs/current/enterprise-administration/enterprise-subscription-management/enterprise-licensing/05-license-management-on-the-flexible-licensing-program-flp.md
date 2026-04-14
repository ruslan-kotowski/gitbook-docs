---
title: Gerenciamento de licenças no Programa de licenças flexíveis (FLP)
article_id: 360018622159
translation_id: 360018622159
locale: pt-br
sidebar_position: 5
created_at: '2020-12-29T10:44:01Z'
updated_at: '2026-02-23T18:22:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'Relevante para: Plano Enterprise'
---

Saiba mais sobre a gestão de licenças no Programa de Licenças Flexíveis (FLP), incluindo quais opções de gestão de licenças estão disponíveis para novos usuários e como converter licenças existentes.

:::tip
Se você é novo na licença FLP, recomendamos primeiro ler [Programa de Licenças Flexíveis](03-flexible-licensing-program-flp.md) e [Níveis de acesso de usuários no Plano Enterprise](../../user-management/11-user-access-levels-on-enterprise-plan.md) para compreender como nossos modelos de licenciamento, tipos de licença e funções da Miro funcionam juntos.
:::

## Atribuindo licenças a novos usuários

Membros Convidados Visitantes

Com base nas configurações de licença padrão da sua empresa, novos membros recebem automaticamente uma licença Free ou uma licença gratuita limitada. Para definir uma licença padrão para novos membros na sua assinatura, entre em contato com a pessoa responsável pela Miro.

Novos membros recebem a licença padrão:

- ao serem convidados por membros que não são Admins
- automaticamente via [provisionamento Just-in-Time](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), [controle de domínio](../../canvas-25-admin-features/domain-control/01-domain-control.md) ou [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)

Os Admins da empresa também têm a opção de selecionar uma licença para os membros convidados.

- selecione **Gratuito** se você quiser que os usuários tenham a opção de editar (eles serão atualizados para uma licença Standard ou Full (legado) assim que editarem ou criarem um board, forem convidados a editar um board, receberem cotitularidade de um board ou forem adicionados a um [projeto](../../../using-miro/sharing-boards/16-projects.md) como Editor)
- selecione **Gratuito Restrito** para convidar o membro sem direitos de edição

Convidados convidados para um board sempre recebem uma licença **Gratuita**. Aprenda como [convidar convidados em um Plano Enterprise](../../../using-miro/sharing-boards/07-collaboration-with-guests.md).

[Visitantes](../../../using-miro/sharing-boards/08-collaboration-with-visitors.md) de boards compartilhados publicamente não têm custos e não possuem licenças.

## Como fazer upgrade ou downgrade de licenças

> **Quem pode fazer isso:** Admins da empresa

**Licenças Free** são automaticamente promovidas para uma licença Standard ou Full (legado) assim que o usuário cria ou edita um board.

Free Restrita para Padrão ou Completa (legado)  Padrão ou Completa (legado) para Free Restrita Conversão em massa de licenças

Licenças gratuitas limitadas podem ser atualizadas para uma licença padrão ou completa (legada) manualmente pelos Admins da empresa ou como parte da [automação de fluxo de trabalho Enterprise](../enterprise-workflow-automation/01-enterprise-workflow-automation.md).

Para atualizar uma licença gratuita limitada para uma licença completa:

1. Abra **Times** ou abra **Configurações da organização** > **Usuários** > **Todos os usuários** > **Usuários ativos**.
2. Clique no ícone dos **três pontos** (**...**) ao lado de um usuário com licença gratuita limitada.
3. Selecione **Alterar para membro padrão**.

Licenças completas podem ser rebaixadas para uma licença gratuita limitada se os Admins da empresa desejarem limitar o acesso do usuário e liberar licenças completas adicionais.

Membros completos não podem ser rebaixados para uma licença gratuita, pois licenças gratuitas só podem ser atribuídas a novos usuários.

Para rebaixar uma licença completa para uma licença gratuita limitada:

1. Abra **Times** ou abra **Configurações da organização** > **Usuários** > **Todos os usuários** >**Usuários ativos**.
2. Clique no ícone dos **três pontos** (**...**) ao lado de um usuário Full.
3. Selecione **Alterar para Free Restricted**.

Para converter várias licenças de uma vez:

1. Abra **Configurações da organização** > **Usuários** > **Todos os usuários** > **Usuários ativos**.
2. Selecione individualmente todos os usuários cujas licenças deseja converter, ou aplique filtros para selecionar usuários. Você pode selecionar até 50 usuários
3. Clique em **Ações em massa** e selecione uma nova opção de licença
