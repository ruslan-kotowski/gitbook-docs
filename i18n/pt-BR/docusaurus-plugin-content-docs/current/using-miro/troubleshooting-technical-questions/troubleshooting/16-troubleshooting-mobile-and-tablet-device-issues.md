---
title: "Solu\xE7\xE3o de problemas de dispositivos m\xF3veis e tablets"
article_id: 360021113559
translation_id: 360021113559
locale: pt-br
sidebar_position: 16
created_at: '2021-04-16T08:25:42Z'
updated_at: '2025-11-25T16:04:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Se você tiver algum problema ao trabalhar no Miro no celular ou tablet, primeiro tente *reinstalar o aplicativo e recarregue seu dispositivo*. Se isso não ajudar, veja os possíveis motivos abaixo.

| **Problemas com dispositivos móveis** | | |
| --- | --- | --- |
| **Item** | **Possível razão** | **Solução:** |
| O aplicativo móvel no iOS trava e não funciona corretamente | A versão do iOS é muito antiga | Atualize sua versão do iOS ou use outro dispositivo. Nosso aplicativo móvel para iOS é compatível com a versão 12 ou superior |
| Consigo fazer login com sucesso no aplicativo de desktop, mas no celular fico preso no logotipo do Miro | Os dados de autenticação estão corrompidos (cache inválido) | Vá para **Configurações do aplicativo > Armazenamento > Limpar armazenamento** ou reinstale o aplicativo da Miro no seu dispositivo. |
| Recebo o erro "Algo deu errado" ao autenticar via SSO no aplicativo móvel | 1. A conexão de rede está protegida e algo bloqueia as solicitações  2. O Chrome é adicionado àlista WIAsupportedUserAgents do ADFS e direciona o usuário incorretamente  3. É possível que este dispositivo específico não consiga acessar o ambiente SSO da empresa | 1. Tente autorizar a conexão a uma rede diferente  2. Entre em contato com o admin do sistema e peça pararemover o Chrome da lista  3. Verifique com seu departamento de TI se há alguma restrição em relação a dispositivos específicos que têm permissão para usar SSO |
| Não consigo encontrar arquivos importados de boards no sistema de arquivos móvel | Quando você baixa um arquivo de um board no celular, ele fica "escondido" para você por algum tempo | Aguarde até que o arquivo apareça na pasta com os arquivos baixados |
| Quando entro no Miro no celular, vejo a mensagem "Nenhuma conta disponível" e não consigo acessar meu perfil | Você foi removido ou [saiu](../../managing-your-profile/06-how-to-leave-a-team.md) de todas as suas times. | Faça login no Miro no desktop ou tablet e crie uma nova time ou peça a outro usuário para convidá-lo para uma time Miro |
| Não consigo editar os boards da Miro em um navegador no celular | Esta é uma limitação conhecida no momento | Por favor, mude para nosso [aplicativo móvel](../../../getting-started/apps-for-devices/08-mobile-app.md), tablet ou desktop |
| Não consigo exportar meu board usando o aplicativo móvel | Esta é uma limitação conhecida no momento | Por favor, mude para outro dispositivo. Saiba mais sobre a exportação do Miro nesta [página](../../import-and-export/export/03-how-to-export-your-board.md) |

| **Problemas com tablets** | | |
| --- | --- | --- |
| **Item** | **Possível razão** | **Solução:** |
| Barra de ferramentas desaparecendo e comportamento estranho ao usar o Miro no iPad | Nosso aplicativo usa o WebView para renderizar os visuais, e uma das regras relacionadas ao gerenciamento de memória é que o processo de renderização não pode usar mais de 25% da memória RAM do dispositivo. Após essa marca, o aplicativo fica limitado e para de carregar corretamente sem apresentar nenhuma mensagem de erro ou travamento | - Feche todos os aplicativos desnecessários em segundo plano antes de usar o Miro - Trabalhar em boards que são *menor*em tamanho - Por fim, tente mudar para *outro dispositivo* (desktop) com melhor RAM |
| Consigo fazer login com sucesso no aplicativo de desktop, mas no tablet, fico preso no logotipo do Miro | Os dados de autenticação estão corrompidos | Vá para **Configurações do aplicativo > Armazenamento > Limpar armazenamento** ou reinstale o aplicativo da Miro no seu dispositivo. |
| Mensagem de erro “Desculpe, você não pode copiar tantos objetos de uma vez” ao colar objetos no iPad | Você excedeu a quantidade de dados que poderia ser colocada em um buffer no iPad | Por favor, copie e cole menos widgets de uma vez |
| Não consigo editar [documentos do Google enviados para meu board](../../../integrations-apps/google/05-google-drive.md) no tablet | Esta é atualmente uma limitação conhecida | Como solução alternativa, você pode abrir o documento por meio do aplicativo Google Doc se clicar no  ícone**Fonte** |
| Eu uso o Apple Pencil no iPad. Quando eu toco duas vezes para alternar entre caneta e borracha, nada acontece | Alternar entre caneta e borracha com toque duplo é um recurso nativo suportado pela segunda geração do Apple Pencil, e não algo desenvolvido especificamente pela Miro . É suportado apenas no aplicativo Tablet | Certifique-se de que seu Apple Pencil suporta o recurso e mude para o [aplicativo Tablet](../../../getting-started/apps-for-devices/11-tablet-app.md) |
| No iPad, as duas coisas a seguir não funcionam:   - zoom quando operado pela roda do mouse - navegação de board quando operada por toques de dois dedos no trackpad | Esta é uma limitação conhecida relacionada às restrições do sistema operacional no iPad | Infelizmente, ainda não há solução para isso. |
