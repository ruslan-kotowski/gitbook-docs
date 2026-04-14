---
title: Miro para Confluence
article_id: 360020712594
translation_id: 13809019235730
locale: pt-br
sidebar_position: 3
created_at: '2023-09-18T15:22:12Z'
updated_at: '2026-03-12T09:15:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: 'Disponível para: todos os planos da Miro; Confluence Cloud (inserção na
    Miro), Confluence Cloud/Server/DC (inserção no Confluence) Quem pode fazer isso:
    admin do Confluence'
---

A Miro e o Confluence trabalham juntos com a sincronização bidirecional para garantir que você obtenha o conteúdo mais atualizado de ambas as plataformas, onde quer que você trabalhe.

## Como a Miro funciona com o Confluence

Insira seus boards da Miro e documentos do Confluence, e acompanhe as alterações com a sincronização instantânea. Você pode definir níveis de acesso de inserção para que os usuários certos tenham acesso às informações certas o tempo todo.

Inserir documentos do Confluence em boards da Miro

Inserir boards da Miro em documentos do Confluence

## Inserir documentos do Confluence nos boards da Miro

Você pode inserir documentos do Confluence na Miro simplesmente colando um link no board da Miro. Observe que **a inserção de documentos do Confluence na Miro requer o Confluence Cloud.**

