---
title: "Problemas com a exporta\xE7\xE3o de boards"
article_id: 360020567820
translation_id: 360020567820
locale: pt-br
sidebar_position: 3
created_at: '2021-03-18T12:15:46Z'
updated_at: '2025-11-05T13:45:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Você pode [exportar seu board da Miro](../../import-and-export/export/03-how-to-export-your-board.md) como imagem, PDF ou arquivo CSV. Se você encontrar problemas para exportar seu board da Miro, explore as soluções possíveis abaixo.

## Não consigo exportar o board

**O botão de exportação está faltando no meu board**

O botão de exportação está localizado no menu dos **três pontinhos** (**...**), em seguida no submenu **Board**.

Nenhuma opção de exportação no [menu do board](../../../getting-started/start-here/your-first-board/05-toolbars.md):

1. Verifique se o titular/cotitular do board permitiu a exportação do board para usuários nas configurações de conteúdo do board.

   Para descobrir o nome do titular do board, clique no nome do board no canto superior esquerdo para abrir o cartão de informações do board. Se você não tiver permissão para ver essas informações, pode verificar o nome do usuário que o convidou para o board no e-mail de convite.

   Entre em contato com o titular do board e peça para ele ativar a opção para você na **Janela Compartilhar** > **Configurações de compartilhamento** > **Permissões**. O titular/cotitular precisa selecionar qual categoria de usuários pode [copiar o conteúdo do board](../../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).
   ![.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044218642_.gif.png)
   *Configurando quem pode copiar o board*
