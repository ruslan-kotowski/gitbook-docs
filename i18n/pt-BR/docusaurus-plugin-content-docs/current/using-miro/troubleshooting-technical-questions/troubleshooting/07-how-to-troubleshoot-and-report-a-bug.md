---
title: Como solucionar problemas e relatar um bug
article_id: 360017731413
translation_id: 360017731413
locale: pt-br
sidebar_position: 7
created_at: '2019-02-11T10:14:28Z'
updated_at: '2025-11-25T16:03:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Se você estiver tendo problemas de desempenho ou não consegue usar a Miro, saiba como relatar o bug ao Suporte da Miro.

## Antes de relatar um bug

1. Consulte a [página de status da Miro](https://status.miro.com/) para ver se tem relatórios sobre a possível degradação do desempenho.
2. Verifique se o problema ocorre no modo de navegação [anônima](https://support.google.com/chrome/answer/95464) **(privado)** e em um **navegador diferente.**
3. [Desabilite as extensões do navegador](https://support.box.com/hc/articles/360044196613-How-To-Disable-Plugins-Add-Ons-Extensions-In-Multiple-Browsers). Às vezes, eles entram em conflito com processos da Miro (por exemplo, Grammarly com os widgets de texto).
4. Se você trabalha no aplicativo para desktop, [redefina os dados do aplicativo](../../../getting-started/apps-for-devices/05-desktop-app.md).
5. Se tiver problemas de desempenho em um board específico, tente [duplicá-lo](../../managing-boards/03-how-to-duplicate-a-board.md) e veja se o problema persiste no board copiado.
6. Confira nossos guias de solução de problemas:

- [Problemas de desempenho e carregamento do board.](../../tools/troubleshooting/04-board-performance-and-loading-issues.md)
- [Não consigo fazer login.](../../tools/troubleshooting/09-i-can't-log-in.md)
- [Não consigo acessar ou editar um board da Miro.](../../tools/troubleshooting/08-i-can't-access-or-edit-a-miro-board.md)
- [Problemas com a exportação de boards.](../../tools/troubleshooting/03-board-export-issues.md)
- [Perdi meu board ou conteúdo.](../../tools/troubleshooting/11-i-lost-my-board-or-content.md)
- Outros guias.

## Como enviar um bug

Forneça quanto mais detalhes possível. Isso nos ajudará a entender seu problema imediatamente, para que possamos ajudar você melhor.

1. Inclua uma descrição do problema e envie capturas de tela, GIFs ou um [vídeo curto](https://chrome.google.com/webstore/detail/openvid-screen-recorder-c/liecbddmkiiihnedobmlmillhodjkdmb). Além disso,

- Se o problema ocorrer em um board específico, [compartilhe esse board](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) com [support@help.miro.com](mailto:support@help.miro.com) e se possível, com as permissões de edição.
- Se o problema estiver relacionado a um arquivo específico que você tenha carregado, envie-nos o arquivo.

2. Especifique seu dispositivo, sistema operacional e versão do navegador.
3. Forneça os logs do console do seu navegador e da rede ou logs do aplicativo para desktop.

### Como gravar os logs do console

**Como gravar os logs do console do navegador**

1. Enquanto estiver no board da Miro, **clique na barra de endereço** do seu navegador (siga esta etapa se o problema ocorrer em um dos boards e não na página de configurações ou no painel).​![mceclip1.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264821010_mceclip1.png)
2. Pressione **F12** ou **fn + F12** para abrir as ferramentas de desenvolvedor do navegador.
3. Escolha a guia **Rede** e marque a caixa **Preservar logs.**
4. Recarregue a página.
5. Tente reproduzir o problema novamente.
6. Clique no ícone de seta Baixar para **exportar** os logs HAR da rede.
   ![network_console_logs.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264822418_network%20console%20logs.jpg)
7. Na guia do **Console**, clique com o botão direito do mouse nos registros e selecione **Salvar como**.​![save_console_logs.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253821970_save%20console%20logs.jpg)
8. Envie-nos os arquivos  .*log* e .*har*. Se o tamanho do arquivo não permitir que ele seja anexado ao seu ticket, carregue o arquivo em qualquer armazenamento em nuvem e envie-nos o link (permita que qualquer pessoa com o link baixe os arquivos).

**Como gravar logs do aplicativo para desktop no Mac**

Se encontrar um bug no aplicativo para desktop no Mac, envie-nos os registros de log.

1. Enquanto estiver no aplicativo para desktop, clique em **Ajuda** no canto superior esquerdo. Selecione **Abrir ferramentas de desenvolvimento para guias.**​​​​​​​​
   ![open_developer_tools_for_tabs.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253822866_open%20developer%20tools%20for%20tabs.jpg)
2. ​Alterne para a guia **Rede**.​​​​ Marque a caixa **Preservar logs.**
3. Abra o board em que deseja solucionar o problema (pule esta etapa se não conseguir acessar os boards).
4. Recarregue a página com o atalho **Ctrl + R.**
5. Reproduza o problema.
6. Clique no ícone de seta Baixar para exportar os logs HAR da rede:
   ![preserve_logs.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253823250_preserve%20logs.jpg)
7. Na guia do console, clique com o botão direito do mouse nos registros e selecione **Salvar como.**​![save_as_.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253825042_save%20as%20.jpg)
8. Clique novamente em **Ajuda** > selecione **Abrir ferramentas para desenvolvedores** e repita as etapas de 2 a 7. Isso permite coletar outro tipo de log que nos forneceria um conjunto diferente de dados para investigarmos o problema mais a fundo.
9. Envie-nos os arquivos .log e .har. Se o tamanho do arquivo não permitir que ele seja anexado ao seu ticket, carregue o arquivo em qualquer armazenamento em nuvem e envie-nos o link (permita que qualquer pessoa com o link baixe os arquivos).

**Como gravar logs do aplicativo para desktop no Windows**

Se você tiver um bug no aplicativo para desktop no Windows, envie-nos os registros de log.

1. Ao usar o aplicativo para desktop, pressione **Alt** > clique em **Ajuda** > **Abrir ferramentas de desenvolvimento para guias.![open_developer_tools_for_tabs_on_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264830994_open%20developer%20tools%20for%20tabs%20on%20Windows.jpg)**
2. ​Alterne para a guia **Rede**.​​​​ Marque a caixa **Preservar logs.**
3. Abra o board em que deseja solucionar o problema (pule esta etapa se não conseguir acessar os boards).
4. Pressione **Ctrl + R** para recarregar a página **Ctrl + R.**
5. Reproduza o problema.
6. Clique no ícone Baixar para exportar os logs HAR da rede.
   ![preserve_logs.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253823250_preserve%20logs.jpg)
7. Na guia do Console, clique com o botão direito do mouse nos registros e selecione **Salvar como.​**
   ![save_as_.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253825042_save%20as%20.jpg)
8. Abra novamente a **Ajuda** > selecione **Abrir ferramentas para desenvolvedores** e repita as etapas de 2 a 7. Isso permite coletar outro tipo de log que nos forneceria um conjunto diferente de dados para investigarmos o problema mais a fundo.
9. Envie-nos os arquivos .log e .har. Se o tamanho do arquivo não permitir que ele seja anexado ao seu ticket, carregue o arquivo em qualquer armazenamento em nuvem e envie-nos o link (permita que qualquer pessoa com o link baixe os arquivos).

### Como coletar um relatório do navegador

Ao relatar problemas de carregamento ou desempenho, o compartilhamento de informações da versão estendida do navegador ajuda o Suporte da Miro a diagnosticar o problema. Para encontrar essas informações, basta inserir um comando específico na **barra de endereço** do seu navegador. Confira abaixo como pode acessar essas informações em diferentes navegadores.

- **Chrome**: chrome://version
- **Microsoft Edge**: edge://version
- **Firefox**: about:support (ou about:version em algumas versões)
- **Opera**: opera://about
- **Navegador do Yandex**: browser://version

> **✏️** Consulte [Como entrar em contato com o Suporte da Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
