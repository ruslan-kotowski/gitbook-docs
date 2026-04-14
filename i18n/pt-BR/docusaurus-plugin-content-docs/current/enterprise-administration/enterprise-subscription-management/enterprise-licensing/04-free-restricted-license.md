---
title: "Licen\xE7a gratuita limitada"
article_id: 360011746739
translation_id: 360011746739
locale: pt-br
sidebar_position: 4
created_at: '2020-02-05T07:29:16Z'
updated_at: '2026-02-19T10:40:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Quando novos usuários ingressam em uma assinatura da Miro, dependendo do [modelo de licenciamento Enterprise](02-enterprise-licensing.md), eles podem receber uma licença gratuita limitada.

> **Relevante para:** Plano Enterprise

## Quando os usuários recebem uma licença gratuita limitada

**No Programa de Licenças Flexíveis (FLP)**, um usuário pode receber a licença gratuita limitada quando:

- A licença padrão para novos usuários é configurada como licença gratuita limitada
- Um Admin da empresa convida o usuário e seleciona a licença gratuita limitada para ele na janela de convite
- Um Admin da empresa converte o usuário para licença gratuita limitada em **Configurações da empresa > Usuários ativos**

:::note
Saiba mais sobre o [Programa de licenças flexíveis (FLP)](03-flexible-licensing-program-flp.md) e o [gerenciamento de licenças no FLP](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

**Em licenciamento não flexível (não-FLP)**, um usuário pode receber a licença gratuita limitada quando:

- O usuário é capturado automaticamente (por [Controle de Domínio](../../canvas-25-admin-features/domain-control/01-domain-control.md) ou [Provisionamento Just-in-Time](../../user-management/13-user-provisioning-on-enterprise-plan.md)) em uma organização que possui um número insuficiente de licenças Avançadas, Standard ou Full (legado) durante o registro no Miro.
- O usuário é convidado para um time na organização que possui um número insuficiente de licenças Avançadas, Standard ou Full (legado).

Quando vários usuários são convidados ao mesmo tempo, eles recebem licenças pela ordem dos seus endereços de e-mail na lista de convidados. Se a organização não tiver licenças suficientes, os usuários no final da lista receberão uma licença gratuita limitada. Nesse caso, o convidador receberá uma notificação pop-up sobre o acesso limitado para alguns usuários.

## Como funcionam as licenças gratuitas limitadas para usuários

Usuários com licença gratuita limitada podem visualizar e comentar nos boards dos times em que participam, e podem solicitar acesso de edição e uma licença Standard ou uma licença Full (legado) aos Admins da empresa. Eles também podem descobrir e participar de times na organização junto com outros membros.

:::note
Admins da empresa podem [configurar as definições de gerenciamento de solicitações](../../user-management/09-request-management-on-enterprise-plan.md).
:::

### Acesso aos boards com licença gratuita limitada

Os seguintes níveis de permissão para visualizar, comentar ou editar se aplicam a usuários com uma licença gratuita limitada:

|  |  |
| --- | --- |
| **Como o board foi compartilhado** | **Nível de acesso** |
| Link público | Usuários Free Restricted podem visualizar e/ou editar, dependendo do nível de acesso concedido. |
| Link de time ou empresa | Usuários Free Restricted podem visualizar e/ou comentar, dependendo do nível de acesso concedido. |
| [Link incorporado](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md) | Usuários com licenças gratuitas limitadas podem visualizar e/ou comentar, dependendo do nível de acesso concedido.  Usuários com licenças gratuitas limitadas não poderão editar ou solicitar acesso de edição, mesmo se o acesso de edição for concedido via permissões de incorporação. |

## Como gerenciar licenças gratuitas limitadas

> **Quem pode fazer isso:** Admins da empresa

Em todas as assinaturas, o Admin da empresa pode atualizar uma licença de usuário de gratuita limitada para uma licença Standard ou Full (legada) na seção **Usuários ativos** das configurações do time ou da empresa.

**Programa de Licenças Flexível (FLP)**

Nas assinaturas do Programa de Licenças Flexíveis, o Admin da empresa também pode fazer downgrade de uma licença Avançada, Padrão ou Completa (legada) para uma licença gratuita limitada a qualquer momento.

Quando um usuário com uma licença gratuita limitada solicita acesso de edição, os Admins da empresa recebem o pedido de acordo com suas [configurações de gerenciamento de solicitações](../../user-management/09-request-management-on-enterprise-plan.md).

:::note
Saiba mais sobre [o gerenciamento de licenças no Programa de Licenças Flexíveis](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

## Perguntas frequentes

**O que acontece com minhas licenças gratuitas limitadas quando adiciono mais licenças Standard ou Full (legado) ao meu plano sem FLP?**

Seus usuários existentes com licença gratuita limitada não são automaticamente atualizados para as novas licenças Standard ou Full (legado). Os Admins da empresa podem atualizar as licenças manualmente.
