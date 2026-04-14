---
title: Adicionar Miro como uma guia no Microsoft Teams
article_id: 4411292563602
translation_id: 4411292563602
locale: pt-br
sidebar_position: 4
created_at: '2021-12-01T04:50:21Z'
updated_at: '2025-11-25T16:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
availability:
  notes: 'Disponível para: planos Free, Starter, Business, Education, Enterprise e
    todos os planos do Microsoft 365'
---

Os usuários podem adicionar boards da Miro às reuniões, canais e eventos de calendário do Microsoft Teams para colaborar e compartilhar o acesso com outros membros do time sem problemas.
Neste artigo, você aprenderá como usar o Miro em:

- Reuniões do Microsoft Teams
- Eventos do calendário do Microsoft Teams
- Canais e chats do Microsoft Teams

## Adicionar Miro em reuniões do Microsoft Teams

- Os usuários que participam de uma reunião no MS Teams por celular ou tablet só podem visualizar um board da Miro anexado e não podem editá-lo nem comentar nele.
- Qualquer usuário do Microsoft Teams que tenha autorizado o aplicativo da Miro pode adicionar o Miro à reunião. Qualquer usuário do Teams com um perfil da Miro pode compartilhar um board no primeiro plano.
- ⚠️ A Microsoft não permite que os usuários convidados usem aplicativos em uma reunião do Teams. Os usuários devem estar conectados ao Teams para usar qualquer aplicativo (incluindo a Miro).

1. Clique no menu suspenso **Mais ações.**
2. Selecione **+Adicionar um aplicativo.**
3. Pesquise e clique no ícone da Miro.
4. Aqui, você será solicitado a se inscrever ou fazer login no seu perfil da Miro.
5. Selecione qual board você deseja compartilhar ou escolha criar um novo board da Miro em branco.
6. Defina permissões para o restante dos participantes da reunião e conceda ou restrinja o acesso ao board. Você pode escolher entre os seguintes tipos de permissão:

- **Qualquer pessoa pode editar** (não é necessário fazer login no Miro )
- **Qualquer pessoa pode comentar** (não é necessário fazer login, não é compatível com boards localizados em uma time Free )
- Qualquer pessoa pode visualizar (não é necessário iniciar a sessão)
- **Privado** (somente aqueles que já tiveram acesso ao board podem colaborar)

“**Qualquer pessoa pode editar, comentar ou visualizar**” permite que qualquer pessoa no seu locatário do Microsoft Teams acesse o board. Isso inclui:

- Outros usuários da Miro que não fazem parte da sua organização.
- Usuários que não têm um perfil da Miro.
- Usuários na sua organização que não estão logados na Miro.

:::note
As configurações de compartilhamento definidas para um board no Miro também podem definir o acesso ao board no Microsoft Teams. Se o board for compartilhado publicamente no Miro, ele estará disponível para qualquer pessoa no Microsoft Teams, mesmo que você tenha fixado o board como [Privado](../../../using-miro/sharing-boards/15-make-a-miro-board-private.md). No entanto, se o seu board for privado no lado do Miro e você o tiver fixado com o acesso Qualquer pessoa pode visualizar/ comentar/editar, o acesso ao board no lado do Miro não será afetado. [Saiba mais](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).
:::

