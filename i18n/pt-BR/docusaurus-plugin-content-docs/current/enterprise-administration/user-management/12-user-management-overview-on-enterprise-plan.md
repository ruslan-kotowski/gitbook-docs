---
title: Visão geral do gerenciamento de usuários no plano Enterprise
article_id: 360017571474
translation_id: 360017571474
locale: pt-br
sidebar_position: 12
created_at: '2019-02-11T10:09:06Z'
updated_at: '2026-02-26T14:12:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-management
availability:
  notes: 'Disponível para: [plano Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
    Configurado por: Admins da empresa'
---

Você pode gerenciar facilmente as permissões de usuários de dezenas, centenas ou milhares de usuários da Miro dentro do seu plano. Os admins podem rastrear e filtrar listas de usuários e visualizar funções de usuários, taxa de atividade e consumo de licenças. Use ações em massa, como convidar, adicionar e remover usuários, atribuir funções e licenças e mover usuários entre times. Economize tempo e obtenha mais transparência sobre como o seu plano da Miro funciona ao dominar operações administrativas rápidas na Miro.

Todos os usuários corporativos que pertencem a domínios reivindicados e verificados por meio do Controle de Domínio são [usuários geridos dentro da sua organização Enterprise](06-managed-users-on-enterprise-plan.md).

## Seção de usuários ativos

Para abrir as configurações do Time, clique no nome do time no canto superior esquerdo do seu painel e depois clique no ícone **Membros do Time**.

As configurações da empresa serão abertas com uma lista de usuários no Time escolhido. Nesta seção, os admins da empresa e do time podem adicionar ou remover usuários do time, bem como promover ou revogar a função de admin do time.

Admins da empresa também podem converter um convidado em membro com uma licença Standard ou Full (legado). Para revogar ou fazer downgrade de uma licença Advanced, Standard ou Full (legado), os admins da empresa podem, em vez disso, conceder ao membro uma licença [Free restricted](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).

:::note
Funcionários que compartilham um domínio verificado são membros com licença Advanced, Standard, Full (legado), Free, Free Restricted. Para planos Enterprise, apenas usuários de domínios externos podem ser adicionados como convidados.
:::

:::note
Admins do time podem convidar novos membros do time se isso for permitido nas [Configurações de convite](05-manage-user-invitations-on-enterprise-plan.md).
:::

Para ver a lista completa de usuários na sua assinatura Enterprise, vá para **Configurações da empresa**. No lado esquerdo, em **Usuários**, selecione **Todos os usuários** para abrir a lista de usuários ativos (você também pode alternar para as guias **Usuários desativados** e **Convites** nesta tela). Você verá a lista de todos os usuários adicionados ou convidados para times ou boards dentro dessa assinatura específica, bem como a data da **última atividade**.

:::note
Para acessar as Configurações da empresa a partir das Configurações do time, clique em **Empresa** no canto superior esquerdo.
:::

Como Admin da empresa, você pode baixar uma lista completa dos usuários da sua organização junto com seu último log-in. Encontre o  **botão Baixar CSV** acima da lista de usuários ativos.

Na seção **usuários ativos**, você verá a lista completa de usuários junto com sua Função, Licença, Times e Atividade.

A **função** define os níveis de acesso dentro do plano. Enquanto o Admin da empresa é a função mais poderosa com a capacidade de gerenciar o plano, um convidado só pode acessar os boards aos quais é convidado. Saiba mais no [artigo sobre níveis de acesso.](11-user-access-levels-on-enterprise-plan.md)

O **tipo de licença** mostra se um usuário está utilizando uma licença Avançada, Padrão, Completa (legado) ou Gratuita.

Os **times** representam a quantidade de times em que um usuário está adicionado dentro do plano.

**Última** **atividade** mostra quando um usuário abriu algum board dentro da assinatura. Filtre usuários ativos/inativos selecionando datas no calendário ou use uma das opções predefinidas: 30, 60, 90, ou 180 dias. Definimos um usuário ativo como alguém que usou a Miro nos últimos 90 dias.

### Alterar o status de um único usuário

Como Admin da empresa, você pode alterar a função, a licença e o número de times de qualquer usuário ou grupo de usuários. Você também pode [desativar um usuário](01-deactivated-users.md) e depois [removê-lo](10-remove-users-on-enterprise-plan.md). Para acessar essas opções, clique no ícone de **três pontos** (**...**) ao lado da linha de qualquer membro do time.

:::tip
O sistema de gerenciamento avançado de usuários ajuda a gerenciar os recursos que você adquiriu de forma mais eficaz. Se você tiver o [Programa de licenças flexíveis](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) ativado, você pode liberar licenças de usuários inativos convertendo-os para Free Restricted.
:::

### Filtros

Se você tem dezenas, centenas ou milhares de usuários da Miro, **pesquise** por e-mail e nome ou **filtre a lista** por um critério específico para encontrar alguém mais rapidamente. Você também pode ocultar usuários convidados para ver apenas os usuários registrados da Miro no seu plano.

Uma vez que os filtros são aplicados, você pode selecionar em massa até 50 usuários na lista e usar ações em massa.

