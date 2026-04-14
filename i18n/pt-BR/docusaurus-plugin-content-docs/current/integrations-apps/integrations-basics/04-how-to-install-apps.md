---
title: Como instalar aplicativos
article_id: 360017731093
translation_id: 360017731093
locale: pt-br
sidebar_position: 4
created_at: '2019-02-11T10:12:46Z'
updated_at: '2025-08-05T07:54:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'Pessoas: Todos os usuários Planos: Todos os planos Plataformas: Navegador,
    aplicativo para desktop Admins do time podem restringir a instalação para não-admins.
    Admins da empresa no plano Enterprise podem restringir ainda mais apenas para
    aplicativos aprovados.'
---

Você pode expandir a funcionalidade da Miro instalando aplicativos do Marketplace da Miro. Este artigo orienta você na instalação e desinstalação de aplicativos, compreensão das permissões de aplicativos e fornece uma visão geral sobre a criação de integrações personalizadas.

## Instalar aplicativos do Marketplace da Miro

O [Marketplace da Miro](https://miro.com/marketplace/) é o seu hub central para descobrir e adicionar aplicativos a fim de aprimorar sua experiência com a Miro. Você pode instalar aplicativos diretamente do seu board ou visitando o site do Marketplace.

![Miro_marketplace.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021611044242_Miro%20marketplace.jpg)*Marketplace da Miro*

Existem duas maneiras principais para os usuários adicionarem aplicativos:

1. **Do seu board:** Clique no ícone **Ferramentas, mídia e integrações (+)** na barra de ferramentas de criação e, em seguida, use a caixa de pesquisa "Pesquisar integrações" na guia Marketplace. Se você encontrar seu aplicativo já listado, basta clicar para adicioná-lo. Você também pode navegar por aplicativos disponíveis neste painel.
   ![marketplace-add-apps.png](../../../../../../docs/integrations-apps/integrations-basics/images/21260776452626_marketplace-add-apps.png)*Marketplace na barra de ferramentas de criação*
2. **Do site do Marketplace:** Você também pode acessar diretamente o site do [Marketplace da Miro](https://miro.com/marketplace/) para navegar e instalar aplicativos de suas respectivas listas.

**Para Admins da empresa:**
Admins da empresa em planos aplicáveis também podem instalar aplicativos para todo o time através das configurações do time. Para fazer isso, acesse **Configurações do time** > **Aplicativos e integrações** > **Instalar aplicativos**. Esta seção permite o gerenciamento e implantação centralizada de aplicativos em todo o time.

![apps_and_integrations_page.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021832338450_apps%20and%20integrations%20page.jpg)*Seção de aplicativos instalados nas configurações do time para admins*

## Desinstalar aplicativos

Você pode gerenciar e desinstalar aplicativos nas configurações do seu time. Observe que os usuários que não são admins podem ter restrições para desinstalar aplicativos, dependendo da configuração do time.

:::warning
Usuários que não são admins não podem desinstalar aplicativos se não tiverem permissão para instalá-los pelo admin nas configurações do time.
:::

Para gerenciar os aplicativos do seu time, acesse **Configurações do time > Aplicativos e integrações**. Esta página lista todos os aplicativos atualmente instalados para o seu time ou por você pessoalmente.

![apps_settings.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021898097682_apps%20settings.jpg)*Aplicativos e integrações nas configurações do time*

Para desinstalar um aplicativo, siga estas etapas:

1. Na lista de **Aplicativos e integrações**, selecione o aplicativo que você deseja remover.
2. Clique em **Desinstalar para o time** ou **Desinstalar para mim**. A opção disponível dependerá de como o aplicativo foi instalado e dos seus direitos administrativos.

![uninstall_an_app.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021797466258_uninstall%20an%20app.jpg)*A opção para desinstalar um aplicativo*

## Permissões de instalação de aplicativos

Os Admins do time e Admins da empresa têm vários controles para gerenciar quem pode instalar aplicativos e quais aplicativos estão disponíveis para sua organização, garantindo segurança e conformidade.

Os admins do time podem configurar se os membros do time que não são admins têm permissão para instalar aplicativos. Esta configuração está localizada em **Configurações do time > Aplicativos e integrações** sob as opções de gerenciamento de aplicativos.

![allow_non-admins_to_install_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021903025170_allow%20non-admins%20to%20install%20apps.jpg)*Opção "Permitir que não-admins instalem aplicativos" nas configurações do time*

Para usuários no [plano Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), Admins da empresa têm acesso a controles mais granulares. Eles podem gerenciar **Aplicativos aprovados** em **Configurações da empresa** > **Aplicativos**. Essa funcionalidade permite que os admins criem uma lista de aplicativos aprovados pela empresa, restringindo os usuários de instalar aplicativos que não estão nessa lista aprovada. [Saiba mais sobre como gerenciar as configurações de descoberta e instalação de aplicativos para planos Enterprise](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).

![Enterprise_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021890162962_Enterprise%20apps.jpg)*Gerenciamento de aplicativos aprovados nas configurações da empresa Enterprise*

## Integrações personalizadas e plataforma de desenvolvedores

Se você precisar de funcionalidades específicas que não estão disponíveis no Marketplace da Miro, você pode criar suas próprias soluções personalizadas usando a [Plataforma da Miro para desenvolvedores](https://miro.com/api/). Esta plataforma oferece ferramentas robustas, incluindo APIs REST, plugins web e incorporações, para ajudar você a construir integrações poderosas adaptadas às suas necessidades.

Aqui estão os pontos principais a considerar ao desenvolver integrações personalizadas:

- **Primeiros passos:** Você pode começar a construir seu aplicativo [criando um time de desenvolvedores](https://developers.miro.com/). Os times padrão de desenvolvedores são destinados a propósitos de desenvolvimento e teste e possuem certas limitações:
  - Até 5 usuários no time.
  - Até 3 boards no time.
  - Uma marca d'água é exibida nos boards.
  - A funcionalidade de exportação do board não está disponível.
- **Desenvolvedores do plano Enterprise:** Se a sua organização está no [plano Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), você pode criar um time de desenvolvedores como parte da sua assinatura. Esses times de desenvolvedores não estão sujeitos às limitações dos padrões e se beneficiam de todas as funcionalidades de segurança de nível Enterprise. [Saiba mais sobre times de desenvolvedores para planos Enterprise](../../enterprise-administration/managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md).

Para obter informações adicionais, suporte e para se conectar com outros desenvolvedores, você pode explorar o [Fórum da Plataforma para Desenvolvedores](https://community.miro.com/developer-platform-forum-57).
