---
title: Plugin Miro para Sketch
article_id: 360017731173
translation_id: 360017731173
locale: pt-br
sidebar_position: 13
created_at: '2019-02-11T10:13:46Z'
updated_at: '2025-02-26T12:15:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

O plugin Miro para Sketch permite uma maneira fácil e rápida de obter imagens do Sketch diretamente para o board. Envie suas pranchetas para o Miro e atualize-as facilmente com um clique. Sincronize todas as suas imagens sempre que fizer uma alteração sem precisar carregá-las novamente.

### Habilitando o plugin

1. Baixe o plugin Sketch do GitHub: siga [este link](https://github.com/miroapp/sketch_plugin) > **Código** > **Baixar ZIP**:

![Baixar_do_Github.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017592683026_Download%20from%20Github.jpg)

2. Extraia o conteúdo do arquivo zip > clique duas vezes no pacote RealtimeBoard.sketchplugin para instalar o plugin.

![plugin_instalado.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017605731986_plugin%20installed.jpg)
*O plugin Miro para Sketch está instalado*

3. Para ativá-lo, abra o Sketch, vá em **Plugins >** **Gerenciar plugins** e marque a caixa **Miro by Miro**.

![Miro_plugin_em_Sketch.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017605733522_Miro%20plugin%20in%20Sketch.jpg)
*O plugin Miro está ativado no Sketch*

4. Depois disso, você precisa se autenticar com suas credenciais do Miro . Para fazer isso, clique em **Plugins -** **Miro:** **Entre no Miro e saia do Miro**.

![Faça login no Miro no Sketch.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017592678546_Log%20in%20to%20Miro%20in%20Sketch.jpg)
*Entrar no Miro*

5. Digite seu e-mail e senha ou clique em **Usar credenciais da empresa** se você efetuar login via SSO.

![Miro_login.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017605735314_Miro%20login.jpg)
*A janela de autenticação para entrar no Miro*

### Adicionando pranchetas de esboço ao Miro

Para adicionar uma prancheta Sketch ao Miro, vá para **Plugins:** **Miro -** **Sincronize todas as pranchetas com o Miro**.

A janela de diálogo lhe dará a opção de escolher entre boards nos quais você tem uma função de editor por meio de convite por e-mail ou acesso [ao projeto](../../using-miro/sharing-boards/16-projects.md)/ time .

> *⚠️ Observe que os boards nos quais você tem função [de visitante](../../using-miro/sharing-boards/08-collaboration-with-visitors.md) não estarão disponíveis.*

Selecione um board a) clicando em uma das sugestões no menu suspenso ou b) digitando o nome do board. Depois disso, clique para adicionar **todas** **as pranchetas ou as selecionadas**. Marque a caixa se quiser **abrir o Miro após a sincronização**:

![selecione_um_quadro.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017592680338_select%20a%20board.jpg)
*Selecionando uma board para sincronização*

Clique em **Sincronizar**e as pranchetas aparecerão no seu board.

![artiboards_em_Miro.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017605731474_artiboards%20in%20Miro.jpg)
*Observe que você pode enviar pranchetas apenas para **boards existentes** no Miro*

:::warning
Observe que copiar e colar pranchetas diretamente está disponível apenas na versão *do navegador* Miro .
:::

### Sincronizando pranchetas do Sketch com o Miro

Para sincronizar as pranchetas que já foram adicionadas ao Miro e depois alteradas no Sketch, vá em **Plugins -****Miro:** **Sincronize todas as pranchetas com o Miro**. O board com o qual você sincronizou as pranchetas anteriormente será selecionado automaticamente na janela de diálogo. Basta escolher se deseja sincronizar **todas**ou apenas **as pranchetas selecionadas**. Marque a caixa se quiser **abrir o Miro após a sincronização**:

![sincronizando_boards.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017605737362_syncing%20boards.jpg)
*Sincronizando pranchetas com o Miro*

### Desabilitar o plugin

Para parar de sincronizar o Sketch e o Miro, vá para **Plugins >** **Gerenciar plugins** e desmarque a caixa **Miro por Miro**.

![desabilitar_Miro_sync.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017605738898_disable%20Miro%20sync.jpg)
*O plugin Miro está desabilitado no Sketch*

### Possíveis problemas e como resolvê-los

|  |  |  |
| --- | --- | --- |
| **Mensagem de erro / problema** | **Possíveis causas** | **Solução:** |
| 1. Ocorreu um erro. Ocorreu um erro durante a sincronização. Por favor, tente novamente" | 1. Você está usando uma versão desatualizada do Sketch.  2. Sua prancheta do Sketch é enorme (há uma imagem muito grande na prancheta do Sketch). | 1. Atualize para a versão mais recente do plugin Sketch.  2. Verifique o tamanho da imagem e diminua-o se necessário. |
| 2. Erro de conexão Algo deu errado | 1. O plugin não consegue se conectar à API do Miro .  2. A taxa é limitada pela API do Miro .  3. Há outros possíveis problemas com a rede. | Saia e entre no seu perfil da Miro no Sketch e tente sincronizar a prancheta novamente. |
| 3. "Ocorreu um erro durante a sincronização. Por favor, tente novamente" | O problema pode ser causado por alterações nas configurações de rede. | Registre logs do console e [envie um relatório de bug para a time de Suporte do Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md). |
| 4. O plugin Sketch congela e funciona inesperadamente ao tentar sincronizar várias pranchetas com o Miro | Isso acontece quando você tem uma board da Miro enorme e tenta sincronizar várias pranchetas por meio do plugin Sketch. | Crie uma nova board da Miro no Miro e sincronize uma única prancheta de cada vez com ela. |
| 5. Os boards não estão aparecendo nos resultados da pesquisa no Sketch | Isso acontece quando um board é movido para outro [projeto](../../using-miro/sharing-boards/16-projects.md) no Miro ou se você não tem um licença no projeto onde o board está localizado | 1. Verifique se uma board que não aparece na lista de sincronização no Sketch foi movida para outro projeto no Miro.  2. Verifique se você tem um licença em um projeto onde há um board . |
| 6. O Sketch não substitui as pranchetas existentes em uma board da Miro - elas são duplicadas na canvas em vez de substituídas | Isso acontece quando uma board sincronizada com o Sketch foi [movida](../../using-miro/managing-boards/04-how-to-move-a-board.md) [para outra time Miro](../../using-miro/managing-boards/04-how-to-move-a-board.md). Neste caso, as imagens serão duplicadas na primeira sincronização. Mais adiante, eles serão substituídos. | Exclua as pranchetas anteriores da board da Miro. As duplicatas serão substituídas posteriormente. |

#### Como registrar logs de esboço para o Suporte Miro

1. [Abrir pesquisa Spotlight](https://www.howtogeek.com/356942/how-to-view-the-system-log-on-a-mac/) (clique no ícone da lupa no canto superior direito da tela) > **Consola**:

![spotlight_search.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017605742098_spotlight%20search.jpg)
*Pesquisa em destaque*

2. Digite**sketch-rtb-error** no campo de pesquisa do console e pesquise por mensagem / qualquer:

![pesquisar_no_Sketch.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017605743762_search%20in%20Sketch.jpg)
*Pesquisa de console*

3. Clique na linha com a mensagem na seção inferior do console, faça uma captura de tela e compartilhe conosco.

![mensagem_de_erro.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017592686610_error%20message.jpg)
*Mensagem de erro do console*