2. Certifique-se de que seu navegador, plano e dispositivo oferecem suporte à exportação. Você pode verificar a disponibilidade abaixo. Se o seu navegador, plano ou dispositivo não oferecer suporte à opção de exportação, recomendamos mudar para outro navegador ou dispositivo ou [fazer um upgrade do seu time](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

   |  |  |  |  |  |  |
   | --- | --- | --- | --- | --- | --- |
   |  | Plano Free | | Planos Starter, Business, Enterprise, Education | | Exportar para CSV (todos os planos) |
   |  | Baixa resolução | Alta resolução sem marca d'água | Baixa  resolução | Alta resolução  sem marca d'água |
   | Google Chrome | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Safari | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Firefox | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Opera | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Edge < 79 | ✘ | ✘ | ✘ | ✔ | ✘ |
   | [Aplicativo para desktop](../../../getting-started/apps-for-devices/05-desktop-app.md) | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Tablet | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Celular | ✘ | ✘ | ✘ | ✘ | ✘ |

**Para exportações de baixa qualidade**

Para solucionar problemas, feche as guias do navegador e as guias em segundo plano. Você também pode tentar trocar de navegador.

Para exportações de alta qualidade, faça o seguinte:

- Oculte quadros que você não deseja exportar. O conteúdo em quadros ocultos não é exportado.
- Divida o board em boards menores para exportação.

**Dicas gerais**

- Coloque tudo o que deseja exportar em quadros, pois apenas widgets dentro de quadros são exportados.
- Evite PDF dentro de PDF. Se você tiver um PDF em um board que gostaria de exportar como PDF, substitua o PDF no board por imagens de baixa qualidade.
- Converta imagens de alta resolução para JPEG ou reduza-as com uma ferramenta externa.
- Verifique a página de Status da Miro para incidentes relevantes.
- Divida o board em quadros e exporte os quadros separadamente. PDFs separados podem ser reunidos posteriormente usando uma ferramenta externa.
- Divida boards grandes em boards menores e use [Espaços](../../spaces/01-spaces.md) para ajudar a se organizar e agrupar boards relacionados.

**"Infelizmente, algo deu errado ao gerar o documento PDF"**

Tente dividir o board em quadros e exportar os quadros separadamente, pois o problema pode ser causado pelo tamanho do board.

Se isso não ajudar, verifique [os logs do console do seu navegador](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md). Se os logs contiverem a seguinte mensagem:

```
ERR_CONNECTION_ABORTED
```

*onde:*

A exportação está bloqueada pelo software de segurança no seu dispositivo ou por um firewall na sua rede.

Você ou o admin do sistema precisam configurar as definições do antivírus e/ou do firewall para permitir que a Miro realize o procedimento de exportação.

Em caso de dúvidas, [contate o Suporte Miro](../../tools/troubleshooting/06-contacting-miro-support.md).

**Nada acontece quando tento exportar um board para PDF, e a Miro não mostra erro**

Esse problema conhecido ocorre principalmente no navegador Safari, quando as janelas pop-up estão desativadas. Para resolver o problema no Safari, [siga estas etapas](https://support.apple.com/en-gb/guide/safari/sfri40696/mac). Certifique-se de que você habilitou as janelas pop-up para miro.com, ou para todos os sites. Retorne à Miro e tente exportar seu board novamente.

Para o Chrome, [siga estas etapas](https://support.google.com/chrome/answer/95472?hl=en&co=GENIE.Platform%3DDesktop).

## Tenho problemas com arquivos exportados (PDFs, imagens, CSVs)

**Imagens/PDFs estão desfocados no documento exportado**

Se imagens ou PDFs carregados estiverem desfocados no seu arquivo salvo:

1. Ajuste o zoom do board para 100% e deixe as imagens/PDFs serem renderizados antes de exportar o board
2. A imagem/PDF carregado pode ser muito complexo ou grande para exportar. Para reduzir o tamanho do arquivo, converta a imagem/PDF para o formato PNG e substitua-o no board. Em seguida, exporte o board novamente

O plano Free oferece exportação somente em baixa qualidade. Se precisar exportar seu board em alta qualidade, recomendamos [movê-lo para um time pago](../../managing-boards/04-how-to-move-a-board.md) ou [atualizar seu time](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

**A ordem das páginas não é a mesma que a ordem dos quadros no board**

A ordem dos quadros exportados em PDF é a mesma do painel de quadros. Para mudar a ordem dos quadros:

1. Abra a visão geral do board no canto inferior esquerdo
2. Arraste os quadros para mudar suas posições na lista. Você também pode usar o [Magic organize](../../essential-tools/07-frames.md) para organizar rapidamente seus quadros na ordem em que estão colocados no board
   ![move_frames.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057584914_move%20frames.gif)
   *Mudando a ordem dos quadros*

**O arquivo exportado está cortado**

Se você **exportar seu board como imagem**, certifique-se de incluir todo o conteúdo que deseja exportar na área selecionada para exportação.

![save_as_image.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057583890_save%20as%20image.gif)
*Exportando um board como imagem*

Se você **exportar seu board como PDF**, certifique-se de criar um quadro que inclua todo o conteúdo que você gostaria de exportar. Em seguida, [exporte o quadro](../../import-and-export/export/03-how-to-export-your-board.md).

**O arquivo PDF exportado não contém nomes dos quadros**

Quando você exporta seu board como um arquivo PDF, os títulos dos quadros não são incluídos na exportação. Você pode substituir os títulos dos quadros usando a [ferramenta de texto](../../essential-tools/16-text.md) e colocar o texto nos quadros. Os títulos aparecerão no seu PDF.

**Os dados em um arquivo CSV exportado não estão estruturados**

Por enquanto, a exportação para CSV não mantém a estrutura ou as relações do board. No entanto, se você exportar [tabelas](../../advanced-tools/05-grid.md) como um arquivo CSV, a estrutura será salva.

Se você precisar exportar um [mapa mental](../../advanced-tools/03-mind-map.md) como um arquivo com dados inteligentes, use o [Mindmap downloader](https://miro.com/marketplace/mindmapdownloader/?backUrl=%2Fmarketplace%2F).

**As fontes no board diferem das fontes no arquivo exportado**

A exportação do Miro utiliza as fontes instaladas no sistema operacional do seu dispositivo. Se a fonte não estiver presente no seu sistema operacional, uma fonte semelhante do seu sistema será usada. Se você precisar da mesma fonte do seu board do Miro, escolha uma fonte diferente no board ou instale a fonte necessária no seu dispositivo.

## Não consigo localizar o arquivo exportado

**Não consigo encontrar o arquivo exportado no meu dispositivo**

**Se você usa a Miro em um navegador**

Os arquivos serão armazenados na pasta onde os downloads do navegador são salvos por padrão. Você pode verificar as opções de download nas configurações do navegador.

**Se você usa o aplicativo para desktop ou de tablet da Miro**

Verifique a pasta Downloads no seu dispositivo. Você também pode buscar seus arquivos usando o nome do board.

**A Miro cria uma nova pasta toda vez que exporto um board**

> **Relevante para**: [aplicativo para desktop Windows](../../../getting-started/apps-for-devices/05-desktop-app.md)

Pode ser que o caminho tenha sido salvo nas configurações do aplicativo da Miro. Para apagar o caminho:

1. Exclua o aplicativo para desktop da Miro
2. No canto inferior esquerdo do Windows (barra de pesquisa), digite **%AppData%** e abra a pasta **Local,** em seguida, exclua a pasta **RealTimeBoard**
3. Abra **%AppData%** novamente, navegue até a pasta **Roaming,** e exclua a pasta **RealTimeBoard**

Reinstale o último [aplicativo Miro](https://miro.com/apps/).

Se nenhuma das soluções ajudar, [entre em contato com o Suporte da Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
