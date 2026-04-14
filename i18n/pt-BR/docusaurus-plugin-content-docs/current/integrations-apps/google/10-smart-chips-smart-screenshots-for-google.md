---
title: Smart chips e smart screenshots para Google
article_id: 11845494577554
translation_id: 11845494577554
locale: pt-br
sidebar_position: 11
created_at: '2023-06-06T12:19:20Z'
updated_at: '2025-08-15T13:44:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-workspace-smart-chips
availability:
  notes: 'Pessoas: Todos os usuários Planos: Todos os planos Plataformas: Desktop,
    navegador (ao usar Documentos Google, Apresentações, Planilhas)'
---

O Google oferece poderosas capacidades de colaboração com seu smart canvas, que utiliza estruturas modulares interativas chamadas smart chips. Com o smart chip da Miro para Google, você pode adicionar um atalho para um board da Miro diretamente em seu Google Doc, Google Slides ou Google Sheets, ampliando suas capacidades de colaboração.

Além disso, a Miro oferece Smart Screenshots, permitindo que você cole boards e widgets da Miro diretamente como imagens no Google Doc, Google Slides e Google Sheets, com funcionalidades aprimoradas para manter o conteúdo sincronizado.

![Miro smart chip board preview in Google Docs](../../../../../../docs/integrations-apps/google/images/21017516136210_miro_smart_chip_board_preview.png)
*O complemento smart chip da Miro nos Documentos Google*

## Configurar smart chips da Miro

Siga estas etapas para integrar links de boards da Miro como smart chips no seu Google Doc, Google Slides ou Google Sheets.

