---
title: Miro para Jira Cloud
article_id: 360017572414
translation_id: 13809042658706
locale: pt-br
sidebar_position: 4
created_at: '2023-09-18T15:21:53Z'
updated_at: '2024-09-06T15:42:54Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Visualize qualquer coisa junto com o seu time — trabalhe no backlog do produto com notas adesivas digitais, crie diagramas de fluxo, diagramas e wireframes. Anexe boards aos itens do Jira e colabore com seu time em tempo real, como em uma reunião de lousa.

> **Disponível em:** planos Starter, Business e Enterprise
> Somente Jira Cloud

:::note
Você também pode inserir boards da Miro com a funcionalidade de link inteligente da Atlassian.
:::

:::note
Observe que a Miro tem dois tipos de integrações com o Jira: **Miro para Jira Cloud** (que permite incorporar boards da Miro no Jira) e **cartões do Jira**. Para saber mais sobre os cartões do Jira, leia [este artigo](https://help.miro.com/hc/articles/360017572434).
:::

## Como instalar

O processo de instalação é padrão para todas as extensões do Jira. Primeiro, faça login no seu Jira com direitos de admin e, em seguida, baixe o complemento [aqui](https://marketplace.atlassian.com/apps/1215456/miro-for-jira-cloud?tab=overview&hosting=cloud) (o aplicativo também pode ser encontrado no **Atlassian Marketplace** > **Encontrar novos aplicativos** > **Miro para Jira Cloud**): clique em **Obter aplicativo**e **compre agora**.
E isso é tudo! A instalação foi concluída.

![Miro_for_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134089234_Miro%20for%20Jira.jpg)
*Notificação do Jira sobre o sucesso da instalação*

Observe que como admin você não precisa mapear os usuários da Miro para os usuários do Jira durante a configuração. Cada usuário terá que se autorizar na Miro no Jira.

## Como usar a extensão

### Como anexar boards aos itens do Jira

Para anexar um board a um item do Jira, abra o item no Jira. Clique em **Adicionar board** na seção de **boards da Miro** .
![add_Miro_boards_in_Jira.jpg](https://help.miro.com/hc/article_attachments/21016134154642)
*O botão de complemento aparece após a instalação*

:::tip
Se não tiver a seção boards da Miro, você pode encontrá-la no menu de contexto do item.
:::

![Miro_boards_section.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134091026_Miro%20boards%20section.jpg)
*Como adicionar a seção boards da Miro a um item do Jira*

Você verá um seletor com boards da Miro. Escolha o board que você deseja adicionar (fique à vontade para alternar entre seus times no seletor). Se você não tiver as autorizações necessárias na Miro, deve fazer login primeiro.

Defina as configurações de compartilhamento do board no menu suspenso. Você pode disponibilizar o board para visualização e comentários para que os usuários que não têm um perfil na Miro também possam acessá-lo.

:::note
Para usuários do [plano Enterprise](https://help.miro.com/hc/articles/360017571534) da Miro, suas configurações de acesso seguirão os controles de acesso definidos para toda a organização, o que pode implicar que algumas opções de compartilhamento sejam restritas. Para mais informações, leia o artigo [Como permitir ou restringir a inserção de boards da Miro em aplicativos compatíveis](https://help.miro.com/hc/articles/4405088016274).
:::

![embed_a_board_in_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134091922_embed%20a%20board%20in%20Jira.jpg)
*Como compartilhar as configurações ao anexar um board a um item do Jira*

Observe que você só pode inserir boards nos quais você tem acesso de editor.

Seu board agora está anexado ao item do Jira escolhido:

![Miro_board_in_Jira.jpg](https://help.miro.com/hc/article_attachments/21016134157842)
*Board da Miro anexado a um item do Jira*

### Como criar novos boards a partir do Jira

Para criar um novo board diretamente a partir de um item do Jira, clique em **Adicionar board** e crie um **novo board** a partir do seletor.

![create_a_new_board_from_the_picker.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016120706322_create%20a%20new%20board%20from%20the%20picker.jpg)
*Como criar um board a partir do seletor*

### Como visualizar, comentar e editar boards

Basta clicar em um board anexado para visualizar/comentar/editar, dependendo dos direitos de acesso definidos. A janela do board será aberta como uma sobreposição, permitindo que você trabalhe e colabore como se estivesse na Miro.

![Miro_embed_in_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016120699410_Miro%20embed%20in%20Jira.jpg)
*A sobreposição do board no Jira*

 Você também pode clicar no botão da fonte para abrir o board na Miro em uma nova guia para sua conveniência.

![source_button.jpg](https://help.miro.com/hc/article_attachments/21016134162066)
*O botão para ir para o aplicativo da Miro*

### Como desanexar boards

Para desanexar um board, basta clicar no ícone da cruz e o anexo será instantaneamente removido do item (no lado da Miro, o board não será afetado).

![remove_an_attached_board.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134095634_remove%20an%20attached%20board.jpg)
*A opção de remover o board anexado*

## Como desabilitar a extensão

Para desabilitar a integração, abra a **Atlassian Marketplace** > **Gerenciar aplicativos** > abra a página da extensão e clique em **Desinstalar**:

![uninstall_Jira_add-on.jpg](https://help.miro.com/hc/article_attachments/21016134163474)
*A opção de **desinstalar** seção de extensões do Jira*

## Link inteligente da Atlassian para a Miro

Você pode inserir boards da Miro nos itens do Jira usando a funcionalidade do link inteligente da Atlassian. A funcionalidade permite que você insira automaticamente um board sem a necessidade de instalar um plugin.

:::note
Observe que apenas os usuários que têm acesso ao board inserido no lado da Miro poderão trabalhar com a pré-visualização após conectar suas contas da Miro e da Atlassian. Se você quiser tornar a pré-visualização disponível para todos os usuários do Jira, fique à vontade para usar a extensão do Jira.
:::

para um item do Jira e basta colar um link do board ou digite /link para inserir. você usar a funcionalidade pela primeira vez, será solicitado que conecte seu time da Miro. Clique em **Conectar para pré-visualizar,** autorize na Miro e escolha um time a partir do qual irá inserir seus boards.

![install_Atllassian_links.jpg](https://help.miro.com/hc/article_attachments/21016120792978)
*Como escolher um time para inserir boards*

Quando você cola o link de um board da Miro em um item do Jira, ele se transforma em um widget do Jira automaticamente. Clique no link e você verá as opções para exibir o link como um cartão ou como uma inserção.

![display_as_link.gif](https://help.miro.com/hc/article_attachments/21016120793874)
*As opções para exibir um link do board da Miro como um link, cartão ou inserção*

Se você optar por exibir o board como uma inserção, pode alterar o tamanho da inserção arrastando seu lado.

![changing_embed_size_in_Jira.gif](../../../../../../docs/integrations-apps/atlassian/images/21016120700306_changing%20embed%20size%20in%20Jira.gif)
*Como alterar o tamanho da inserção da Miro no Jira*

:::warning
Se os cookies de terceiros forem bloqueados no seu navegador, pode haver problemas inesperados exibindo boards incorporados.
:::

## Perguntas frequentes

Posso ocultar a seção boards da Miro nos itens do Jira?

Sim, clique nos três pontos no canto superior direito da seção e escolha **Ocultar boards da Miro**.
![hide_Miro_boards.jpg](https://help.miro.com/hc/article_attachments/21016134167314)
*Como ocultar boards da Miro no Jira*

A extensão funciona nos projetos da próxima geração do Jira?

Sim, você pode anexar seus boards a esses projetos.

Há um preço adicional para a extensão do Jira?

A Miro para Jira Cloud está disponível para todos os planos pagos sem custo adicional (planos Starter, Business e Enterprise).

Vamos migrar o Jira de uma instância da nuvem para outra. Os boards da Miro incorporados nos itens do Jira serão afetados?

Não deve haver nenhum problema com os boards inseridos da Miro se o conteúdo for movido sem alterações.
