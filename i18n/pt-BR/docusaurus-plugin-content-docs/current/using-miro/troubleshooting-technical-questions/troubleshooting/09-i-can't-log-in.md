---
title: "N\xE3o consigo fazer login"
article_id: 360020993079
translation_id: 360020993079
locale: pt-br
sidebar_position: 9
created_at: '2021-04-09T06:31:47Z'
updated_at: '2025-11-25T16:04:24Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Siga este guia se você tiver problemas para fazer login no seu perfil da Miro.

## Problemas com e-mail e/ou senha

Meu email/senha não está funcionando.

Confira aqui duas soluções que você pode tentar:

1. Verifique se o email/senha que você usa para fazer login não contém erros de digitação.
2. Se as credenciais inseridas estiverem corretas, [redefina sua senha](../../managing-your-profile/05-how-to-change-your-password.md).
3. Se o seu e-mail ou senha incluir um dos símbolos **& " < >**, [fale com nossa equipe de suporte.](https://help.miro.com/hc/requests/new?)

:::warning
Vale ressaltar que seu **perfil é bloqueado** após dez tentativas de inserir seu e-mail e senha. Talvez seja necessário [desbloquear o perfil](../../tools/troubleshooting/14-profile-lockout.md) primeiro e depois redefinir a sua senha.
:::

Não consigo redefinir a minha senha.

Se você não receber um e-mail de redefinição de senha, pode ser por três motivos:

1. **O e-mail está incorreto.**
Verifique se não há erros de digitação no e-mail que você enviou. Se encontrar um erro de digitação, solicite uma nova redefinição.

2. **O e-mail ainda não está cadastrado na Miro.**
Neste caso, o link de redefinição de senha não será enviado para seu endereço de e-mail. Cadastre um novo perfil na [página de inscrição](https://miro.com/signup/). Se o seu e-mail estiver cadastrado, você verá a mensagem correspondente:
![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)

3. **Há problemas com a entrega de e-mail.**

- Abra suas pastas de **Spam, Promoções, Lixo, Social** e **Atualizações**, e verifique se o e-mail da solicitação de redefinição está lá.
- Também pode ser que um firewall esteja impedindo o e-mail de chegar à sua caixa de entrada.

  Entre em contato com seu *admin de sistema* e peça para autorizar nossos domínios e subdomínios: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) e [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/) e adicione o IPS do nosso sistema de envio de e-mail à sua lista de permissões.

  Confira a lista de IPs dedicados: 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. [Veja este artigo](../../tools/troubleshooting/02-allowlist-miro-mailers.md) com mais informações sobre quais remetentes você deve permitir.

Redefini a minha senha, mas ainda não consigo fazer login.

Caso ainda não consiga acessar o seu perfil:

1. Certifique-se de inserir a nova senha.
2. Faça login no modo privado (anônimo) do seu navegador ou tente usar outro navegador.

Faço login com um e-mail, mas o sistema me redireciona e me conecta com outro e-mail.

Esse problema pode surgir se você usa um método de autenticação alternativo para fazer login (Google, Slack, Office 365, Apple ID, Facebook).

![new-sing-in-third-party.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)
*Outras opções de login na página de iniciar sessão*

Você pode ter vinculado acidentalmente seu endereço de e-mail do Google/Office 365, etc. ao seu perfil da Miro cadastrado com um e-mail diferente. Se isso acontecer, tente o seguinte:

1. Remova a associação de e-mail errada acessando **Configurações de perfil** > **Integrações** e clicando em **Sair** ao lado de Google/Office 365, etc.
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Como remover a associação com o login do Google*
2. Saia e faça login com o seu e-mail novamente.

:::note
Configure uma conexão com o e-mail do Google/Office 365/Slack que corresponda ao e-mail do seu perfil da Miro para evitar esse problema.
:::

## Iniciar sessão com logon único não funciona

