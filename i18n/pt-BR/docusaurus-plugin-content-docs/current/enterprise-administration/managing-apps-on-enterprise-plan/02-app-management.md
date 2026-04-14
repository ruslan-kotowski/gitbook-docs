---
title: Gerenciamento de aplicativos
article_id: 4404659741458
translation_id: 4404659741458
locale: pt-br
sidebar_position: 2
created_at: '2021-08-03T15:46:50Z'
updated_at: '2026-01-29T10:00:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: apps-management
---

Saiba como gerenciar aplicativos e permissões no nível da organização e do time.

> **Relevante para:** Plano Business, Plano Enterprise
> **Quem pode fazer isto:** admin do time, Admin da empresa

### Quem pode gerenciar aplicativos?

O gerenciamento de aplicativos no nível da organização está disponível somente no plano Enterprise para Admins da empresa. O gerenciamento de aplicativos no nível do time está disponível nos planos Business e Enterprise para admins do time e Admins da empresa.

### Adicionar aplicativos para uma organização ou times específicos

Adicione e autorize aplicativos para todos os usuários ou times específicos da sua organização através dos controles de gerenciamento de aplicativos.
Vá para as **configurações da empresa** > **Apps e integrações** > **Apps**. Nesta seção, os Admins da empresa podem adicionar aplicativos para todos ou times específicos.

![apps-access.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803476626_apps-access.png)*Controle de gerenciamento de aplicativos nas configurações da empresa*

Insira um nome de aplicativo ou ID de cliente na barra de pesquisa. Selecione um aplicativo no menu suspenso e clique em **Adicionar**.

![add-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780909714_add-app.png)*Como adicionar um aplicativo pelas configurações da empresa*

Você pode adicionar o aplicativo para todos os times da sua organização ou escolher times específicos. Se um aplicativo já estiver disponível para alguns times, a tag correspondente será exibida. Se você adicionar novamente o aplicativo a um time, os membros do time deverão reautorizar esse aplicativo. Clique em **Adicionar** para finalizar.

![add-apps-where.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780917010_add-apps-where.png)
*Como selecionar para quem o aplicativo Google Drive será instalado*

Ao adicionar um aplicativo para todos os times, o aplicativo também será adicionado para todos os times recém-criados.

### Aplicativos pré-adicionados

Alguns aplicativos já foram pré-adicionados para os usuários. Eles podem exigir autorizações adicionais ou início de sessão individual. Estes aplicativos pré-adicionados são: [Box](../../integrations-apps/more-integrations/05-box-legacy.md), [Dropbox](../../integrations-apps/more-integrations/06-dropbox.md), [Google Drive](../../integrations-apps/google/05-google-drive.md), [OneDrive](../../integrations-apps/microsoft/06-onedrive.md), [Smartsheet](../../integrations-apps/more-integrations/15-smartsheet-app-for-miro.md), [Azure Cards](../../integrations-apps/microsoft/03-azure-cards.md), [Jira Cards](../../integrations-apps/atlassian/03-jira-cards.md),[Brandfetch](https://miro.com/marketplace/brandfetch/), [Google Images](../../integrations-apps/google/06-google-images.md), [Slack](../../integrations-apps/more-integrations/14-slack.md). Estes aplicativos não serão pré-adicionados se não constarem na lista aprovada pela empresa. Você pode gerenciar essa lista se for um Admin da empresa.

### Pré-autorizar aplicativos para uma organização

Se adicionar um aplicativo, também pode pré-autorizá-lo ao mesmo tempo. Se um aplicativo for previamente adicionado e autorizado por um admin, os usuários da organização podem começar a usá-lo de imediato. Alguns aplicativos podem requerer início de sessão individual em um serviço de terceiros.

Esta funcionalidade está disponível somente para aplicativos criados com o Web SDK da Miro. O Web SDK da Miro permite estender as funcionalidades da Miro. É uma caixa de ferramentas que permite criar aplicativos avançados que são executados em um board da Miro.

### Como aprovar aplicativos para gerenciamento de usuários individuais

Por padrão, os usuários podem adicionar qualquer aplicativo para seu time. Os Admins da empresa podem restringir o gerenciamento de aplicativos de usuários para permitir que somente determinados aplicativos sejam adicionados por seus times.

Os Admins da empresa podem habilitar ou limitar a adição de determinados aplicativos para seus usuários, acessando as configurações da **Empresa** > **Aplicativos e integrações** > **Aplicativos** > **Gerenciar aplicativos** e habilitando a opção **Restringir membros a adicionar somente os aplicativos da lista abaixo**.

![manage-apps.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780921490_manage-apps.png)*Como limitar a instalação de aplicativos aprovados no plano Enterprise*

Se esse limite estiver habilitado, somente os aplicativos aprovados podem ser adicionados pelos usuários Enterprise. Para aprovar um aplicativo para usuários, habilite a opção ao lado do aplicativo ou cole um ID de cliente no campo correspondente para aprovar um aplicativo desenvolvido internamente.

Para restringir um aplicativo adicionado anteriormente, localize o aplicativo na lista e verifique se a opção ao lado do aplicativo está desabilitada. Observe que os usuários de todos os times Enterprise não poderão usar o aplicativo se ele estiver restrito.

Caso um aplicativo esteja restrito na sua organização, os usuários poderão enviar [solicitações de uso do aplicativo aos Admins da empresa](03-app-request-flow.md).

Os usuários podem ver os aplicativos aprovados no Marketplace nos boards da Miro armazenados no plano Enterprise.

### Permitir ou restringir o uso de aplicativos em times

Os Admins do time e Admins da empresa também podem gerenciar o uso de aplicativos no nível do time: podem permitir ou restringir que os membros do time adicionem novos aplicativos para o time. A configuração é definida para cada time separadamente.

![add-apps-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780928914_add-apps-team.png)*Aplicativos e integrações nas configurações do time*

Saiba mais sobre [aplicativos e integrações da Miro.](../../integrations-apps/integrations-basics)