### Ações em massa

O **botão de ações em massa** ajuda você a gerenciar grupos de usuários mais rapidamente. Selecione vários usuários para aplicar as alterações necessárias em massa.

Você pode selecionar usuários um por um marcando as caixas à esquerda ou aplicar filtros e selecionar até 50 usuários de uma vez.

#### Gerenciar usuários ativos em massa

Na lista de **usuários ativos**, selecione a lista de usuários para aplicar uma das ações abaixo.

1. Gerenciar a membresia do time em massa.
   1. Adicionar ou mover usuários para um time.
   2. [Criar um novo time](../managing-enterprise-teams-and-content/09-create-a-new-team-on-enterprise-plan.md) e adicionar usuários.
2. Gerenciar licenças e funções em massa.
   1. Mudar para Membro Avançado. As licenças avançadas não são suportadas embaixo do Programa de Licenças Flexíveis (PLP) e operam sempre em um modelo de limite fixo. Você só pode atribuir até o número de licenças avançadas que sua organização adquiriu. As organizações que usam o PLP para o modelo Padrão podem continuar a fazê-lo mantendo o Avançado com um limite fixo, permitindo um modelo de licenciamento misto: o Padrão pode continuar no PLP (licenças gratuitas ilimitadas com downgrade automático para Free Restrito), enquanto o Avançado permanece fixo na quantidade de licença adquirida. Usuários que precisam de funcionalidades avançadas devem ser explicitamente atribuídos uma licença Avançada ou seguir o fluxo de atualização ou solicitação de sua organização.
   2. Mudar para Membro Padrão ou Membro com Acesso Total (legado).
   3. Alterar para membro básico.
   4. Alterar para convidado ou convidado do time.
   5. Alterar para Free Restrito (disponível para [assinaturas Enterprise FLP](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)).
3. Mudar o grupo de cobrança ou criar um novo.
4. Revogar restrições.
5. Desativar em massa [usuários](01-deactivated-users.md)

#### Gerenciar convites em massa

Alterne para a guia Convites para ver os usuários convidados (usuários não registrados que receberam convites para entrar na sua assinatura há menos de 30 dias e ainda não se registraram na Miro). Selecione a lista de convidados para aplicar uma das ações abaixo.

1. Gerenciar membros do time em massa.
   1. Adicionar usuários a vários times, com ou sem remoção dos atuais.
   2. Adicionar usuários a um novo time ([criar um novo](../managing-enterprise-teams-and-content/09-create-a-new-team-on-enterprise-plan.md)).
2. Desativar [usuários em massa](01-deactivated-users.md).
3. Alterar licenças de usuários em massa.

#### Excluir em massa de um time

Na lista de **Times**, selecione o Time do qual você gostaria de excluir usuários. Depois de selecionar os usuários, você pode excluí-los em massa do time.

### Informações do usuário

As informações do usuário são um cartão individual e editável para cada usuário no seu plano. Ao contrário da gestão em massa, você pode ver o status e gerenciar uma pessoa individualmente. Cada usuário tem um **Perfil de usuário** com foto, nome, e-mail, número de boards, número de projetos, número de templates, times atuais e licença. Para abrir um cartão de usuário, clique no ícone de **três pontos** (**...**) na linha dele e selecione **Informações do usuário**.

:::note
Os detalhes do usuário incluem uma classificação **Interna** ou **Externa**. Usuários internos iniciam sessão com um e-mail de um domínio verificado. Usuários externos não. Para mais informações, veja [Controle de Domínio: Usuários internos e externos](../canvas-25-admin-features/domain-control/01-domain-control.md).
:::

Admins da empresa podem alterar a participação no time e conceder direitos de Admin a um usuário diretamente do cartão. Note que Admins não podem alterar detalhes de usuários como nome, foto de perfil, e-mail - ao invés, os usuários podem fazer isso nas configurações do próprio perfil. Se você usa [logon único](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), os dados são automaticamente atribuídos pelo seu provedor de identidade após o login bem sucedido.

### Perguntas frequentes

1. *Estou recebendo muitos pedidos de usuários para adicioná-los a diferentes times. Quero parar de receber essas notificações.*
   - Sua [privacidade do time](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) provavelmente está desabilitada, o que significa que os usuários Enterprise podem descobrir novos times para se juntar dentro da organização. Se você quer parar de receber esses pedidos, pode:
   - Habilite a privacidade, assim os usuários não poderão descobrir novos times na organização ou
   - Deixe os times completamente abertos, de modo que os usuários não precisem de sua aprovação para ingressar no time
2. *Muitos usuários estão recebendo uma licença Standard ou Full (legada) atribuída, mas eu não atribuí nenhuma. Por quê?*
   - Para cada time, você pode definir quem deve poder convidar usuários para um time específico. Certifique-se de configurar suas [configurações de convite](03-invitation-settings-on-enterprise-plan.md). Você também pode ativar o [Programa de licenças flexíveis](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) e definir a licença padrão (Free ou licença gratuita limitada) que os usuários receberão ao ingressar no seu plano.