Ao colar um link do Confluence pela primeira vez em um board da Miro, ele aparecerá como um [link inteligente da Miro](https://help.miro.com/hc/articles/360017730993). Ao colar o link do Confluence pela primeira vez, será necessário clicar em **Conectar** para autorizar o acesso ao Confluence.

:::warning
Por motivos de segurança, não mostramos os detalhes de um link do Confluence em boards públicos da Miro, e os usuários só podem visualizar o título de um link do Confluence em boards privados. Os usuários só poderão ver o título da página quando autorizarem sua conta do Confluence, após o que poderão expandir e editar o documento do Confluence (dependendo das permissões de nível de acesso fornecidas).
:::

![Connect_Confluence.png](https://help.miro.com/hc/article_attachments/21019694152594)*Como conectar a página do Confluence na Miro*

Quando o Confluence for autorizado, os usuários que acessam o board agora poderão ver o título do documento, o ícone do provedor e a fonte do link. Os usuários também poderão expandir o link inteligente da Miro para o modo de tela inteira.

:::tip
Os títulos de links inteligentes da Miro são extraídos do URL. Se você editar o título do documento do Confluence, deverá colar o link novamente para ver o título atualizado no seu link inteligente da Miro.
:::

![Connected_Confluence_card.png](https://help.miro.com/hc/article_attachments/21019705246738)*Uma página do Confluence conectada como um link inteligente da Miro*

Quando os usuários clicam no ícone de expandir, será solicitado que autorizem sua própria conta do Confluence antes, para que possam visualizar e editar o documento na Miro.

![Expanded_Confluence_card.png](https://help.miro.com/hc/article_attachments/21019705229586)*O documento do Confluence expandido*

## Inserir boards da Miro nos Documentos do Confluence

Você pode incorporar boards do Miro em documentos do Confluence com o Plugin da Miro para Confluence, ou diretamente através dos Atlassian Smart Links. Isso pode ser feito com Confluence Cloud, Server ou DC.

### Passo 1: Configurar o Plugin da Miro

Primeiro, instale o [aplicativo da Miro para Confluence](https://marketplace.atlassian.com/apps/1217530/miro-for-confluence?tab=reviews&hosting=cloud) a partir do Marketplace da Atlassian.

**Como instalar o aplicativo da Miro para Confluence**

> **Quem pode fazer isso**: admin do Confluence

1. Faça login na sua instância do Confluence como admin
2. Clique no menu suspenso de admin e escolha **Complementos (aplicativos)**
3. Selecione **Encontrar novos aplicativos** ou **Encontrar novos complementos**
4. Pesquise por **Miro para Confluence**
5. Clique em **Obter app**

![Miro_for_Confluence.png](https://help.miro.com/hc/article_attachments/21019705233042)*O aplicativo da Miro para Confluence*

Você verá a seguinte mensagem quando o aplicativo for instalado com sucesso:

![success_message.jpg](https://help.miro.com/hc/article_attachments/21019694158610)
*O aplicativo foi instalado com sucesso*

### Passo 2: Inserir um board na página do Confluence

Há três maneiras de inserir um board da Miro em uma página do Confluence:

1. Digitando **/miro** diretamente no documento do Confluence.
   ![Typing_miro_on_the_doc.png](https://help.miro.com/hc/article_attachments/21019705236498)
   *Como digitar /miro na página do Confluence para inserir um board*
2. Pesquisando pela Miro a partir da barra de ferramentas do aplicativo. No documento do Confluence, clique em **Inserir** e selecione **Miro** da lista de aplicativos.
   ![Miro_plugin.jpg](https://help.miro.com/hc/article_attachments/21019705226770)
   *Selecionando Miro da lista de aplicativos para incorporar um board*
3. Colando um link da Miro diretamente no Confluence com os links inteligentes da Atlassian.

### Passo 3: selecione um board a partir do seletor de boards

O seletor do board será aberto. Selecione o board que deseja inserir no menu suspenso ou pesquise por um board. Os usuários só verão os boards disponíveis para eles na Miro e só poderão inserir boards se tiverem acesso de edição a eles.

![Board_picker.png](https://help.miro.com/hc/article_attachments/21019705240594)*Como escolher um board para inserir a partir do seletor do board*

Selecione a **Visualização inicial** para o board inserido.

![Set-the-starting-view-for-your-embed.png](https://help.miro.com/hc/article_attachments/21019705263890)*Como definir a visualização inicial para o board inserido da Miro*

Escolha o nível de acesso para **Todos os visitantes** da página do Confluence.

- **Podem visualizar:** permite que qualquer visitante da página do Confluence veja o board.
- **Requer acesso:** limita a visualização a quem tem acesso ao board na Miro.

![Access-level-for-embed.png](https://help.miro.com/hc/article_attachments/21019705260562)*Como definir o nível de acesso ao board da Miro na página do Confluence*

### Passo 4: Inserir o board

Depois de clicar em **Inserir board**, o board da Miro será inserido na página do Confluence como um iFrame. Os usuários podem visualizar e navegar pelo board.

:::note
Para os usuários do plano Enterprise, os níveis de acesso seguirão as configurações de acesso para toda a organização e, portanto, algumas permissões podem ser restritas. Saiba mais sobre o [gerenciamento de boards inseridos para o plano Enterprise](https://help.miro.com/hc/articles/4405088016274).
:::

![Miro-board-embedded-in-confluence.png](https://help.miro.com/hc/article_attachments/21029821397010)*Board da Miro inserido em uma página do Confluence*

Para abrir o board diretamente na Miro, clique no logotipo da Miro.

![Open-embedded-board-in-miro.png](https://help.miro.com/hc/article_attachments/21029820289426)
*A opção para abrir o board no Miro*

#### **Experiência do usuário no Confluence Cloud versus servidor do Confluence**

O menu do tamanho da janela para boards inseridos é diferente para o Confluence Cloud e o servidor do Confluence.

No Confluence Cloud, você verá o seguinte menu do tamanho da janela com a opção de **Ir para largura total**:

![Go-full-width-Miro-board-confluence.png](https://help.miro.com/hc/article_attachments/21029820290322)
*Menu do tamanho da janela no navegador do Confluence*

No servidor do Confluence, você verá um menu com a opção de selecionar um tamanho de janela pequeno, médio ou grande (**S/M/L**):

![Miro_in_Confluence_Server.jpg](https://help.miro.com/hc/article_attachments/21019694181010)*Menu do tamanho da janela no aplicativo do Confluence*

## Inserir boards da Miro por meio dos links inteligentes da Atlassian

Você também pode inserir boards da Miro no Confluence usando a funcionalidade de links inteligentes da Atlassian. A funcionalidade permite que você insira automaticamente um board sem a necessidade de instalar um aplicativo.

Vá para uma página do Confluence e basta colar um link do board ou digitar **/link** para inserir. Se você usar a funcionalidade pela primeira vez, será solicitado que conecte um time da Miro. Clique em **Conectar para pré-visualizar,** autorize na Miro e escolha um time a partir do qual irá inserir seus boards.

:::note
Somente os usuários que têm acesso ao board inserido na Miro poderão trabalhar com a pré-visualização do board inserido da Miro depois de conectar suas contas da Miro e da Atlassian. Se você quiser tornar a pré-visualização do board disponível para todos os usuários do Confluence, pode usar o aplicativo da Miro.
:::

![install_Atllassian_links.jpg](https://help.miro.com/hc/article_attachments/21019705256466)
*Escolhendo um time para inserir boards*

Ao colar um link do board da Miro em uma página do Confluence, ele se transforma automaticamente em um widget. Clique no link para ver as opções de exibição. Você pode escolher exibir o board da Miro como uma **URL**, texto **in-line**, um **card** ou uma **incorporação**.

![Confluence_widget.png](https://help.miro.com/hc/article_attachments/21019705242770)*Widget do board da Miro no Confluence*

Se você optar por exibir o board como uma inserção, pode alterar o tamanho da inserção arrastando os lados.

![changing_embed_size.gif](https://help.miro.com/hc/article_attachments/21019694183058)
*Como alterar o tamanho da inserção da Miro no Confluence*

:::warning
Se os cookies de terceiros forem bloqueados no seu navegador, pode haver problemas inesperados ao exibir boards incorporados.
:::

## Como desativar o aplicativo da Miro para o Confluence

Para desabilitar o aplicativo, vá para **Atlassian Marketplace** > **Gerenciar aplicativos** > **Miro para Confluence Cloud** > **Desinstalar.**

*![Uninstall_Confluence_plugin.jpg](https://help.miro.com/hc/article_attachments/21019694186386)*
*Aplicativo da Miro para Confluence na lista dos aplicativos instalados da Atlassian*

## Migração e impacto nos boards no Confluence

Seja migrando de uma instância On-premise para a Cloud, ou de Cloud para Cloud, o plugin da Miro não requer etapas de migração dedicadas. O Confluence exibe boards da Miro via iFrames, que são inserções baseadas em URL, significando que o Confluence armazena apenas o link do board, enquanto o board permanece na Miro.
