---
title: Times de desenvolvedores do Enterprise
article_id: 4766759572114
translation_id: 4766759572114
locale: pt-br
sidebar_position: 4
created_at: '2022-03-22T14:13:15Z'
updated_at: '2025-04-29T13:25:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: developer-teams
---

Conheça a opção de configurar times de desenvolvedores em assinaturas Enterprise - uma maneira fácil e segura de criar aplicativos personalizados para seu plano Enterprise .

> **Disponível para:** [Plano Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Configurado por:** Admins da empresa
> Usuários em outros planos Miro podem criar times de desenvolvedores [nesta página](https://developers.miro.com/docs/rest-api-build-your-first-hello-world-app#step-1-create-a-developer-team-in-miro)

### Criando uma time de desenvolvedores

Para configurar uma time de desenvolvedores, abra Configurações **da empresa** > **Equipes** e clique em **Criar nova time** no canto superior direito.

No próximo pop-up, insira o nome da time e escolha o nível de permissões da time : você pode definir as configurações de permissões padrão ou selecionar um time para copiar as permissões da time (saiba mais sobre[permissões e configurações padrão](../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)). Marque a caixa **time de desenvolvedores**, confirme sua autorização e clique em **Criar time**.

![criar-dev-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803173266_create-dev-team.png)
*Criando uma time de desenvolvedores*

### Permissões da time do desenvolvedor Enterprise

Você pode criar aplicativos com segurança para a time de desenvolvedores Enterprise , que fornece todos os recursos de segurança Enterprise enquanto faz parte da sua assinatura Enterprise .

A time de desenvolvedores Enterprise tem boards ilimitados e não há limite de membros.

Os boards criados na time terão uma marca d'água para diferenciá-los de outras times da organização.

A time tem todas as configurações padrão para configurar permissões de usuário no plano Enterprise : você pode permitir/proibir membros do time de convidar novos usuários, compartilhar boards com a time/Empresa/por link público, mover boards, restringir domínios permitidos, etc. Para mais informações, confira [este artigo](../managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md).

### Criação e instalação de aplicativos

> **Configurado por:** Admins do time
> Se você quiser convidar desenvolvedores para criar um aplicativo na time, certifique-se de [conceder permissões de admin do time](../../administration/user-management/06-how-to-manage-admin-roles.md)

Para criar um novo aplicativo no seu Miro Enterprise usando a time Enterprise Developer, navegue até [**Configurações do perfil**](../../using-miro/managing-your-profile/01-profile-settings.md) **> Seus aplicativos**, concorde com os termos e condições e clique em **Criar novo aplicativo.**

![perfil-criar-novo-aplicativo.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780634770_profile-create-new-app.png)
*Seus aplicativos nas configurações do perfil*

:::tip
Você também pode navegar até a página clicando em **Criar um aplicativo** no canto superior direito do painel da equipe do desenvolvedor.
:::

![dev-team-cria-um-aplicativo.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780641298_dev-team-build-an-app.png)
*A opção de criar novos aplicativos personalizados*

Insira o nome do aplicativo, selecione sua time de desenvolvedores para o aplicativo e clique em **Criar aplicativo.**

*![criar_um_novo_aplicativo.jpg](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/21017516016146_create%20a%20new%20app.jpg)*
*Criando um novo aplicativo para a time de desenvolvedores Enterprise*

Na página do aplicativo, role para baixo e selecione o escopo de acesso que você deseja conceder ao seu aplicativo e clique em **Instalar aplicativo e obter token OAuth.**

*![permissões_de_aplicativo.jpg](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/21017529025810_app%20permissions.jpg)*
*Permissões do aplicativo*

Ao instalar o aplicativo, selecione um time (diferente da time de desenvolvedores) da sua organização Enterprise e clique em **Instalar e autorizar**. O token de acesso será exibido na próxima etapa.

![instalando_o_aplicativo.jpg](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/21017516017426_installing%20the%20app.jpg)
*Instalando o aplicativo*

### Excluindo uma time de desenvolvedores

Você pode excluir a time de desenvolvedores como faria com qualquer outra time na sua organização Enterprise , mas primeiro precisa excluir todos os aplicativos criados nessa time. Depois que os aplicativos forem excluídos, navegue até [**Equipes**](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md), clique no nome da time , selecione a guia **Perfil** e, em seguida, selecione **Excluir time**.

:::warning
Observe que ao excluir a time de desenvolvedores Enterprise , todos os tokens associados a ela não serão mais válidos.
:::

![delete-dev-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803181586_delete-dev-team.png)*Excluir a time Enterprise Developer*