Confira o artigo: [Possíveis problemas ao conectar com logon único](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## Carregamento interminável ao fazer login

Para usuários que enfrentam problemas de carregamento intermináveis após inserir suas credenciais da Miro, recomendamos o seguinte:

1. Faça login em um **navegador diferente**.
2. Faça login usando o **modo privado (anônimo) do seu navegador.** Se o problema não persistir no modo de navegação anônima/outro navegador, limpe o cache do seu navegador.

   Como limpar o cache do Chrome.

   1. Vá para `https://miro.com/` e abra as **ferramentas para desenvolvedores**do Chrome (**Command + Option + J** *no Mac*, **Ctrl + Shift + J***no Windows*).
   2. Selecione a guia **Aplicativo > Armazenamento**. Você verá o botão azul **Limpar dados do site.**​  Clique no botão e todos os dados da Miro salvos no seu navegador do Chrome devem ser excluídos, para que você possa iniciar uma nova sessão de trabalho.
   ![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
   *A opção de limpar os dados do site no Chrome*
3. Se você estiver usando uma **VPN**, habilite-a ou desabilite-a.
4. Verifique com seu departamento de TI se sua empresa usa firewalls ou um proxy que possa bloquear a Miro. Siga [estas diretrizes](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md) para **autorizar a Miro** ou forneça um bypass.
5. Verifique sua conexão com a internet. Se a largura de banda da sua rede não atingir o mínimo de 8 Mb/s, **mude para outra rede, de preferência** **mais rápida**.
6. Tente se conectar a um **ponto de acesso móvel**, se tiver um disponível. Em seguida, reconecte-se à sua rede original.
7. Se isso não ajudar, [envie uma solicitação](https://miro.com/contact/recover/) e [envie os logs do console do seu navegador para o Suporte](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

## Problemas de login no aplicativo para desktop da Miro

1. Se não conseguir acessar a Miro no aplicativo para desktop, faça login pelo seu navegador. Se mesmo assim não conseguir fazer login, siga as etapas acima. Se você conseguir acessar a Miro pelo navegador, siga as etapas abaixo.
2. Redefina os dados do aplicativo.

Como redefinir os dados do aplicativo no Windows.

Pressione **Alt > Ajuda**e escolha redefinir os dados do aplicativo como mostrado na captura de tela abaixo:

​​![reset_app_data_on_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725434514_reset%20app%20data%20on%20Windows.jpg)
*Como redefinir os dados do aplicativo no aplicativo para desktop no Windows*

Se não conseguir encontrar o menu, é bem provável que use o aplicativo baixado da MS Store. Neste caso, para redefinir os dados do aplicativo, abra as **Configurações** do Windows > **Aplicativos** > **Aplicativos e funcionalidades** > encontre a **Miro** na lista >  **Opções avançadas**> **Redefinir**.

Se isso não ajudar imediatamente, exclua todos os arquivos do aplicativo de **C:\Users\username\AppData\Roaming\RealtimeBoard** e **C:\Users\username\AppData\Local\RealtimeBoard.**

> **✏️** Se a pasta do **Appdata** estiver oculta, confira [aqui](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) como pode revelá-la.

Como redefinir os dados do aplicativo no Mac.

Clique no menu superior da Miro e selecione **Redefinir os dados do aplicativo** conforme mostrado na captura de tela abaixo:

![reset_app_data_on_Mac.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
*Como redefinir os dados do aplicativo no Mac*

Depois disso, tente fazer login no aplicativo novamente e verifique se o problema foi resolvido.

Se a redefinição não ajudar de imediato, abra uma janela do Finder > pressione **Command + Shift + G**> cole **~/Library/Application Support/RealtimeBoard**e exclua todos os arquivos do aplicativo.

3. Se o problema persistir, verifique se está usando a versão mais recente do aplicativo baixado [do nosso site.](https://miro.com/apps/)

## Login com o Google/Office 365/Slack, etc.

Não consigo fazer login pelo Google/Office/Slack, etc.

1. Faça login na Miro usando suas credenciais padrão (e-mail e senha). Se você não se lembrar ou não tiver a senha, [redefina a sua senha](../../managing-your-profile/05-how-to-change-your-password.md).
2. Vá para **Configurações do perfil** > **Integrações**, clique em **Sair** ao lado de Google/Office 365, etc. e reconfigure a conexão.
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Como remover a associação com o login do Google*

Não consigo fazer login pelo Google/Office/Slack, etc. no aplicativo para desktop.

Consulte estas etapas de solução de problemas.

Eu fazia login na Miro pelo Google/Office 365, etc., mas meu serviço de e-mail mudou. Como posso fazer login agora?

Faça login na Miro usando suas novas credenciais desse serviço (e-mail e senha). Se você não se lembrar ou não tiver a senha, [redefina-a](../../managing-your-profile/05-how-to-change-your-password.md).

## Problemas de login no tablet/celular

1. Verifique se consegue fazer login na versão do navegador. Se não conseguir, recomendamos estas etapas de solução de problemas.
2. Se conseguir se conectar pelo navegador, pode ser que os dados de autenticação do seu dispositivo estejam corrompidos. Vá para **Configurações do aplicativo > Armazenamento > Limpar armazenamento** ou reinstale o aplicativo da Miro no seu dispositivo.

## Dicas de solução de problemas

Se você não conseguir encontrar uma solução acima, faça login na Miro em **outro navegador** ou **pelo modo de navegação anônima**. Se tudo estiver bem no modo de navegação anônima do seu navegador, limpe o cache e os cookies do navegador e faça login na Miro no modo padrão.

Como limpar o cache do Chrome.

1. Vá para `https://miro.com/` e abra as **ferramentas para desenvolvedores**do Chrome (**Command + Option + J** *no Mac*, **Ctrl + Shift + J***no Windows*).
2. Selecione a guia **Aplicativo > Armazenamento**. Você verá o botão azul **Limpar dados do site.**​  Clique no botão e todos os dados da Miro salvos no seu navegador do Chrome devem ser excluídos, para que você possa iniciar uma nova sessão de trabalho.

![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
*A opção de limpar os dados do site no Chrome*

Caso isso não ajude, [entre em contato com o Suporte da Miro](https://miro.com/contact/recover/). Descreva o problema detalhadamente.

:::note
Se você estiver tendo problemas ao se cadastrar na Miro, confira[Problemas com código de confirmação](../../tools/troubleshooting/12-issues-with-confirmation-code-or-password-reset-emails.md).
:::
