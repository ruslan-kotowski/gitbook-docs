---
title: Problemas de desempenho e carregamento do board.
article_id: 360013588560
translation_id: 360013588560
locale: pt-br
sidebar_position: 4
created_at: '2020-05-06T08:17:24Z'
updated_at: '2025-04-01T16:57:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Aprenda dicas para melhorar o desempenho do board durante as sessões colaborativas e em boards grandes, e para solucionar problemas como desempenho e navegação lentos, congelamento de boards e carregamento interminável.

## Como melhorar o desempenho do board

O desempenho do board pode ficar mais lento durante as **sessões colaborativas** com muitos usuários, bem como em **boards grandes** que contêm muito conteúdo.

Dicas para sessões colaborativas Dicas para boards grandes

O crescente número de usuários em um board e sua atividade intensa podem influenciar o desempenho do board.  Os usuários com dispositivos mais antigos e menos potentes correm um risco maior de sofrer perda de desempenho./span>

**Se você estiver participando de uma sessão colaborativa, certifique-se de:**

- feche ou minimize todas as guias e janelas redundantes, se estiver trabalhando em um [navegador](../technical-guidelines/02-supported-browsers-browser-restrictions.md) de desktop
- ocultar os cursores dos colaboradores e fechar todas as barras laterais
- Evitar selecionar e alterar vários objetos do board ao mesmo tempo.
- Minimizar a navegação em todo o board.
- Se você acessar a Miro em um notebook, certifique-se de que esteja no modo de alto desempenho, em vez de um modo de economia de energia.

**Se você estiver planejando uma sessão colaborativa na Miro:**

- Convide usuários que não precisam de acesso de edição como visualizadores.  Saiba como configurar os [direitos de acesso ao board](../../sharing-boards/01-board-access-rights.md).
- Certifique-se de manter o conteúdo do board arrumado. Para orientações, leia **Dicas para boards grandes,** encontradas na segunda guia acima.

O número máximo de objetos que você pode adicionar a um board é 100.000.  No entanto, o desempenho pode ser afetado a partir de 1.000 objetos. Para uma melhor experiência, recomendamos manter o número de objetos no board abaixo de 5.000.
Para encontrar o número de objetos no seu board:

- Selecione todos os objetos no board (ctrl-A no Windows, cmd-A no Mac ou arraste uma caixa de seleção em torno de todos os seus objetos).
- O menu de contexto aparecerá, indicando o número total de objetos.
- Clique em **Filtrar** para ver o número de objetos por tipo.

![número-de-objetos.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/25736281544466_number-of-objects.gif)
*Como saber o número de objetos em um board*

Além do número de objetos, objetos mais pesados ​​ou complexos (especialmente arquivos e documentos enviados) também podem deixar seu board mais lento.

Para acelerar um board grande, mantenha-o organizado:

- Exclua o conteúdo desnecessário, principalmente os arquivos e documentos carregados pesados (por exemplo, PDFs vetoriais com muitos detalhes ou imagens de alta resolução).
- Converta PDFs e imagens pesadas em alta resolução para arquivos PNG/JPG e recarregue-os no board.
- Reduza a escala do conteúdo do seu board se ele parecer muito grande com o nível de zoom de 100%:
  - Vá para o mapa no canto inferior direito e defina o zoom para 100%.
  - Se, neste nível de zoom, seu conteúdo parecer muito grande, selecione-o usando **Ctrl + A** (para Windows) ou **Cmd + A** (para Mac) e diminua-o.
  - Considere também reduzir a escala de quaisquer imagens grandes
    **![redimensionar-objetos-do-quadro.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/25736308553874_resize-board-objects.gif)**
    *Como reduzir a escala de conteúdo*
- [Resolva os comentários.](../../facilitation-tools/asynchronous-tools/01-comments.md)
- Converta a escrita com [caneta](../../essential-tools/10-pen.md) em imagens:
  - Faça uma captura de tela de um desenho.
  - Carregue-o para o board.
  - Exclua o desenho.
- Se possível, divida o board em vários boards:
  - Copie uma parte do conteúdo do board selecionando-o e pressionando **Ctrl + C** (para Windows) ou **Cmd + C** (para Mac).
  - [Crie um novo board](../../../getting-started/start-here/your-first-board/01-create-a-miro-board.md) e cole o conteúdo no board.
  - Exclua o conteúdo copiado do board original.

## Como solucionar problemas de desempenho ruim ou carregamento interminável

Seu dispositivo, conexão com a internet, navegador e outros fatores podem influenciar o desempenho do board e a velocidade de carregamento.  Se você tiver um desempenho ruim ou seu board, ou painel, não carregar em um navegador, aplicativo para desktop, em um tablet ou dispositivo móvel, experimente nossas etapas de solução de problemas.