:::note
O admin do seu Google Workspace pode precisar instalar o complemento da Miro para sua organização ou time no Google Workspace. Verifique com seu admin se não estiver disponível. [Saiba mais](https://support.google.com/a/topic/1056395?hl=en&ref_topic=27380).
:::

1. Dentro do seu documento do Google, cole um link para o seu board da Miro e pressione **Tab**. O Google verificará se o link é um link de chip.
2. A partir daqui, o Google verificará se você já tem o complemento do Google Workspace da Miro instalado. Então, uma de duas ações ocorrerá:
   1. Se você já tiver o complemento do Google Workspace instalado, não há necessidade de instalar smart chips — você já os tem. Você verá uma pré-visualização do seu board quando clicar no link.
   2. Se você não instalou o complemento, será solicitado a instalá-lo a partir do Google Workspace Marketplace.

      > ✏️ Você pode precisar do seu admin do Google para instalar o complemento para você.
3. Em seguida, o Google pedirá para você conectar-se à sua conta da Miro. Isso é necessário para exibir certas informações do board e determinar se você tem acesso ao board para o qual está criando o link. Clique em **Conectar à Miro**.

   ![Connect Miro to Google Workspaces dialog](../../../../../../docs/integrations-apps/google/images/21017529158034_Google%20Smart%20Chips%20connect.png)
*Conectando a Miro ao Google Workspaces*
4. A partir daqui, uma de duas ações ocorrerá:
   1. Se você já está autorizado a acessar este board, verá o chip com uma pré-visualização do board e metadados como o titular do board e a data da última modificação.
   2. Se precisar ser autorizado, verá um botão **Solicitar Acesso**. Clique nele e sua solicitação será enviada ao titular do board.

      ![Miro smart chip request access to board button](../../../../../../docs/integrations-apps/google/images/21017529156882_miro_smart_chip_request_access_to_board.png)*Solicitando acesso a um board privado*
5. Assim que seu acesso for aprovado, você verá o chip com uma pré-visualização do board. Se você não vir a pré-visualização, atualize seu documento.
6. Seu board agora está adicionado ao documento, e ao clicar nele você será levado para o board da Miro. Qualquer pessoa com acesso ao board pode criar um smart chip em seu documento do Google.

   ![Connected Miro smart chip board link in Google Docs](../../../../../../docs/integrations-apps/google/images/21017516138642_Connecting%20Google%20Smart%20Chip.gif)
*Conectando um link de board de smart chip da Miro aos espaços de trabalho do Google*

## Usar capturas de tela inteligentes da Miro

A integração do painel lateral da Miro permite incorporar conteúdo de board da Miro diretamente nos Documentos, Slides ou Planilhas do Google sem sair do seu documento. Essa funcionalidade oferece acesso contínuo aos seus boards da Miro e permite inserir conteúdo visual com funcionalidade aprimorada.

### Painel lateral da Miro

O painel lateral da Miro no Documentos, Slides ou Sheets inclui as seguintes capacidades:

- **Acesso direto ao board:** Acesse seus boards Miro diretamente do Documentos, Slides ou Sheets sem trocar de aplicativos.
- **Seleção de board:** Escolha entre seus boards Miro disponíveis usando o botão "Selecionar board Miro para incorporar".
- **Pré-visualização interativa:** Visualize e selecione conteúdo específico do seu board da Miro antes de inserir.
- **Posicionamento preciso:** Insira o conteúdo exatamente onde o cursor está posicionado no documento.
- **Funcionalidade inteligente:** O conteúdo incorporado mantém a conexão com o board original da Miro.

### Como usar o painel lateral da Miro

1. No seu Documentos, Slides ou Sheets do Google, posicione o cursor no documento onde deseja inserir o conteúdo da Miro.
2. Abra o painel do lado direito clicando no ícone de integração da Miro.
   ![Screenshot 2025-07-11 at 11.05.03.png](../../../../../../docs/integrations-apps/google/images/28006926984466_Screenshot%202025-07-11%20at%2011.05.03.png)
3. Clique em **Selecionar board da Miro para incorporar** para escolher entre os seus boards disponíveis.
   ![Screenshot 2025-07-11 at 11.09.05.png](../../../../../../docs/integrations-apps/google/images/28006941150482_Screenshot%202025-07-11%20at%2011.09.05.png)
4. Navegue e selecione a área específica, quadro ou conteúdo que deseja incorporar do preview do board.
   ![Screenshot 2025-07-11 at 11.10.17.png](../../../../../../docs/integrations-apps/google/images/28006926986130_Screenshot%202025-07-11%20at%2011.10.17.png)
5. Use qualquer opção disponível no menu suspenso para escolher diferentes configurações de visualização ou seleções.
6. Clique em **Confirmar** para inserir o conteúdo na posição do seu cursor.

O conteúdo incorporado aparecerá como uma captura de tela no seu documento com uma conexão de smart chip ao board original da Miro.

:::note
**Nota:** O painel lateral da Miro requer que o complemento da Miro para Google Workspace esteja instalado. A funcionalidade funciona tanto com Documentos Google, Slides Google, quanto com Planilhas Google.
:::

## Gerencie o complemento como admin

Revise estes pontos se você for um admin do Google Workspace gerenciando o complemento da Miro:

1. O complemento do Google Workspace pode ser instalado ou removido apenas no lado do Google.
2. Se você quiser restringir o acesso aos smart chips do Google, isso deve ser feito no lado do Google; a Miro não tem controle sobre quais usuários instalam e usam os smart chips.

## Perguntas frequentes

Respostas para as dúvidas mais frequentes sobre os smart chips da Miro para o Google.

Qual é a diferença entre os Smart Chips e o painel lateral da Miro?

Os Smart Chips criam links clicáveis para boards da Miro dentro dos seus documentos Google, enquanto o painel lateral da Miro permite incorporar conteúdo visual dos seus boards da Miro diretamente nos Documentos e Slides do Google. O painel lateral fornece uma maneira integrada de selecionar e inserir conteúdo específico do board sem sair do seu documento.

Quais aplicações do Google Workspace têm integração com a Miro?

Os Smart Chips funcionam com o Google Documentos, e o painel lateral da Miro funciona tanto com o Google Documentos quanto com o Google Slides. O suporte para Google Sheets é determinado pelo Google - por favor, consulte a Central de ajuda para atualizações.

Com que tipo de links os smart chips funcionam?

O smart chip da Miro para o Google suporta links para boards da Miro e objetos de board.

Como os elementos de board da Miro incorporados são mantidos atualizados?

O conteúdo incorporado através do painel lateral da Miro mantém uma conexão com o board original da Miro. Embora não sincronize automaticamente, você pode atualizar o conteúdo incorporado para garantir que ele reflita a versão mais recente do seu board da Miro.

Como funciona o painel lateral do Google Documentos?

O painel lateral do Google Documentos oferece acesso direto aos seus boards da Miro sem sair do seu documento. Clique no ícone de integração da Miro para abrir o painel do lado direito e, em seguida, use "Selecionar board da Miro para incorporar" para escolher entre os boards disponíveis. O painel permite que você visualize e selecione áreas ou quadros específicos antes de inseri-los em seu documento na posição do cursor.