:::note
Para os usuários do plano Enterprise da Miro, suas configurações de acesso seguirão os controles de acesso para toda a organização. O compartilhamento de links públicos para incorporações precisa ser habilitado pelos admins em **Configurações da empresa** > **Segurança**. Saiba mais em [Gerenciando a política de compartilhamento Enterprise para integrações incorporadas](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

Se você precisar alterar os direitos de acesso de um board inserido, remova a guia e adicione novamente com um nível de acesso diferente.

Agora você pode acessar o board da Miro a qualquer momento durante a reunião na aba específica. Se você criar vários boards, haverá uma única guia para cada board.

Se clicar na Miro, verá a guia da Miro no lado direito com o board que você anexou a esta reunião.

Você pode selecionar o botão Compartilhar em tela para enviar o board para todos os participantes e colaborarem ao mesmo tempo. Você pode parar de compartilhar o board a qualquer momento ao clicar no botão Parar a apresentação, localizado na parte superior.

## Fixar boards em eventos do calendário do Microsoft Teams

:::note
O calendário do Outlook ainda não é suportado.
:::

- Os eventos do calendário do Teams devem ser salvos e ter pelo menos um participante antes que um board da Miro possa ser anexado à reunião.
- Não há como remover um board da Miro de um convite de reunião do Teams ([artigo de referência da Microsoft](https://support.microsoft.com/en-gb/office/remove-a-tab-in-microsoft-teams-c18c875c-0738-40ec-a228-61d7eb27f745#:~:text=In%20one%2Don%2Done%20and,the%20tab%20and%20select%20Remove.)). Os usuários devem excluir o convite e criar um novo sem um board.

1. Primeiro, agende uma nova reunião no calendário do Microsoft Teams. Não se esqueça de adicionar um nome para a reunião e convidar os participantes.
2. Clique em **Enviar** para compartilhar o convite.
3. Depois que a reunião for salva, clique nela novamente e selecione **Editar**para poder anexar um board da Miro.
4. Você poderá fixar o Miro como uma guia usando o sinal de mais na parte superior da tela (**+**).
5. Na próxima tela, você será solicitado a adicionar o aplicativo da Miro. Procure por Miro na barra de pesquisa ou selecione Miro se você já o vir.
6. Selecione **Adicionar** para poder adicionar o Miro.
7. Você será solicitado a entrar no seu perfil da Miro dentro do Teams.
8. Depois de entrar no Miro, você será solicitado a selecionar qual board deseja adicionar à reunião. Você pode pesquisar e selecionar um board existente ou criar um novo board em branco.
9. Aqui, você também pode definir permissões para o restante dos participantes da reunião e conceder ou restringir acesso ao board. Então s**eleger Salvar para que você possa anexar o board da Miro selecionado à reunião do Teams. Você pode escolher entre os seguintes tipos de permissão:**

- **Qualquer pessoa pode editar** (não é necessário iniciar a sessão)
- **Qualquer pessoa pode comentar** (não é necessário iniciar a sessão)
- **Qualquer pessoa pode visualizar** (não é necessário iniciar a sessão)
- **Privado**

## Fixar boards em canais e chats do Microsoft Teams

> **Função necessária:** [titulares e](../../../using-miro/sharing-boards/01-board-access-rights.md) [editores do board](../../../using-miro/sharing-boards/01-board-access-rights.md) que são membros da time onde o board está localizado

Você pode fixar boards nos canais do Microsoft Teams criando uma nova aba.

1. Clique no ícone de adição.
2. Um seletor será aberto com vários aplicativos.
3. Encontre e selecione a Miro na lista de aplicativos.
4. Caso você não tenha autorização na Miro no mesmo navegador ou no aplicativo para desktop, será necessário iniciar sessão na sua conta da Miro. Clique em **Começar** e faça login ou [crie sua conta na Miro](../../../getting-started/start-here/02-how-to-register-with-miro.md).
5. Uma vez autorizado, você verá um seletor com boards da Miro. Esse seletor mostrará os boards aos quais você tem acesso no lado da Miro. Observe que você pode receber autorização na Miro e no Microsoft Teams por meio de e-mails diferentes.
6. Еscolha um board que gostaria de adicionar ao seu canal do Microsoft Teams. Se você escolher um board no qual não possui o nível de acesso necessário, verá uma mensagem de aviso.
7. Defina permissões para o restante dos participantes da reunião e conceda ou restrinja o acesso ao board. Você pode escolher entre os seguintes tipos de permissão:

   - **Qualquer pessoa pode editar** (não é necessário iniciar a sessão)
   - **Qualquer pessoa pode comentar** (não é necessário iniciar a sessão)
   - **Qualquer pessoa pode visualizar** (não é necessário iniciar a sessão)
   - **Privado**
   > ✏️ Os usuários do Microsoft Teams que usam a Miro no aplicativo móvel do Microsoft Teams podem visualizar e comentar nos boards dependendo das permissões definidas. Para editar boards, recomendamos que os usuários instalem nosso [aplicativo móvel](../../../getting-started/apps-for-devices/08-mobile-app.md) nativo, para o qual otimizamos a interface do usuário.

   ## Perguntas frequentes

É necessário que cada membro do time tenha um perfil da Miro para visualizar os boards incorporados no Microsoft Teams?

- Se você escolher **Qualquer pessoa pode visualizar/comentar/editar** ao incorporar o board, mesmo usuários não cadastrados poderão visualizar/comentar no board. Ainda, se o board for compartilhado publicamente no lado da Miro, estará disponível para qualquer pessoa no Microsoft Teams.

Depois que um board é incorporado, quem pode alterar o acesso do board no MS Teams (por exemplo, de “Qualquer pessoa pode visualizar” para “Privado”)?

- Ninguém pode alterar o acesso ao board inserido, nem mesmo quem o inseriu. No entanto, qualquer pessoa pode clicar em **Configurações** na aba e, em seguida, escolher outro (ou o mesmo) board para a mesma aba e selecionar outro nível de acesso para o board escolhido.

Tenho duas conta na Miro com dois e-mails diferentes e gostaria de incorporar um board da Miro do meu segundo perfil da Miro. Como posso mudar o perfil da Miro?

- O seletor mostra os boards do usuário com o qual você iniciou sessão na Miro no mesmo navegador. Abra a Miro em outra guia do navegador, saia e faça login no seu segundo perfil da Miro.

Se usar o aplicativo para desktop do Microsoft Teams, encerre a sessão no aplicativo. Você também será desconectado da Miro dentro do aplicativo. Em seguida, faça login no aplicativo e tente [incorporar um board](05-embed-miro-boards-in-microsoft-teams.md). Você será solicitado a fazer login na Miro e poderá fazer login em outro perfil da Miro.
