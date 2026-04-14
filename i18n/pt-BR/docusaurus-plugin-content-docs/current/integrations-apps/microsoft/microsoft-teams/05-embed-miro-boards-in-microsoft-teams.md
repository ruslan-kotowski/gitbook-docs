---
title: Como incorporar boards da Miro no Microsoft Teams
article_id: 360017572514
translation_id: 360017572514
locale: pt-br
sidebar_position: 5
created_at: '2019-02-11T10:13:30Z'
updated_at: '2025-04-24T13:52:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ms-teams
---

Incorpore boards da Miro aos canais do Microsoft Teams e compartilhe-os perfeitamente com os membros do time. Mantenha seus boards da Miro sempre acessíveis e o time todo sempre alinhado.

:::note
Veja como você pode incorporar boards da Miro em reuniões do Microsoft Teams: [Miro para Microsoft Teams Meetings (guia do admin)](01-miro-for-microsoft-teams-admin-guide.md), [Miro para Microsoft Teams Meetings (guia do usuário)](02-miro-for-microsoft-teams-user-guide.md).
:::

> **Disponível para:** todos os planos da Miro

### Como instalar o plugin

Primeiro, encontre a **Miro** na **loja do Microsoft Teams** ou siga o [link direto](https://teams.microsoft.com/l/app/8216e453-3db5-48ee-a3d6-5122f505c8a3).

:::warning
Observe que o admin locatário do Microsoft Teams deve habilitar o aplicativo da Miro em seu catálogo de aplicativos de terceiros para Teams. Se a Miro não for aprovada, não será exibida na lista dos aplicativos da loja do Microsoft Teams.
:::

Clique em **Adicionar** para instalar o plugin.

![Miro_plugin_installation.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790725266_Miro%20plugin%20installation.jpg)
*Instalação do plugin da Miro*

Depois de instalar o plugin da Miro, você será redirecionado para o chat onde poderá configurar o recebimento de notificações da Miro. Para saber mais, confira [este artigo](10-miro-notifications-in-microsoft-teams.md).

Porém, desde este instante você já pode começar a incorporar boards da Miro em um canal do Microsoft Teams sem qualquer configuração adicional.

### Como incorporar boards em canais do Microsoft Teams

> **Criado por:** [titulares](../../../using-miro/sharing-boards/01-board-access-rights.md) e [editores](../../../using-miro/sharing-boards/01-board-access-rights.md) do board, que também sejam membros do time onde o board está localizado.

Você pode incorporar seus boards aos canais do Microsoft Teams criando uma nova guia. Clique no ícone de adição. Será exibido um seletor com vários aplicativos. Encontre e selecione a Miro na lista de aplicativos. Caso você não tenha autorização na Miro no mesmo navegador ou no aplicativo para desktop, será necessário iniciar sessão na sua conta da Miro. Clique em **Começar** e faça login ou [crie sua conta na Miro](../../../getting-started/start-here/02-how-to-register-with-miro.md).

![embed_in_MS_teams.gif](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734975122_embed%20in%20MS%20teams.gif)
*Modal que solicita autorização do perfil da Miro*

Uma vez autorizado, você verá um seletor com boards da Miro. Esse seletor mostrará os boards aos quais você tem acesso no lado da Miro. Observe que você pode receber autorização na Miro e no Microsoft Teams por meio de e-mails diferentes.

Еscolha um board que gostaria de adicionar ao seu canal do Microsoft Teams.

![MS_teams_embed_picker.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734978322_MS%20teams%20embed%20picker.jpg)
*Seletor de boards da Miro*

Observe que apenas titulares e editores de board que são membros do time podem incorporar boards da Miro. Se você escolher um board no qual não possui o nível de acesso necessário, verá uma mensagem de aviso.

![incapaz_to_embed_boards.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790732690_unable%20to%20embed%20boards.jpg)
*Mensagem de aviso de que seu nível de acesso não permite incorporar um board*

Aqui, você pode definir permissões para o resto dos participantes da reunião e dar ou restringir o acesso ao board. Você pode escolher entre os seguintes tipos de permissão:

- **Qualquer pessoa pode editar** (não é necessário iniciar a sessão)
- **Qualquer pessoa pode comentar** (não é necessário iniciar a sessão)
- **Qualquer pessoa pode visualizar** (não é necessário iniciar a sessão)
- **Privado**

![nível_de_compartilhamento.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790733586_sharing%20level.jpg)
*Configurações de acesso para um board incorporado*

:::note
Observe que as configurações de compartilhamento definidas para um board na Miro também podem definir o acesso ao board no Microsoft Teams. Se o board for compartilhado publicamente na Miro, estará disponível para qualquer pessoa no Microsoft Teams, mesmo que você tenha incorporado o board como **Privado**. No entanto, se o seu board for privado no lado da Miro e você o tiver incorporado com acesso Qualquer pessoa pode visualizar/comentar/editar, o acesso ao board na Miro não será afetado. Saiba mais.
:::

:::note
Para usuários do [plano Enterprise](../../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md) da Miro, suas configurações de acesso seguirão os controles de acesso definidos para toda a organização, o que pode implicar que algumas opções de compartilhamento sejam restritas. Saiba mais: [Como permitir ou restringir a inserção de boards da Miro em aplicativos compatíveis](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

> **⚠️ A opção [Qualquer pessoa pode comentar](../../../plans-billing/miro-plans/09-free-plan.md) não é compatível com a inserção de um board localizado em um time gratuito.**

Depois que o board for incorporado, você poderá começar a interagir com ele imediatamente.

![Miro_embed_in_MS_teams.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734972562_Miro%20embed%20in%20MS%20teams.jpg)
*Board incorporado em um canal do Microsoft Teams*

> *✏️* Os usuários do Microsoft Teams que usam a Miro no aplicativo móvel do Microsoft Teams podem visualizar e comentar nos boards dependendo das permissões definidas. Para editar boards, recomendamos que os usuários instalem nosso [aplicativo móvel](../../../getting-started/apps-for-devices/08-mobile-app.md) nativo, para o qual otimizamos a interface do usuário.

![Miro_in_MS_Team_on_mobile.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734976146_Miro%20in%20MS%20Team%20on%20mobile.jpg)
*Board da Miro no MS Teams para dispositivos móveis: pressione **Abrir no aplicativo** para instalar o aplicativo móvel nativo da Miro*

### Perguntas frequentes

1. *É necessário que cada membro do time tenha um perfil da Miro para visualizar os boards incorporados no Microsoft Teams?
   - Se você escolher **Qualquer pessoa pode visualizar/comentar/editar** ao incorporar o board, mesmo usuários não cadastrados poderão visualizar/comentar no board. Ainda, se o board for [compartilhado publicamente](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#compartilhar-boards-por-meio-de-um-link-publico) no lado da Miro, estará disponível para qualquer pessoa no Microsoft Teams.*
2. *Depois que um board é incorporado, quem pode alterar o acesso do board no MS Teams (por exemplo, de “Qualquer pessoa pode visualizar” para “Privado”)?
   - Ninguém pode alterar o acesso ao board inserido, nem mesmo quem o inseriu. No entanto, qualquer pessoa pode clicar em **Configurações** na aba e, em seguida, escolher outro (ou o mesmo) board para a mesma aba e selecionar outro nível de acesso para o board escolhido.*
3. *Tenho duas conta na Miro com dois e-mails diferentes e gostaria de incorporar um board da Miro do meu segundo perfil da Miro. Como posso mudar o perfil da Miro?
   - O seletor mostra os boards do usuário com o qual você iniciou sessão na Miro no mesmo navegador. Abra a Miro em outra guia do navegador, saia e faça login no seu segundo perfil da Miro.
   Se usar o aplicativo para desktop do Microsoft Teams, encerre a sessão no aplicativo. Você também será desconectado da Miro dentro do aplicativo. Em seguida, faça login no aplicativo e tente [incorporar um board](#h_5af20ae6-78c0-4e6c-ab20-e4968c89c97f). Você será solicitado a fazer login na Miro e poderá fazer login em outro perfil da Miro.*