:::warning
Antes de explorar as soluções abaixo, consulte a [página de status da Miro](https://status.miro.com/) para ver os relatórios de degradação de desempenho.
:::

Navegador Aplicativo para desktop Tablet, celular

1. 1. Abra a Miro no modo de navegação anônima/span> [(privado)](https://support.google.com/chrome/answer/95464) **e/ou em um** navegador diferenteSe a Miro funcionar no modo de navegação anônima ou em um navegador diferente, limpe o cache e os cookies do seu navegador.

**Como limpar os dados do site da Miro no Chrome**

1. Vá para https://miro.com/ e abra as /span>[ferramentas para desenvolvedores](https://miro.com/) do Chrome (**Command + Option + J** **no Mac***,* Ctrl + Shift + J **no Windows***)*. Selecione a guia **Aplicativo > Armazenamento**. Clique em **Limpar dados do site.** Isso deve remover quaisquer dados da Miro salvos no seu navegador do Chrome e você pode iniciar uma nova sessão. Observe que você será desconectado do seu perfil da Miro![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)*A opção de limpar dados do site no Chrome*

Você também pode precisar atualizar o navegador para a versão mais recente ou desabilitar determinadas extensões. Verifique a lista de [navegadores compatíveis](../technical-guidelines/02-supported-browsers-browser-restrictions.md).

2. Verifique sua conexão com a internet. Se a largura de banda da sua rede não atingir o mínimo de 8 Mb/s, mude para outra rede, de preferência mais rápida.

3. Certifique-se de que seu dispositivo atenda aos [**requisitos do sistema**](../technical-guidelines/01-system-requirements.md):

- CPU — 3 GHz (2 núcleos/4 threads)
- Memória RAM — 8 GB

4. Se você acessar a Miro em um notebook, certifique-se de estar no modo de alto desempenho/span>, em vez de no modo de economia de energia.

5. 5. Se você tiver um problema com boards específicos, tente [duplicá-los](../../managing-boards/03-how-to-duplicate-a-board.md)/span> **e veja se o problema persiste no board copiado.**Para usuários que não podem carregar e acessar a Miro:

6. 6. Verifique se sua conexão é compatível com WebSockets. /span> Leia mais sobre WebSockets e as etapas de solução de problemas em Como adicionar a Miro a aplicativos permitidos.

7. Verifique se o seu navegador suporta **WebAssembly**. O Miro conta com o WebAssembly para renderizar o conteúdo do board . Se o seu navegador, extensões ou configurações de segurança bloquearem o WebAssembly, os boards poderão não carregar. Para verificar se o seu navegador suporta WebAssembly, tente abrir [esta página de teste](https://wasm.joway.io/). Se esse não for o caso, consulte sua time de TI ou revise as configurações do seu navegador para garantir que o WebAssembly seja **permitido**.

8. Verifique com seu departamento de TI se sua empresa usa firewalls ou um proxy que possa bloquear a Miro. Siga as diretrizes para adicionar a Miro à lista de permissões ou forneça uma solução alternativa em Como adicionar a Miro a aplicativos permitidos.

Se o problema persistir, [entre em contato com o suporte da Miro](../../tools/troubleshooting/06-contacting-miro-support.md) e envie-nos [os logs do console do navegador](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

1. Verifique se está com um desempenho lento ou um carregamento interminável usando uma [**versão da web**](https://miro.com/app/dashboard/). Se você não conseguir acessar a Miro a partir da versão web, tente o guia de solução de problemas para navegador.
2. Se você não tiver nenhum problema no seu navegador, **redefina os dados do aplicativo.**

   **Como redefinir os dados do aplicativo no Windows**

   Pressione Alt, clique em **Ajuda** no canto superior direito e escolha **Redefinir os dados do aplicativo**:

   ![reset_app_data_on_Windows.jpg](https://help.miro.com/hc/article_attachments/12305900586898)
   *Como redefinir os dados do aplicativo no aplicativo para desktop no Windows*

   Se não conseguir encontrar o menu, é bem provável que use o aplicativo baixado da MS Store. Neste caso, para redefinir os dados do aplicativo, abra as**Configurações** **do Windows** > **Aplicativos**>Aplicativos e funcionalidades > encontre a Miro na lista >  Opções avançadas > Redefinir.

   **Como redefinir os dados do aplicativo para macOS**

   No aplicativo da Miro, clique em **Ajuda** no menu superior e escolha **Redefinir os dados do aplicativo**:

   ![reset_app_data_on_Mac.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
   *Como redefinir os dados do aplicativo no Mac*
3. Se o problema persistir, tente excluir e [**reinstalar o aplicativo.**](https://miro.com/apps/)

Se você ainda estiver enfrentando problemas, [entre em contato com o suporte da Miro](../../tools/troubleshooting/06-contacting-miro-support.md) e envie-nos [os logs do console do aplicativo](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

1. Verifique sua conexão com a internet. Se a largura de banda da sua rede não atingir o mínimo de 8 Mb/s, mude para outra rede, de preferência mais rápida.
2. Certifique-se de que seu dispositivo atenda aos **requisitos técnicos**:

- Para a Miro em tablets:— 6 GB de RAM— iOS 12.0 ou superior, Android 6.0 ou superior, Windows 10 versão 1607 ou superior— Resolução da tela de 768×1024 pixels ou superior
- Para a Miro no celular:— iOS 12.0 ou superior— Android 6.0 ou superior

Exclua e **reinstale o aplicativo** no seu dispositivo.

**Para usuários de iPad:**Observe que a degradação do desempenho da board no iPad pode ser causado por limitações de RAM do iPad. Tente o seguinte:

1. Antes de usar a Miro, feche todos os aplicativos desnecessários em segundo plano. Isso deve melhorar o desempenho.
2. Trabalhe em boards com tamanhos menores. Isso deve aliviar a carga do aplicativo no sistema.
3. Alterne para outro dispositivo (notebook ou computador) com melhor RAM e use a versão do navegador da Miro.

## Como solucionar problemas típicos

Sincronizando...  Aguarde Conexão restaurada/span>

A notificação pop-up **Sincronizando... Aguarde geralmente significa que uma carga pesada está sendo processada e o processo está necessitando de mais energia para ser concluído no tempo esperado. Portanto, a mensagem pode aparecer se você estiver trabalhando em um board extremamente pesado, por exemplo, se mover muitos objetos em massa ou se houver uma perda de pacote. Observe que, mesmo que seu board pareça relativamente simples, para a Miro, os objetos pesados seriam imagens de alta resolução, arquivos PDF ou desenhos com caneta (porque são gráficos vetoriais difíceis de renderizar), ou tabelas. Isso pode causar a degradação de desempenho que aciona a mensagem.**

Tente dividir seu board em outros menores copiando e colando seu conteúdo em um novo board e veja se o problema persiste.  Se isso não ajudar:

- Certifique-se de que seu dispositivo atenda aos requisitos mínimos do sistema e que seu navegador seja atualizado para a versão mais recente.
- Se você tiver muitas guias abertas no navegador, tente fechá-las ou congelá-las antes de trabalhar na Miro, para que seu navegador possa direcionar todo o seu poder de processamento para o aplicativo da Miro sem dividi-lo entre muitas guias.
- Teste a Miro no modo de navegação anônima (privado) (para excluir a possibilidade de interferência das extensões do navegador) e em um navegador diferente. Feche todas as guias do navegador e aplicativos rodando em segundo plano, se necessário.
- Limpe o cache e os cookies do seu navegador, reinicie o navegador e atualize a página clicando em F5 (ou Ctrl/Cmd + R) várias vezes.
- Se você tiver problemas com boards específicos, tente duplicá-los e verifique se o problema persiste nos novos boards. Você também pode tentar abrir um board com menos itens/board menor para ver se o problema ainda ocorre.
- Se você usar uma VPN, verifique se o problema persiste quando a desabilita.
- Tente duplicar o board e verifique se o erro é reproduzido no novo.

Geralmente, os erros **Reconectando...**, **Conexão restaurada** podem aparecer nos seguintes casos:

- Quando houver alguns problemas de conectividade do seu lado.  Garanta que sua conexão de rede atenda aos requisitos mínimos. Se possível, tente alternar para uma rede mais rápida.
- Quando você está trabalhando em vários boards pesados abertos no mesmo navegador.  Se este for o seu caso, feche todas as guias extras e aplicativos em execução no seu navegador e atualize a página do navegador.

Também vale a pena verificar sua conexão com o WebSocket (ainda mais se você estiver tendo problemas em todos os boards, mesmo os menores).  Entre em contato com seu departamento de TI e peça para que eles habilitem as conexões do WebSocket nas portas 80 e 443 (SSL) e [verifique duas vezes se a causa pode ser outra](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)/span>.

## Perguntas frequentes

*O desempenho do board depende do plano que estou usando (gratuito/pago)?*

Não, o desempenho do board não é afetado pelo seu plano.

*As configurações de compartilhamento do meu board afetam o desempenho?*

As configurações de compartilhamento não devem afetar o desempenho do board, mas o número de usuários no seu board pode influenciá-lo.  Você pode usar as dicas para as sessões colaborativas acima.
