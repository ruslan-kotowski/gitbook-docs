---
title: "Provisionamento de usu\xE1rios no plano Enterprise"
article_id: 4403139914130
translation_id: 4403139914130
locale: pt-br
sidebar_position: 13
created_at: '2021-07-01T07:59:23Z'
updated_at: '2025-11-25T16:05:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: scim
---

Com o auto-provisionamento, todos os novos usuários em seus domínios corporativos são direcionados para sua assinatura Enterprise e têm acesso aos ativos da sua empresa.

A Enterprise da Miro oferece várias opções de provisionamento: convites, provisionamento Just-in-Time (JIT), System for Cross-domain Identity Management (SCIM) e controle de domínio.

> **Disponível para:** Plano Enterprise

## Convites

Você pode convidar usuários para sua assinatura usando o botão **Convidar membros** no seu painel. Os convites são enviados imediatamente e não requerem nenhuma configuração adicional.

Saiba mais sobre como compartilhar seu trabalho e colaborar na Miro visitando [Gerenciar convites no Enterprise Plan](05-manage-user-invitations-on-enterprise-plan.md) e [Compartilhar boards e convidar colaboradores](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

![invite_members_button.jpg](../../../../../../docs/enterprise-administration/user-management/images/21017653284754_invite%20members%20button.jpg)*A opção para convidar membros no painel da Miro*

## Provisionamento just-in-time (JIT)

O provisionamento JIT, integrado ao [logon único (SSO)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), adiciona automaticamente todos os novos usuários registrados sob seus domínios corporativos de SSO a um time específico no seu plano Enterprise.
O provisionamento JIT pode ser facilmente habilitado nas configurações de SSO da Miro. Saiba [como configurar o SSO](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

![user_provisioning_jit_provisioning.png](../../../../../../docs/enterprise-administration/user-management/images/21017682931730_user_provisioning_jit_provisioning.png)*Habilitando o provisionamento Just-in-Time (JIT) nas configurações de SSO*

## Sistema para gerenciamento de identidades entre domínios (SCIM)

SCIM, integrado com [Logon Único (SSO)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), permite o provisionamento e gerenciamento automático de usuários no seu Plano Enterprise através do provedor de identidade escolhido.

Com o SCIM ativado, você pode adicionar usuários a times específicos, atualizar seus dados e e-mails e gerenciar seu status de ativação diretamente dentro do provedor de identidade escolhido. Essa funcionalidade automatiza a troca de informações de usuários entre sua conta Miro e seu provedor de identidade.

SCIM automatiza a troca de informações de usuários entre a Miro e o seu provedor de identidade, permitindo que você gerencie o acesso dos funcionários ao seu Plano Enterprise centralmente a partir do provedor de identidade.

Saiba mais sobre as [funcionalidades do SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) e revise as etapas de configuração para o [Entra ID](../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md), [OKTA](../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md) ou [OneLogin](../security-integrations/system-for-cross-domain-identity-management-scim/06-setting-up-automated-provisioning-with-onelogin.md).

## Controle de domínio

[Controle de domínio](../canvas-25-admin-features/domain-control/01-domain-control.md) permite que você adicione usuários automaticamente à sua assinatura Enterprise, limite a capacidade de usuários corporativos criarem assinaturas Miro separadas e monitore a atividade do usuário dentro do seu domínio.

Com o domínio controlado, você pode definir uma regra de provisionamento para seus usuários corporativos:

- usuários recém-registrados em seu domínio podem solicitar acesso à sua assinatura
- usuários recém-registrados em seu domínio entram automaticamente na sua assinatura
- usuários recém-registrados em seu domínio entram automaticamente na sua assinatura e usuários em seu domínio não têm permissão para criar novos times no Miro

![Add-a-domain-Image1.png](../../../../../../docs/enterprise-administration/user-management/images/21017653288082_Add-a-domain-Image1.png)*Domínio controlado nas configurações de segurança do Miro*

## Como funciona a licença

Ao convidar novos usuários, os Admins da empresa podem escolher uma licença para o convidado, dependendo da configuração da assinatura.

Usuários convidados por não-admins ou provisionados automaticamente para sua assinatura via JIT, SCIM ou controle de domínio, receberão a *licença padrão*:

- **para planos com licença não flexível (não FLP):** a licença padrão é uma licença completa (se a organização não tiver licenças completas suficientes, os usuários auto-capturados receberão uma licença [gratuita limitada](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)).
- **para planos com o Programa de Licenças Flexíveis (FLP):** a licença padrão pode ser Free ou [gratuita limitada](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).

:::note
Saiba mais sobre nossos [modelos de licença Enterprise](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md), [Gerenciamento de licença no Programa de licenças flexíveis](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md), como gerenciar a alocação e upgrades de licença com [Gerenciamento de solicitações](09-request-management-on-enterprise-plan.md), e como acompanhar o uso da licença com [Gestão de ativos de software](../security-integrations/software-asset-management/01-software-asset-management-miro-enterprise.md).
:::

## Perguntas frequentes

Quando o controle de domínios é configurado para capturar novos usuários, ele funciona de maneira similar ao JIT, atribuindo automaticamente usuários de domínios específicos a um time padrão dentro da assinatura Enterprise?

Sim, mas o controle de domínios não requer que o logon único esteja configurado para o plano Enterprise, ele pode funcionar sem logon único.

Podemos impedir que usuários provisionados automaticamente recebam uma licença completa até começarem a trabalhar ativamente em um board?

Sim, isso é possível com o [Programa de licenças flexíveis](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

Posso configurar várias opções de provisionamento para minha assinatura Enterprise?

Sim, você pode usar várias opções de provisionamento ao mesmo tempo.
