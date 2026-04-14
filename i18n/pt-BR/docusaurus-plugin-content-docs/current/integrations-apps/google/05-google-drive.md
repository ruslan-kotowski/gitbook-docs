---
title: Google Drive
article_id: 360017731253
translation_id: 360017731253
locale: pt-br
sidebar_position: 6
created_at: '2019-02-11T10:14:01Z'
updated_at: '2025-01-13T14:51:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-drive-onedrive
---

O **Google Drive** permite armazenar arquivos online com segurança, acessá-los de qualquer lugar e colaborar com outras pessoas. Com a integração do Google Drive, facilitamos o foco nas suas tarefas e o rastreamento dos seus documentos diretamente no board.

![Google_Drive_on_the_Upload_menu.jpg](https://help.miro.com/hc/article_attachments/21016134647058)

> **Configurado por:** cada usuário separadamente (os admins podem restringir a instalação do aplicativo por usuários que não sejam admins)
> **Disponível em:** versão para navegador, [aplicativo para desktop](../../getting-started/apps-for-devices/05-desktop-app.md) (funcionalidade completa e edição de arquivos); [aplicativo para tablet](../../getting-started/apps-for-devices/11-tablet-app.md), [aplicativo para celular](../../getting-started/apps-for-devices/08-mobile-app.md) (funcionalidade limitada, não é compatível com edição)

### Como ativar o Google Drive

Para começar a adicionar arquivos do Google Drive, você deve instalar o plugin e conectar seu Google Drive à Miro.

Instale o aplicativo do [Marketplace da Miro](https://miro.com/marketplace/google-drive/?backUrl=%2Fmarketplace%2F). Depois de clicar em **Obter aplicativo**, você verá a sugestão de escolher um time para instalar o plugin. ![install_Google_Drive.jpg](https://help.miro.com/hc/article_attachments/21016134651282)*Como escolher um time ao instalar o plugin do Google Drive*

Você também pode instalar o plugin a partir de um board. Na barra de Criação, selecione **Ferramentas, mídia e integrações** (**+**). Um painel é aberto. Na aba **Ferramentas**, procure por Google Drive. Selecione **Upload** e depois **Google Drive**.

![Google_Drive_on_the_toolbar.jpg](../../../../../../docs/integrations-apps/google/images/21016121227026_Google%20Drive%20on%20the%20toolbar.jpg)

Em seguida, conecte o Google Drive à Miro. Há duas maneiras simples.

1.  Nas configurações do seu perfil. Na barra do board, selecione o ícone de três traços. A barra lateral é aberta. Selecione seu avatar e depois selecione **Configurações**. As configurações do seu perfil serão abertas em uma nova janela. Selecione a aba **Integrações**. Para o **Google Drive**, selecione **Conectar**.

![connect_Google_Drive.jpg](../../../../../../docs/integrations-apps/google/images/21016121228306_connect%20Google%20Drive.jpg)*Google Drive na página de integrações*

2. Conecte seu perfil da Miro ao Google Drive a partir do board, clicando no **Google Drive** no menu **Carregar**na barra de ferramentas:

![Google_Drive_on_the_Upload_menu.jpg](https://help.miro.com/hc/article_attachments/21016134647058)*Ícone do Google Drive na barra de ferramentas*

Confirme a autorização para a conta do Google necessária e **permita** que o aplicativo acesse seus arquivos:

![permissions.jpg](https://help.miro.com/hc/article_attachments/21016134655122)
*Permissões do Google Drive*

Observe que essas são as permissões padrão para o Google Drive.

– **Veja e baixe todos os seus arquivos do Google Drive** — para um seletor de arquivos do Google Drive em um board. Isso permite a importação de documentos do Google Drive para a Miro.

– **Veja, edite, crie e exclua somente os arquivos específicos do Google Drive que você usa com este aplicativo** — para poder salvar um board da Miro no Google Drive.

O aplicativo do Google Drive gerencia apenas os arquivos que criamos no Drive (links para boards, etc).  A Miro não pode gerenciar nenhum conteúdo no seu Google Drive. Para implementar a integração, usamos a **API do Google Drive v3**. Nesta API, os escopos são agrupados de tal forma que as permissões de acesso de edição não podem ser solicitadas separadamente das permissões de acesso total ao disco. Se você quiser dar uma olhada, confira as permissões no artigo do Google, [Escopos para APIs do Google](https://developers.google.com/identity/protocols/googlescopes).

Se você precisar alterar a conta do Google conectada à Miro, vá para **Configurações do perfil** > **Integrações**, clique em **Sair** ao lado do **Google Drive** e conecte-se a outra conta.

![Google_Drive_log_out_in_settings.jpg](../../../../../../docs/integrations-apps/google/images/21016121230610_Google%20Drive%20log%20out%20in%20settings.jpg)*Conexão do Google Drive nas configurações do perfil*

### Como adicionar arquivos do Google Drive e das unidades compartilhadas

> **Disponível em:** versão para navegador, [aplicativo para desktop](../../getting-started/apps-for-devices/05-desktop-app.md), [aplicativo para tablet](../../getting-started/apps-for-devices/11-tablet-app.md), [aplicativo móvel](../../getting-started/apps-for-devices/08-mobile-app.md) (funcionalidade limitada)

:::warning
Qualquer pessoa com acesso a um board da Miro pode extrair seus documentos importados, mesmo que eles sejam restritos pelo Google. Para proteger seus arquivos, é importante evitar o compartilhamento do board com indivíduos que não devem ter acesso aos documentos.
:::

Para adicionar um arquivo do Google Drive:

1. Cole o URL do documento diretamente no board (observe que colar um URL em uma [forma](../../using-miro/essential-tools/11-shapes.md) ou uma [nota adesiva](../../using-miro/essential-tools/14-sticky-notes.md) não insere seu documento no board, mas adiciona o link como texto simples). Quando você copia um link para uma planilha específica das planilhas do Google e cola no board da Miro, a planilha colada ainda começará a partir da primeira página da Miro.

   ou
2. Clique no botão **Carregar**na barra de ferramentas (mostrada na captura de tela acima) e escolha o **Google Drive**. Você verá o menu do seletor. Selecione todos os documentos que você gostaria de adicionar e clique em **Selecionar**. Você também pode usar a barra de pesquisa para encontrar documentos no seu Google Drive.

:::tip
Para adicionar um documento do Google Drive em um board no [aplicativo móvel](../../getting-started/apps-for-devices/08-mobile-app.md), cole o URL do documento por meio do menu Carregar.
:::

![select_a_file_in_Google_Drive.gif](https://help.miro.com/hc/article_attachments/21016134656786)*Como selecionar um documento no Google Drive*

Adicione documentos de **unidades compartilhadas**: alterne para a guia e escolha arquivos.

![team_drive.jpg](https://help.miro.com/hc/article_attachments/21016134659730)*Drive do time no seletor do Google Drive*

### Como editar os documentos do Google

> **Disponível em:** versão para navegador, [aplicativo para desktop](../../getting-started/apps-for-devices/05-desktop-app.md)

Você pode inserir os documentos, as planilhas e os slides do Google diretamente no board, mover e redimensioná-los, bem como deslizar as páginas dos documentos.

Clique no documento e você verá um menu de contexto com as opções para alternar páginas, **fixar** uma página, **extrair páginas**, **editar** conteúdo, **recarregar**, **atualizar**ou ir para a **fonte**.

Para começar a editar o documento, clique no ícone da caneta no menu de contexto ou clique duas vezes no documento. O documento é aberto em uma janela pop-up e você pode editá-lo como se estivesse no seu Google Drive. Clique em **Fechar**ou na área cinza para concluir a edição. Todas as alterações são salvas automaticamente e ficam visíveis no board, bem como nos documentos do Google.

![google_drive_edit_docs.gif](https://help.miro.com/hc/article_attachments/21016121345938)*Como editar um documento do Google incorporado*

Se preferir, você também pode clicar no botão da **fonte**e o documento será aberto para edição na próxima guia.

Se você fez alguma edição diretamente do seu Google Drive (especialmente ao trabalhar offline), atualize a inserção no board usando o botão **Atualizar**no menu de contexto. Os arquivos inseridos do Google Drive não são atualizados automaticamente nos boards da Miro (a menos que o arquivo seja editado na Miro).

![update_button.jpg](../../../../../../docs/integrations-apps/google/images/21016121232274_update%20button.jpg)*Botão de atualização*

### Como gerenciar os direitos de acesso

Observe que os direitos de acesso no Google Drive e na Miro são definidos *separadamente*. Isso significa que, para deixar alguém editar um documento do Google no board, você precisa compartilhar o documento com esse usuário no Google Drive com os direitos de *edição* e também [convidá-lo para o board como *editor.*](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)

Se você permitir que alguém edite o documento no Google, mas convidar para o board com [direitos somente de visualização ou de comentário](../../using-miro/sharing-boards/01-board-access-rights.md), esse usuário não poderá ativar o modo de edição do documento. Por outro lado, se você convidar uma pessoa para o board com acesso de edição, mas não compartilhar o documento com ela no Google Drive, o Google não permitirá que ela o edite.

Certifique-se de que você e os membros do seu time recebam o nível de acesso necessário para uma colaboração bem-sucedida.

### Como salvar seu board no Google Drive

> **Configurado por:** titulares dos boards

Na barra do board, selecione os três pontos verticais. O **menu principal** é aberto. Selecione **Board** > **Exportar** > **Salvar no Google Drive**.

No Google Drive, você agora pode clicar no board salvo e ele será aberto em uma guia separada do navegador. Se você excluir o board do Google Drive, ele ainda estará disponível na Miro. No entanto, se você excluir o board na Miro, não poderá mais acessá-lo do Google Drive.

:::warning
Se você não for titular do board, receberá a mensagem de erro abaixo.
:::

![Google_Drive_error.jpg](https://help.miro.com/hc/article_attachments/21016121338898)*Mensagem de erro: o usuário não tem direitos suficientes para salvar o board*

### Como desinstalar o plugin

Para desinstalar o plugin para um time, encontre-o na seção **Aplicativos e integrações** das configurações do time e clique em **Desinstalar para o time**.

![uninstall_Google_Drive_app.jpg](https://help.miro.com/hc/article_attachments/21016134662546)*Como desinstalar o Google Drive para um time*

Para desconectar a Miro do Google Drive, abra a página **Integrações** das configurações do seu perfil e clique em**Sair** perto do ícone do Google Drive.

![Google_Drive_log_out_in_settings.jpg](../../../../../../docs/integrations-apps/google/images/21016121230610_Google%20Drive%20log%20out%20in%20settings.jpg)*Como desconectar o Google Drive da Miro*

### As funcionalidades não disponíveis para arquivos do Google Drive

**Geral**

- Página inicial do Google Drive
- Como mover arquivos entre pastas
- Compartilhamento
- Pesquisa na ajuda

**Apresentações do Google**

- Modo de apresentação

### Possíveis problemas e como resolvê-los

**Não é possível carregar o erro**

Se você receber a mensagem de erro **Infelizmente, parece que você não tem permissão para carregar este arquivo ou o arquivo foi excluído. Verifique o direito de acesso e tente novamente** ao tentar carregar um arquivo do Google Drive para um board da Miro. Peça ao seu admin do Google para permitir que os usuários acessem o Google Drive com a API do SDK do Drive:

1. Faça login no [Admin Console do Google.](https://admin.google.com/)
2. Clique em **Página Inicial > Aplicativos > Espaço de trabalho do Google**. Certifique-se de que o **Drive e Docs** estejam **HABILITADOS para todos os usuários.**
3. Clique em **Drive e Docs > Funcionalidades e aplicativos**. Na seção **SDK do Drive** , certifique-se de que **permitir que os usuários acessem o Google Drive com a API do SDK do Drive** esteja **HABILITADO**.

![unable_to_upload.png](https://help.miro.com/hc/article_attachments/21016134663954)
*Não é possível carregar a mensagem de aviso*

**Problema de autorização**

Se você não puder conectar seu Google Drive à Miro, certifique-se de fornecer acesso à Miro para **visualizar e baixar todos os seus arquivos do Google Drive** e para **visualizar, editar, criar e excluir somente os arquivos específicos do Google Drive que você usa com este aplicativo** ao conectar o Google Drive. Para isso, vá para as [configurações do seu perfil da Miro](../../using-miro/managing-your-profile/01-profile-settings.md) > **Integrações**, remova a conexão com o Google Drive e configure-o novamente.

![Permissions.png](https://help.miro.com/hc/article_attachments/21016121341330)
*Acesso da Miro à conta do Google Drive*

### Perguntas frequentes

1. *Posso abrir um arquivo incorporado no Google Drive?*
   - Sim, selecione o documento e clique no botão  **fonte** no menu de contexto.
2. *Posso colar o conteúdo do board da Miro em um arquivo do Google Drive?*
   - Você pode [copiar o conteúdo do board como texto ou imagem](../../using-miro/working-on-the-board/09-copy-as-text-or-as-an-image.md) e colá-lo em um arquivo do Google Drive.
